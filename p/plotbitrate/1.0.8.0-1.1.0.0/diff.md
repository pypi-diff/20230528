# Comparing `tmp/plotbitrate-1.0.8.0-py3-none-any.whl.zip` & `tmp/plotbitrate-1.1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11594 bytes, number of entries: 10
--rw-r--r--  2.0 unx    22646 b- defN 21-Jul-24 19:48 plotbitrate.py
+Zip file size: 11621 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    22701 b- defN 23-May-28 03:53 plotbitrate.py
 -rw-r--r--  2.0 unx      323 b- defN 21-Apr-04 22:56 frame/__init__.py
 -rw-r--r--  2.0 unx      231 b- defN 21-Apr-04 22:56 frame/_frame_class.py
 -rw-r--r--  2.0 unx      252 b- defN 21-Apr-04 22:56 frame/_frame_dataclass.py
--rw-r--r--  2.0 unx     1364 b- defN 21-Jul-24 19:54 plotbitrate-1.0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2975 b- defN 21-Jul-24 19:54 plotbitrate-1.0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-24 19:54 plotbitrate-1.0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 21-Jul-24 19:54 plotbitrate-1.0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 21-Jul-24 19:54 plotbitrate-1.0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      820 b- defN 21-Jul-24 19:54 plotbitrate-1.0.8.0.dist-info/RECORD
-10 files, 28771 bytes uncompressed, 10188 bytes compressed:  64.6%
+-rw-r--r--  2.0 unx     1364 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2992 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 23-May-28 04:03 plotbitrate-1.1.0.0.dist-info/RECORD
+10 files, 28842 bytes uncompressed, 10215 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: frame/_frame_class.py
 Comment: 
 
 Filename: frame/_frame_dataclass.py
 Comment: 
 
-Filename: plotbitrate-1.0.8.0.dist-info/LICENSE
+Filename: plotbitrate-1.1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: plotbitrate-1.0.8.0.dist-info/METADATA
+Filename: plotbitrate-1.1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: plotbitrate-1.0.8.0.dist-info/WHEEL
+Filename: plotbitrate-1.1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: plotbitrate-1.0.8.0.dist-info/entry_points.txt
+Filename: plotbitrate-1.1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: plotbitrate-1.0.8.0.dist-info/top_level.txt
+Filename: plotbitrate-1.1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: plotbitrate-1.0.8.0.dist-info/RECORD
+Filename: plotbitrate-1.1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plotbitrate.py

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 #
 # FFProbe Bitrate Graph
 #
-# Original work Copyright (c) 2013-2021, Eric Work
+# Original work Copyright (c) 2013-2023, Eric Work
 # Modified work Copyright (c) 2019-2021, Steve Schmidt
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 #   Redistributions of source code must retain the above copyright notice,
@@ -25,15 +25,15 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = "1.0.8.0"
+__version__ = "1.1.0.0"
 
 import argparse
 import csv
 import datetime
 import math
 import multiprocessing
 import platform
@@ -80,17 +80,17 @@
 
 # prefer C-based ElementTree
 try:
     import xml.etree.cElementTree as eTree
 except ImportError:
     import xml.etree.ElementTree as eTree  # type: ignore
 
-# check for PyQt5
-if util.find_spec("PyQt5") is None:
-    exit_with_error("Missing package 'PyQt5'")
+# check for PyQt5 or PyQt6
+if util.find_spec("PyQt6") is None and util.find_spec("PyQt5") is None:
+    exit_with_error("Missing package 'PyQt5' or 'PyQt6'")
 
 # check for matplot lib
 try:
     import matplotlib  # type: ignore
     import matplotlib.pyplot as matplot  # type: ignore
 except ImportError as err:
     # satisfy undefined variable warnings
@@ -622,15 +622,15 @@
     # check if an output is requested, otherwise try to initialize backend, and exit if it fails
     if not args.output:
         # init backend
         try:
             if is_wsl():
                 backend = "TkAgg"
             else:
-                backend = "Qt5Agg"
+                backend = "QtAgg"
             matplotlib.use(backend)
         except ImportError as err:
             exit_with_error(err.msg)
 
     # if the output is raw xml, just call the function and exit
     if args.format == "xml_raw":
         save_raw_xml(
```

## Comparing `plotbitrate-1.0.8.0.dist-info/LICENSE` & `plotbitrate-1.1.0.0.dist-info/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Original work Copyright (c) 2013-2021, Eric Work
+Original work Copyright (c) 2013-2023, Eric Work
 Modified work Copyright (c) 2019-2021, Steve Schmidt
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
```

## Comparing `plotbitrate-1.0.8.0.dist-info/METADATA` & `plotbitrate-1.1.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: plotbitrate
-Version: 1.0.8.0
+Version: 1.1.0.0
 Summary: A simple bitrate plotter for media files
 Home-page: https://github.com/zeroepoch/plotbitrate
 Author: Eric Work
 Author-email: work.eric@gmail.com
 License: BSD
 Keywords: ffprobe bitrate plot
-Platform: UNKNOWN
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.5
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: matplotlib
-Requires-Dist: pyqt5
+Requires-Dist: pyqt6
 
 PlotBitrate
 ===========
 
 FFProbe Bitrate Graph
 
 This project contains a script for plotting the bitrate of an audio or video
@@ -30,17 +30,18 @@
 
 Possible outputs are:
 * Image types (png, svg, pdf, ...)
 * Raw frame data (csv, xml)
 
 Requirements:
 
-* Python >= 3.5
-* FFMpeg >= 1.2 with the ffprobe command
+* Python >= 3.6
+* FFmpeg >= 1.2 with the ffprobe command
 * Matplotlib
+* PyQt5 or PyQt6
 
 For using the script from source, install the requirements with
 `pip install -r requirements.txt` or use the `requirements-dev.txt`
 for development purposes.
 
 Installation
 ------------
@@ -105,9 +106,7 @@
 ```
 
 Show bitrate graph from raw xml.
 
 ```
 plotbitrate frames.xml
 ```
-
-
```

## Comparing `plotbitrate-1.0.8.0.dist-info/RECORD` & `plotbitrate-1.1.0.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-plotbitrate.py,sha256=e_s-8mYhCGPuYbx0yJhcsSTe2E0fNk0a50jWh7fRI74,22646
+plotbitrate.py,sha256=iUQkJWY6u8PhoDTT1RBy_hIx6u0QSBliiPF3XvVj8fQ,22701
 frame/__init__.py,sha256=lreLJjeFT9pLvyyf2stOlYFdyFzQRyhwKan6l3GIk8s,323
 frame/_frame_class.py,sha256=13_0I0ppVdU8CwzuawmEWlHdYbLONKAQULdaeYzrPOY,231
 frame/_frame_dataclass.py,sha256=-e_aeJVO6tMx64o0tYFodaT3iHtlrh715RIHv-PLfSE,252
-plotbitrate-1.0.8.0.dist-info/LICENSE,sha256=M--7FULwvASKnc8iawLHqBHxgejPj9pgE9PC1E4zuSc,1364
-plotbitrate-1.0.8.0.dist-info/METADATA,sha256=hJWTsF3BuNwTWKODFppz6RZ1WvIGnsikfy9w8Ne3i_E,2975
-plotbitrate-1.0.8.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-plotbitrate-1.0.8.0.dist-info/entry_points.txt,sha256=UZFyEAoODzZEh_0Y29aBcxi4lOM-gVqZgRV4nEnmS74,50
-plotbitrate-1.0.8.0.dist-info/top_level.txt,sha256=JeWBr1OWk8x_JVHfQRr10u6A3R8vLaV9XT6iEs1RzKU,18
-plotbitrate-1.0.8.0.dist-info/RECORD,,
+plotbitrate-1.1.0.0.dist-info/LICENSE,sha256=TbeSqT2UnRfLzmdFG7iGXZMBzRQB1cfzFyJPq6E8qG4,1364
+plotbitrate-1.1.0.0.dist-info/METADATA,sha256=b1jMfQ13d4ZyXp0WGyA-VWLuI4vHv5G44SgQRgoF3Ik,2992
+plotbitrate-1.1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+plotbitrate-1.1.0.0.dist-info/entry_points.txt,sha256=DCDetfld1tV6cn8F2n8ZJJrGvq-RUtlR-a4Bqi1B2tA,49
+plotbitrate-1.1.0.0.dist-info/top_level.txt,sha256=JeWBr1OWk8x_JVHfQRr10u6A3R8vLaV9XT6iEs1RzKU,18
+plotbitrate-1.1.0.0.dist-info/RECORD,,
```

