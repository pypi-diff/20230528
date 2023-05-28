# Comparing `tmp/pygamal-1.0.2.tar.gz` & `tmp/pygamal-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygamal-1.0.2.tar", last modified: Sun May 28 00:01:23 2023, max compression
+gzip compressed data, was "pygamal-1.0.4.tar", last modified: Sun May 28 00:04:30 2023, max compression
```

## Comparing `pygamal-1.0.2.tar` & `pygamal-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:01:23.644142 pygamal-1.0.2/
--rw-rw-rw-   0        0        0      861 2023-05-28 00:01:23.642880 pygamal-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 00:01:23.623840 pygamal-1.0.2/pygamal/
--rw-rw-rw-   0        0        0       38 2023-05-28 00:00:42.000000 pygamal-1.0.2/pygamal/__init__.py
--rw-rw-rw-   0        0        0     4308 2023-05-27 23:24:32.000000 pygamal-1.0.2/pygamal/el_gamal_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:01:23.641395 pygamal-1.0.2/pygamal.egg-info/
--rw-rw-rw-   0        0        0      861 2023-05-28 00:01:23.000000 pygamal-1.0.2/pygamal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-28 00:01:23.000000 pygamal-1.0.2/pygamal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:01:23.000000 pygamal-1.0.2/pygamal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-28 00:01:23.000000 pygamal-1.0.2/pygamal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 00:01:23.000000 pygamal-1.0.2/pygamal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 00:01:23.644142 pygamal-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1126 2023-05-28 00:01:15.000000 pygamal-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:04:30.182495 pygamal-1.0.4/
+-rw-rw-rw-   0        0        0      861 2023-05-28 00:04:30.182495 pygamal-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 00:04:30.161890 pygamal-1.0.4/pygamal/
+-rw-rw-rw-   0        0        0       75 2023-05-28 00:03:57.000000 pygamal-1.0.4/pygamal/__init__.py
+-rw-rw-rw-   0        0        0     4308 2023-05-27 23:24:32.000000 pygamal-1.0.4/pygamal/pygamal.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:04:30.180396 pygamal-1.0.4/pygamal.egg-info/
+-rw-rw-rw-   0        0        0      861 2023-05-28 00:04:29.000000 pygamal-1.0.4/pygamal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-28 00:04:30.000000 pygamal-1.0.4/pygamal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 00:04:29.000000 pygamal-1.0.4/pygamal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-28 00:04:29.000000 pygamal-1.0.4/pygamal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 00:04:29.000000 pygamal-1.0.4/pygamal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 00:04:30.182495 pygamal-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-05-28 00:04:18.000000 pygamal-1.0.4/setup.py
```

### Comparing `pygamal-1.0.2/PKG-INFO` & `pygamal-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 1.0.2
+Version: 1.0.4
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pygamal-1.0.2/pygamal/el_gamal_wrapper.py` & `pygamal-1.0.4/pygamal/pygamal.py`

 * *Files identical despite different names*

### Comparing `pygamal-1.0.2/pygamal.egg-info/PKG-INFO` & `pygamal-1.0.4/pygamal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 1.0.2
+Version: 1.0.4
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pygamal-1.0.2/setup.py` & `pygamal-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 This module have been made for the project of discret math CSC281 at ksu university.
 The project supervisor is Aqil Alazimi. LinkedIn: https://www.linkedin.com/in/aqil-azmi-20903960/
 The project repo is: https://github.com/Wouze/csc281-project
 """
 
 setup(name="pygamal",
-      version="1.0.2",
+      version="1.0.4",
       author="Wouze (Mohammad)",
       author_email="m7mdwats1@hotmail.com",
       description="This module is for csc281 encryption project ",
       long_description_content_type="text/markdown",
       long_description=long_description,
       url='https://github.com/Wouze/csc281-project',
       keywords=['python', 'c', 'primitive root', 'encryption', 'algamal', 'prime'],
```

