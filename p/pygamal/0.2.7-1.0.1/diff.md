# Comparing `tmp/pygamal-0.2.7.tar.gz` & `tmp/pygamal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygamal-0.2.7.tar", last modified: Sat May 27 23:37:29 2023, max compression
+gzip compressed data, was "pygamal-1.0.1.tar", last modified: Sat May 27 23:56:49 2023, max compression
```

## Comparing `pygamal-0.2.7.tar` & `pygamal-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 23:37:29.939018 pygamal-0.2.7/
--rw-rw-rw-   0        0        0      809 2023-05-27 23:37:29.939018 pygamal-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     9714 2023-05-27 23:26:46.000000 pygamal-0.2.7/encryptmodule.c
-drwxrwxrwx   0        0        0        0 2023-05-27 23:37:29.939018 pygamal-0.2.7/pygamal.egg-info/
--rw-rw-rw-   0        0        0      809 2023-05-27 23:37:29.000000 pygamal-0.2.7/pygamal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-27 23:37:29.000000 pygamal-0.2.7/pygamal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 23:37:29.000000 pygamal-0.2.7/pygamal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 23:37:29.000000 pygamal-0.2.7/pygamal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 23:37:29.939018 pygamal-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-05-27 23:37:20.000000 pygamal-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:56:49.912320 pygamal-1.0.1/
+-rw-rw-rw-   0        0        0      861 2023-05-27 23:56:49.912320 pygamal-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-27 23:56:49.890424 pygamal-1.0.1/pygamal/
+-rw-rw-rw-   0        0        0       30 2023-05-27 23:36:28.000000 pygamal-1.0.1/pygamal/__init__.py
+-rw-rw-rw-   0        0        0     4308 2023-05-27 23:24:32.000000 pygamal-1.0.1/pygamal/el_gamal_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:56:49.912320 pygamal-1.0.1/pygamal.egg-info/
+-rw-rw-rw-   0        0        0      861 2023-05-27 23:56:49.000000 pygamal-1.0.1/pygamal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-27 23:56:49.000000 pygamal-1.0.1/pygamal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 23:56:49.000000 pygamal-1.0.1/pygamal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-27 23:56:49.000000 pygamal-1.0.1/pygamal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 23:56:49.000000 pygamal-1.0.1/pygamal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 23:56:49.912320 pygamal-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-05-27 23:55:39.000000 pygamal-1.0.1/setup.py
```

### Comparing `pygamal-0.2.7/PKG-INFO` & `pygamal-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 0.2.7
+Version: 1.0.1
 Summary: This module is for csc281 encryption project 
+Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `pygamal-0.2.7/pygamal.egg-info/PKG-INFO` & `pygamal-1.0.1/pygamal.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 0.2.7
+Version: 1.0.1
 Summary: This module is for csc281 encryption project 
+Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `pygamal-0.2.7/setup.py` & `pygamal-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from distutils.core import setup, Extension
+from distutils.core import setup
+
 long_description =\
 """
 This module have been made for the project of discret math CSC281 at ksu university.
 The project supervisor is Aqil Alazimi. LinkedIn: https://www.linkedin.com/in/aqil-azmi-20903960/
 The project repo is: https://github.com/Wouze/csc281-project
 """
 
-module = Extension("ElGamal_c", sources=["encryptmodule.c"]
-                  #  ,extra_compile_args=['/openmp']
-                   )
-
 setup(name="pygamal",
-      version="0.2.7",
+      version="1.0.1",
       author="Wouze (Mohammad)",
       author_email="m7mdwats1@hotmail.com",
       description="This module is for csc281 encryption project ",
       long_description_content_type="text/markdown",
       long_description=long_description,
+      url='https://github.com/Wouze/csc281-project',
       keywords=['python', 'c', 'primitive root', 'encryption', 'algamal', 'prime'],
+      install_requires=["ElGamal-c==1.0.1"],
       classifiers=[
             "Development Status :: 1 - Planning",
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3",
             "Operating System :: Unix",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
-      ],
-      ext_modules=[module])
+      ])
```

