# Comparing `tmp/Pybag-2.2.7.tar.gz` & `tmp/Pybag-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pybag-2.2.7.tar", last modified: Tue Oct 25 01:26:22 2022, max compression
+gzip compressed data, was "Pybag-2.2.8.tar", last modified: Sun May 28 20:21:39 2023, max compression
```

## Comparing `Pybag-2.2.7.tar` & `Pybag-2.2.8.tar`

### file list

```diff
@@ -1,39 +1,59 @@
-drwxrwxrwx   0        0        0        0 2022-10-25 01:26:22.134766 Pybag-2.2.7/
--rw-rw-rw-   0        0        0     1092 2022-10-25 01:25:03.000000 Pybag-2.2.7/LICENSE
--rw-rw-rw-   0        0        0     2843 2022-10-25 01:26:22.134766 Pybag-2.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-25 01:26:22.119144 Pybag-2.2.7/Pybag.egg-info/
--rw-rw-rw-   0        0        0     2843 2022-10-25 01:26:22.000000 Pybag-2.2.7/Pybag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2022-10-25 01:26:22.000000 Pybag-2.2.7/Pybag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-25 01:26:22.000000 Pybag-2.2.7/Pybag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2022-10-25 01:26:22.000000 Pybag-2.2.7/Pybag.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-10-25 01:26:22.000000 Pybag-2.2.7/Pybag.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2043 2022-10-25 01:25:03.000000 Pybag-2.2.7/README.md
-drwxrwxrwx   0        0        0        0 2022-10-25 01:26:22.119144 Pybag-2.2.7/pybag/
--rw-rw-rw-   0        0        0     1183 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/__init__.py
--rw-rw-rw-   0        0        0      245 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/crashdbg.py
-drwxrwxrwx   0        0        0        0 2022-10-25 01:26:22.119144 Pybag-2.2.7/pybag/dbgeng/
--rw-rw-rw-   0        0        0        0 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/__init__.py
--rw-rw-rw-   0        0        0     4420 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/breakpoints.py
--rw-rw-rw-   0        0        0    18336 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/callbacks.py
--rw-rw-rw-   0        0        0     1984 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/core.py
--rw-rw-rw-   0        0        0     2173 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/dbgengstructs.py
--rw-rw-rw-   0        0        0     2144 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/exception.py
--rw-rw-rw-   0        0        0     3923 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/idebugadvanced.py
--rw-rw-rw-   0        0        0     4408 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/idebugbreakpoint.py
--rw-rw-rw-   0        0        0    16988 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/idebugclient.py
--rw-rw-rw-   0        0        0    23790 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/idebugcontrol.py
--rw-rw-rw-   0        0        0     5608 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/idebugdataspaces.py
--rw-rw-rw-   0        0        0     3980 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/idebugregisters.py
--rw-rw-rw-   0        0        0    16070 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/idebugsymbols.py
--rw-rw-rw-   0        0        0     6477 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/idebugsystemobjects.py
--rw-rw-rw-   0        0        0     7501 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/modules.py
--rw-rw-rw-   0        0        0   244089 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/pefile2.py
--rw-rw-rw-   0        0        0     3772 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/registers.py
-drwxrwxrwx   0        0        0        0 2022-10-25 01:26:22.119144 Pybag-2.2.7/pybag/dbgeng/tlb/
--rw-rw-rw-   0        0        0   401520 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/tlb/dbgeng.tlb
--rw-rw-rw-   0        0        0     3470 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/dbgeng/util.py
--rw-rw-rw-   0        0        0      736 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/kerneldbg.py
--rw-rw-rw-   0        0        0    24305 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/pydbg.py
--rw-rw-rw-   0        0        0     3006 2022-10-25 01:25:03.000000 Pybag-2.2.7/pybag/userdbg.py
--rw-rw-rw-   0        0        0       42 2022-10-25 01:26:22.134766 Pybag-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1303 2022-10-25 01:25:03.000000 Pybag-2.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:21:39.562283 Pybag-2.2.8/
+-rw-rw-rw-   0        0        0     1092 2023-05-28 20:20:27.000000 Pybag-2.2.8/LICENSE
+-rw-rw-rw-   0        0        0     2891 2023-05-28 20:21:39.562283 Pybag-2.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 20:21:39.531042 Pybag-2.2.8/Pybag.egg-info/
+-rw-rw-rw-   0        0        0     2891 2023-05-28 20:21:39.000000 Pybag-2.2.8/Pybag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1326 2023-05-28 20:21:39.000000 Pybag-2.2.8/Pybag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 20:21:39.000000 Pybag-2.2.8/Pybag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-28 20:21:39.000000 Pybag-2.2.8/Pybag.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 20:21:39.000000 Pybag-2.2.8/Pybag.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2091 2023-05-28 20:20:27.000000 Pybag-2.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 20:21:39.531042 Pybag-2.2.8/pybag/
+-rw-rw-rw-   0        0        0     1183 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/__init__.py
+-rw-rw-rw-   0        0        0      245 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/crashdbg.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:21:39.546657 Pybag-2.2.8/pybag/dbgeng/
+-rw-rw-rw-   0        0        0        0 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/__init__.py
+-rw-rw-rw-   0        0        0     4420 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/breakpoints.py
+-rw-rw-rw-   0        0        0    18336 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/callbacks.py
+-rw-rw-rw-   0        0        0     1984 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/core.py
+-rw-rw-rw-   0        0        0     2173 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/dbgengstructs.py
+-rw-rw-rw-   0        0        0     2144 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/exception.py
+-rw-rw-rw-   0        0        0     3923 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/idebugadvanced.py
+-rw-rw-rw-   0        0        0     4408 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/idebugbreakpoint.py
+-rw-rw-rw-   0        0        0    16988 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/idebugclient.py
+-rw-rw-rw-   0        0        0    23790 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/idebugcontrol.py
+-rw-rw-rw-   0        0        0     5608 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/idebugdataspaces.py
+-rw-rw-rw-   0        0        0     3980 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/idebugregisters.py
+-rw-rw-rw-   0        0        0    16070 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/idebugsymbols.py
+-rw-rw-rw-   0        0        0     6477 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/idebugsystemobjects.py
+-rw-rw-rw-   0        0        0     7501 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/modules.py
+-rw-rw-rw-   0        0        0   244089 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/pefile2.py
+-rw-rw-rw-   0        0        0     3772 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/registers.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:21:39.546657 Pybag-2.2.8/pybag/dbgeng/tlb/
+-rw-rw-rw-   0        0        0   401520 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/tlb/dbgeng.tlb
+-rw-rw-rw-   0        0        0     3470 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/util.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:21:39.562283 Pybag-2.2.8/pybag/dbgeng/win32/
+-rw-rw-rw-   0        0        0     8352 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/__init__.py
+-rw-rw-rw-   0        0        0   126301 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/advapi32.py
+-rw-rw-rw-   0        0        0    25810 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/context_amd64.py
+-rw-rw-rw-   0        0        0    16442 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/context_i386.py
+-rw-rw-rw-   0        0        0    47999 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/dbghelp.py
+-rw-rw-rw-   0        0        0    24251 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/defines.py
+-rw-rw-rw-   0        0        0    12625 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/gdi32.py
+-rw-rw-rw-   0        0        0   169784 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/kernel32.py
+-rw-rw-rw-   0        0        0    23339 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/ntdll.py
+-rw-rw-rw-   0        0        0   162625 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/peb_teb.py
+-rw-rw-rw-   0        0        0    14098 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/psapi.py
+-rw-rw-rw-   0        0        0    15167 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/shell32.py
+-rw-rw-rw-   0        0        0    26526 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/shlwapi.py
+-rw-rw-rw-   0        0        0    59574 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/user32.py
+-rw-rw-rw-   0        0        0    47136 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/version.py
+-rw-rw-rw-   0        0        0    11462 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/dbgeng/win32/wtsapi32.py
+-rw-rw-rw-   0        0        0      736 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/kerneldbg.py
+-rw-rw-rw-   0        0        0    24305 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/pydbg.py
+-rw-rw-rw-   0        0        0     3006 2023-05-28 20:20:27.000000 Pybag-2.2.8/pybag/userdbg.py
+-rw-rw-rw-   0        0        0       42 2023-05-28 20:21:39.562283 Pybag-2.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2023-05-28 20:20:27.000000 Pybag-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:21:39.562283 Pybag-2.2.8/tests/
+-rw-rw-rw-   0        0        0      472 2023-05-28 20:20:27.000000 Pybag-2.2.8/tests/test_idebugclient.py
+-rw-rw-rw-   0        0        0     3421 2023-05-28 20:20:27.000000 Pybag-2.2.8/tests/test_target.py
```

### Comparing `Pybag-2.2.7/LICENSE` & `Pybag-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/PKG-INFO` & `Pybag-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pybag
-Version: 2.2.7
+Version: 2.2.8
 Summary: Python wrappers for DbgEng from Windbg
 Home-page: https://github.com/dshikashio/Pybag
 Author: Doug S
 License: MIT
 Keywords: windows,debugging,dbgeng,windbg,reverseengineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -72,14 +72,16 @@
 
 k = KernelDbg()
 k.attach("net:port=50000,key=1.2.3.4")
 ```
 
 
 ## Release History
+* 2.2.8
+  * Fixed missing files install issue
 * 2.2.7
   * Fixed access violation when using oneshot breakpoints
   * Added 'count' option to breakpoints
 * 2.2.6
   * Added support for more dbgeng calls
     * Symbol handling
     * Set / get thread contexts
```

### Comparing `Pybag-2.2.7/Pybag.egg-info/PKG-INFO` & `Pybag-2.2.8/Pybag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pybag
-Version: 2.2.7
+Version: 2.2.8
 Summary: Python wrappers for DbgEng from Windbg
 Home-page: https://github.com/dshikashio/Pybag
 Author: Doug S
 License: MIT
 Keywords: windows,debugging,dbgeng,windbg,reverseengineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -72,14 +72,16 @@
 
 k = KernelDbg()
 k.attach("net:port=50000,key=1.2.3.4")
 ```
 
 
 ## Release History
+* 2.2.8
+  * Fixed missing files install issue
 * 2.2.7
   * Fixed access violation when using oneshot breakpoints
   * Added 'count' option to breakpoints
 * 2.2.6
   * Added support for more dbgeng calls
     * Symbol handling
     * Set / get thread contexts
```

### Comparing `Pybag-2.2.7/README.md` & `Pybag-2.2.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 
 k = KernelDbg()
 k.attach("net:port=50000,key=1.2.3.4")
 ```
 
 
 ## Release History
+* 2.2.8
+  * Fixed missing files install issue
 * 2.2.7
   * Fixed access violation when using oneshot breakpoints
   * Added 'count' option to breakpoints
 * 2.2.6
   * Added support for more dbgeng calls
     * Symbol handling
     * Set / get thread contexts
```

### Comparing `Pybag-2.2.7/pybag/__init__.py` & `Pybag-2.2.8/pybag/__init__.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/breakpoints.py` & `Pybag-2.2.8/pybag/dbgeng/breakpoints.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/callbacks.py` & `Pybag-2.2.8/pybag/dbgeng/callbacks.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/core.py` & `Pybag-2.2.8/pybag/dbgeng/core.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/dbgengstructs.py` & `Pybag-2.2.8/pybag/dbgeng/dbgengstructs.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/exception.py` & `Pybag-2.2.8/pybag/dbgeng/exception.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/idebugadvanced.py` & `Pybag-2.2.8/pybag/dbgeng/idebugadvanced.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/idebugbreakpoint.py` & `Pybag-2.2.8/pybag/dbgeng/idebugbreakpoint.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/idebugclient.py` & `Pybag-2.2.8/pybag/dbgeng/idebugclient.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/idebugcontrol.py` & `Pybag-2.2.8/pybag/dbgeng/idebugcontrol.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/idebugdataspaces.py` & `Pybag-2.2.8/pybag/dbgeng/idebugdataspaces.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/idebugregisters.py` & `Pybag-2.2.8/pybag/dbgeng/idebugregisters.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/idebugsymbols.py` & `Pybag-2.2.8/pybag/dbgeng/idebugsymbols.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/idebugsystemobjects.py` & `Pybag-2.2.8/pybag/dbgeng/idebugsystemobjects.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/modules.py` & `Pybag-2.2.8/pybag/dbgeng/modules.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/pefile2.py` & `Pybag-2.2.8/pybag/dbgeng/pefile2.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/registers.py` & `Pybag-2.2.8/pybag/dbgeng/registers.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/tlb/dbgeng.tlb` & `Pybag-2.2.8/pybag/dbgeng/tlb/dbgeng.tlb`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/dbgeng/util.py` & `Pybag-2.2.8/pybag/dbgeng/util.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/kerneldbg.py` & `Pybag-2.2.8/pybag/kerneldbg.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/pydbg.py` & `Pybag-2.2.8/pybag/pydbg.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/pybag/userdbg.py` & `Pybag-2.2.8/pybag/userdbg.py`

 * *Files identical despite different names*

### Comparing `Pybag-2.2.7/setup.py` & `Pybag-2.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(name='Pybag',
-      version='2.2.7',
+      version='2.2.8',
       description='Python wrappers for DbgEng from Windbg',
       long_description=README,
       long_description_content_type="text/markdown",
       author='Doug S',
       url='https://github.com/dshikashio/Pybag',
       license="MIT",
       keywords=['windows', 'debugging', 'dbgeng', 'windbg', 'reverseengineering'],
@@ -21,15 +21,15 @@
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'Natural Language :: English',
           'Operating System :: Microsoft :: Windows',
           'Programming Language :: Python',
           'Topic :: Software Development :: Libraries :: Python Modules',
       ],
-      packages=['pybag', 'pybag.dbgeng'],
+      packages=['pybag', 'pybag.dbgeng', 'pybag.dbgeng.win32'],
       package_data={'pybag': ['dbgeng/tlb/*.tlb']},
       include_package_data=True,
       install_requires=[
           'capstone>=4.0.2',
           'comtypes>=1.1.14',
           'pywin32>=301',
       ],
```

