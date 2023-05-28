# Comparing `tmp/pyaodbc-0.1.9a1.tar.gz` & `tmp/pyaodbc-0.1.9a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyaodbc-0.1.9a1.tar", last modified: Sun May 28 16:42:15 2023, max compression
+gzip compressed data, was "dist\pyaodbc-0.1.9a3.tar", last modified: Sun May 28 16:59:55 2023, max compression
```

## Comparing `pyaodbc-0.1.9a1.tar` & `pyaodbc-0.1.9a3.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 16:42:15.883761 pyaodbc-0.1.9a1/
--rw-rw-rw-   0        0        0    11558 2023-05-28 15:33:53.000000 pyaodbc-0.1.9a1/LICENSE
--rw-rw-rw-   0        0        0     3332 2023-05-28 16:42:15.883761 pyaodbc-0.1.9a1/PKG-INFO
--rw-rw-rw-   0        0        0     2327 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 16:42:15.783332 pyaodbc-0.1.9a1/pyaodbc.egg-info/
--rw-rw-rw-   0        0        0     3332 2023-05-28 16:42:15.000000 pyaodbc-0.1.9a1/pyaodbc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-05-28 16:42:15.000000 pyaodbc-0.1.9a1/pyaodbc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 16:42:15.000000 pyaodbc-0.1.9a1/pyaodbc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 16:42:15.000000 pyaodbc-0.1.9a1/pyaodbc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 16:42:15.883761 pyaodbc-0.1.9a1/setup.cfg
--rw-rw-rw-   0        0        0     3526 2023-05-28 16:42:10.000000 pyaodbc-0.1.9a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 16:42:15.868170 pyaodbc-0.1.9a1/src/
--rw-rw-rw-   0        0        0    12560 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/src/connection.c
--rw-rw-rw-   0        0        0    17962 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/src/cursor.c
--rw-rw-rw-   0        0        0    18076 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/src/get_data.c
--rw-rw-rw-   0        0        0     8372 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/src/input_data.c
--rw-rw-rw-   0        0        0     1520 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/src/linux.c
--rw-rw-rw-   0        0        0     7512 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/src/module.c
--rw-rw-rw-   0        0        0     2226 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/src/pyaodbc.pyi
-drwxrwxrwx   0        0        0        0 2023-05-28 16:42:15.868170 pyaodbc-0.1.9a1/tests/
--rw-rw-rw-   0        0        0    18605 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a1/tests/test_mssql.py
+drwxrwxrwx   0        0        0        0 2023-05-28 16:59:55.748813 pyaodbc-0.1.9a3/
+-rw-rw-rw-   0        0        0    11558 2023-05-28 15:33:53.000000 pyaodbc-0.1.9a3/LICENSE
+-rw-rw-rw-   0        0        0     3332 2023-05-28 16:59:55.748813 pyaodbc-0.1.9a3/PKG-INFO
+-rw-rw-rw-   0        0        0     2327 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 16:59:55.701952 pyaodbc-0.1.9a3/pyaodbc.egg-info/
+-rw-rw-rw-   0        0        0     3332 2023-05-28 16:59:55.000000 pyaodbc-0.1.9a3/pyaodbc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-05-28 16:59:55.000000 pyaodbc-0.1.9a3/pyaodbc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 16:59:55.000000 pyaodbc-0.1.9a3/pyaodbc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 16:59:55.000000 pyaodbc-0.1.9a3/pyaodbc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 16:59:55.748813 pyaodbc-0.1.9a3/setup.cfg
+-rw-rw-rw-   0        0        0     3395 2023-05-28 16:58:15.000000 pyaodbc-0.1.9a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 16:59:55.733198 pyaodbc-0.1.9a3/src/
+-rw-rw-rw-   0        0        0     1707 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/aodbc_types.h
+-rw-rw-rw-   0        0        0    12560 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/connection.c
+-rw-rw-rw-   0        0        0      704 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/connection.h
+-rw-rw-rw-   0        0        0    17962 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/cursor.c
+-rw-rw-rw-   0        0        0     1021 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/cursor.h
+-rw-rw-rw-   0        0        0    18076 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/get_data.c
+-rw-rw-rw-   0        0        0     1138 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/get_data.h
+-rw-rw-rw-   0        0        0      816 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/headers.h
+-rw-rw-rw-   0        0        0     8372 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/input_data.c
+-rw-rw-rw-   0        0        0     1178 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/input_data.h
+-rw-rw-rw-   0        0        0     1520 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/linux.c
+-rw-rw-rw-   0        0        0      678 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/linux.h
+-rw-rw-rw-   0        0        0     7512 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/module.c
+-rw-rw-rw-   0        0        0      427 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/module.h
+-rw-rw-rw-   0        0        0     2226 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/src/pyaodbc.pyi
+drwxrwxrwx   0        0        0        0 2023-05-28 16:59:55.733198 pyaodbc-0.1.9a3/tests/
+-rw-rw-rw-   0        0        0    18605 2023-05-28 15:43:10.000000 pyaodbc-0.1.9a3/tests/test_mssql.py
```

### Comparing `pyaodbc-0.1.9a1/LICENSE` & `pyaodbc-0.1.9a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/PKG-INFO` & `pyaodbc-0.1.9a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaodbc
-Version: 0.1.9a1
+Version: 0.1.9a3
 Summary: Library for asynchronous connection and execution of queries to the database via ODBC driver
 Home-page: https://github.com/SergioMorelo/pyaodbc
 Download-URL: https://pypi.org/project/pyaodbc/
 Author: Sergio Morello
 Author-email: mail.Krik@gmail.com
 Maintainer: Sergio Morello
 Maintainer-email: mail.Krik@gmail.com
```

### Comparing `pyaodbc-0.1.9a1/README.md` & `pyaodbc-0.1.9a3/README.md`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/pyaodbc.egg-info/PKG-INFO` & `pyaodbc-0.1.9a3/pyaodbc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaodbc
-Version: 0.1.9a1
+Version: 0.1.9a3
 Summary: Library for asynchronous connection and execution of queries to the database via ODBC driver
 Home-page: https://github.com/SergioMorelo/pyaodbc
 Download-URL: https://pypi.org/project/pyaodbc/
 Author: Sergio Morello
 Author-email: mail.Krik@gmail.com
 Maintainer: Sergio Morello
 Maintainer-email: mail.Krik@gmail.com
```

### Comparing `pyaodbc-0.1.9a1/setup.py` & `pyaodbc-0.1.9a3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import sys
 
 from setuptools import setup, Extension
 
 
 LIBRARY_NAME = 'pyaodbc'
-VERSION = '0.1.9a1'
+VERSION = '0.1.9a3'
 
 
 def uninstall_pyaodbc():
     print('***** start uninstall pyaodbc *****')
     subprocess.check_call([sys.executable, '-m', 'pip', 'uninstall', '-y', LIBRARY_NAME])
     print('***** finish uninstall pyaodbc *****')
 
@@ -46,31 +46,29 @@
     libraries = []
 
     if platform == 'win32':
         libraries.append('odbc32')
     elif platform == 'linux':
         libraries.append('odbc')
 
-    headers = [os.path.relpath(os.path.join('src', file)) for file in os.listdir('src') if file.endswith('.h')]
     sources = [os.path.relpath(os.path.join('src', file)) for file in os.listdir('src') if file.endswith('.c')]
 
     if not libraries:
         raise SystemError('Unsupported platform!')
 
     modules = [Extension(
         name=LIBRARY_NAME,
-        headers=headers,
         sources=sources,
         libraries=libraries
     )]
 
     data_files = [('', [
         os.path.relpath(os.path.join('src', file))
         for file in os.listdir('src')
-        if file.endswith('.pyi')
+        if file.endswith(('.h', '.pyi'))
     ])]
 
     if dev:
         uninstall_pyaodbc()
         remove_tmp_directories()
 
     with open('README.md') as readme_file:
```

### Comparing `pyaodbc-0.1.9a1/src/connection.c` & `pyaodbc-0.1.9a3/src/connection.c`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/src/cursor.c` & `pyaodbc-0.1.9a3/src/cursor.c`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/src/get_data.c` & `pyaodbc-0.1.9a3/src/get_data.c`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/src/input_data.c` & `pyaodbc-0.1.9a3/src/input_data.c`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/src/linux.c` & `pyaodbc-0.1.9a3/src/linux.c`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/src/module.c` & `pyaodbc-0.1.9a3/src/module.c`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/src/pyaodbc.pyi` & `pyaodbc-0.1.9a3/src/pyaodbc.pyi`

 * *Files identical despite different names*

### Comparing `pyaodbc-0.1.9a1/tests/test_mssql.py` & `pyaodbc-0.1.9a3/tests/test_mssql.py`

 * *Files identical despite different names*

