# Comparing `tmp/superkabuki-0.0.41.tar.gz` & `tmp/superkabuki-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superkabuki-0.0.41.tar", last modified: Fri Mar 24 19:26:39 2023, max compression
+gzip compressed data, was "superkabuki-0.0.43.tar", last modified: Sun May 28 05:03:14 2023, max compression
```

## Comparing `superkabuki-0.0.41.tar` & `superkabuki-0.0.43.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-03-24 19:26:39.227806 superkabuki-0.0.41/
--rw-r--r--   0 a         (1000) a         (1000)     1295 2023-02-13 15:56:53.000000 superkabuki-0.0.41/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)     6641 2023-03-24 19:26:39.227806 superkabuki-0.0.41/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)     6030 2023-03-24 19:26:04.000000 superkabuki-0.0.41/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-03-24 19:26:39.223806 superkabuki-0.0.41/bin/
--rw-r--r--   0 a         (1000) a         (1000)      127 2023-03-24 19:26:04.000000 superkabuki-0.0.41/bin/superkabuki
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-03-24 19:26:39.227806 superkabuki-0.0.41/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1003 2023-03-24 19:26:04.000000 superkabuki-0.0.41/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-03-24 19:26:39.227806 superkabuki-0.0.41/superkabuki.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)     6641 2023-03-24 19:26:39.000000 superkabuki-0.0.41/superkabuki.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      231 2023-03-24 19:26:39.000000 superkabuki-0.0.41/superkabuki.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-03-24 19:26:39.000000 superkabuki-0.0.41/superkabuki.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       44 2023-03-24 19:26:39.000000 superkabuki-0.0.41/superkabuki.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       12 2023-03-24 19:26:39.000000 superkabuki-0.0.41/superkabuki.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)    12745 2023-03-24 19:26:30.000000 superkabuki-0.0.41/superkabuki.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 05:03:14.248524 superkabuki-0.0.43/
+-rw-r--r--   0 a         (1000) a         (1000)     1295 2023-05-28 05:02:44.000000 superkabuki-0.0.43/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)     6641 2023-05-28 05:03:14.244523 superkabuki-0.0.43/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)     6030 2023-05-28 05:02:44.000000 superkabuki-0.0.43/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 05:03:14.244523 superkabuki-0.0.43/bin/
+-rw-r--r--   0 a         (1000) a         (1000)      127 2023-05-28 05:02:44.000000 superkabuki-0.0.43/bin/superkabuki
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-28 05:03:14.248524 superkabuki-0.0.43/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1003 2023-05-28 05:02:44.000000 superkabuki-0.0.43/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-28 05:03:14.244523 superkabuki-0.0.43/superkabuki.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)     6641 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      231 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       44 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       12 2023-05-28 05:03:14.000000 superkabuki-0.0.43/superkabuki.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)    12922 2023-05-28 05:02:44.000000 superkabuki-0.0.43/superkabuki.py
```

### Comparing `superkabuki-0.0.41/LICENSE` & `superkabuki-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `superkabuki-0.0.41/PKG-INFO` & `superkabuki-0.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superkabuki
-Version: 0.0.41
+Version: 0.0.43
 Summary: superkabuki is SCTE-35 Packet injection for the people
 Home-page: https://github.com/futzu/superkabuki
 Author: Adrian of Doom
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SuperKabuki
 SCTE-35 Packet Injection for MPEGTS.
-# SuperKabuki v.0.0.39 is now Released.
+# SuperKabuki v.0.0.41 is now Released.
 ![image](https://user-images.githubusercontent.com/52701496/222034768-b8b1b34c-a645-461c-9408-6fffe2d40d63.png)
 
  
 <details> <summary><h1>Fast Start</h1> </summary>
 
 * Install SuperKabuki
 ```js
```

### Comparing `superkabuki-0.0.41/README.md` & `superkabuki-0.0.43/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SuperKabuki
 SCTE-35 Packet Injection for MPEGTS.
-# SuperKabuki v.0.0.39 is now Released.
+# SuperKabuki v.0.0.41 is now Released.
 ![image](https://user-images.githubusercontent.com/52701496/222034768-b8b1b34c-a645-461c-9408-6fffe2d40d63.png)
 
  
 <details> <summary><h1>Fast Start</h1> </summary>
 
 * Install SuperKabuki
 ```js
```

### Comparing `superkabuki-0.0.41/setup.py` & `superkabuki-0.0.43/setup.py`

 * *Files identical despite different names*

### Comparing `superkabuki-0.0.41/superkabuki.egg-info/PKG-INFO` & `superkabuki-0.0.43/superkabuki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superkabuki
-Version: 0.0.41
+Version: 0.0.43
 Summary: superkabuki is SCTE-35 Packet injection for the people
 Home-page: https://github.com/futzu/superkabuki
 Author: Adrian of Doom
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SuperKabuki
 SCTE-35 Packet Injection for MPEGTS.
-# SuperKabuki v.0.0.39 is now Released.
+# SuperKabuki v.0.0.41 is now Released.
 ![image](https://user-images.githubusercontent.com/52701496/222034768-b8b1b34c-a645-461c-9408-6fffe2d40d63.png)
 
  
 <details> <summary><h1>Fast Start</h1> </summary>
 
 * Install SuperKabuki
 ```js
```

### Comparing `superkabuki-0.0.41/superkabuki.py` & `superkabuki-0.0.43/superkabuki.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 """
 import argparse
 import sys
 from collections import deque
 from functools import partial
 from operator import itemgetter
-from threefive import Stream, Cue, TimeSignal
+from threefive import Stream, Cue, TimeSignal, print2
 from threefive.crc import crc32
 from threefive.bitn import NBin
 from new_reader import reader
 from iframes import IFramer
 
 MAJOR = "0"
 MINOR = "0"
-MAINTAINENCE = "41"
+MAINTAINENCE = "43"
 
 
 def version():
     """
     version prints version as a string
 
     Odd number versions are releases.
@@ -38,21 +38,14 @@
     version_number returns version as an int.
     if version() returns 2.3.01
     version_number will return 2301
     """
     return int(f"{MAJOR}{MINOR}{MAINTAINENCE}")
 
 
-def to_stderr(data):
-    """
-    print to sys.stderr.buffer aka 2
-    """
-    print(data, file=sys.stderr)
-
-
 class SuperKabuki(Stream):
     """
     Super Kabuki - SCTE-35 Packet injection
 
     """
 
     CUEI_DESCRIPTOR = b"\x05\x04CUEI"
@@ -101,16 +94,16 @@
             "--sidecar",
             default="sidecar.txt",
             help=""" Sidecar file for SCTE35 (default sidecar.txt)""",
         )
         parser.add_argument(
             "-p",
             "--scte35_pid",
-            default=0x86,
-            type=int,
+            default="0x86",
+            # type=int,
             help="""Pid for SCTE-35 packets, can be hex or integer. (default 0x86)""",
         )
 
         parser.add_argument(
             "-t",
             "--time_signals",
             action="store_const",
@@ -132,19 +125,25 @@
 
     def _apply_args(self, args):
         if args.scte35_pid and args.input:
             self.outfile = args.output
             self.infile = args.input
             self.sidecar_file = args.sidecar
             self._tsdata = reader(args.input)
-            #self.pid2int(args.scte35_pid)
-            self.scte35_pid = args.scte35_pid
+            self.pid2int(args.scte35_pid)
             self.time_signals = args.time_signals
-        #else:
-         #   sys.exit()
+
+    def pid2int(self, pid):
+        try:
+            self.scte35_pid = int(args.scte35_pid)
+        except:
+            try:
+                self.scte35_pid = int(args.scte35_pid, 16)
+            except:
+                self.scte35_pid = 0x86
 
     def _bump_cc(self):
         self.scte35_cc = (self.scte35_cc + 1) % 16
 
     def _pmt_scte35_stream(self):
         if self.scte35_pid:
             nbin = NBin()
@@ -162,15 +161,15 @@
         """
         encode parses the video input,
         adds the SCTE-35 PID to the PMT,
         parses the sidecar file,
         and injects SCTE-35 Packets,
 
         """
-        to_stderr(f"Writing {self.outfile}")
+        print2(f"Writing {self.outfile}")
         if isinstance(self.outfile, str):
             self.outfile = open(self.outfile, "wb")
         with self.outfile as out_file:
             for pkt in self._find_start():
                 pid = self._parse_info(pkt)
                 if self._pusi_flag(pkt):
                     self._parse_pts(pkt, pid)
@@ -225,15 +224,15 @@
                     if len(line):
                         insert_pts, cue = line.split(",", 1)
                         insert_pts = float(insert_pts)
                         if insert_pts == 0.0:
                             insert_pts = pts
                         if insert_pts >= pts:
                             if [insert_pts, cue] not in self.sidecar:
-                                to_stderr((insert_pts, cue))
+                                print2((insert_pts, cue))
                                 self.sidecar.append([insert_pts, cue])
                                 self.sidecar = deque(
                                     sorted(self.sidecar, key=itemgetter(0))
                                 )
         except:
             pass
 
@@ -269,40 +268,41 @@
         nbin.add_int(self.scte35_cc, 4)  # cont
         nbin.add_bites(b"\x00")
         nbin.add_bites(cue.bites)
         pad_size = 188 - len(nbin.bites)
         padding = b"\xff" * pad_size
         nbin.add_bites(padding)
         self._bump_cc()
-        # to_stderr(nbin.bites)
+        # print2(nbin.bites)
         return nbin.bites
 
     def _program_stream_map(self, pkt, pid):
         pay = self._parse_payload(pkt)
         if pay.startswith(b"\x00\x00\x01\xbc"):
-            to_stderr("psm")
-            to_stderr((pid, pay))
+            print2("psm")
+            print2((pid, pay))
 
-    def _regen_pmt(self, n_seclen, pcr_pid, n_proginfolen, n_info_bites, n_streams):
+    def _regen_pmt(self, pcr_pid, n_info_bites, n_streams):
         nbin = NBin()
         nbin.add_int(2, 8)  # 0x02
         nbin.add_int(1, 1)  # section Syntax indicator
         nbin.add_int(0, 1)  # 0
         nbin.add_int(3, 2)  # reserved
-        nbin.add_int(n_seclen, 12)  # section length
-        nbin.add_int(1, 16)  # program number
-        nbin.add_int(3, 2)  # reserved
-        nbin.add_int(0, 5)  # version
-        nbin.add_int(1, 1)  # current_next_indicator
-        nbin.add_int(0, 8)  # section number
-        nbin.add_int(0, 8)  # last section number
-        nbin.add_int(7, 3)  # res
-        nbin.add_int(pcr_pid, 13)
-        nbin.add_int(15, 4)  # res
-        nbin.add_int(n_proginfolen, 12)
+        seclen = 9 + len(n_info_bites) + len(n_streams) + 4
+        nbin.add_int(seclen, 12)  # section length
+        nbin.add_int(1, 16)  # program number                   16
+        nbin.add_int(3, 2)  # reserved                          18
+        nbin.add_int(0, 5)  # version                           23
+        nbin.add_int(1, 1)  # current_next_indicator            24
+        nbin.add_int(0, 8)  # section number                    32
+        nbin.add_int(0, 8)  # last section number               40
+        nbin.add_int(7, 3)  # res                               43
+        nbin.add_int(pcr_pid, 13)  #                            56
+        nbin.add_int(15, 4)  # res                              60
+        nbin.add_int(len(n_info_bites), 12)  #                  72 bits
         nbin.add_bites(n_info_bites)
         nbin.add_bites(n_streams)
         a_crc = crc32(nbin.bites)
         nbin.add_int(a_crc, 32)
         n_payload = nbin.bites
         pad = 187 - (len(n_payload) + 4)
         pointer_field = b"\x00"
@@ -314,71 +314,68 @@
         """
         parse program maps for streams
         """
         pay = self._chk_partial(pay, pid, self._PMT_TID)
         if not pay:
             return False
         seclen = self._parse_length(pay[1], pay[2])
-        # to_stderr("seclen", seclen)
-        n_seclen = seclen + 6
+        # print2("seclen", seclen)
+        n_seclen = seclen
         if self._section_incomplete(pay, pid, seclen):
             return False
         program_number = self._parse_program(pay[3], pay[4])
-        # to_stderr("program_number", program_number)
+        # print2("program_number", program_number)
         pcr_pid = self._parse_pid(pay[8], pay[9])
-        # to_stderr("pcr_pid", pcr_pid)
+        # print2("pcr_pid", pcr_pid)
         self.pids.pcr.add(pcr_pid)
         self.maps.pid_prgm[pcr_pid] = program_number
         proginfolen = self._parse_length(pay[10], pay[11])
-        # to_stderr("pif", proginfolen)
+        # print2("pif", proginfolen)
         idx = 12
-        n_proginfolen = proginfolen + len(self.CUEI_DESCRIPTOR)
         end = idx + proginfolen
         info_bites = pay[idx:end]
         n_info_bites = info_bites + self.CUEI_DESCRIPTOR
         while idx < end:
             d_type = pay[idx]
             idx += 1
             d_len = pay[idx]
             idx += 1
             d_bytes = pay[idx - 2 : idx + d_len]
             idx += d_len
-            to_stderr(f"type: {d_type} len: { d_len} bytes: {d_bytes}")
-        si_len = seclen - 9
+            print2(f"type: {d_type} len: { d_len} bytes: {d_bytes}")
+        si_len = n_seclen - 9
         si_len -= proginfolen
         streams = self._parse_program_streams(si_len, pay, idx, program_number)
         n_streams = self._pmt_scte35_stream() + streams
-        self._regen_pmt(n_seclen, pcr_pid, n_proginfolen, n_info_bites, n_streams)
+        self._regen_pmt(pcr_pid, n_info_bites, n_streams)
         return True
 
     def _parse_program_streams(self, si_len, pay, idx, program_number):
         """
         parse the elementary streams
         from a program
         """
         # 5 bytes for stream_type info
         chunk_size = 5
         end_idx = (idx + si_len) - 4
         start = idx
         while idx < end_idx:
             stream_type, pid, ei_len = self._parse_stream_type(pay, idx)
-            # to_stderr("Stream: type:", stream_type,"PID:", pid, "EI Len:",ei_len)
+            print2(("Stream: type:", stream_type, "PID:", pid, "EI Len:", ei_len))
             idx += chunk_size
             idx += ei_len
             self.maps.pid_prgm[pid] = program_number
             self._chk_pid_stream_type(pid, stream_type)
-        # crc = pay[idx : idx + 4]
         streams = pay[start:end_idx]
         return streams
 
     def _parse_stream_type(self, pay, idx):
         """
         extract stream pid and type
         """
-        # npay = pay
         stream_type = pay[idx]
         el_pid = self._parse_pid(pay[idx + 1], pay[idx + 2])
         ei_len = self._parse_length(pay[idx + 3], pay[idx + 4])
         return stream_type, el_pid, ei_len
 
     def _chk_pid_stream_type(self, pid, stream_type):
         """
```

