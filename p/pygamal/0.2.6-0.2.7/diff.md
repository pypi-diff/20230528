# Comparing `tmp/pygamal-0.2.6.tar.gz` & `tmp/pygamal-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygamal-0.2.6.tar", last modified: Sat May 27 23:33:02 2023, max compression
+gzip compressed data, was "pygamal-0.2.7.tar", last modified: Sat May 27 23:37:29 2023, max compression
```

## Comparing `pygamal-0.2.6.tar` & `pygamal-0.2.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 23:33:02.850446 pygamal-0.2.6/
--rw-rw-rw-   0        0        0      809 2023-05-27 23:33:02.850446 pygamal-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     9714 2023-05-27 23:26:46.000000 pygamal-0.2.6/encryptmodule.c
-drwxrwxrwx   0        0        0        0 2023-05-27 23:33:02.848435 pygamal-0.2.6/pygamal.egg-info/
--rw-rw-rw-   0        0        0      809 2023-05-27 23:33:02.000000 pygamal-0.2.6/pygamal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-27 23:33:02.000000 pygamal-0.2.6/pygamal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 23:33:02.000000 pygamal-0.2.6/pygamal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 23:33:02.000000 pygamal-0.2.6/pygamal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 23:33:02.850446 pygamal-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-05-27 23:28:49.000000 pygamal-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 23:37:29.939018 pygamal-0.2.7/
+-rw-rw-rw-   0        0        0      809 2023-05-27 23:37:29.939018 pygamal-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9714 2023-05-27 23:26:46.000000 pygamal-0.2.7/encryptmodule.c
+drwxrwxrwx   0        0        0        0 2023-05-27 23:37:29.939018 pygamal-0.2.7/pygamal.egg-info/
+-rw-rw-rw-   0        0        0      809 2023-05-27 23:37:29.000000 pygamal-0.2.7/pygamal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-27 23:37:29.000000 pygamal-0.2.7/pygamal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 23:37:29.000000 pygamal-0.2.7/pygamal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 23:37:29.000000 pygamal-0.2.7/pygamal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 23:37:29.939018 pygamal-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-05-27 23:37:20.000000 pygamal-0.2.7/setup.py
```

### Comparing `pygamal-0.2.6/PKG-INFO` & `pygamal-0.2.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 0.2.6
+Version: 0.2.7
 Summary: This module is for csc281 encryption project 
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygamal-0.2.6/encryptmodule.c` & `pygamal-0.2.7/encryptmodule.c`

 * *Files identical despite different names*

### Comparing `pygamal-0.2.6/pygamal.egg-info/PKG-INFO` & `pygamal-0.2.7/pygamal.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 0.2.6
+Version: 0.2.7
 Summary: This module is for csc281 encryption project 
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygamal-0.2.6/setup.py` & `pygamal-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 module = Extension("ElGamal_c", sources=["encryptmodule.c"]
                   #  ,extra_compile_args=['/openmp']
                    )
 
 setup(name="pygamal",
-      version="0.2.6",
+      version="0.2.7",
       author="Wouze (Mohammad)",
       author_email="m7mdwats1@hotmail.com",
       description="This module is for csc281 encryption project ",
       long_description_content_type="text/markdown",
       long_description=long_description,
       keywords=['python', 'c', 'primitive root', 'encryption', 'algamal', 'prime'],
       classifiers=[
```

