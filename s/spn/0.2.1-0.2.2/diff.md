# Comparing `tmp/spn-0.2.1.tar.gz` & `tmp/spn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spn-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spn-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spn-0.2.1.tar` & `spn-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1080 2023-05-27 16:16:32.016856 spn-0.2.1/LICENSE
--rw-r--r--   0        0        0     1056 2023-05-28 18:08:52.749698 spn-0.2.1/README.md
--rw-r--r--   0        0        0      430 2023-05-28 17:54:31.264179 spn-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    10998 2023-05-28 18:10:23.975538 spn-0.2.1/src/spn.py
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 spn-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-27 16:16:32.016856 spn-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1058 2023-05-28 18:48:18.128387 spn-0.2.2/README.md
+-rw-r--r--   0        0        0      430 2023-05-28 17:54:31.264179 spn-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    11116 2023-05-28 18:48:05.791831 spn-0.2.2/src/spn.py
+-rw-r--r--   0        0        0     1433 1970-01-01 00:00:00.000000 spn-0.2.2/PKG-INFO
```

### Comparing `spn-0.2.1/LICENSE` & `spn-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spn-0.2.1/README.md` & `spn-0.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Simple command-line interface for the Wayback Machine's Save Page Now (SPN) API.
+Unofficial command-line interface for the Wayback Machine's Save Page Now API.
 
 ## Installation
 ```bash
 pip install spn
 ```
 
 ## API Keys
@@ -36,11 +36,11 @@
 spn https://www.theguardian.com/politics/2023/may/28/more-than-half-of-voters-now-want-britain-to-forge-closer-ties-with-the-eu-poll-reveals
 
 # save urls from a file
 spn -i urls
 
 # save urls from a pipe and only save urls not already saved in the last 3 days
 some-command-that-outputs-urls | spn -i - --if-not-archived-within=3d
-```
 
-## Official API Documentation
-https://docs.google.com/document/d/1Nsv52MvSjbLb2PCpHlat0gkzw0EvtSgpKHu4mk0MnrA/edit
+# save urls from a pipe and wait for the remote save jobs to complete
+some-command-that-outputs-urls | spn -i - --wait
+```
```

### Comparing `spn-0.2.1/src/spn.py` & `spn-0.2.2/src/spn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 '''Unofficial CLI for the Wayback Machine's Save Page Now API.'''
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 import asyncio
 import collections
 import sys
 
 import click
 import confuse
@@ -237,7 +237,10 @@
 
     return int(error)
 
 
 def main():
     return _main(auto_envvar_prefix='SPN',
                  default_map=confuse.Configuration('spn').flatten())
+
+# official API documentation:
+# https://docs.google.com/document/d/1Nsv52MvSjbLb2PCpHlat0gkzw0EvtSgpKHu4mk0MnrA/edit
```

### Comparing `spn-0.2.1/PKG-INFO` & `spn-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: spn
-Version: 0.2.1
+Version: 0.2.2
 Summary: Unofficial CLI for the Wayback Machine's Save Page Now API.
 Author-email: Chris Coleman <chris@chriscoleman.uk>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click
 Requires-Dist: confuse
 Requires-Dist: httpx
 Requires-Dist: jsonlines
 Requires-Dist: tenacity
 
-Simple command-line interface for the Wayback Machine's Save Page Now (SPN) API.
+Unofficial command-line interface for the Wayback Machine's Save Page Now API.
 
 ## Installation
 ```bash
 pip install spn
 ```
 
 ## API Keys
@@ -49,12 +49,12 @@
 spn https://www.theguardian.com/politics/2023/may/28/more-than-half-of-voters-now-want-britain-to-forge-closer-ties-with-the-eu-poll-reveals
 
 # save urls from a file
 spn -i urls
 
 # save urls from a pipe and only save urls not already saved in the last 3 days
 some-command-that-outputs-urls | spn -i - --if-not-archived-within=3d
-```
 
-## Official API Documentation
-https://docs.google.com/document/d/1Nsv52MvSjbLb2PCpHlat0gkzw0EvtSgpKHu4mk0MnrA/edit
+# save urls from a pipe and wait for the remote save jobs to complete
+some-command-that-outputs-urls | spn -i - --wait
+```
```

