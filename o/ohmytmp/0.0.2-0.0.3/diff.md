# Comparing `tmp/ohmytmp-0.0.2.tar.gz` & `tmp/ohmytmp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmytmp-0.0.2.tar", last modified: Sun May 28 11:53:31 2023, max compression
+gzip compressed data, was "ohmytmp-0.0.3.tar", last modified: Sun May 28 14:15:05 2023, max compression
```

## Comparing `ohmytmp-0.0.2.tar` & `ohmytmp-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:53:31.206068 ohmytmp-0.0.2/
--rw-rw-rw-   0        0        0     1064 2023-05-28 04:17:27.000000 ohmytmp-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1818 2023-05-28 11:53:31.205068 ohmytmp-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-05-28 04:17:27.000000 ohmytmp-0.0.2/README.md
--rw-rw-rw-   0        0        0      697 2023-05-28 11:52:23.000000 ohmytmp-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 11:53:31.206068 ohmytmp-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 11:53:31.184071 ohmytmp-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 11:53:31.192072 ohmytmp-0.0.2/src/ohmytmp/
--rw-rw-rw-   0        0        0      178 2023-05-28 11:43:56.000000 ohmytmp-0.0.2/src/ohmytmp/__init__.py
--rw-rw-rw-   0        0        0     1827 2023-05-28 11:36:09.000000 ohmytmp-0.0.2/src/ohmytmp/constant.py
--rw-rw-rw-   0        0        0     1042 2023-05-28 11:50:14.000000 ohmytmp-0.0.2/src/ohmytmp/destination.py
--rw-rw-rw-   0        0        0     1949 2023-05-28 04:26:51.000000 ohmytmp-0.0.2/src/ohmytmp/guesstype.py
--rw-rw-rw-   0        0        0     2457 2023-05-28 11:50:39.000000 ohmytmp-0.0.2/src/ohmytmp/initialization.py
--rw-rw-rw-   0        0        0     1631 2023-05-28 04:26:51.000000 ohmytmp-0.0.2/src/ohmytmp/plugin.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:53:31.204069 ohmytmp-0.0.2/src/ohmytmp.egg-info/
--rw-rw-rw-   0        0        0     1818 2023-05-28 11:53:31.000000 ohmytmp-0.0.2/src/ohmytmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-28 11:53:31.000000 ohmytmp-0.0.2/src/ohmytmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:53:31.000000 ohmytmp-0.0.2/src/ohmytmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 11:53:31.000000 ohmytmp-0.0.2/src/ohmytmp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 14:15:05.583579 ohmytmp-0.0.3/
+-rw-rw-rw-   0        0        0     1064 2023-05-28 04:17:27.000000 ohmytmp-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1826 2023-05-28 14:15:05.583579 ohmytmp-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-05-28 04:17:27.000000 ohmytmp-0.0.3/README.md
+-rw-rw-rw-   0        0        0      705 2023-05-28 14:14:09.000000 ohmytmp-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 14:15:05.583579 ohmytmp-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 14:15:05.564580 ohmytmp-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 14:15:05.571580 ohmytmp-0.0.3/src/ohmytmp/
+-rw-rw-rw-   0        0        0      149 2023-05-28 14:10:34.000000 ohmytmp-0.0.3/src/ohmytmp/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-05-28 13:42:56.000000 ohmytmp-0.0.3/src/ohmytmp/constant.py
+-rw-rw-rw-   0        0        0     1033 2023-05-28 14:10:26.000000 ohmytmp-0.0.3/src/ohmytmp/core.py
+-rw-rw-rw-   0        0        0     2101 2023-05-28 14:04:45.000000 ohmytmp-0.0.3/src/ohmytmp/guesstype.py
+-rw-rw-rw-   0        0        0      756 2023-05-28 14:03:56.000000 ohmytmp-0.0.3/src/ohmytmp/plugin.py
+drwxrwxrwx   0        0        0        0 2023-05-28 14:15:05.582579 ohmytmp-0.0.3/src/ohmytmp.egg-info/
+-rw-rw-rw-   0        0        0     1826 2023-05-28 14:15:05.000000 ohmytmp-0.0.3/src/ohmytmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-28 14:15:05.000000 ohmytmp-0.0.3/src/ohmytmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 14:15:05.000000 ohmytmp-0.0.3/src/ohmytmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 14:15:05.000000 ohmytmp-0.0.3/src/ohmytmp.egg-info/top_level.txt
```

### Comparing `ohmytmp-0.0.2/LICENSE` & `ohmytmp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmytmp-0.0.2/PKG-INFO` & `ohmytmp-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ohmytmp
-Version: 0.0.2
-Summary: core
+Version: 0.0.3
+Summary: ohmytmp-core
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ohmytmp-0.0.2/pyproject.toml` & `ohmytmp-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "ohmytmp"
-version = "0.0.2"
-description = "core"
+version = "0.0.3"
+description = "ohmytmp-core"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["file"]
 
 authors = [
   {name = "userElaina", email = "userelaina@pm.me" }
```

### Comparing `ohmytmp-0.0.2/src/ohmytmp/constant.py` & `ohmytmp-0.0.3/src/ohmytmp/constant.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,17 +20,15 @@
                 ans[i] = eval('self.%s' % i)
         return ans
 
 
 class __func(Const):
     def __init__(self) -> None:
         super().__init__()
-        self.GUESSTYPE = 'guesstype'
         self.ANALYSIS = 'analysis'
-        self.DESTINATION = 'destination'
         self.AFTER = 'after'
 
 
 FUNC = __func()
 
 
 class __type(Const):
@@ -54,19 +52,22 @@
 
 
 class Info(Const):
     def __init__(self, src: str) -> None:
         super().__init__()
         self.SRC = os.path.abspath(os.path.expanduser(src))
         self.BASE = os.path.basename(self.SRC)
-        self.DST = None
-        self.EXT = None
+        self.EXT = os.path.splitext(self.BASE)[1][1:]
         self.TYPE = TYPE.UNKNOWN
         self.TAGS = list()
 
+        self.DST = None
+        self.SHA256 = None
+        self.UUID = None
+
     def to_taglist(self, addlist: list = ['EXT', 'TYPE']) -> list:
         ans = self.TAGS.copy()
         d = self.to_dict()
         for i in addlist:
             if i in d and isinstance(d[i], str):
                 ans.append('%s_%s' % (i, d[i]))
         return ans
```

### Comparing `ohmytmp-0.0.2/src/ohmytmp/destination.py` & `ohmytmp-0.0.3/src/ohmytmp/plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import os
+from typing import Callable
 
-from .constant import Info, TYPE
-from .plugin import PluginDestination
+from .constant import Info, FUNC
 
 
-class DstOneDir(PluginDestination):
-    def __init__(self, dst: str) -> None:
-        self.__dst = os.path.abspath(os.path.expanduser(dst))
-
-        def __func(info: Info) -> str:
-            return self.__dst
-        super().__init__(__func)
-        self.start()
-
-    def start(self) -> None:
-        self.mkdir(self.__dst)
-        self.flag = True
-
-
-class DstExtType(PluginDestination):
-    def __init__(self, dst: str) -> None:
-        self.__dst = os.path.abspath(os.path.expanduser(dst))
-        self.data = {i: os.path.abspath(os.path.join(self.__dst, i))
-            for i in TYPE.to_dict().values()}
-
-        def __func(info: Info) -> str:
-            return self.data.get(info.TYPE, self.data[TYPE.UNKNOWN])
-        super().__init__(__func)
-        self.start()
-
-    def start(self) -> None:
-        self.mkdir(self.__dst)
-        for i in self.data:
-            self.mkdir(self.data[i])
-        self.flag = True
+class PluginBase:
+    def __init__(self, func: Callable = None) -> None:
+        self.TYPE = None
+        if func is not None:
+            self.func = func
+
+    def func(self, *l, **d):
+        pass
+
+
+class PluginAnalysis(PluginBase):
+    def __init__(self, func: Callable[[Info], None] = None) -> None:
+        super().__init__(func)
+        self.TYPE = FUNC.ANALYSIS
+
+    # def func(self, info: Info) -> None:
+    #     pass
+
+
+class PluginAfter(PluginBase):
+    def __init__(self, func: Callable[[Info], None] = None) -> None:
+        super().__init__(func)
+        self.TYPE = FUNC.AFTER
+
+    # def func(self, _info: Info) -> None:
+    #     pass
```

### Comparing `ohmytmp-0.0.2/src/ohmytmp/guesstype.py` & `ohmytmp-0.0.3/src/ohmytmp/guesstype.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import mimetypes
 
-from .constant import TYPE
+from .constant import TYPE, Info
 
 
 def get_ext(p: str) -> str:
     return os.path.splitext(p)[1][1:]
 
 
 def guess_mime(p: str) -> str:
@@ -59,9 +59,15 @@
 ext_re = dict()
 for i in ext_type:
     for j in ext_type[i].split(' '):
         assert j not in ext_re
         ext_re[j] = i
 
 
-def guess_ext(p: str) -> str:
-    return ext_re.get(get_ext(p), TYPE.UNKNOWN)
+def guess_ext(e: str) -> str:
+    return ext_re.get(e, TYPE.UNKNOWN)
+
+
+def guesstype(info: Info) -> None:
+    info.TYPE = guess_ext(info.EXT)
+    if info.TYPE == TYPE.UNKNOWN:
+        info.TYPE == guess_mime(info.SRC)
```

### Comparing `ohmytmp-0.0.2/src/ohmytmp.egg-info/PKG-INFO` & `ohmytmp-0.0.3/src/ohmytmp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ohmytmp
-Version: 0.0.2
-Summary: core
+Version: 0.0.3
+Summary: ohmytmp-core
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

