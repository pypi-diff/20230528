# Comparing `tmp/superkabuki-0.0.45.tar.gz` & `tmp/superkabuki-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superkabuki-0.0.45.tar", last modified: Sun May 28 18:18:03 2023, max compression
+gzip compressed data, was "superkabuki-0.0.47.tar", last modified: Sun May 28 19:42:56 2023, max compression
```

## Comparing `superkabuki-0.0.45.tar` & `superkabuki-0.0.47.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 18:18:03.897341 superkabuki-0.0.45/
--rw-r--r--   0 a         (1000) a         (1000)     1295 2023-05-28 05:02:44.000000 superkabuki-0.0.45/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)     6531 2023-05-28 18:18:03.897341 superkabuki-0.0.45/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)     5920 2023-05-28 18:17:59.000000 superkabuki-0.0.45/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 18:18:03.893342 superkabuki-0.0.45/bin/
--rw-r--r--   0 a         (1000) a         (1000)      127 2023-05-28 05:02:44.000000 superkabuki-0.0.45/bin/superkabuki
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-28 18:18:03.897341 superkabuki-0.0.45/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1003 2023-05-28 05:02:44.000000 superkabuki-0.0.45/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 18:18:03.897341 superkabuki-0.0.45/superkabuki.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)     6531 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      231 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       44 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       12 2023-05-28 18:18:03.000000 superkabuki-0.0.45/superkabuki.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)    13080 2023-05-28 18:17:22.000000 superkabuki-0.0.45/superkabuki.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 19:42:56.552316 superkabuki-0.0.47/
+-rw-r--r--   0 a         (1000) a         (1000)     1295 2023-05-28 05:02:44.000000 superkabuki-0.0.47/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)     6531 2023-05-28 19:42:56.552316 superkabuki-0.0.47/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)     5920 2023-05-28 18:17:59.000000 superkabuki-0.0.47/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 19:42:56.552316 superkabuki-0.0.47/bin/
+-rw-r--r--   0 a         (1000) a         (1000)      127 2023-05-28 05:02:44.000000 superkabuki-0.0.47/bin/superkabuki
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-28 19:42:56.552316 superkabuki-0.0.47/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1003 2023-05-28 05:02:44.000000 superkabuki-0.0.47/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 19:42:56.552316 superkabuki-0.0.47/superkabuki.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)     6531 2023-05-28 19:42:56.000000 superkabuki-0.0.47/superkabuki.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      231 2023-05-28 19:42:56.000000 superkabuki-0.0.47/superkabuki.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-28 19:42:56.000000 superkabuki-0.0.47/superkabuki.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       44 2023-05-28 19:42:56.000000 superkabuki-0.0.47/superkabuki.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       12 2023-05-28 19:42:56.000000 superkabuki-0.0.47/superkabuki.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)    13396 2023-05-28 19:42:51.000000 superkabuki-0.0.47/superkabuki.py
```

### Comparing `superkabuki-0.0.45/LICENSE` & `superkabuki-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `superkabuki-0.0.45/PKG-INFO` & `superkabuki-0.0.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superkabuki
-Version: 0.0.45
+Version: 0.0.47
 Summary: superkabuki is SCTE-35 Packet injection for the people
 Home-page: https://github.com/futzu/superkabuki
 Author: Adrian of Doom
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `superkabuki-0.0.45/README.md` & `superkabuki-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `superkabuki-0.0.45/setup.py` & `superkabuki-0.0.47/setup.py`

 * *Files identical despite different names*

### Comparing `superkabuki-0.0.45/superkabuki.egg-info/PKG-INFO` & `superkabuki-0.0.47/superkabuki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superkabuki
-Version: 0.0.45
+Version: 0.0.47
 Summary: superkabuki is SCTE-35 Packet injection for the people
 Home-page: https://github.com/futzu/superkabuki
 Author: Adrian of Doom
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `superkabuki-0.0.45/superkabuki.py` & `superkabuki-0.0.47/superkabuki.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from threefive.crc import crc32
 from threefive.bitn import NBin
 from new_reader import reader
 from iframes import IFramer
 
 MAJOR = "0"
 MINOR = "0"
-MAINTAINENCE = "45"
+MAINTAINENCE = "47"
 
 
 def version():
     """
     version prints version as a string
 
     Odd number versions are releases.
@@ -48,20 +48,20 @@
 
     """
 
     CUEI_DESCRIPTOR = b"\x05\x04CUEI"
 
     def __init__(self, tsdata=None):
         self.infile = None
-        self.outfile = "outfile.ts"
+        self.outfile = "superkabuki-out.ts"
         if isinstance(tsdata, str):
             self.outfile = f'superkabuki-{tsdata.rsplit("/",1)[1]}'
         super().__init__(tsdata)
         self.pmt_payload = None
-        self.scte35_pid = 0x86
+        self.scte35_pid = None
         self.scte35_cc = 0
         self.iframer = IFramer(shush=True)
         self.sidecar = deque()
         self.sidecar_file = "sidecar.txt"
         self.time_signals = False
         self._parse_args()
         super().__init__(self.infile)
@@ -94,16 +94,16 @@
             "--sidecar",
             default="sidecar.txt",
             help=""" Sidecar file for SCTE35 (default sidecar.txt)""",
         )
         parser.add_argument(
             "-p",
             "--scte35_pid",
-            default="0x86",
-            # type=int,
+            #default=1000,
+            #type=int,
             help="""Pid for SCTE-35 packets, can be hex or integer. (default 0x86)""",
         )
 
         parser.add_argument(
             "-t",
             "--time_signals",
             action="store_const",
@@ -120,52 +120,58 @@
             help="Show version",
         )
 
         args = parser.parse_args()
         self._apply_args(args)
 
     def _apply_args(self, args):
-        self._args_version(args)
+        """
+        _apply_args applies command line args
+        """
         if args.scte35_pid and args.input:
             self.outfile = args.output
             self.infile = args.input
             self.sidecar_file = args.sidecar
             self._tsdata = reader(args.input)
             self.pid2int(args.scte35_pid)
             self.time_signals = args.time_signals
-
-    @staticmethod
-    def _args_version(args):
-        if args.version:
-            print(version())
+        else:
+            print2("scte35 pid must be set")
             sys.exit()
 
     def pid2int(self, pid):
+        """
+        pid2int converts a string pid
+        like "0x86" or "1000" to an int.
+        """
         try:
-            self.scte35_pid = int(args.scte35_pid)
+            self.scte35_pid = int(pid)
         except:
             try:
-                self.scte35_pid = int(args.scte35_pid, 16)
+                self.scte35_pid = int(pid, 16)
             except:
                 self.scte35_pid = 0x86
 
     def _bump_cc(self):
         self.scte35_cc = (self.scte35_cc + 1) % 16
 
     def _pmt_scte35_stream(self):
         if self.scte35_pid:
             nbin = NBin()
-            stream_type = b"\x86"
-            nbin.add_bites(stream_type)
+            stream_type = 0x86
+            nbin.add_int(stream_type,8)
             nbin.add_int(7, 3)  # reserved  0b111
             nbin.add_int(self.scte35_pid, 13)
             nbin.add_int(15, 4)  # reserved 0b1111
             es_info_length = 0
             nbin.add_int(es_info_length, 12)
             scte35_stream = nbin.bites
+            print2("Stream Added:")
+            print2(f"Stream Type: {stream_type} PID: {self.scte35_pid} EI Len:  {es_info_length}")
+
             return scte35_stream
 
     def encode(self):
         """
         encode parses the video input,
         adds the SCTE-35 PID to the PMT,
         parses the sidecar file,
@@ -326,25 +332,26 @@
             return False
         seclen = self._parse_length(pay[1], pay[2])
         # print2("seclen", seclen)
         n_seclen = seclen
         if self._section_incomplete(pay, pid, seclen):
             return False
         program_number = self._parse_program(pay[3], pay[4])
-        # print2("program_number", program_number)
+        print2(f"Program Number {program_number}")
         pcr_pid = self._parse_pid(pay[8], pay[9])
-        # print2("pcr_pid", pcr_pid)
+        print2(f"PCR PID {pcr_pid}")
         self.pids.pcr.add(pcr_pid)
         self.maps.pid_prgm[pcr_pid] = program_number
         proginfolen = self._parse_length(pay[10], pay[11])
         # print2("pif", proginfolen)
         idx = 12
         end = idx + proginfolen
         info_bites = pay[idx:end]
         n_info_bites = info_bites + self.CUEI_DESCRIPTOR
+        print2(f"Registration Descriptor added {self.CUEI_DESCRIPTOR}")
         while idx < end:
             d_type = pay[idx]
             idx += 1
             d_len = pay[idx]
             idx += 1
             d_bytes = pay[idx - 2 : idx + d_len]
             idx += d_len
@@ -361,17 +368,18 @@
         parse the elementary streams
         from a program
         """
         # 5 bytes for stream_type info
         chunk_size = 5
         end_idx = (idx + si_len) - 4
         start = idx
+        print2("Streams Found:")
         while idx < end_idx:
             stream_type, pid, ei_len = self._parse_stream_type(pay, idx)
-            print2(("Stream: type:", stream_type, "PID:", pid, "EI Len:", ei_len))
+            print2(f"Stream Type: {stream_type}  PID: { pid}  EI Len:  {ei_len}")
             idx += chunk_size
             idx += ei_len
             self.maps.pid_prgm[pid] = program_number
             self._chk_pid_stream_type(pid, stream_type)
         streams = pay[start:end_idx]
         return streams
```

