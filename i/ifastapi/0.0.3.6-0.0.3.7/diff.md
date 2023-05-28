# Comparing `tmp/ifastapi-0.0.3.6-py3-none-any.whl.zip` & `tmp/ifastapi-0.0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 15087 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat     3308 b- defN 23-May-28 05:15 iFastApi/__init__.py
+Zip file size: 15082 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     3356 b- defN 23-May-28 06:15 iFastApi/__init__.py
 -rw-rw-rw-  2.0 fat      884 b- defN 23-May-04 01:58 iFastApi/api/BaseModel.py
 -rw-rw-rw-  2.0 fat     2934 b- defN 23-May-28 02:57 iFastApi/api/BaseRoute.py
 -rw-rw-rw-  2.0 fat      606 b- defN 23-May-04 01:58 iFastApi/api/RoureManager.py
 -rw-rw-rw-  2.0 fat      947 b- defN 23-May-04 01:58 iFastApi/api/RouteInfo.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 05:15 iFastApi/api/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 06:15 iFastApi/api/__init__.py
 -rw-rw-rw-  2.0 fat      802 b- defN 23-Apr-23 10:00 iFastApi/db/BaseQuery.py
 -rw-rw-rw-  2.0 fat     7016 b- defN 23-May-28 02:54 iFastApi/db/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 05:15 iFastApi/jobs/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 06:15 iFastApi/jobs/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-04 01:58 iFastApi/tests/__init__.py
 -rw-rw-rw-  2.0 fat      938 b- defN 23-May-28 02:21 iFastApi/tests/config.py
 -rw-rw-rw-  2.0 fat      258 b- defN 23-May-28 02:54 iFastApi/utils/__init__.py
 -rw-rw-rw-  2.0 fat      407 b- defN 23-May-28 02:21 iFastApi/utils/functionPipe.py
 -rw-rw-rw-  2.0 fat      164 b- defN 23-May-28 02:21 iFastApi/utils/globals.py
--rw-rw-rw-  2.0 fat     2447 b- defN 23-May-28 05:15 iFastApi/utils/iResponse.py
+-rw-rw-rw-  2.0 fat     2359 b- defN 23-May-28 06:15 iFastApi/utils/iResponse.py
 -rw-rw-rw-  2.0 fat     2461 b- defN 23-May-28 02:21 iFastApi/utils/jwtToken.py
 -rw-rw-rw-  2.0 fat      396 b- defN 23-May-04 01:58 iFastApi/utils/singleton.py
 -rw-rw-rw-  2.0 fat     3739 b- defN 23-Apr-24 10:54 iFastApi/utils/time.py
 -rw-rw-rw-  2.0 fat      258 b- defN 23-May-28 02:54 iFastApi/utils/toolfuns.py
--rw-rw-rw-  2.0 fat      355 b- defN 23-May-28 05:15 ifastapi-0.0.3.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 05:15 ifastapi-0.0.3.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-28 05:15 ifastapi-0.0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1852 b- defN 23-May-28 05:15 ifastapi-0.0.3.6.dist-info/RECORD
-23 files, 30062 bytes uncompressed, 12081 bytes compressed:  59.8%
+-rw-rw-rw-  2.0 fat      355 b- defN 23-May-28 06:15 ifastapi-0.0.3.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 06:15 ifastapi-0.0.3.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-28 06:15 ifastapi-0.0.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1852 b- defN 23-May-28 06:15 ifastapi-0.0.3.7.dist-info/RECORD
+23 files, 30022 bytes uncompressed, 12076 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: iFastApi/utils/time.py
 Comment: 
 
 Filename: iFastApi/utils/toolfuns.py
 Comment: 
 
-Filename: ifastapi-0.0.3.6.dist-info/METADATA
+Filename: ifastapi-0.0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: ifastapi-0.0.3.6.dist-info/WHEEL
+Filename: ifastapi-0.0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: ifastapi-0.0.3.6.dist-info/top_level.txt
+Filename: ifastapi-0.0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ifastapi-0.0.3.6.dist-info/RECORD
+Filename: ifastapi-0.0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iFastApi/__init__.py

```diff
@@ -1,14 +1,14 @@
 # Author: IFCZT
 # Email: ifczt@qq.com
 from urllib.request import Request
 
 from fastapi import FastAPI, Depends
 from fastapi.exceptions import RequestValidationError
-from starlette.exceptions import HTTPException
+from starlette.exceptions import HTTPException as StarletteException
 from starlette.middleware.cors import CORSMiddleware
 
 from .api.BaseRoute import BaseRoute
 from .db import DBManager
 from .utils.globals import g
 from .utils.iResponse import HTTPStatus, Error, JSONResponse
 
@@ -49,56 +49,56 @@
 
     def run(self, config):
         self.config = IFastAPI.config = config
         g.config = config
         self.setup()
 
     @staticmethod
-    @app.exception_handler(HTTPException)  # 自定义HttpRequest 请求异常
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
+    @app.exception_handler(StarletteException)  # 自定义HttpRequest 请求异常
     async def http_exception_handle(request, exc):
         match exc.status_code:
             case HTTPStatus.METHOD_NOT_ALLOWED:
                 message = '未定义该接口'
             case HTTPStatus.NOT_FOUND:
                 message = '访问接口不存在'
             case _:
                 message = exc.detail
-        return Error(message=message, status_code=exc.status_code)
+        return JSONResponse(message=message, status_code=exc.status_code)
 
     @staticmethod
     @app.exception_handler(Exception)
     async def global_exception_handler(request, exc):
-        return Error(
+        return JSONResponse(
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
                 locs.extend(list(i.get('loc')))
         locs = list(set(locs))
         locs = [D.get(i, i) for i in locs]
         if 'body' in locs:
             locs.remove('body')
 
         message = f"参数[{','.join(locs) if isinstance(locs, list) else locs}]未通过验证" if locs else '未接受到任何有效参数'
-        return Error(message=message, status_code=HTTPStatus.UNPROCESSABLE_ENTITY)
+        return JSONResponse(message=message, status_code=HTTPStatus.UNPROCESSABLE_ENTITY)
```

## iFastApi/utils/iResponse.py

```diff
@@ -1,7 +1,8 @@
+from fastapi import HTTPException
 from starlette.responses import JSONResponse as _JSONResponse
 
 from ..db import BaseDB
 
 
 class HTTPStatus:
     OK = 200  # 请求成功
@@ -18,33 +19,34 @@
     INTERNAL_SERVER_ERROR = 500  # 服务器内部错误
     BAD_GATEWAY = 502  # 服务器作为网关或者代理，从上游服务器接收到了一个无效的响应
     SERVICE_UNAVAILABLE = 503  # 请求的服务不可用
     GATEWAY_TIMEOUT = 504  # 作为网关或代理的服务器在等待上游服务器响应时超时
 
 
 class JSONResponse(_JSONResponse):
-    def __init__(self, content=None, status_code=HTTPStatus.OK, headers=None, media_type=None, background=None):
+    def __init__(self, content=None, message=None, status_code=HTTPStatus.OK, headers=None, media_type=None, background=None):
+        if content is None:
+            content = {}
         content = dict(filter(lambda item: item[1] is not None and item[1] != '', content.items()))
         if isinstance(content.get('data', None), BaseDB):
             content['data'] = dict(content['data'])
+        if message:
+            content['message'] = message
         super().__init__(content=content, status_code=status_code, headers=headers, media_type=media_type, background=background)
 
 
-class Success(JSONResponse):
-    def __init__(self, data=None, message=None, status_code=HTTPStatus.OK):
-        body = {"success": True, "message": message, "data": data}
-        super().__init__(content=body, status_code=status_code)
-
-
-# class Error(JSONResponse):
-#     def __init__(self, data=None, message=None, status_code=HTTPStatus.BAD_REQUEST):
-#         body = {"is_success": False, "message": message, "data": data}
-#         super().__init__(content=body, status_code=status_code)
-
-
 class Error(Exception):
     def __init__(self, status_code: int = HTTPStatus.BAD_REQUEST, message: str = '未知错误', data=None):
         if data is None:
             data = {}
+
         self.message = message
         self.status_code = status_code
-        self.data = data
+        self.data = data
+
+
+class Success(JSONResponse):
+    def __init__(self, data=None, message=None, status_code=HTTPStatus.OK):
+        body = {"success": True, "message": message, "data": data}
+        super().__init__(content=body, status_code=status_code)
+
+
```

## Comparing `ifastapi-0.0.3.6.dist-info/RECORD` & `ifastapi-0.0.3.7.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-iFastApi/__init__.py,sha256=6hJXCBnZHRyQ6jrUmW7vRVfbZza7tJfT4oiLCtU1rkE,3308
+iFastApi/__init__.py,sha256=tMQsN6qIS-cw5PwG-v0ofkH9A_7GHHZfG7zenvZ9iUk,3356
 iFastApi/api/BaseModel.py,sha256=O0NHf41fPNxydmmJeZzgZLTOW3zUjS4evVIq7pN6FCE,884
 iFastApi/api/BaseRoute.py,sha256=8crY_j2d7w7Q0TvqW6-nv5GQFt-yrEjmM_5pxpqXr9g,2934
 iFastApi/api/RoureManager.py,sha256=1Qlbpw1y9PjA2i1sQMVuHMF1XWj5g_Djsf175CunavI,606
 iFastApi/api/RouteInfo.py,sha256=GgLH6dN3wPF4gRVxx-vZQ-x5ZSVg0TMCFRBDIMqcAQw,947
 iFastApi/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 iFastApi/db/BaseQuery.py,sha256=AXp0ehNPoPO9hXQ0OLoDO7mbpwvCuqEIqitc1zKuFeM,802
 iFastApi/db/__init__.py,sha256=y_m-7264oqj3suSPwLQQxbkJ7BleBsqZ2i5tWV8W06o,7016
 iFastApi/jobs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 iFastApi/tests/__init__.py,sha256=VEN_qiGMp1ie6M3QadOV1XJZQaZMUzVX4akSRJCQsGw,189
 iFastApi/tests/config.py,sha256=eTV43qIlOIyiimFHt-qpe5so5AdjOE1YEGZnTnv_0MA,938
 iFastApi/utils/__init__.py,sha256=lhcPwK-Q1n4omVhoSXCCygQOLOUZ1etHqoqiCSK-FhI,258
 iFastApi/utils/functionPipe.py,sha256=3REtMcT5_KYPTk_5mNKaC3L8XfF7bv8iVm1WPd7u1N0,407
 iFastApi/utils/globals.py,sha256=qsryfGLuSZHx-Jdd7EGMWr9g1WUQ1sNAdtW8sUHQwzQ,164
-iFastApi/utils/iResponse.py,sha256=e2txNEo5D43Uo3VVnLwmTQ7pkp6aI1UrSoaHBlC6Ybw,2447
+iFastApi/utils/iResponse.py,sha256=ahM-hNyde9mMyGAJoYUt2IZ3sV8awol_JqupR_HVDug,2359
 iFastApi/utils/jwtToken.py,sha256=uqZ7RB7-6GWZJlkgcEQR3I2T0tRKIdGwf2Rxez-c900,2461
 iFastApi/utils/singleton.py,sha256=XpzG6YhDrg74n9dq-RTPozlAi3hByf5JWJwOYyM8Z-0,396
 iFastApi/utils/time.py,sha256=EchJPTqqKQ52aPMTS5IAWbEYQXWfwoogn5yHIceW-mE,3739
 iFastApi/utils/toolfuns.py,sha256=69FP3FjR6-FTkaX1QuKIkRo2qI3jq2rptB04ePAXCpQ,258
-ifastapi-0.0.3.6.dist-info/METADATA,sha256=Bu3tH9PS6CnMCNICDBwWpp7_avlQ0PftfV5wXKDpM3U,355
-ifastapi-0.0.3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ifastapi-0.0.3.6.dist-info/top_level.txt,sha256=52hwNyIJr9Ehl5tfXXlfkFOg7ZC9uzMGDnCLQQstEwU,9
-ifastapi-0.0.3.6.dist-info/RECORD,,
+ifastapi-0.0.3.7.dist-info/METADATA,sha256=odPpqyO4pgFxpA6v_zbZlQCX4SZpd_66NuVjEN_px4o,355
+ifastapi-0.0.3.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ifastapi-0.0.3.7.dist-info/top_level.txt,sha256=52hwNyIJr9Ehl5tfXXlfkFOg7ZC9uzMGDnCLQQstEwU,9
+ifastapi-0.0.3.7.dist-info/RECORD,,
```

