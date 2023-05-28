# Comparing `tmp/ifastapi-0.0.3.3-py3-none-any.whl.zip` & `tmp/ifastapi-0.0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 14788 bytes, number of entries: 22
--rw-rw-rw-  2.0 fat     3433 b- defN 23-May-28 02:21 iFastApi/__init__.py
+Zip file size: 14978 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     3012 b- defN 23-May-28 02:54 iFastApi/__init__.py
 -rw-rw-rw-  2.0 fat      884 b- defN 23-May-04 01:58 iFastApi/api/BaseModel.py
--rw-rw-rw-  2.0 fat     2927 b- defN 23-May-28 02:21 iFastApi/api/BaseRoute.py
+-rw-rw-rw-  2.0 fat     2934 b- defN 23-May-28 02:57 iFastApi/api/BaseRoute.py
 -rw-rw-rw-  2.0 fat      606 b- defN 23-May-04 01:58 iFastApi/api/RoureManager.py
 -rw-rw-rw-  2.0 fat      947 b- defN 23-May-04 01:58 iFastApi/api/RouteInfo.py
--rw-rw-rw-  2.0 fat       40 b- defN 23-May-28 02:21 iFastApi/api/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 02:57 iFastApi/api/__init__.py
 -rw-rw-rw-  2.0 fat      802 b- defN 23-Apr-23 10:00 iFastApi/db/BaseQuery.py
--rw-rw-rw-  2.0 fat     7007 b- defN 23-May-04 01:58 iFastApi/db/__init__.py
--rw-rw-rw-  2.0 fat       40 b- defN 23-May-28 02:21 iFastApi/jobs/__init__.py
+-rw-rw-rw-  2.0 fat     7016 b- defN 23-May-28 02:54 iFastApi/db/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 02:57 iFastApi/jobs/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-04 01:58 iFastApi/tests/__init__.py
 -rw-rw-rw-  2.0 fat      938 b- defN 23-May-28 02:21 iFastApi/tests/config.py
--rw-rw-rw-  2.0 fat      330 b- defN 23-May-04 01:58 iFastApi/utils/__init__.py
+-rw-rw-rw-  2.0 fat      258 b- defN 23-May-28 02:54 iFastApi/utils/__init__.py
 -rw-rw-rw-  2.0 fat      407 b- defN 23-May-28 02:21 iFastApi/utils/functionPipe.py
 -rw-rw-rw-  2.0 fat      164 b- defN 23-May-28 02:21 iFastApi/utils/globals.py
--rw-rw-rw-  2.0 fat     2155 b- defN 23-May-28 02:21 iFastApi/utils/iResponse.py
+-rw-rw-rw-  2.0 fat     2186 b- defN 23-May-28 02:54 iFastApi/utils/iResponse.py
 -rw-rw-rw-  2.0 fat     2461 b- defN 23-May-28 02:21 iFastApi/utils/jwtToken.py
 -rw-rw-rw-  2.0 fat      396 b- defN 23-May-04 01:58 iFastApi/utils/singleton.py
 -rw-rw-rw-  2.0 fat     3739 b- defN 23-Apr-24 10:54 iFastApi/utils/time.py
--rw-rw-rw-  2.0 fat      355 b- defN 23-May-28 02:26 ifastapi-0.0.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 02:26 ifastapi-0.0.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-28 02:26 ifastapi-0.0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1772 b- defN 23-May-28 02:26 ifastapi-0.0.3.3.dist-info/RECORD
-22 files, 29693 bytes uncompressed, 11910 bytes compressed:  59.9%
+-rw-rw-rw-  2.0 fat      258 b- defN 23-May-28 02:54 iFastApi/utils/toolfuns.py
+-rw-rw-rw-  2.0 fat      355 b- defN 23-May-28 02:57 ifastapi-0.0.3.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 02:57 ifastapi-0.0.3.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-28 02:57 ifastapi-0.0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1852 b- defN 23-May-28 02:57 ifastapi-0.0.3.4.dist-info/RECORD
+23 files, 29505 bytes uncompressed, 11972 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -48,20 +48,23 @@
 
 Filename: iFastApi/utils/singleton.py
 Comment: 
 
 Filename: iFastApi/utils/time.py
 Comment: 
 
-Filename: ifastapi-0.0.3.3.dist-info/METADATA
+Filename: iFastApi/utils/toolfuns.py
 Comment: 
 
-Filename: ifastapi-0.0.3.3.dist-info/WHEEL
+Filename: ifastapi-0.0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: ifastapi-0.0.3.3.dist-info/top_level.txt
+Filename: ifastapi-0.0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: ifastapi-0.0.3.3.dist-info/RECORD
+Filename: ifastapi-0.0.3.4.dist-info/top_level.txt
+Comment: 
+
+Filename: ifastapi-0.0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iFastApi/__init__.py

```diff
@@ -9,15 +9,15 @@
 from fastapi import FastAPI, Depends
 from starlette.exceptions import HTTPException
 from starlette.middleware.cors import CORSMiddleware
 
 from .utils.globals import g
 from .api.BaseRoute import BaseRoute
 from .db import DBManager
-from .utils.iResponse import HTTPStatus, Error, JSONResponse
+from .utils.iResponse import HTTPStatus, Error
 
 
 class IFastAPI:
     """
     config: 配置文件
         - ORIGINS: 允许跨域的域名 默认为'*'
     """
@@ -72,28 +72,14 @@
     async def global_exception_handler(request, exc):
         return Error(
             status_code=500,
             message="服务器内部错误"
         )
 
     @staticmethod
-    @app.exception_handler(Error)
-    async def unicorn_exception_handler(request: Request, exc: Error):
-        content = {
-            "success": False,
-            "status_code": exc.status_code,
-            "message": exc.message,
-        }
-        content.update(exc.data)
-        return JSONResponse(
-            status_code=200,
-            content=content
-        )
-
-    @staticmethod
     @app.exception_handler(RequestValidationError)
     async def validation_exception_handler(request, exc):
         D = IFastAPI.config.PARAM_TRANSLATE
         errors = exc.errors()
         locs = []
         for i in errors:
             if i.get('loc'):
```

## iFastApi/api/BaseRoute.py

```diff
@@ -1,18 +1,17 @@
 import inspect
 
 from fastapi import APIRouter
 
 from .BaseModel import ListModel, QueryModel, UpdateModel
 from .RoureManager import RouteManager
 from .RouteInfo import RouteInfo
-from ..utils import path_to_key
+from ..utils.toolfuns import path_to_key
 from ..utils.iResponse import Error, HTTPStatus
 
-
 class BaseRoute:
     __is_initialized = False
 
     def __init__(self, prefix=None):
         self._db = None
         _name = f'/{prefix or self.__class__.__name__.lower()}'
         self.router = APIRouter(prefix=_name)
```

## iFastApi/api/__init__.py

```diff
@@ -1,3 +0,0 @@
-00000000: 2320 4175 7468 6f72 3a20 4946 435a 540d  # Author: IFCZT.
-00000010: 0a23 2045 6d61 696c 3a20 6966 637a 7440  .# Email: ifczt@
-00000020: 7171 2e63 6f6d 0d0a                      qq.com..
```

## iFastApi/db/__init__.py

```diff
@@ -6,15 +6,15 @@
 from starlette.requests import Request
 
 from sqlalchemy import Column, Integer, SmallInteger, text, and_
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker, scoped_session
 
-from ..utils import path_to_key
+from ..utils.toolfuns import path_to_key
 from .BaseQuery import BaseQuery
 from ..utils.singleton import Singleton
 from ..utils.time import time as t
 
 
 @Singleton
 class DBManager:
```

## iFastApi/jobs/__init__.py

```diff
@@ -1,3 +0,0 @@
-00000000: 2320 4175 7468 6f72 3a20 4946 435a 540d  # Author: IFCZT.
-00000010: 0a23 2045 6d61 696c 3a20 6966 637a 7440  .# Email: ifczt@
-00000020: 7171 2e63 6f6d 0d0a                      qq.com..
```

## iFastApi/utils/__init__.py

```diff
@@ -1,18 +1,20 @@
 # Author: IFCZT
 # Email: ifczt@qq.com
-import re
 
 
-def path_to_key(path):
-    return re.sub(r'/', ':', path.strip('/'))
+
+
 
 
 # 多个装饰器合并
 # 列如 @icompose(classmethod, idb)
 def icompose(*funs):
     def deco(f):
         for fun in reversed(funs):
             f = fun(f)
         return f
 
     return deco
+
+
+
```

## iFastApi/utils/iResponse.py

```diff
@@ -31,11 +31,14 @@
 
 class Success(JSONResponse):
     def __init__(self, data=None, message=None, status_code=HTTPStatus.OK):
         body = {"success": True, "message": message, "data": data}
         super().__init__(content=body, status_code=status_code)
 
 
-class Error(JSONResponse):
-    def __init__(self, data=None, message=None, status_code=HTTPStatus.BAD_REQUEST):
-        body = {"is_success": False, "message": message, "data": data}
-        super().__init__(content=body, status_code=status_code)
+class Error(Exception):
+    def __init__(self, status_code: int = HTTPStatus.BAD_REQUEST, message: str = '未知错误', data=None):
+        if data is None:
+            data = {}
+        self.message = message
+        self.status_code = status_code
+        self.data = data
```

