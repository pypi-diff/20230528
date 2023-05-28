# Comparing `tmp/ifastapi-0.0.3.2.1-py3-none-any.whl.zip` & `tmp/ifastapi-0.0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,24 @@
-Zip file size: 11978 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     2955 b- defN 23-May-04 01:58 iFastApi/__init__.py
+Zip file size: 14788 bytes, number of entries: 22
+-rw-rw-rw-  2.0 fat     3433 b- defN 23-May-28 02:21 iFastApi/__init__.py
 -rw-rw-rw-  2.0 fat      884 b- defN 23-May-04 01:58 iFastApi/api/BaseModel.py
--rw-rw-rw-  2.0 fat     2817 b- defN 23-May-04 01:58 iFastApi/api/BaseRoute.py
+-rw-rw-rw-  2.0 fat     2927 b- defN 23-May-28 02:21 iFastApi/api/BaseRoute.py
 -rw-rw-rw-  2.0 fat      606 b- defN 23-May-04 01:58 iFastApi/api/RoureManager.py
 -rw-rw-rw-  2.0 fat      947 b- defN 23-May-04 01:58 iFastApi/api/RouteInfo.py
--rw-rw-rw-  2.0 fat       40 b- defN 23-May-04 03:53 iFastApi/api/__init__.py
+-rw-rw-rw-  2.0 fat       40 b- defN 23-May-28 02:21 iFastApi/api/__init__.py
 -rw-rw-rw-  2.0 fat      802 b- defN 23-Apr-23 10:00 iFastApi/db/BaseQuery.py
 -rw-rw-rw-  2.0 fat     7007 b- defN 23-May-04 01:58 iFastApi/db/__init__.py
--rw-rw-rw-  2.0 fat       40 b- defN 23-May-04 03:53 iFastApi/jobs/__init__.py
+-rw-rw-rw-  2.0 fat       40 b- defN 23-May-28 02:21 iFastApi/jobs/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-04 01:58 iFastApi/tests/__init__.py
+-rw-rw-rw-  2.0 fat      938 b- defN 23-May-28 02:21 iFastApi/tests/config.py
 -rw-rw-rw-  2.0 fat      330 b- defN 23-May-04 01:58 iFastApi/utils/__init__.py
--rw-rw-rw-  2.0 fat     2155 b- defN 23-May-04 01:58 iFastApi/utils/iResponse.py
+-rw-rw-rw-  2.0 fat      407 b- defN 23-May-28 02:21 iFastApi/utils/functionPipe.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-May-28 02:21 iFastApi/utils/globals.py
+-rw-rw-rw-  2.0 fat     2155 b- defN 23-May-28 02:21 iFastApi/utils/iResponse.py
+-rw-rw-rw-  2.0 fat     2461 b- defN 23-May-28 02:21 iFastApi/utils/jwtToken.py
 -rw-rw-rw-  2.0 fat      396 b- defN 23-May-04 01:58 iFastApi/utils/singleton.py
 -rw-rw-rw-  2.0 fat     3739 b- defN 23-Apr-24 10:54 iFastApi/utils/time.py
--rw-rw-rw-  2.0 fat      357 b- defN 23-May-04 03:53 ifastapi-0.0.3.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 03:53 ifastapi-0.0.3.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-04 03:53 ifastapi-0.0.3.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1450 b- defN 23-May-04 03:53 ifastapi-0.0.3.2.1.dist-info/RECORD
-18 files, 24815 bytes uncompressed, 9598 bytes compressed:  61.3%
+-rw-rw-rw-  2.0 fat      355 b- defN 23-May-28 02:26 ifastapi-0.0.3.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 02:26 ifastapi-0.0.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-28 02:26 ifastapi-0.0.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1772 b- defN 23-May-28 02:26 ifastapi-0.0.3.3.dist-info/RECORD
+22 files, 29693 bytes uncompressed, 11910 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -24,32 +24,44 @@
 
 Filename: iFastApi/jobs/__init__.py
 Comment: 
 
 Filename: iFastApi/tests/__init__.py
 Comment: 
 
+Filename: iFastApi/tests/config.py
+Comment: 
+
 Filename: iFastApi/utils/__init__.py
 Comment: 
 
+Filename: iFastApi/utils/functionPipe.py
+Comment: 
+
+Filename: iFastApi/utils/globals.py
+Comment: 
+
 Filename: iFastApi/utils/iResponse.py
 Comment: 
 
+Filename: iFastApi/utils/jwtToken.py
+Comment: 
+
 Filename: iFastApi/utils/singleton.py
 Comment: 
 
 Filename: iFastApi/utils/time.py
 Comment: 
 
-Filename: ifastapi-0.0.3.2.1.dist-info/METADATA
+Filename: ifastapi-0.0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: ifastapi-0.0.3.2.1.dist-info/WHEEL
+Filename: ifastapi-0.0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: ifastapi-0.0.3.2.1.dist-info/top_level.txt
+Filename: ifastapi-0.0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ifastapi-0.0.3.2.1.dist-info/RECORD
+Filename: ifastapi-0.0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iFastApi/__init__.py

```diff
@@ -6,17 +6,18 @@
 from fastapi.exception_handlers import request_validation_exception_handler
 from fastapi.exceptions import ValidationError, RequestValidationError
 import uvicorn
 from fastapi import FastAPI, Depends
 from starlette.exceptions import HTTPException
 from starlette.middleware.cors import CORSMiddleware
 
+from .utils.globals import g
 from .api.BaseRoute import BaseRoute
 from .db import DBManager
-from .utils.iResponse import HTTPStatus, Error
+from .utils.iResponse import HTTPStatus, Error, JSONResponse
 
 
 class IFastAPI:
     """
     config: 配置文件
         - ORIGINS: 允许跨域的域名 默认为'*'
     """
@@ -47,14 +48,15 @@
 
     def setup_route(self):
         """配置路由"""
         BaseRoute.init_router(self.app)
 
     def run(self, config):
         self.config = IFastAPI.config = config
+        g.config = config
         self.setup()
 
     @staticmethod
     @app.exception_handler(HTTPException)  # 自定义HttpRequest 请求异常
     async def http_exception_handle(request, exc):
         match exc.status_code:
             case HTTPStatus.METHOD_NOT_ALLOWED:
@@ -70,14 +72,28 @@
     async def global_exception_handler(request, exc):
         return Error(
             status_code=500,
             message="服务器内部错误"
         )
 
     @staticmethod
+    @app.exception_handler(Error)
+    async def unicorn_exception_handler(request: Request, exc: Error):
+        content = {
+            "success": False,
+            "status_code": exc.status_code,
+            "message": exc.message,
+        }
+        content.update(exc.data)
+        return JSONResponse(
+            status_code=200,
+            content=content
+        )
+
+    @staticmethod
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
@@ -2,14 +2,15 @@
 
 from fastapi import APIRouter
 
 from .BaseModel import ListModel, QueryModel, UpdateModel
 from .RoureManager import RouteManager
 from .RouteInfo import RouteInfo
 from ..utils import path_to_key
+from ..utils.iResponse import Error, HTTPStatus
 
 
 class BaseRoute:
     __is_initialized = False
 
     def __init__(self, prefix=None):
         self._db = None
@@ -24,15 +25,15 @@
         ]
         self.roure_manager = RouteManager()
         self.routers = []
 
     @property
     def db(self):
         if not self._db:
-            raise NotImplementedError()
+            raise Error(message='未初始化数据库', status_code=HTTPStatus.SERVICE_UNAVAILABLE)
         return self._db
 
     @db.setter
     def db(self, db):
         self._db = db
 
     def remove(self, data: QueryModel):
```

## Comparing `ifastapi-0.0.3.2.1.dist-info/RECORD` & `ifastapi-0.0.3.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-iFastApi/__init__.py,sha256=MH6d0eoWiPQnA1pg4RJ-zwFz8ar1pi2LDFymgk3oCN0,2955
+iFastApi/__init__.py,sha256=kkdkCP9SxbAQvnO-PohDqGp4Q-Bk7_v2hR_e_a9X79M,3433
 iFastApi/api/BaseModel.py,sha256=O0NHf41fPNxydmmJeZzgZLTOW3zUjS4evVIq7pN6FCE,884
-iFastApi/api/BaseRoute.py,sha256=SW7meAR5Yd6zA0upOSp4-rVoQkxgSFBFCdbQigipMxI,2817
+iFastApi/api/BaseRoute.py,sha256=rJODMOeCEbR_h3_0pzKvZOPGJ8gCPfYmTwzPe7CAXIk,2927
 iFastApi/api/RoureManager.py,sha256=1Qlbpw1y9PjA2i1sQMVuHMF1XWj5g_Djsf175CunavI,606
 iFastApi/api/RouteInfo.py,sha256=GgLH6dN3wPF4gRVxx-vZQ-x5ZSVg0TMCFRBDIMqcAQw,947
 iFastApi/api/__init__.py,sha256=h9qkXQA_IyzgWqqzonzFDdm1N58G3XwQdq2cV9ny6eo,40
 iFastApi/db/BaseQuery.py,sha256=AXp0ehNPoPO9hXQ0OLoDO7mbpwvCuqEIqitc1zKuFeM,802
 iFastApi/db/__init__.py,sha256=MEe3WlnbDWRvRa8bw2OujJEVvDAHOvDhAXrIRurazuI,7007
 iFastApi/jobs/__init__.py,sha256=h9qkXQA_IyzgWqqzonzFDdm1N58G3XwQdq2cV9ny6eo,40
 iFastApi/tests/__init__.py,sha256=VEN_qiGMp1ie6M3QadOV1XJZQaZMUzVX4akSRJCQsGw,189
+iFastApi/tests/config.py,sha256=eTV43qIlOIyiimFHt-qpe5so5AdjOE1YEGZnTnv_0MA,938
 iFastApi/utils/__init__.py,sha256=-5UKDLDRdghm9Cdv9Lzzvm4KgdQiIZU3bUOxwTvFuG4,330
+iFastApi/utils/functionPipe.py,sha256=3REtMcT5_KYPTk_5mNKaC3L8XfF7bv8iVm1WPd7u1N0,407
+iFastApi/utils/globals.py,sha256=qsryfGLuSZHx-Jdd7EGMWr9g1WUQ1sNAdtW8sUHQwzQ,164
 iFastApi/utils/iResponse.py,sha256=7LK-WLlb4b2a1UqEZeHjsbIZCsgGTR5OUudIHDwkr2Q,2155
+iFastApi/utils/jwtToken.py,sha256=uqZ7RB7-6GWZJlkgcEQR3I2T0tRKIdGwf2Rxez-c900,2461
 iFastApi/utils/singleton.py,sha256=XpzG6YhDrg74n9dq-RTPozlAi3hByf5JWJwOYyM8Z-0,396
 iFastApi/utils/time.py,sha256=EchJPTqqKQ52aPMTS5IAWbEYQXWfwoogn5yHIceW-mE,3739
-ifastapi-0.0.3.2.1.dist-info/METADATA,sha256=5Qisqf71w_tlmrKMj1I7nIkVw_Hsni1FX5hj69UFwpc,357
-ifastapi-0.0.3.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ifastapi-0.0.3.2.1.dist-info/top_level.txt,sha256=52hwNyIJr9Ehl5tfXXlfkFOg7ZC9uzMGDnCLQQstEwU,9
-ifastapi-0.0.3.2.1.dist-info/RECORD,,
+ifastapi-0.0.3.3.dist-info/METADATA,sha256=31aG0tUtgbFK25ejH8CmGQC5uOyvgHxcCm0pg7MWhD8,355
+ifastapi-0.0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ifastapi-0.0.3.3.dist-info/top_level.txt,sha256=52hwNyIJr9Ehl5tfXXlfkFOg7ZC9uzMGDnCLQQstEwU,9
+ifastapi-0.0.3.3.dist-info/RECORD,,
```

