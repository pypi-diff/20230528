# Comparing `tmp/murloc-0.0.3.tar.gz` & `tmp/murloc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murloc-0.0.3.tar", last modified: Sat May 27 20:49:48 2023, max compression
+gzip compressed data, was "murloc-0.0.4.tar", last modified: Sat May 27 21:58:27 2023, max compression
```

## Comparing `murloc-0.0.3.tar` & `murloc-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 20:49:48.910487 murloc-0.0.3/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-05-26 21:19:51.000000 murloc-0.0.3/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)     3182 2023-05-27 20:49:48.910487 murloc-0.0.3/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     2818 2023-05-27 20:48:16.000000 murloc-0.0.3/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 20:49:48.909487 murloc-0.0.3/murloc/
--rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.3/murloc/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4409 2023-05-27 19:45:13.000000 murloc-0.0.3/murloc/murloc.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 20:49:48.910487 murloc-0.0.3/murloc.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3182 2023-05-27 20:49:48.000000 murloc-0.0.3/murloc.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-05-27 20:49:48.000000 murloc-0.0.3/murloc.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-27 20:49:48.000000 murloc-0.0.3/murloc.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-05-27 20:49:48.000000 murloc-0.0.3/murloc.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-27 20:49:48.910487 murloc-0.0.3/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-05-27 20:49:24.000000 murloc-0.0.3/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 21:58:27.618814 murloc-0.0.4/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-05-26 21:19:51.000000 murloc-0.0.4/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3182 2023-05-27 21:58:27.618814 murloc-0.0.4/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2818 2023-05-27 20:48:16.000000 murloc-0.0.4/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 21:58:27.618814 murloc-0.0.4/murloc/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.4/murloc/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4505 2023-05-27 21:57:01.000000 murloc-0.0.4/murloc/murloc.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 21:58:27.618814 murloc-0.0.4/murloc.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3182 2023-05-27 21:58:27.000000 murloc-0.0.4/murloc.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-05-27 21:58:27.000000 murloc-0.0.4/murloc.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-27 21:58:27.000000 murloc-0.0.4/murloc.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-05-27 21:58:27.000000 murloc-0.0.4/murloc.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-27 21:58:27.618814 murloc-0.0.4/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-05-27 21:57:50.000000 murloc-0.0.4/setup.py
```

### Comparing `murloc-0.0.3/LICENSE` & `murloc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `murloc-0.0.3/PKG-INFO` & `murloc-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murloc
-Version: 0.0.3
+Version: 0.0.4
 Summary: extensible api server
 Home-page: 
 Author: Chris Varga
 Author-email: 
 Keywords: extensible api server
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `murloc-0.0.3/README.md` & `murloc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `murloc-0.0.3/murloc/murloc.py` & `murloc-0.0.4/murloc/murloc.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,17 +102,19 @@
     def handle_connection(self, conn, addr):
         while True:
             try:
                 data = self.recvall(conn)
             except Exception as e:
                 if self.mode == "debug":
                     self.log(f"recv: {e}")
+                conn.shutdown(socket.SHUT_RDWR)
                 conn.close()
                 break
             if not data:
+                conn.shutdown(socket.SHUT_RDWR)
                 conn.close()
                 break
             req = data.decode().strip()
             res = f"{self.parse(req)}\n"
             conn.sendall(res.encode())
 
     def handle_sigint(self, sig, frame):
```

### Comparing `murloc-0.0.3/murloc.egg-info/PKG-INFO` & `murloc-0.0.4/murloc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murloc
-Version: 0.0.3
+Version: 0.0.4
 Summary: extensible api server
 Home-page: 
 Author: Chris Varga
 Author-email: 
 Keywords: extensible api server
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `murloc-0.0.3/setup.py` & `murloc-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="murloc",
-    version="0.0.3",
+    version="0.0.4",
     author="Chris Varga",
     author_email="",
     description="extensible api server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
```

