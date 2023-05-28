# Comparing `tmp/passgeneration-0.0.1.tar.gz` & `tmp/passgeneration-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passgeneration-0.0.1.tar", last modified: Sun May 28 04:36:27 2023, max compression
+gzip compressed data, was "passgeneration-0.0.2.tar", last modified: Sun May 28 04:39:58 2023, max compression
```

## Comparing `passgeneration-0.0.1.tar` & `passgeneration-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 04:36:27.443629 passgeneration-0.0.1/
--rw-rw-rw-   0        0        0     1081 2023-05-28 04:22:02.000000 passgeneration-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      847 2023-05-28 04:36:27.443629 passgeneration-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-28 04:35:02.000000 passgeneration-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 04:36:27.415286 passgeneration-0.0.1/passgeneration/
--rw-rw-rw-   0        0        0       30 2023-05-28 03:38:18.000000 passgeneration-0.0.1/passgeneration/__init__.py
--rw-rw-rw-   0        0        0      728 2023-05-28 03:38:53.000000 passgeneration-0.0.1/passgeneration/generate.py
-drwxrwxrwx   0        0        0        0 2023-05-28 04:36:27.442624 passgeneration-0.0.1/passgeneration.egg-info/
--rw-rw-rw-   0        0        0      847 2023-05-28 04:36:27.000000 passgeneration-0.0.1/passgeneration.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-28 04:36:27.000000 passgeneration-0.0.1/passgeneration.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 04:36:27.000000 passgeneration-0.0.1/passgeneration.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-28 04:36:27.000000 passgeneration-0.0.1/passgeneration.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 04:36:27.443629 passgeneration-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-28 04:36:06.000000 passgeneration-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 04:39:58.594883 passgeneration-0.0.2/
+-rw-rw-rw-   0        0        0     1081 2023-05-28 04:22:02.000000 passgeneration-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      847 2023-05-28 04:39:58.594883 passgeneration-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-28 04:35:02.000000 passgeneration-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 04:39:58.576856 passgeneration-0.0.2/passgeneration/
+-rw-rw-rw-   0        0        0       30 2023-05-28 03:38:18.000000 passgeneration-0.0.2/passgeneration/__init__.py
+-rw-rw-rw-   0        0        0      742 2023-05-28 04:39:13.000000 passgeneration-0.0.2/passgeneration/generate.py
+drwxrwxrwx   0        0        0        0 2023-05-28 04:39:58.593883 passgeneration-0.0.2/passgeneration.egg-info/
+-rw-rw-rw-   0        0        0      847 2023-05-28 04:39:58.000000 passgeneration-0.0.2/passgeneration.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-28 04:39:58.000000 passgeneration-0.0.2/passgeneration.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 04:39:58.000000 passgeneration-0.0.2/passgeneration.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-28 04:39:58.000000 passgeneration-0.0.2/passgeneration.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 04:39:58.595884 passgeneration-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-28 04:39:19.000000 passgeneration-0.0.2/setup.py
```

### Comparing `passgeneration-0.0.1/LICENSE` & `passgeneration-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `passgeneration-0.0.1/PKG-INFO` & `passgeneration-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passgeneration
-Version: 0.0.1
+Version: 0.0.2
 Summary: Password Generating Library. Fixed Name Version
 Home-page: https://github.com/Aroko001/PassGeneration-py
 Author: aroko900
 Author-email: aro0ko1@xmailer.be
 License: MIT
 Keywords: password generator,password
 Classifier: Programming Language :: Python
```

### Comparing `passgeneration-0.0.1/passgeneration/generate.py` & `passgeneration-0.0.2/passgeneration/generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,11 +18,11 @@
     if numbers:
         alphabet += number_chars
     if special:
         alphabet += special_chars
     
     if length == 8:
         password = ''.join(random.choice(alphabet) for i in range(8))
-        return password
+        return print(password)
     else:
         password = ''.join(random.choice(alphabet) for i in range(length))
-        return password
+        return print(password)
```

### Comparing `passgeneration-0.0.1/passgeneration.egg-info/PKG-INFO` & `passgeneration-0.0.2/passgeneration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passgeneration
-Version: 0.0.1
+Version: 0.0.2
 Summary: Password Generating Library. Fixed Name Version
 Home-page: https://github.com/Aroko001/PassGeneration-py
 Author: aroko900
 Author-email: aro0ko1@xmailer.be
 License: MIT
 Keywords: password generator,password
 Classifier: Programming Language :: Python
```

### Comparing `passgeneration-0.0.1/setup.py` & `passgeneration-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='passgeneration',
-    version='0.0.1',
+    version='0.0.2',
     description='Password Generating Library. Fixed Name Version',
     author='aroko900',
     author_email='aro0ko1@xmailer.be',
     license='MIT',
     keywords = ['password generator', 'password'],
     packages=["passgeneration"],
     url="https://github.com/Aroko001/PassGeneration-py",
```

