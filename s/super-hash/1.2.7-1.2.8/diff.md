# Comparing `tmp/super_hash-1.2.7.tar.gz` & `tmp/super_hash-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_hash-1.2.7.tar", last modified: Thu May 25 20:21:01 2023, max compression
+gzip compressed data, was "super_hash-1.2.8.tar", last modified: Sun May 28 13:59:02 2023, max compression
```

## Comparing `super_hash-1.2.7.tar` & `super_hash-1.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:21:01.584510 super_hash-1.2.7/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-05-25 20:21:01.584343 super_hash-1.2.7/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-25 20:21:01.584561 super_hash-1.2.7/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2022-11-20 16:13:35.000000 super_hash-1.2.7/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:21:01.583281 super_hash-1.2.7/super_hash/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12054 2023-05-25 20:20:06.000000 super_hash-1.2.7/super_hash/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    74569 2023-05-25 19:39:10.000000 super_hash-1.2.7/super_hash/instuctions.ignore.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:21:01.584160 super_hash-1.2.7/super_hash.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-05-25 20:21:01.000000 super_hash-1.2.7/super_hash.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2023-05-25 20:21:01.000000 super_hash-1.2.7/super_hash.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-25 20:21:01.000000 super_hash-1.2.7/super_hash.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-05-25 20:21:01.000000 super_hash-1.2.7/super_hash.egg-info/top_level.txt
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 13:59:02.123817 super_hash-1.2.8/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-05-28 13:59:02.123681 super_hash-1.2.8/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-28 13:59:02.123860 super_hash-1.2.8/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2022-11-20 16:13:35.000000 super_hash-1.2.8/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 13:59:02.122606 super_hash-1.2.8/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12071 2023-05-28 13:58:30.000000 super_hash-1.2.8/super_hash/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    74569 2023-05-25 19:39:10.000000 super_hash-1.2.8/super_hash/instuctions.ignore.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 13:59:02.123516 super_hash-1.2.8/super_hash.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-05-28 13:59:01.000000 super_hash-1.2.8/super_hash.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2023-05-28 13:59:02.000000 super_hash-1.2.8/super_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-28 13:59:01.000000 super_hash-1.2.8/super_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-05-28 13:59:02.000000 super_hash-1.2.8/super_hash.egg-info/top_level.txt
```

### Comparing `super_hash-1.2.7/PKG-INFO` & `super_hash-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super_hash
-Version: 1.2.7
+Version: 1.2.8
 Summary: hash the unhashable, hash everything
 Home-page: https://github.com/jeff-hykin/super_hash.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `super_hash-1.2.7/setup.py` & `super_hash-1.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `super_hash-1.2.7/super_hash/__init__.py` & `super_hash-1.2.8/super_hash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             if function_reference is None:
                 continue
             try:
                 instructions = dis.get_instructions(function_reference)
             except TypeError as error:
                 continue
             instruction_hashes.append(function_hashers.instructions_to_hash(instructions))
-            child_names = get_referenced_function_names(instructions)
+            child_names = function_hashers.get_referenced_function_names(instructions)
             for child_name in child_names:
                 if child_name not in closed_set:
                     frontier.add(child_name)
         hash_str = ' '.join(instruction_hashes).encode('utf-8')
         return consistent_hash(hash_str)
     
 try:
```

### Comparing `super_hash-1.2.7/super_hash/instuctions.ignore.py` & `super_hash-1.2.8/super_hash/instuctions.ignore.py`

 * *Files identical despite different names*

### Comparing `super_hash-1.2.7/super_hash.egg-info/PKG-INFO` & `super_hash-1.2.8/super_hash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-hash
-Version: 1.2.7
+Version: 1.2.8
 Summary: hash the unhashable, hash everything
 Home-page: https://github.com/jeff-hykin/super_hash.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

