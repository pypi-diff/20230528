# Comparing `tmp/ifastapi-0.0.3.4-py3-none-any.whl.zip` & `tmp/ifastapi-0.0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 14978 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat     3012 b- defN 23-May-28 02:54 iFastApi/__init__.py
+Zip file size: 14955 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     2851 b- defN 23-May-28 03:20 iFastApi/__init__.py
 -rw-rw-rw-  2.0 fat      884 b- defN 23-May-04 01:58 iFastApi/api/BaseModel.py
 -rw-rw-rw-  2.0 fat     2934 b- defN 23-May-28 02:57 iFastApi/api/BaseRoute.py
 -rw-rw-rw-  2.0 fat      606 b- defN 23-May-04 01:58 iFastApi/api/RoureManager.py
 -rw-rw-rw-  2.0 fat      947 b- defN 23-May-04 01:58 iFastApi/api/RouteInfo.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 02:57 iFastApi/api/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 03:20 iFastApi/api/__init__.py
 -rw-rw-rw-  2.0 fat      802 b- defN 23-Apr-23 10:00 iFastApi/db/BaseQuery.py
 -rw-rw-rw-  2.0 fat     7016 b- defN 23-May-28 02:54 iFastApi/db/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 02:57 iFastApi/jobs/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 03:20 iFastApi/jobs/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-04 01:58 iFastApi/tests/__init__.py
 -rw-rw-rw-  2.0 fat      938 b- defN 23-May-28 02:21 iFastApi/tests/config.py
 -rw-rw-rw-  2.0 fat      258 b- defN 23-May-28 02:54 iFastApi/utils/__init__.py
 -rw-rw-rw-  2.0 fat      407 b- defN 23-May-28 02:21 iFastApi/utils/functionPipe.py
 -rw-rw-rw-  2.0 fat      164 b- defN 23-May-28 02:21 iFastApi/utils/globals.py
--rw-rw-rw-  2.0 fat     2186 b- defN 23-May-28 02:54 iFastApi/utils/iResponse.py
+-rw-rw-rw-  2.0 fat     2453 b- defN 23-May-28 03:20 iFastApi/utils/iResponse.py
 -rw-rw-rw-  2.0 fat     2461 b- defN 23-May-28 02:21 iFastApi/utils/jwtToken.py
 -rw-rw-rw-  2.0 fat      396 b- defN 23-May-04 01:58 iFastApi/utils/singleton.py
 -rw-rw-rw-  2.0 fat     3739 b- defN 23-Apr-24 10:54 iFastApi/utils/time.py
 -rw-rw-rw-  2.0 fat      258 b- defN 23-May-28 02:54 iFastApi/utils/toolfuns.py
--rw-rw-rw-  2.0 fat      355 b- defN 23-May-28 02:57 ifastapi-0.0.3.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 02:57 ifastapi-0.0.3.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-28 02:57 ifastapi-0.0.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1852 b- defN 23-May-28 02:57 ifastapi-0.0.3.4.dist-info/RECORD
-23 files, 29505 bytes uncompressed, 11972 bytes compressed:  59.4%
+-rw-rw-rw-  2.0 fat      355 b- defN 23-May-28 03:21 ifastapi-0.0.3.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 03:21 ifastapi-0.0.3.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-28 03:21 ifastapi-0.0.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1852 b- defN 23-May-28 03:21 ifastapi-0.0.3.5.dist-info/RECORD
+23 files, 29611 bytes uncompressed, 11949 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: iFastApi/utils/time.py
 Comment: 
 
 Filename: iFastApi/utils/toolfuns.py
 Comment: 
 
-Filename: ifastapi-0.0.3.4.dist-info/METADATA
+Filename: ifastapi-0.0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: ifastapi-0.0.3.4.dist-info/WHEEL
+Filename: ifastapi-0.0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: ifastapi-0.0.3.4.dist-info/top_level.txt
+Filename: ifastapi-0.0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ifastapi-0.0.3.4.dist-info/RECORD
+Filename: ifastapi-0.0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iFastApi/__init__.py

```diff
@@ -1,22 +1,18 @@
 # Author: IFCZT
 # Email: ifczt@qq.com
-import atexit
-from urllib.request import Request
 
-from fastapi.exception_handlers import request_validation_exception_handler
-from fastapi.exceptions import ValidationError, RequestValidationError
-import uvicorn
 from fastapi import FastAPI, Depends
+from fastapi.exceptions import RequestValidationError
 from starlette.exceptions import HTTPException
 from starlette.middleware.cors import CORSMiddleware
 
-from .utils.globals import g
 from .api.BaseRoute import BaseRoute
 from .db import DBManager
+from .utils.globals import g
 from .utils.iResponse import HTTPStatus, Error
 
 
 class IFastAPI:
     """
     config: 配置文件
         - ORIGINS: 允许跨域的域名 默认为'*'
```

## iFastApi/utils/iResponse.py

```diff
@@ -31,14 +31,20 @@
 
 class Success(JSONResponse):
     def __init__(self, data=None, message=None, status_code=HTTPStatus.OK):
         body = {"success": True, "message": message, "data": data}
         super().__init__(content=body, status_code=status_code)
 
 
-class Error(Exception):
-    def __init__(self, status_code: int = HTTPStatus.BAD_REQUEST, message: str = '未知错误', data=None):
-        if data is None:
-            data = {}
-        self.message = message
-        self.status_code = status_code
-        self.data = data
+class Error(JSONResponse):
+    def __init__(self, data=None, message=None, status_code=HTTPStatus.BAD_REQUEST):
+        body = {"is_success": False, "message": message, "data": data}
+        super().__init__(content=body, status_code=status_code)
+
+
+# class Error(Exception):
+#     def __init__(self, status_code: int = HTTPStatus.BAD_REQUEST, message: str = '未知错误', data=None):
+#         if data is None:
+#             data = {}
+#         self.message = message
+#         self.status_code = status_code
+#         self.data = data
```

## Comparing `ifastapi-0.0.3.4.dist-info/RECORD` & `ifastapi-0.0.3.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-iFastApi/__init__.py,sha256=OvP0Ex3Uy0q71dnPYyJxElUrQGF36fKoCSWgmClR7aU,3012
+iFastApi/__init__.py,sha256=yYjJFK0jfYACa7pnjIUWsUivuGaygcl9QsHc0CZvOfU,2851
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
-iFastApi/utils/iResponse.py,sha256=FZE34tLOeNemcwktDAgjKU68XerTSZX9PsMIkhDt7M8,2186
+iFastApi/utils/iResponse.py,sha256=6KrmyLKAmnLUK8YRqmTnTDe4FB8OVZ5Qr8h4o8q_WuU,2453
 iFastApi/utils/jwtToken.py,sha256=uqZ7RB7-6GWZJlkgcEQR3I2T0tRKIdGwf2Rxez-c900,2461
 iFastApi/utils/singleton.py,sha256=XpzG6YhDrg74n9dq-RTPozlAi3hByf5JWJwOYyM8Z-0,396
 iFastApi/utils/time.py,sha256=EchJPTqqKQ52aPMTS5IAWbEYQXWfwoogn5yHIceW-mE,3739
 iFastApi/utils/toolfuns.py,sha256=69FP3FjR6-FTkaX1QuKIkRo2qI3jq2rptB04ePAXCpQ,258
-ifastapi-0.0.3.4.dist-info/METADATA,sha256=-hJSU2ZKhGyqHvzrltYCEt2W9HQYIh-Ho8_YgJ5mOZk,355
-ifastapi-0.0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ifastapi-0.0.3.4.dist-info/top_level.txt,sha256=52hwNyIJr9Ehl5tfXXlfkFOg7ZC9uzMGDnCLQQstEwU,9
-ifastapi-0.0.3.4.dist-info/RECORD,,
+ifastapi-0.0.3.5.dist-info/METADATA,sha256=ioXXLMiH2pkK5GxDGkqaqnGE79HZdJuvxVIFzLQoXIw,355
+ifastapi-0.0.3.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ifastapi-0.0.3.5.dist-info/top_level.txt,sha256=52hwNyIJr9Ehl5tfXXlfkFOg7ZC9uzMGDnCLQQstEwU,9
+ifastapi-0.0.3.5.dist-info/RECORD,,
```

