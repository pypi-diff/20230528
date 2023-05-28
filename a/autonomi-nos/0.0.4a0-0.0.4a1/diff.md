# Comparing `tmp/autonomi_nos-0.0.4a0-py3-none-any.whl.zip` & `tmp/autonomi_nos-0.0.4a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,28 @@
-Zip file size: 55583 bytes, number of entries: 57
+Zip file size: 55824 bytes, number of entries: 58
 -rw-rw-r--  2.0 unx       50 b- defN 23-May-21 21:25 nos/__init__.py
 -rw-rw-r--  2.0 unx      561 b- defN 23-May-16 21:26 nos/constants.py
 -rw-rw-r--  2.0 unx       93 b- defN 23-May-11 04:43 nos/exceptions.py
 -rw-rw-r--  2.0 unx      940 b- defN 23-May-09 22:15 nos/logging.py
 -rw-rw-r--  2.0 unx     2778 b- defN 23-May-19 22:25 nos/protoc.py
--rw-rw-r--  2.0 unx       23 b- defN 23-May-23 00:10 nos/version.py
+-rw-rw-r--  2.0 unx       24 b- defN 23-May-28 01:41 nos/version.py
 -rw-rw-r--  2.0 unx      110 b- defN 23-May-05 08:07 nos/cli/benchmark.py
 -rw-rw-r--  2.0 unx      455 b- defN 23-May-15 21:47 nos/cli/cli.py
 -rw-rw-r--  2.0 unx     1983 b- defN 23-May-15 21:47 nos/cli/docker.py
 -rw-rw-r--  2.0 unx     1294 b- defN 23-May-05 08:07 nos/cli/hub.py
 -rw-rw-r--  2.0 unx     6202 b- defN 23-May-26 22:01 nos/cli/serve_grpc.py
 -rw-rw-r--  2.0 unx     5962 b- defN 23-May-15 21:47 nos/cli/serve_http.py
 -rw-rw-r--  2.0 unx     3479 b- defN 23-May-15 21:47 nos/cli/system.py
 -rw-rw-r--  2.0 unx      425 b- defN 23-May-09 22:15 nos/cli/utils.py
 -rw-rw-r--  2.0 unx      372 b- defN 23-May-26 22:01 nos/client/__init__.py
 -rw-rw-r--  2.0 unx       92 b- defN 23-May-11 04:42 nos/client/exceptions.py
--rw-rw-r--  2.0 unx    12657 b- defN 23-May-26 22:01 nos/client/grpc.py
--rw-rw-r--  2.0 unx      286 b- defN 23-May-26 22:01 nos/common/__init__.py
--rw-rw-r--  2.0 unx     3715 b- defN 23-May-27 23:58 nos/common/spec.py
+-rw-rw-r--  2.0 unx    12621 b- defN 23-May-28 01:27 nos/client/grpc.py
+-rw-rw-r--  2.0 unx      235 b- defN 23-May-28 01:27 nos/common/__init__.py
+-rw-rw-r--  2.0 unx      178 b- defN 23-May-28 01:28 nos/common/cloudpickle.py
+-rw-rw-r--  2.0 unx     3720 b- defN 23-May-28 01:25 nos/common/spec.py
 -rw-rw-r--  2.0 unx      518 b- defN 23-May-26 22:01 nos/common/tasks.py
 -rw-rw-r--  2.0 unx     4851 b- defN 23-May-27 23:51 nos/common/types.py
 -rw-rw-r--  2.0 unx     3470 b- defN 23-May-08 23:12 nos/examples/vid2bbox.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-18 17:00 nos/executors/__init__.py
 -rw-rw-r--  2.0 unx     7401 b- defN 23-May-26 22:01 nos/executors/ray.py
 -rw-rw-r--  2.0 unx     1246 b- defN 23-May-15 21:47 nos/experimental/conversion_flows/openmmlab/tensorrt/run_model.py
 -rw-rw-r--  2.0 unx     4559 b- defN 23-May-15 21:47 nos/experimental/http/__init__.py
@@ -42,18 +43,18 @@
 -rw-rw-r--  2.0 unx      304 b- defN 23-May-09 22:15 nos/models/openmmlab/mmdetection/configs/_base_/schedules/schedule_1x.py
 -rw-rw-r--  2.0 unx     5340 b- defN 23-May-09 22:15 nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py
 -rw-rw-r--  2.0 unx      177 b- defN 23-May-10 02:43 nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py
 -rw-rw-r--  2.0 unx     2437 b- defN 23-May-26 22:01 nos/proto/nos_service.proto
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-23 17:24 nos/server/__init__.py
 -rw-rw-r--  2.0 unx     6229 b- defN 23-May-19 03:42 nos/server/docker.py
 -rw-rw-r--  2.0 unx     2976 b- defN 23-May-22 17:53 nos/server/runtime.py
--rw-rw-r--  2.0 unx     9887 b- defN 23-May-26 22:01 nos/server/service.py
+-rw-rw-r--  2.0 unx     9887 b- defN 23-May-28 01:27 nos/server/service.py
 -rw-rw-r--  2.0 unx      373 b- defN 23-May-05 08:07 nos/test/benchmark.py
 -rw-rw-r--  2.0 unx     5764 b- defN 23-May-26 22:01 nos/test/conftest.py
 -rw-rw-r--  2.0 unx     1347 b- defN 23-May-21 21:52 nos/test/utils.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6257 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4934 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/RECORD
-57 files, 144316 bytes uncompressed, 47687 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-28 01:42 autonomi_nos-0.0.4a1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6257 b- defN 23-May-28 01:42 autonomi_nos-0.0.4a1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-28 01:42 autonomi_nos-0.0.4a1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-28 01:42 autonomi_nos-0.0.4a1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 23-May-28 01:42 autonomi_nos-0.0.4a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5015 b- defN 23-May-28 01:42 autonomi_nos-0.0.4a1.dist-info/RECORD
+58 files, 144494 bytes uncompressed, 47802 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -48,14 +48,17 @@
 
 Filename: nos/client/grpc.py
 Comment: 
 
 Filename: nos/common/__init__.py
 Comment: 
 
+Filename: nos/common/cloudpickle.py
+Comment: 
+
 Filename: nos/common/spec.py
 Comment: 
 
 Filename: nos/common/tasks.py
 Comment: 
 
 Filename: nos/common/types.py
@@ -147,26 +150,26 @@
 
 Filename: nos/test/conftest.py
 Comment: 
 
 Filename: nos/test/utils.py
 Comment: 
 
-Filename: autonomi_nos-0.0.4a0.dist-info/LICENSE
+Filename: autonomi_nos-0.0.4a1.dist-info/LICENSE
 Comment: 
 
-Filename: autonomi_nos-0.0.4a0.dist-info/METADATA
+Filename: autonomi_nos-0.0.4a1.dist-info/METADATA
 Comment: 
 
-Filename: autonomi_nos-0.0.4a0.dist-info/WHEEL
+Filename: autonomi_nos-0.0.4a1.dist-info/WHEEL
 Comment: 
 
-Filename: autonomi_nos-0.0.4a0.dist-info/entry_points.txt
+Filename: autonomi_nos-0.0.4a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: autonomi_nos-0.0.4a0.dist-info/top_level.txt
+Filename: autonomi_nos-0.0.4a1.dist-info/top_level.txt
 Comment: 
 
-Filename: autonomi_nos-0.0.4a0.dist-info/RECORD
+Filename: autonomi_nos-0.0.4a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nos/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.4a"
+__version__ = "0.0.4a1"
```

## nos/client/grpc.py

```diff
@@ -1,21 +1,20 @@
 """gRPC client for NOS service."""
 import time
 from dataclasses import dataclass, field
 from functools import lru_cache
 from typing import Any, Callable, Dict, List, Union
 
-import cloudpickle
 import grpc
 import numpy as np
 from google.protobuf import empty_pb2
 from PIL import Image
 
 from nos.client.exceptions import NosClientException
-from nos.common import ModelSpec, TaskType
+from nos.common import ModelSpec, TaskType, loads
 from nos.constants import DEFAULT_GRPC_PORT
 from nos.logging import logger
 from nos.protoc import import_module
 from nos.version import __version__
 
 
 nos_service_pb2 = import_module("nos_service_pb2")
@@ -203,15 +202,15 @@
         try:
             response: nos_service_pb2.ModelInfoResponse = self.stub.GetModelInfo(
                 nos_service_pb2.ModelInfoRequest(
                     request=nos_service_pb2.ModelInfo(task=model_spec.task.value, name=model_spec.name)
                 )
             )
             logger.debug(response)
-            spec: ModelSpec = cloudpickle.loads(response.response_bytes)
+            spec: ModelSpec = loads(response.response_bytes)
             return spec
         except grpc.RpcError as e:
             raise NosClientException(f"Failed to get model info ({e})")
 
     @lru_cache(maxsize=32)  # noqa: B019
     def Module(self, task: TaskType, model_name: str) -> "InferenceModule":
         """Instantiate a model module.
@@ -327,12 +326,12 @@
                 task=self.task.value,
                 name=self.model_name,
             ),
             inputs=inputs,
         )
         try:
             response = self.stub.Run(request)
-            response = cloudpickle.loads(response.response_bytes)
+            response = loads(response.response_bytes)
             logger.debug(response)
             return response
         except grpc.RpcError as e:
             raise NosClientException(f"Failed to run model {self.model_name} ({e})")
```

## nos/common/__init__.py

```diff
@@ -1,11 +1,6 @@
 from typing import Any
 
-import cloudpickle
-
+from .cloudpickle import dumps, loads
 from .spec import FunctionSignature, ModelSpec  # noqa: F401
 from .tasks import TaskType  # noqa: F401
 from .types import EmbeddingSpec, ImageSpec, TensorSpec  # noqa: F401
-
-
-def dumps(obj: Any):
-    return cloudpickle.dumps(obj, protocol=4)
```

## nos/common/spec.py

```diff
@@ -1,14 +1,14 @@
 from dataclasses import field
 from typing import Any, Callable, Dict, Optional, Tuple, Type, Union
 
-import cloudpickle
 from pydantic import validator
 from pydantic.dataclasses import dataclass
 
+from nos.common.cloudpickle import dumps, loads
 from nos.common.tasks import TaskType
 from nos.common.types import EmbeddingSpec, ImageSpec, TensorSpec  # noqa: F401
 
 
 @dataclass(frozen=True)
 class FunctionSignature:
     """Function signature."""
@@ -35,20 +35,20 @@
             raise ValueError(f"Invalid inputs, provided={set(inputs.keys())}, expected={set(self.inputs.keys())}.")
         # TODO (spillai): Validate input types and shapes.
         return inputs
 
     def encode_inputs(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """Encode inputs based on defined signature."""
         inputs = self.validate_inputs(inputs)
-        return {k: cloudpickle.dumps(v) for k, v in inputs.items()}
+        return {k: dumps(v) for k, v in inputs.items()}
 
     def decode_inputs(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """Decode inputs based on defined signature."""
         inputs = self.validate_inputs(inputs)
-        return {k: cloudpickle.loads(v) for k, v in inputs.items()}
+        return {k: loads(v) for k, v in inputs.items()}
 
 
 @dataclass(frozen=True)
 class ModelSpec:
     """Model specification for the registry.
 
     The ModelSpec defines all the relevant information for
```

## Comparing `autonomi_nos-0.0.4a0.dist-info/LICENSE` & `autonomi_nos-0.0.4a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `autonomi_nos-0.0.4a0.dist-info/METADATA` & `autonomi_nos-0.0.4a1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomi-nos
-Version: 0.0.4a0
+Version: 0.0.4a1
 Summary: Nitrous oxide system (NOS) for computer-vision.
 License: MIT License
         
         Copyright (c) 2023 Autonomi AI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autonomi-nos Version: 0.0.4a0 Summary: Nitrous
+Metadata-Version: 2.1 Name: autonomi-nos Version: 0.0.4a1 Summary: Nitrous
 oxide system (NOS) for computer-vision. License: MIT License Copyright (c) 2023
 Autonomi AI Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

## Comparing `autonomi_nos-0.0.4a0.dist-info/RECORD` & `autonomi_nos-0.0.4a1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 nos/__init__.py,sha256=51Y_o2LsEI8SmKeCFOZfz1aTYOCqrv8plfrpDyr_ILo,50
 nos/constants.py,sha256=j-nz48q31rE7eclMqkZH6xFJ0eGmtx2Jt5yr_wQA_1Y,561
 nos/exceptions.py,sha256=ocRCxTbzT_Q8WTobAbkbo4jl5a6F3xC_D2N7rtzfWeg,93
 nos/logging.py,sha256=D0QDNFGmAYshfnSC-ctEDSIeBO6TnLPz1babUmJGRSA,940
 nos/protoc.py,sha256=xUck1U30UqUEnTaFuWMGWagyDcIrjmcQo8xozqbypmI,2778
-nos/version.py,sha256=rJdPE5XDOIi-BiClP-ph78BgHXH62hS9N_VMAlrufd0,23
+nos/version.py,sha256=efUYlBE_8IYxzh4ow8CwCB8ftBdPoAhSch4ySvNaFrY,24
 nos/cli/benchmark.py,sha256=p-EGzEUDMFFv2hpB9Nn8-Xk1zW-hrYDaUzyNvWmSgzk,110
 nos/cli/cli.py,sha256=nO0Eg_zp7L6xt5ST0QteypNHky8TIms8JSOLsvtHhjY,455
 nos/cli/docker.py,sha256=uPGrLe8FlvwSNFGUqp-vw5VAZhCeyvrfUfwJZdqXypk,1983
 nos/cli/hub.py,sha256=USdzVgaZlPZABrrIZzCA7ySwXg1iseEk7GJ7iwanXIg,1294
 nos/cli/serve_grpc.py,sha256=ymFv5qfehj5jNnEOiku-Kp5oqjMUbl7pzG4eVYP3KhE,6202
 nos/cli/serve_http.py,sha256=xMwSE46-_uHLgif1gnJCRoLbBE3ttC2zkm2JXVooWg0,5962
 nos/cli/system.py,sha256=gFm8ngxyxcPThhjkgB8S8ZBmtYBcqLdSo4unaWTl0N8,3479
 nos/cli/utils.py,sha256=uR1lGZyyDEuflNvxKuAmVUP-DTE55PzZL5c0c3l2h4U,425
 nos/client/__init__.py,sha256=-J19VTXOiv9joF7SwPpoUW4_nBwq5_cBp8A1ghhFg70,372
 nos/client/exceptions.py,sha256=Lqqeu_6oNSZgOUipXHFx20yeASJi9bEewpG1UYuy1gk,92
-nos/client/grpc.py,sha256=mY0YT9n8DwsvvKX8kJBu8yHJ8ayoXt844T__3i9BTXE,12657
-nos/common/__init__.py,sha256=83smCPabdvR79BJB3iiGQ2rg1a_hYhUwgPVfw4iXgOQ,286
-nos/common/spec.py,sha256=9ypTvsmUO_9yZ9zfyc7_uzLr4MJ72aXEvBGogEVsGVc,3715
+nos/client/grpc.py,sha256=Wu4CmXJX2Vq2LvfXgLGcMJuhPyh-DOvoCc9uy_DiEZY,12621
+nos/common/__init__.py,sha256=Khg1qL0KMrW2-mMXipUktq2S43pVpb-pVqLsC7dSlo8,235
+nos/common/cloudpickle.py,sha256=vQHSKlYjc1BVoYWviNjkREbekX52bc0SfjIyaZjdwVY,178
+nos/common/spec.py,sha256=PGJxit5LeTGsPT2Dnn5k4uoJHJuJWz3YaM7O6lqpbJI,3720
 nos/common/tasks.py,sha256=AcEbh5gbpKt_77Ar9zRrRyiD8tyw264Wv2buyX9yxZ8,518
 nos/common/types.py,sha256=PgE1M1FdOhEc6AurFBAXrWk-j_br_pyR2scHasX3sLM,4851
 nos/examples/vid2bbox.py,sha256=UNEYmxI5RILgpOz14m2LEr-WJdgrdHnFeIIsN91k88E,3470
 nos/executors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nos/executors/ray.py,sha256=aurGem2kgMMCdV-38kN6ozsNMbmKuIh4ywDEIuWNkBk,7401
 nos/experimental/conversion_flows/openmmlab/tensorrt/run_model.py,sha256=A8LoCm4YvApkw_AAAyGqNLKeAoqzK1xvBy4pLI_Y9TE,1246
 nos/experimental/http/__init__.py,sha256=5LrWYhbfJy60b1eHj_p5gq7huQqFxxt_ThErTEkrKyc,4559
@@ -45,13 +46,13 @@
 nos/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nos/server/docker.py,sha256=Wbob_pkHXKdMWliD2VTWw1U7R7dojBImYWZTeSNDfLY,6229
 nos/server/runtime.py,sha256=BzQsaMCBAxC73xfj2AR6RCjfWWOWwMQBAU0gxKut8rI,2976
 nos/server/service.py,sha256=CEmaKrdp-8f_Bdcxr70xGO8EXYJH3fuYCv_SQVtVf7Y,9887
 nos/test/benchmark.py,sha256=b_QMHfStY5iRjHGPZwaY7VrXzy_VeFKfjld9UEVbn-g,373
 nos/test/conftest.py,sha256=-mZNh-D-LsalJ5oL0NOW1B7G88o0W6rJ8dwNA08N8Ys,5764
 nos/test/utils.py,sha256=F8RTOZKIuYPguUOz3beERNbmCg3pYjvLFwS7bMp6ejw,1347
-autonomi_nos-0.0.4a0.dist-info/LICENSE,sha256=9TQFxQ2AkXOQuIHy9GueB_a18hayRXT7pDt9fJv9WLo,1068
-autonomi_nos-0.0.4a0.dist-info/METADATA,sha256=-oR1BExuNhspEPyQCDDULzn0YiuFkmJowgcU_NbQrWc,6257
-autonomi_nos-0.0.4a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-autonomi_nos-0.0.4a0.dist-info/entry_points.txt,sha256=UYtJAmFT3RPWmlKM11MMZvZPRHTeKyIh1BbZ3QpbsJs,86
-autonomi_nos-0.0.4a0.dist-info/top_level.txt,sha256=RgOntmzdTkyrY-Fj9H6bSke7af3bHLscoZnK1-7Aa8o,12
-autonomi_nos-0.0.4a0.dist-info/RECORD,,
+autonomi_nos-0.0.4a1.dist-info/LICENSE,sha256=9TQFxQ2AkXOQuIHy9GueB_a18hayRXT7pDt9fJv9WLo,1068
+autonomi_nos-0.0.4a1.dist-info/METADATA,sha256=g2FIQzHvFgUgQx4rDPQ5RwlFGvP2645KS-SqG0YxX3A,6257
+autonomi_nos-0.0.4a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+autonomi_nos-0.0.4a1.dist-info/entry_points.txt,sha256=UYtJAmFT3RPWmlKM11MMZvZPRHTeKyIh1BbZ3QpbsJs,86
+autonomi_nos-0.0.4a1.dist-info/top_level.txt,sha256=RgOntmzdTkyrY-Fj9H6bSke7af3bHLscoZnK1-7Aa8o,12
+autonomi_nos-0.0.4a1.dist-info/RECORD,,
```

