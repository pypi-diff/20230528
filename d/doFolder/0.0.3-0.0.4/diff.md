# Comparing `tmp/doFolder-0.0.3.tar.gz` & `tmp/doFolder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.0.3.tar", last modified: Fri May 26 06:31:49 2023, max compression
+gzip compressed data, was "doFolder-0.0.4.tar", last modified: Sun May 28 09:02:09 2023, max compression
```

## Comparing `doFolder-0.0.3.tar` & `doFolder-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 06:31:49.887162 doFolder-0.0.3/
--rw-rw-rw-   0        0        0     3245 2023-05-26 06:31:49.886162 doFolder-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2553 2023-05-26 06:30:22.000000 doFolder-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-26 06:31:49.841162 doFolder-0.0.3/doFolder/
--rw-rw-rw-   0        0        0       63 2023-05-25 15:20:42.000000 doFolder-0.0.3/doFolder/__init__.py
--rw-rw-rw-   0        0        0     9443 2023-05-26 06:31:25.000000 doFolder-0.0.3/doFolder/compare.py
--rw-rw-rw-   0        0        0    17480 2023-05-25 14:42:53.000000 doFolder-0.0.3/doFolder/main.py
--rw-rw-rw-   0        0        0    13265 2023-05-26 05:13:05.000000 doFolder-0.0.3/doFolder/terminal.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:31:49.884161 doFolder-0.0.3/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3245 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 06:31:49.000000 doFolder-0.0.3/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 06:31:49.887162 doFolder-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-26 04:09:05.000000 doFolder-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 09:02:09.217024 doFolder-0.0.4/
+-rw-rw-rw-   0        0        0     3260 2023-05-28 09:02:09.217024 doFolder-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2535 2023-05-28 08:47:54.000000 doFolder-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-28 09:02:09.151024 doFolder-0.0.4/doFolder/
+-rw-rw-rw-   0        0        0      569 2023-05-26 13:44:53.000000 doFolder-0.0.4/doFolder/__init__.py
+-rw-rw-rw-   0        0        0    10825 2023-05-28 09:01:39.000000 doFolder-0.0.4/doFolder/compare.py
+-rw-rw-rw-   0        0        0    19027 2023-05-28 08:57:56.000000 doFolder-0.0.4/doFolder/main.py
+-rw-rw-rw-   0        0        0    13319 2023-05-28 09:02:05.000000 doFolder-0.0.4/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-05-28 09:02:09.214024 doFolder-0.0.4/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3260 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 09:02:09.000000 doFolder-0.0.4/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 09:02:09.218025 doFolder-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-05-28 08:38:02.000000 doFolder-0.0.4/setup.py
```

### Comparing `doFolder-0.0.3/PKG-INFO` & `doFolder-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.3
+Version: 0.0.4
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
 Platform: linux
 Platform: macos
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: English
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 
 文件夹管理(doFolder)
@@ -38,14 +39,15 @@
 部分功能
 ~~~~~~~~
 
 -  ``Folder`` 指一个文件夹
 
    -  *参数* ``path`` 文件夹路径:``str|doFolder.Path``
    -  *参数* ``onlisten`` 是否监听比同步文件夹变动:``bool``
+   -  *参数* ``scan`` 是否在现在扫描(否则会在访问时进行扫描)
    -  *属性* ``files`` 文件夹中的文件列表:``FileList``
    -  *属性* ``subfolder`` 文件夹中的子文件夹:``FolderList``
    -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
       ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
@@ -57,41 +59,37 @@
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
 
 -  ``Path`` 指一个路径
 
-   -  *参数* ``path`` 路径(绝对或相对):``str``
+-  *参数* ``path`` 路径(绝对或相对):``str``
+
    -  *属性* ``partition`` 将路径(不包含驱动器)切片
    -  *方法* ``add`` 将内容加载路径后面
    -  *方法* ``findRest`` 去除两个路径的共同部分
 
 -  ``compare``\ 提供比较文件夹的API
 
    -  *函数* ``compare`` 比较两个文件夹
 
       -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
-      -  *参数* ``compareContent`` 文件内容的比较方法
-
-         -  ``ignore`` 忽略文件内容
-         -  ``hash`` 比较文件哈希值
-         -  ``content`` 比较文件内容
-         -  ``size`` 比较文件大小
-
+      -  *参数* ``compareContent``
+         文件内容的比较方法:``str|Callable[[doFolder.File,doFolder.File],bool]``
       -  *参数* ``threaded`` 是否线程化 ``bool``
       -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
 
-   compare Folder1 Folder2 [-c ignore|hash|content|size]
+   compare Folder1 Folder2 [-c ignore|hash|content|size] [-t [-n num]]
 
 具体作用参见
 
 .. code:: bash
 
    compare -h
```

### Comparing `doFolder-0.0.3/README.rst` & `doFolder-0.0.4/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 部分功能
 ~~~~~~~~
 
 -  ``Folder`` 指一个文件夹
 
    -  *参数* ``path`` 文件夹路径:``str|doFolder.Path``
    -  *参数* ``onlisten`` 是否监听比同步文件夹变动:``bool``
+   -  *参数* ``scan`` 是否在现在扫描(否则会在访问时进行扫描)
    -  *属性* ``files`` 文件夹中的文件列表:``FileList``
    -  *属性* ``subfolder`` 文件夹中的子文件夹:``FolderList``
    -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
       ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
@@ -37,41 +38,37 @@
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
 
 -  ``Path`` 指一个路径
 
-   -  *参数* ``path`` 路径(绝对或相对):``str``
+-  *参数* ``path`` 路径(绝对或相对):``str``
+
    -  *属性* ``partition`` 将路径(不包含驱动器)切片
    -  *方法* ``add`` 将内容加载路径后面
    -  *方法* ``findRest`` 去除两个路径的共同部分
 
 -  ``compare``\ 提供比较文件夹的API
 
    -  *函数* ``compare`` 比较两个文件夹
 
       -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
-      -  *参数* ``compareContent`` 文件内容的比较方法
-
-         -  ``ignore`` 忽略文件内容
-         -  ``hash`` 比较文件哈希值
-         -  ``content`` 比较文件内容
-         -  ``size`` 比较文件大小
-
+      -  *参数* ``compareContent``
+         文件内容的比较方法:``str|Callable[[doFolder.File,doFolder.File],bool]``
       -  *参数* ``threaded`` 是否线程化 ``bool``
       -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
 
-   compare Folder1 Folder2 [-c ignore|hash|content|size]
+   compare Folder1 Folder2 [-c ignore|hash|content|size] [-t [-n num]]
 
 具体作用参见
 
 .. code:: bash
 
    compare -h
```

### Comparing `doFolder-0.0.3/doFolder/compare.py` & `doFolder-0.0.4/doFolder/compare.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,20 @@
+"""
+Copyright (c) 2023 Gou Haoming
+doFolder is licensed under Mulan PSL v2.
+You can use this software according to the terms and conditions of the Mulan PSL v2.
+You may obtain a copy of Mulan PSL v2 at:
+         http://license.coscl.org.cn/MulanPSL2
+THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
+EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
+MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
+See the Mulan PSL v2 for more details.
+"""
 import doFolder.main as doFolder
-from typing import Literal,List,Union
+from typing import Literal,List,Union,Callable,Dict
 from concurrent.futures import ThreadPoolExecutor
 class RepeatedExecutionError(Exception):
     def __init__(self,message:str):
         self.message=message
     def __str__(self):
         return self.message
 class FileMissing(doFolder._HasName):
@@ -62,30 +73,30 @@
         return self.__str__()
 class FileDifferent(doFolder._HasName):
     def __init__(self,file1:doFolder.File,file2:doFolder.File,root1:doFolder.Folder,root2:doFolder.Folder):
         self.file1 = file1
         self.file2 = file2
         self.root1 = root1
         self.root2 = root2
-        self.statue:Literal["choice1","choice2","removed","waiting"]="waiting"
+        self.statue:Literal["overwrited","removed","waiting"]="waiting"
     @property
     def path(self)->List[str]:
         return self.file1.path.findRest(self.root1.path)
     @property
     def name(self)->str:
         return self.file1.name
     def copy(self,choice:Literal[1,2])->None:
         if self.statue!="waiting":
             raise RepeatedExecutionError(f"This file has already been {self.statue}")
         if choice==1:
-            self.statue="choice1"
+            self.statue="overwrited"
             pathto=self.root2.path.adds(self.path)
             self.file1.copy(pathto)
         else:
-            self.statue="choice2"
+            self.statue="overwrited"
             pathto=self.root1.path.adds(self.path)
             self.file2.copy(pathto)
     def remove(self)->None:
         if self.statue!="waiting":
             raise RepeatedExecutionError(f"This file has already been {self.statue}")
         self.statue="removed"
         self.file1.remove()
@@ -142,30 +153,46 @@
             self.cacheFolderMissingList=self._folderMissingList.values
             for  i in self._FolderDifferentList:
                 self.cacheFolderMissingList+=i.folderMissingList
         return self.cacheFolderMissingList
     @property
     def differentList(self)->List[Union[FileMissing,FolderMissing,FileDifferent]]:
         return self.fileMissingList+self.folderMissingList+self.fileDifferentList
-def _compareFile(result:CompareResult,file1:doFolder.File,file2:doFolder.File,compareContent:Literal["ignore","hash","content","size"],root1:doFolder.Folder
-            ,root2:doFolder.Folder)->None:
-    if compareContent=="hash" and file1.hash!=file2.hash:
-        result.newDifferent(FileDifferent(file1,file2,root1,root2))
-    elif compareContent=="content" and file1.content!=file2.content:
-        result.newDifferent(FileDifferent(file1,file2,root1,root2))
-    elif compareContent=="size" and file1.size!=file2.size:
-        result.newDifferent(FileDifferent(file1,file2,root1,root2))
-def compare(folder1:doFolder.Folder,folder2:doFolder.Folder,compareContent:Literal["ignore","hash","content","size"]="ignore",threaded:bool=False,threads:Union[None,int]=None)->CompareResult:
+formatedCompareContent=Callable[[doFolder.File,doFolder.File],bool]
+unformatedCompareContent=Union[Literal["ignore","md5","sha1","sha256","sha512","hash","content","size"],formatedCompareContent]
+def _normalizedCompareContent(compareContent:unformatedCompareContent)->formatedCompareContent:
+    if callable(compareContent):
+        return compareContent
+    elif type(compareContent)==str:
+        ma:Dict[str,formatedCompareContent]={
+            "ignore":lambda f1,f2:True,
+            "hash":lambda f1,f2:f1.hash==f2.hash,
+            "sha1":lambda f1,f2:f1.sha1==f2.sha1,
+            "sha256":lambda f1,f2:f1.sha256==f2.sha256,
+            "sha512":lambda f1,f2:f1.sha512==f2.sha512,
+            "md5":lambda f1,f2:f1.md5==f2.md5,
+            "size":lambda f1,f2:f1.size==f2.size,
+            "content":lambda f1,f2:f1.content==f2.content,
+        }
+        if compareContent in ma:
+            return ma[compareContent]
+        raise ValueError(f"compareContent is not valid. If you want to customize the comparison method, please pass in a comparison function")
+    raise ValueError(f"compareContent must be callable or str,but \"{compareContent}\" is given")
+def compare(folder1:doFolder.Folder,folder2:doFolder.Folder,compareContent:unformatedCompareContent="ignore",threaded:bool=False,threads:Union[None,int]=None)->CompareResult:
     threadPool=ThreadPoolExecutor(max_workers=threads) if threaded else None
-    result=_compare(folder1,folder2,folder1,folder2,compareContent,threadPool)
+    result=_compare(folder1,folder2,folder1,folder2,_normalizedCompareContent(compareContent),threadPool)
     assert result
     if threadPool:threadPool.shutdown(wait=True)
     return result
+def _compareFile(result:CompareResult,file1:doFolder.File,file2:doFolder.File,compareContent:formatedCompareContent,root1:doFolder.Folder
+            ,root2:doFolder.Folder)->None:
+    if not compareContent(file1,file2):
+        result.newDifferent(FileDifferent(file1,file2,root1,root2))
 def _compare(folder1:doFolder.Folder,folder2:doFolder.Folder,root1:doFolder.Folder
-            ,root2:doFolder.Folder,compareContent:Literal["ignore","hash","content","size"]="ignore",threadPool:Union[ThreadPoolExecutor,None]=None,parent:Union[CompareResult,None]=None)->Union[CompareResult,None]:
+            ,root2:doFolder.Folder,compareContent:formatedCompareContent,threadPool:Union[ThreadPoolExecutor,None]=None,parent:Union[CompareResult,None]=None)->Union[CompareResult,None]:
     result=CompareResult(folder1,folder2)
     for file1 in folder1.files:
         file2=folder2.files[file1.name]
         if file2==None:
             result.newDifferent(FileMissing(file1,root1,root2))
         else:
             if threadPool:threadPool.submit(_compareFile,result,file1,file2,compareContent,root1,root2)
```

### Comparing `doFolder-0.0.3/doFolder/main.py` & `doFolder-0.0.4/doFolder/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""
+Copyright (c) 2023 Gou Haoming
+doFolder is licensed under Mulan PSL v2.
+You can use this software according to the terms and conditions of the Mulan PSL v2.
+You may obtain a copy of Mulan PSL v2 at:
+         http://license.coscl.org.cn/MulanPSL2
+THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
+EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
+MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
+See the Mulan PSL v2 for more details.
+"""
 import os
 import re
 from typing import Any,Union,Callable,Literal,List,Tuple,Iterable,TypeVar,Generic,Protocol
 import shutil
 import copy
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler,FileSystemEvent,FileSystemMovedEvent,EVENT_TYPE_CREATED,EVENT_TYPE_DELETED,EVENT_TYPE_MOVED,EVENT_TYPE_MODIFIED
@@ -188,15 +199,18 @@
         self.dev=state.st_dev
         self.uid=state.st_uid
         self.gid=state.st_gid
         self.size=state.st_size
         self.mtime=state.st_mtime
         self.ctime=state.st_ctime
         self.atime=state.st_atime
-        self._hash:Union[None,str]=None
+        self._md5:Union[None,str]=None
+        self._sha1:Union[None,str]=None
+        self._sha256:Union[None,str]=None
+        self._sha512:Union[None,str]=None
     @property
     def name(self)->str:
         return self.path.name
     def open(self,*args,**kw):
         """open the file by function open"""
         return open(self.path,*args,**kw)
     def __str__(self)->str:
@@ -204,50 +218,75 @@
     def __repr__(self) -> str:
         return f"<File \"{self.name}\">"
     @property
     def content(self)->bytes:
         with self.open("rb") as f:
             return f.read()
     @property
+    def md5(self)->str:
+        if self._md5:
+            return self._md5
+        self._md5=hashlib.md5(self.content).hexdigest()
+        return self._md5
+    @property
+    def sha1(self)->str:
+        if self._sha1:
+            return self._sha1
+        self._sha1=hashlib.sha1(self.content).hexdigest()
+        return self._sha1
+    @property
+    def sha256(self)->str:
+        if self._sha256:
+            return self._sha256
+        self._sha256=hashlib.sha256(self.content).hexdigest()
+        return self._sha256
+    @property
+    def sha512(self)->str:
+        if self._sha512:
+            return self._sha512
+        self._sha512=hashlib.sha512(self.content).hexdigest()
+        return self._sha512
+    @property
     def hash(self)->str:
-        if self._hash:
-            return self._hash
-        self._hash=hashlib.md5(self.content).hexdigest()
-        return self._hash
+        return self.md5
     def remove(self):
         os.remove(self.path)
     def copy(self,path:str):
         shutil.copy(self.path,path)
     def move(self,path:str):
         shutil.move(self.path,path)
 class Folder(_HasName):
     """Means a folder on disk"""
-    def __init__(self,path:Union[str,Path],onlisten:bool=False,parent:Union["Folder",None]=None):
+    def __init__(self,path:Union[str,Path],onlisten:bool=False,parent:Union["Folder",None]=None,scan:bool=False):
         if type(path)!=Path:
             path=Path(path)
         self.onlisten=onlisten
         self.path=path
         self.parent=parent
+        self.scaned=scan
+        self.scan=scan
         if self.onlisten:
             self.event_handler = _FolderUpdateHeader(self)
             self.observer = Observer()
             self.observer.schedule(self.event_handler, path=path, recursive=True)
             self.observer.start()
-        self.refresh()
+        if scan:
+            self.refresh()
     def refresh(self):
         """Rebuild all of this folder object"""
+        self.scaned=True
         self.dir:List[str]=os.listdir(self.path)
         self.files:FileList = FileList([])
         self.subfolder:FolderList=FolderList([])
         for i in self.dir:
             newPath=self.path.add(i)
             if os.path.isfile(newPath):
                 self.files.append(File(newPath))
             elif os.path.isdir(newPath):
-                self.subfolder.append(Folder(newPath,parent=self))
+                self.subfolder.append(Folder(newPath,parent=self,scan=self.scan))
     @property
     def name(self)->str:
         return self.path.name
     def __str__(self)->str:
         return f"<Folder \"{self.name}\">"
     def __repr__(self) -> str:
         return self.__str__()
@@ -265,14 +304,16 @@
                 return item
         for item in self.files:
             if item.name==key:
                 return item
         return None
     def _update(self,path:List[str],eventType:str,eventTarget:Path,isDirectory:bool):
         """Update when something changes"""
+        if not self.scaned:
+            return
         if len(path)>1:
             nextFolder=self[path[0]]
             if type(nextFolder)==Folder:
                 nextFolder._update(path[1:],eventType,eventTarget,isDirectory)
                 return
             else:
                 raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contain folder \"{path[0]}\"")
@@ -286,14 +327,16 @@
             elif type(target)==File:self.files.remove(target)
             else:raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contain item \"{name}\"")
         if eventType==EVENT_TYPE_MODIFIED:
             target=self[name]
             if type(target)==File:target.refresh()
             else:raise FolderOrFileNotFoundError(f"Directory \"{self.path}\" does not contains file \"{name}\"")
     def __getattribute__(self, name: str) -> Any:
+        if not super().__getattribute__("scaned") and name in ["dir","files","subfolder"]:
+            self.refresh()
         try:
             return super().__getattribute__(name)
         except AttributeError:
             target=self[name]
             if target:
                 return target
             raise AttributeError(f"\"{name}\" is not a attribute ,a subfolder or a file")
@@ -312,15 +355,14 @@
         if rootPosition=="last":
             callback(self)
     def forEachFile(self,callback:Callable[[File],Any])->None:
         """
         Go through each of these file
         :param callback:The function to call
         """
-            
         for item in self.files:
             callback(item)
         for item in self.subfolder:
             item.forEachFile(callback)
     def forEachFolder(self,callback:Callable[["Folder"],Any],rootPosition:Literal["first","last"]="first")->None:
         """
         Go through each of these folder
```

### Comparing `doFolder-0.0.3/doFolder/terminal.py` & `doFolder-0.0.4/doFolder/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import doFolder.compare as comp
 from rich.console import Console
 from rich.table import Table,Column
 from rich.style import Style
 import datetime
 import sys
 from typing import List,Union,Set
+import os
 
 def docompare():
     import argparse
     statueMapping={
         'copied':"[green]copied[/green]",
         "removed":'[red]removed[/red]', 
         'waiting':"[yellow]waiting[/yellow]", 
-        'choice1':"[cyan]choice1[/cyan]",
-        'choice2':"[cyan]choice2[/cyan]"
+        'overwrited':"[cyan]overwrited[/cyan]",
     }
     argparser = argparse.ArgumentParser()
     argparser.add_argument('folder1',type = str, help = 'The first folder to compare')
     argparser.add_argument('folder2',type = str, help = 'The second folder to compare')
-    argparser.add_argument('-c', '--content', type = str, choices=["ignore","hash","content","size"] ,default="ignore", help = 'How to compare the content of the file')
+    argparser.add_argument('-c', '--content', type = str, choices=['ignore', 'md5', 'sha1', 'sha256', 'sha512', 'hash', 'content', 'size'] ,default="ignore", help = 'How to compare the content of the file')
     argparser.add_argument('-t', '--threaded', action="store_true", help = 'Use multithreaded scanning')
     argparser.add_argument('-n', '--num', help = 'Maximum number of threads')
     args = argparser.parse_args()
     folder1 = doFolder.Folder(args.folder1)
     folder2 = doFolder.Folder(args.folder2)
     retsult=comp.compare(folder1, folder2,args.content,args.threaded,args.num)
     fileMissingList=retsult.fileMissingList
@@ -209,14 +209,15 @@
             for i in showChoice:
                 selectedItemTable.add_row(i.name,statueMapping[i.statue],i.root.path if type(i) == comp.FileMissing or type(i) == comp.FolderMissing else "--BOTH--","/".join(i.path))
             return selectedItemTable
         errSum+=1
         return "[red]Unknown Command[/red]"
     def showTable():
         console.clear()
+        os.system("cls")
         nonlocal all
         all.clear()
         if fileMissingList:
             fileMissingTable = Table(
                 Column(header="ID",no_wrap=True),
                 Column(header="File Name",no_wrap=True),
                 Column(header="Statue",no_wrap=True),
@@ -224,15 +225,15 @@
                 Column(header="Relative Path",max_width=40,no_wrap=True),
                 title="File Missing",
                 title_style=Style(color="yellow",bold=True),
                 title_justify="left"
             )
             for i in fileMissingList:
                 all.append(i)
-                fileMissingTable.add_row(str(len(all)-1),i.name,i.statue,i.root.path,"/".join(i.path))
+                fileMissingTable.add_row(str(len(all)-1),i.name,statueMapping[i.statue],i.root.path,"/".join(i.path))
             console.print(fileMissingTable)
         if folderMissingList:
             folderMissingTable = Table(
                 Column(header="ID",no_wrap=True),
                 Column(header="Folder Name",no_wrap=True),
                 Column(header="Statue",no_wrap=True),
                 Column(header="Found Root",no_wrap=True),
```

### Comparing `doFolder-0.0.3/doFolder.egg-info/PKG-INFO` & `doFolder-0.0.4/doFolder.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.3
+Version: 0.0.4
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
 Platform: linux
 Platform: macos
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: English
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 
 文件夹管理(doFolder)
@@ -38,14 +39,15 @@
 部分功能
 ~~~~~~~~
 
 -  ``Folder`` 指一个文件夹
 
    -  *参数* ``path`` 文件夹路径:``str|doFolder.Path``
    -  *参数* ``onlisten`` 是否监听比同步文件夹变动:``bool``
+   -  *参数* ``scan`` 是否在现在扫描(否则会在访问时进行扫描)
    -  *属性* ``files`` 文件夹中的文件列表:``FileList``
    -  *属性* ``subfolder`` 文件夹中的子文件夹:``FolderList``
    -  *方法* ``hasFolder,hasFile`` 是否包括某个文件/文件夹,参数为
       ``str``\ 时默认匹配 ``.name``\ 属性
    -  *方法* ``remove,copy,move`` 文件夹操作
    -  *方法* ``search`` 搜索文件夹的内容
 
@@ -57,41 +59,37 @@
 
    -  *参数* ``path`` 文件路径:``str|doFolder.Path``
    -  *方法* ``remove,copy,move`` 文件操作
    -  *属性* ``mode,ino,dev,uid,gid...`` 参见 ``os.stat``
 
 -  ``Path`` 指一个路径
 
-   -  *参数* ``path`` 路径(绝对或相对):``str``
+-  *参数* ``path`` 路径(绝对或相对):``str``
+
    -  *属性* ``partition`` 将路径(不包含驱动器)切片
    -  *方法* ``add`` 将内容加载路径后面
    -  *方法* ``findRest`` 去除两个路径的共同部分
 
 -  ``compare``\ 提供比较文件夹的API
 
    -  *函数* ``compare`` 比较两个文件夹
 
       -  *参数* ``folder1&folder2`` *比较的文件夹:``Folder``*
-      -  *参数* ``compareContent`` 文件内容的比较方法
-
-         -  ``ignore`` 忽略文件内容
-         -  ``hash`` 比较文件哈希值
-         -  ``content`` 比较文件内容
-         -  ``size`` 比较文件大小
-
+      -  *参数* ``compareContent``
+         文件内容的比较方法:``str|Callable[[doFolder.File,doFolder.File],bool]``
       -  *参数* ``threaded`` 是否线程化 ``bool``
       -  *参数* ``threaded`` 最大线程数:``int``
       -  *返回* 比较结果:``CompareResult``
 
 命令行使用
 ~~~~~~~~~~
 
 .. code:: bash
 
-   compare Folder1 Folder2 [-c ignore|hash|content|size]
+   compare Folder1 Folder2 [-c ignore|hash|content|size] [-t [-n num]]
 
 具体作用参见
 
 .. code:: bash
 
    compare -h
```

### Comparing `doFolder-0.0.3/setup.py` & `doFolder-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'doFolder',
-    version = '0.0.3',
+    version = '0.0.4',
     keywords = ['file',"foler","path","filesystem"],
     description = 'download files quickly',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
@@ -19,16 +19,17 @@
     license = 'Mulan PSL v2',
     platforms=[
         "windows",
         "linux",
         "macos"
     ] ,
     classifiers = [
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: End Users/Desktop',
+        "Natural Language :: English",
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Operating System :: MacOS',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)'
     ],
     entry_points = {
```

