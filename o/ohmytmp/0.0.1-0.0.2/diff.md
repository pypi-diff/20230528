# Comparing `tmp/ohmytmp-0.0.1.tar.gz` & `tmp/ohmytmp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmytmp-0.0.1.tar", last modified: Sun May 28 04:25:51 2023, max compression
+gzip compressed data, was "ohmytmp-0.0.2.tar", last modified: Sun May 28 11:53:31 2023, max compression
```

## Comparing `ohmytmp-0.0.1.tar` & `ohmytmp-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 04:25:51.276035 ohmytmp-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-05-28 04:17:27.000000 ohmytmp-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1818 2023-05-28 04:25:51.275034 ohmytmp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-05-28 04:17:27.000000 ohmytmp-0.0.1/README.md
--rw-rw-rw-   0        0        0      697 2023-05-28 04:21:59.000000 ohmytmp-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 04:25:51.276035 ohmytmp-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 04:25:51.255033 ohmytmp-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 04:25:51.263034 ohmytmp-0.0.1/src/ohmytmp/
--rw-rw-rw-   0        0        0      165 2023-05-28 03:21:55.000000 ohmytmp-0.0.1/src/ohmytmp/__init__.py
--rw-rw-rw-   0        0        0     1827 2023-05-28 03:28:44.000000 ohmytmp-0.0.1/src/ohmytmp/constant.py
--rw-rw-rw-   0        0        0     1068 2023-05-28 03:38:02.000000 ohmytmp-0.0.1/src/ohmytmp/destination.py
--rw-rw-rw-   0        0        0     1949 2023-05-25 12:55:58.000000 ohmytmp-0.0.1/src/ohmytmp/guesstype.py
--rw-rw-rw-   0        0        0     2426 2023-05-28 03:31:07.000000 ohmytmp-0.0.1/src/ohmytmp/initialization.py
--rw-rw-rw-   0        0        0     1631 2023-05-28 03:28:04.000000 ohmytmp-0.0.1/src/ohmytmp/plugin.py
-drwxrwxrwx   0        0        0        0 2023-05-28 04:25:51.274033 ohmytmp-0.0.1/src/ohmytmp.egg-info/
--rw-rw-rw-   0        0        0     1818 2023-05-28 04:25:51.000000 ohmytmp-0.0.1/src/ohmytmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-28 04:25:51.000000 ohmytmp-0.0.1/src/ohmytmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 04:25:51.000000 ohmytmp-0.0.1/src/ohmytmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 04:25:51.000000 ohmytmp-0.0.1/src/ohmytmp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 11:53:31.206068 ohmytmp-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-05-28 04:17:27.000000 ohmytmp-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1818 2023-05-28 11:53:31.205068 ohmytmp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-05-28 04:17:27.000000 ohmytmp-0.0.2/README.md
+-rw-rw-rw-   0        0        0      697 2023-05-28 11:52:23.000000 ohmytmp-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 11:53:31.206068 ohmytmp-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 11:53:31.184071 ohmytmp-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 11:53:31.192072 ohmytmp-0.0.2/src/ohmytmp/
+-rw-rw-rw-   0        0        0      178 2023-05-28 11:43:56.000000 ohmytmp-0.0.2/src/ohmytmp/__init__.py
+-rw-rw-rw-   0        0        0     1827 2023-05-28 11:36:09.000000 ohmytmp-0.0.2/src/ohmytmp/constant.py
+-rw-rw-rw-   0        0        0     1042 2023-05-28 11:50:14.000000 ohmytmp-0.0.2/src/ohmytmp/destination.py
+-rw-rw-rw-   0        0        0     1949 2023-05-28 04:26:51.000000 ohmytmp-0.0.2/src/ohmytmp/guesstype.py
+-rw-rw-rw-   0        0        0     2457 2023-05-28 11:50:39.000000 ohmytmp-0.0.2/src/ohmytmp/initialization.py
+-rw-rw-rw-   0        0        0     1631 2023-05-28 04:26:51.000000 ohmytmp-0.0.2/src/ohmytmp/plugin.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:53:31.204069 ohmytmp-0.0.2/src/ohmytmp.egg-info/
+-rw-rw-rw-   0        0        0     1818 2023-05-28 11:53:31.000000 ohmytmp-0.0.2/src/ohmytmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-28 11:53:31.000000 ohmytmp-0.0.2/src/ohmytmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:53:31.000000 ohmytmp-0.0.2/src/ohmytmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 11:53:31.000000 ohmytmp-0.0.2/src/ohmytmp.egg-info/top_level.txt
```

### Comparing `ohmytmp-0.0.1/LICENSE` & `ohmytmp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmytmp-0.0.1/PKG-INFO` & `ohmytmp-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp
-Version: 0.0.1
+Version: 0.0.2
 Summary: core
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
```

### Comparing `ohmytmp-0.0.1/pyproject.toml` & `ohmytmp-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ohmytmp"
-version = "0.0.1"
+version = "0.0.2"
 description = "core"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["file"]
 
 authors = [
```

### Comparing `ohmytmp-0.0.1/src/ohmytmp/constant.py` & `ohmytmp-0.0.2/src/ohmytmp/constant.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,9 +64,9 @@
         self.TAGS = list()
 
     def to_taglist(self, addlist: list = ['EXT', 'TYPE']) -> list:
         ans = self.TAGS.copy()
         d = self.to_dict()
         for i in addlist:
             if i in d and isinstance(d[i], str):
-                ans.append('%s:%s' % (i, d[i]))
+                ans.append('%s_%s' % (i, d[i]))
         return ans
```

### Comparing `ohmytmp-0.0.1/src/ohmytmp/destination.py` & `ohmytmp-0.0.2/src/ohmytmp/destination.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 class DstExtType(PluginDestination):
     def __init__(self, dst: str) -> None:
         self.__dst = os.path.abspath(os.path.expanduser(dst))
         self.data = {i: os.path.abspath(os.path.join(self.__dst, i))
             for i in TYPE.to_dict().values()}
-        print(self.data)
 
         def __func(info: Info) -> str:
             return self.data.get(info.TYPE, self.data[TYPE.UNKNOWN])
         super().__init__(__func)
         self.start()
 
     def start(self) -> None:
```

### Comparing `ohmytmp-0.0.1/src/ohmytmp/guesstype.py` & `ohmytmp-0.0.2/src/ohmytmp/guesstype.py`

 * *Files identical despite different names*

### Comparing `ohmytmp-0.0.1/src/ohmytmp/initialization.py` & `ohmytmp-0.0.2/src/ohmytmp/initialization.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,13 +64,14 @@
         info.EXT = e
         info.TYPE = self.exec_guesstype(info.SRC)
 
     def init_file(self, p: str) -> Info:
         info = Info(p)
         self.exec_analysis(info)
         info.DST = self.exec_destination(info)
+        self.exec_after(info)
         return info
 
     def walk(self, d: str):
         for p, _, f in os.walk(d):
             for i in f:
                 self.init_file(os.path.join(p, i))
```

### Comparing `ohmytmp-0.0.1/src/ohmytmp/plugin.py` & `ohmytmp-0.0.2/src/ohmytmp/plugin.py`

 * *Files identical despite different names*

### Comparing `ohmytmp-0.0.1/src/ohmytmp.egg-info/PKG-INFO` & `ohmytmp-0.0.2/src/ohmytmp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp
-Version: 0.0.1
+Version: 0.0.2
 Summary: core
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
```

