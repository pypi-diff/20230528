# Comparing `tmp/simplejob-0.0.5-py3-none-any.whl.zip` & `tmp/simplejob-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7235 bytes, number of entries: 8
+Zip file size: 7312 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      138 b- defN 23-May-26 20:52 simplejob/__init__.py
 -rw-rw-rw-  2.0 fat      878 b- defN 23-May-27 03:49 simplejob/__main__.py
--rw-rw-rw-  2.0 fat    10127 b- defN 23-May-27 02:48 simplejob/simplejob.py
--rw-rw-rw-  2.0 fat     1090 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5658 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      630 b- defN 23-May-27 03:50 simplejob-0.0.5.dist-info/RECORD
-8 files, 18623 bytes uncompressed, 6139 bytes compressed:  67.0%
+-rw-rw-rw-  2.0 fat    10558 b- defN 23-May-28 13:07 simplejob/simplejob.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-May-28 13:08 simplejob-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-May-28 13:08 simplejob-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 13:08 simplejob-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-28 13:08 simplejob-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      630 b- defN 23-May-28 13:08 simplejob-0.0.6.dist-info/RECORD
+8 files, 18925 bytes uncompressed, 6216 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: simplejob/__main__.py
 Comment: 
 
 Filename: simplejob/simplejob.py
 Comment: 
 
-Filename: simplejob-0.0.5.dist-info/LICENSE
+Filename: simplejob-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: simplejob-0.0.5.dist-info/METADATA
+Filename: simplejob-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: simplejob-0.0.5.dist-info/WHEEL
+Filename: simplejob-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: simplejob-0.0.5.dist-info/top_level.txt
+Filename: simplejob-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: simplejob-0.0.5.dist-info/RECORD
+Filename: simplejob-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplejob/simplejob.py

```diff
@@ -8,14 +8,15 @@
 import time
 from datetime import datetime
 import enum
 import os
 import uuid
 from collections import Counter
 import json
+import contextlib
 
 class JobRunningStatus(enum.IntEnum):
     Ready = 0
     Running = 1
     Completed = 2
     RetryOut = 3
 
@@ -53,15 +54,20 @@
         return waitsIds - ids
     
     def detectInvalidIds(self, jobContexts:list) -> list:
         return [ index for index, context in enumerate(jobContexts) if not context.get("id", None) ]
 
     def entryFromJson(self, filename:str):
         with open(filename, "r") as f:
-            self.entry(json.load(f)["jobContexts"])
+            jobContexts = json.load(f)["jobContexts"]
+
+            if len([ context for context in jobContexts if context.get("semaphore", None) is not None ]) > 0:
+                raise ValueError("Key 'semaphore' can not be specified for JSON data read from a file.")
+
+            self.entry(jobContexts)
 
     def entry(self, jobContexts:list) -> None:
         elementIndices = self.detectInvalidIds(jobContexts)
         if len(elementIndices) > 0:
             raise ValueError(f"Invalid Id detected. element indices={elementIndices}")
 
         invalidWaitsIds = self.detectInvalidWaitsIds(jobContexts)
@@ -146,21 +152,22 @@
 
         return json.dumps(report, indent=4)
 
     def getRunningStatus(self):
         return Counter([ job.runningStatus.name for job in self.jobs ])
 
 class SimpleJob(threading.Thread):
-    def entry(self, commandLine:str, id:str="", timeout:int=None, retry:int=1, delay:int=0, backoff:int=1, waits:list = [], logOutputDirectory:str="", jobManager:SimpleJobManager=None) -> None:
+    def entry(self, commandLine:str, id:str="", timeout:int=None, retry:int=1, delay:int=0, backoff:int=1, waits:list=[], semaphore=None, logOutputDirectory:str="", jobManager:SimpleJobManager=None) -> None:
         if not jobManager and len(waits) > 0:
             raise ValueError("waits list can set the JobManager together.")
 
         self.commandLine:str = commandLine
         self.id:str = id if id != "" else uuid.uuid4()
         self.waits:list = waits
+        self.semaphore = semaphore
         self.logOutputDirectory:str = logOutputDirectory
         self.logFileName:str = "" if not self.logOutputDirectory else os.path.join(self.logOutputDirectory, f"{self.id}.log")
         self.jobManager:SimpleJobManager = jobManager
         self.exitCode:int = 0
         self.runningStatus:JobRunningStatus = JobRunningStatus.Ready
         self.startDateTime:datetime = None
         self.finishDateTime:datetime = None
@@ -216,15 +223,16 @@
     def run(self) -> None:
         self.runningStatus = JobRunningStatus.Running
         self.startTime = time.perf_counter()
         self.startDateTime = datetime.now()
 
         for trialCounter in range(0, self.retry + 1):
             try:
-                completePocess = subprocess.run(self.commandLine, capture_output=True, text=True, timeout=self.timeout)
+                with self.semaphore if self.semaphore is not None else contextlib.nullcontext():
+                    completePocess = subprocess.run(self.commandLine, capture_output=True, text=True, timeout=self.timeout)
                 self.writeLog(completePocess.stdout)
             except subprocess.TimeoutExpired as e:
                 self.writeLog(e.output)
                 self.writeLog(f"Error: Timed out({trialCounter}/{self.retry})")
 
                 self.retried = trialCounter
                 time.sleep((trialCounter + 1) ** self.backoff + self.delay)       # Exponential backoff
```

## Comparing `simplejob-0.0.5.dist-info/LICENSE` & `simplejob-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simplejob-0.0.5.dist-info/METADATA` & `simplejob-0.0.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplejob
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple Batch job executor
 Home-page: https://github.com/Hajime-Saitou/simplejob
 Author: Hajime Saito
 Author-email: g.hajime.saitou@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/Hajime-Saitou/simplejob
 Keywords: batch,job
@@ -71,18 +71,18 @@
 
     if jobManager.completed():
         break
 
     time.sleep(1)
 ```
 
-It can be written on a single line using wait(). If error occred in the wait(), Raise CalledJobException.
+It can be written on a single line using run(). If error occred in the run(), Raise CalledJobException.
 
 ```
-jobManager.wait()
+jobManager.run()
 ```
 
 ### report
 
 You can output the execution result as a report by calling report(). Returns an empty result for jobs that have not run.
 
 Example for SimpleJobManager.report()
@@ -158,19 +158,18 @@
     "finishDateTime": "2023/05/18 21:47:43.594701",
     "elapsedTime": "00:00:05.65712"
 }
 ```
 
 ### rerun
 
-After the cause of the error has been resolved, the job can be rerun using rerun(). The remaining jobs use wait() to run the job until all jobs have finished or until the error occurs again.
+After the cause of the error has been resolved, the job can be rerun using rerun().
 
 ```
 jobManager.rerun()
-jobManager.wait()
 ```
 
 ## Output the job log
 
 To output logs, specify the logOutputDirectory parameter to constructor of SimpleJobManager class. The log file name is the job id with a "log" extension.
 
 ```
```

## Comparing `simplejob-0.0.5.dist-info/RECORD` & `simplejob-0.0.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 simplejob/__init__.py,sha256=6uL_mCITP-B5IsHQnH_EdLOuOra_h8qhcsc4JzwQg5Y,138
 simplejob/__main__.py,sha256=P6WnVLNpP-OlOzQckCtLOPzQnNDQUnLEoQTcAnWHR5w,878
-simplejob/simplejob.py,sha256=8Pw2osHzIicE6apgbN29T7l6hZ0uZkS7o8Cyo7Dcdq8,10127
-simplejob-0.0.5.dist-info/LICENSE,sha256=Vagqa5lmdjnJU04Y4FZYFRpvkLGv8mB_8XGGXQ1ODg0,1090
-simplejob-0.0.5.dist-info/METADATA,sha256=NkeI7yCRrb0HtWoDlrOm9Vi-ON_9qFz7xVHCa53nCcA,5658
-simplejob-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-simplejob-0.0.5.dist-info/top_level.txt,sha256=YTc5tkhXcB0dLc0EIlpQRHYmt8Q63ucEgdP0-QSAFng,10
-simplejob-0.0.5.dist-info/RECORD,,
+simplejob/simplejob.py,sha256=xdquENIqCSC_nZFc5kQeIofy0M2SSdzURVhQpBUXFrE,10558
+simplejob-0.0.6.dist-info/LICENSE,sha256=Vagqa5lmdjnJU04Y4FZYFRpvkLGv8mB_8XGGXQ1ODg0,1090
+simplejob-0.0.6.dist-info/METADATA,sha256=VCNvA0ct_HKzxlaRCuyUVrH2oguJisJISCGS1RfINJo,5529
+simplejob-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+simplejob-0.0.6.dist-info/top_level.txt,sha256=YTc5tkhXcB0dLc0EIlpQRHYmt8Q63ucEgdP0-QSAFng,10
+simplejob-0.0.6.dist-info/RECORD,,
```

