# Comparing `tmp/llm_rs-0.2.6.tar.gz` & `tmp/llm_rs-0.2.7.tar.gz`

## Comparing `llm_rs-0.2.6.tar` & `llm_rs-0.2.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.6/Cargo.toml
--rw-r--r--   0     1001      123      610 2023-05-27 15:31:39.000000 llm_rs-0.2.6/.github/workflows/BuildDoc.yml
--rw-r--r--   0     1001      123     2796 2023-05-27 15:31:39.000000 llm_rs-0.2.6/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      564 2023-05-27 15:31:39.000000 llm_rs-0.2.6/.github/workflows/Clippy.yml
--rw-r--r--   0     1001      123      602 2023-05-27 15:31:39.000000 llm_rs-0.2.6/.github/workflows/PublishDocs.yml
--rw-r--r--   0     1001      123     3455 2023-05-27 15:31:39.000000 llm_rs-0.2.6/.gitignore
--rw-r--r--   0     1001      123       72 2023-05-27 15:31:39.000000 llm_rs-0.2.6/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-05-27 15:31:39.000000 llm_rs-0.2.6/LICENSE
--rw-r--r--   0     1001      123     3380 2023-05-27 15:31:39.000000 llm_rs-0.2.6/README.md
--rw-r--r--   0     1001      123     4799 2023-05-27 15:31:39.000000 llm_rs-0.2.6/docs/docs/conversion.md
--rw-r--r--   0     1001      123     9355 2023-05-27 15:31:39.000000 llm_rs-0.2.6/docs/docs/index.md
--rw-r--r--   0     1001      123     1181 2023-05-27 15:31:39.000000 llm_rs-0.2.6/docs/mkdocs.yml
--rw-r--r--   0     1001      123       31 2023-05-27 15:31:39.000000 llm_rs-0.2.6/docs/requirements.txt
--rw-r--r--   0     1001      123      334 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/__init__.py
--rw-r--r--   0     1001      123    14929 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/auto.py
--rw-r--r--   0     1001      123     1848 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/base_model.py
--rw-r--r--   0     1001      123     1351 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/config.pyi
--rw-r--r--   0     1001      123       78 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/__init__.py
--rw-r--r--   0     1001      123     2223 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/auto_converter.py
--rw-r--r--   0     1001      123      199 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/models/__init__.py
--rw-r--r--   0     1001      123     5581 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/models/_base.py
--rw-r--r--   0     1001      123     3177 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/models/bloom.py
--rw-r--r--   0     1001      123     5221 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/models/gpt2.py
--rw-r--r--   0     1001      123     2032 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/models/gptj.py
--rw-r--r--   0     1001      123     2138 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/models/gptneox.py
--rw-r--r--   0     1001      123     6334 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/models/llama.py
--rw-r--r--   0     1001      123     1893 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/convert/models/mpt.py
--rw-r--r--   0     1001      123       36 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/langchain/__init__.py
--rw-r--r--   0     1001      123     3156 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/langchain/langchain.py
--rw-r--r--   0     1001      123        0 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123      579 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/py.typed
--rw-r--r--   0     1001      123     2915 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/repository.py
--rw-r--r--   0     1001      123      697 2023-05-27 15:31:39.000000 llm_rs-0.2.6/llm_rs/results.pyi
--rw-r--r--   0     1001      123     1007 2023-05-27 15:31:39.000000 llm_rs-0.2.6/pyproject.toml
--rw-r--r--   0     1001      123     4808 2023-05-27 15:31:39.000000 llm_rs-0.2.6/src/configs.rs
--rw-r--r--   0     1001      123     1700 2023-05-27 15:31:39.000000 llm_rs-0.2.6/src/lib.rs
--rw-r--r--   0     1001      123    15124 2023-05-27 15:31:39.000000 llm_rs-0.2.6/src/model_base.rs
--rw-r--r--   0     1001      123      300 2023-05-27 15:31:39.000000 llm_rs-0.2.6/src/models.rs
--rw-r--r--   0     1001      123     2576 2023-05-27 15:31:39.000000 llm_rs-0.2.6/src/quantize.rs
--rw-r--r--   0     1001      123     1352 2023-05-27 15:31:39.000000 llm_rs-0.2.6/src/results.rs
--rw-r--r--   0     1001      123     1756 2023-05-27 15:31:39.000000 llm_rs-0.2.6/src/stopwords.rs
--rw-r--r--   0     1001      123    14030 2023-05-27 15:33:33.000000 llm_rs-0.2.6/Cargo.lock
--rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 llm_rs-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.7/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-05-28 08:28:01.000000 llm_rs-0.2.7/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     2796 2023-05-28 08:28:01.000000 llm_rs-0.2.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-05-28 08:28:01.000000 llm_rs-0.2.7/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-05-28 08:28:01.000000 llm_rs-0.2.7/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3455 2023-05-28 08:28:01.000000 llm_rs-0.2.7/.gitignore
+-rw-r--r--   0     1001      123       72 2023-05-28 08:28:01.000000 llm_rs-0.2.7/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-05-28 08:28:01.000000 llm_rs-0.2.7/LICENSE
+-rw-r--r--   0     1001      123     3380 2023-05-28 08:28:01.000000 llm_rs-0.2.7/README.md
+-rw-r--r--   0     1001      123     4799 2023-05-28 08:28:01.000000 llm_rs-0.2.7/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     9355 2023-05-28 08:28:01.000000 llm_rs-0.2.7/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-05-28 08:28:01.000000 llm_rs-0.2.7/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-05-28 08:28:01.000000 llm_rs-0.2.7/docs/requirements.txt
+-rw-r--r--   0     1001      123      334 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/__init__.py
+-rw-r--r--   0     1001      123    15727 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/auto.py
+-rw-r--r--   0     1001      123     1848 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/base_model.py
+-rw-r--r--   0     1001      123     1402 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/config.pyi
+-rw-r--r--   0     1001      123       78 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/__init__.py
+-rw-r--r--   0     1001      123     2223 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/auto_converter.py
+-rw-r--r--   0     1001      123      199 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/models/__init__.py
+-rw-r--r--   0     1001      123     5820 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/models/_base.py
+-rw-r--r--   0     1001      123     3177 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/models/bloom.py
+-rw-r--r--   0     1001      123     5221 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/models/gpt2.py
+-rw-r--r--   0     1001      123     2032 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/models/gptj.py
+-rw-r--r--   0     1001      123     2138 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/models/gptneox.py
+-rw-r--r--   0     1001      123     6334 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/models/llama.py
+-rw-r--r--   0     1001      123     1893 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/convert/models/mpt.py
+-rw-r--r--   0     1001      123       36 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/langchain/__init__.py
+-rw-r--r--   0     1001      123     3156 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/langchain/langchain.py
+-rw-r--r--   0     1001      123        0 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123      579 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/py.typed
+-rw-r--r--   0     1001      123     2915 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/repository.py
+-rw-r--r--   0     1001      123      697 2023-05-28 08:28:01.000000 llm_rs-0.2.7/llm_rs/results.pyi
+-rw-r--r--   0     1001      123     1007 2023-05-28 08:28:01.000000 llm_rs-0.2.7/pyproject.toml
+-rw-r--r--   0     1001      123     4808 2023-05-28 08:28:01.000000 llm_rs-0.2.7/src/configs.rs
+-rw-r--r--   0     1001      123     1700 2023-05-28 08:28:01.000000 llm_rs-0.2.7/src/lib.rs
+-rw-r--r--   0     1001      123    15124 2023-05-28 08:28:01.000000 llm_rs-0.2.7/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-05-28 08:28:01.000000 llm_rs-0.2.7/src/models.rs
+-rw-r--r--   0     1001      123     2774 2023-05-28 08:28:01.000000 llm_rs-0.2.7/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-05-28 08:28:01.000000 llm_rs-0.2.7/src/results.rs
+-rw-r--r--   0     1001      123     1756 2023-05-28 08:28:01.000000 llm_rs-0.2.7/src/stopwords.rs
+-rw-r--r--   0     1001      123    14875 2023-05-28 08:29:53.000000 llm_rs-0.2.7/Cargo.lock
+-rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 llm_rs-0.2.7/PKG-INFO
```

### Comparing `llm_rs-0.2.6/.github/workflows/BuildDoc.yml` & `llm_rs-0.2.7/.github/workflows/BuildDoc.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/.github/workflows/CI.yml` & `llm_rs-0.2.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/.github/workflows/Clippy.yml` & `llm_rs-0.2.7/.github/workflows/Clippy.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/.github/workflows/PublishDocs.yml` & `llm_rs-0.2.7/.github/workflows/PublishDocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/.gitignore` & `llm_rs-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/LICENSE` & `llm_rs-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/README.md` & `llm_rs-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/docs/docs/conversion.md` & `llm_rs-0.2.7/docs/docs/conversion.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/docs/docs/index.md` & `llm_rs-0.2.7/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/docs/mkdocs.yml` & `llm_rs-0.2.7/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/auto.py` & `llm_rs-0.2.7/llm_rs/auto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .config import QuantizationType,ContainerType,SessionConfig
 import os
 import pathlib
 from .models import Mpt,GptNeoX,GptJ,Gpt2,Bloom,Llama
 from .base_model import Model
 import logging
-from typing import Optional, List, Union,Type
+from typing import Optional, List, Union,Type,Dict
 import os
 from enum import Enum, auto
 from dataclasses import dataclass
 import json
 from blake3 import blake3
 from huggingface_hub import snapshot_download
 from huggingface_hub.utils import validate_repo_id, HFValidationError
@@ -27,14 +27,17 @@
     Bloom = auto()
     Llama = auto()
 
 
 _QUANTIZATION_TYPE_MAP = {
     "Q4_0": QuantizationType.Q4_0,
     "Q4_1": QuantizationType.Q4_1,
+    "Q5_0": QuantizationType.Q5_0,
+    "Q5_1": QuantizationType.Q5_1,
+    "Q8_0": QuantizationType.Q8_0,
     "F16": QuantizationType.F16
 }
 
 _CONTAINER_TYPE_MAP = {
     "GGML": ContainerType.GGML,
     "GGJT": ContainerType.GGJT
 }
@@ -44,29 +47,30 @@
     KnownModels.Mpt: Mpt,
     KnownModels.GptJ: GptJ,
     KnownModels.Gpt2: Gpt2,
     KnownModels.Bloom: Bloom,
     KnownModels.Llama: Llama
 }
 
+CURRENT_QUANTIZATION_VERSION = QuantizationVersions.V2
 
 class PathType(Enum):
     DIR = auto()
     FILE = auto()
     REPO = auto()
     UNKNOWN = auto() 
 
 def _get_path_type(path: Union[str,os.PathLike]) -> PathType:
     p = pathlib.Path(path)
     if p.is_file():
         return PathType.FILE
     elif p.is_dir():
         return PathType.DIR
     try:
-        validate_repo_id(path)
+        validate_repo_id(str(path))
         return PathType.REPO
     except HFValidationError:
         pass
     return PathType.UNKNOWN
 
 
 @dataclass()
@@ -76,14 +80,15 @@
     """
     model: KnownModels
     quantization: QuantizationType
     container: ContainerType
     quantization_version: QuantizationVersions=QuantizationVersions.Not_Quantized
     converter:str="llm-rs"
     hash:Optional[str]=None
+    base_model:Optional[str]=None
 
     def add_hash(self,model_path:Union[str,os.PathLike]):
         h  = blake3(max_threads=blake3.AUTO)
         b  = bytearray(128_000_000)
         mv = memoryview(b)
         with open(model_path, 'rb', buffering=0) as f:
             for n in iter(lambda : f.readinto(mv), 0):
@@ -93,26 +98,28 @@
     def serialize(self):
         return {
             "model": self.model.name,
             "quantization": repr(self.quantization).split(".")[-1],
             "quantization_version": self.quantization_version.name,
             "container": repr(self.container).split(".")[-1],
             "converter": self.converter,
-            "hash": self.hash
+            "hash": self.hash,
+            "base_model": self.base_model
         }
     
     @staticmethod
-    def deserialize(metadata_dict):
+    def deserialize(metadata_dict:Dict[str,str])->"ModelMetadata":
         return ModelMetadata(
             model = KnownModels[metadata_dict["model"]],
             quantization = _QUANTIZATION_TYPE_MAP[metadata_dict["quantization"]],
             quantization_version= QuantizationVersions[metadata_dict["quantization_version"]],
             container = _CONTAINER_TYPE_MAP[metadata_dict["container"]],
             converter = metadata_dict["converter"],
-            hash = metadata_dict["hash"]
+            hash = metadata_dict.get("hash"),
+            base_model = metadata_dict.get("base_model")
         )
 
 
 @dataclass
 class AutoConfig():
     repo_type:Optional[str] = None
     model_type: Optional[str] = None
@@ -130,36 +137,36 @@
         elif path_type == PathType.FILE:
             raise ValueError(
                 f"Model path '{model_path_or_repo_id}' is a file. "
                 "Please provide a directory or a repo id.")
         
         auto_config = AutoConfig()
         if path_type == PathType.DIR:
-            cls._update_from_dir(model_path_or_repo_id, auto_config)
+            cls._update_from_dir(str(model_path_or_repo_id), auto_config)
         elif path_type == PathType.REPO:
-            cls._update_from_repo(model_path_or_repo_id, auto_config)
+            cls._update_from_repo(str(model_path_or_repo_id), auto_config)
 
         return auto_config
 
     @classmethod
     def _update_from_repo(
         cls,
         repo_id: str,
         auto_config: 'AutoConfig',
     ) -> None:
         path = snapshot_download(repo_id=repo_id, allow_patterns='config.json')
         cls._update_from_dir(path, auto_config)
 
     @classmethod
     def _update_from_dir(cls, path: str, auto_config: 'AutoConfig') -> None:
-        path = (pathlib.Path(path) / 'config.json').resolve()
-        if path.is_file():
-            cls._update_from_file(path, auto_config)
+        resolved_path = (pathlib.Path(path) / 'config.json').resolve()
+        if resolved_path.is_file():
+            cls._update_from_file(str(resolved_path), auto_config)
         else:
-            raise ValueError(f"Config path '{path}' doesn't exist.")
+            raise ValueError(f"Config path '{resolved_path}' doesn't exist.")
 
     @classmethod
     def _update_from_file(cls, path: str, auto_config: 'AutoConfig') -> None:
         with open(path) as f:
             config = json.load(f)
         auto_config.model_type = config.get('model_type')
         auto_config.repo_type = config.get('repo_type')
@@ -237,20 +244,23 @@
                     config = AutoConfig(repo_type="GGML")
                        
 
                 if config.repo_type != "GGML":
                     logging.warning("Found normal HuggingFace model, starting conversion...")
                     return cls.from_transformer(model_path_or_repo_id, session_config, lora_paths, verbose, default_quantization, default_container)
             
-                resolved_path = cls._find_model_path_from_repo(model_path_or_repo_id,model_file)
+                resolved_path = cls._find_model_path_from_repo(str(model_path_or_repo_id),model_file)
                 return cls.from_file(resolved_path,model_type,session_config,lora_paths,verbose)
             
             elif path_type == PathType.DIR:
-                resolved_path = cls._find_model_path_from_dir(model_path_or_repo_id,model_file)
+                resolved_path = cls._find_model_path_from_dir(str(model_path_or_repo_id),model_file)
                 return cls.from_file(resolved_path,model_type,session_config,lora_paths,verbose)
+            
+            else:
+                raise ValueError(f"Unknown path type '{path_type}'")
 
 
     @classmethod
     def _find_model_path_from_dir(
         cls,
         directory: str,
         filename: Optional[str] = None,
@@ -329,14 +339,23 @@
         model_name = get_name_from_config(config)
         export_path = cached_assets_path("llm-rs",namespace=model_name)
         converted_model = AutoConverter.convert(model_path_or_repo_id,export_path)
         if default_quantization != QuantizationType.F16:
             converted_model = AutoQuantizer.quantize(converted_model,quantization=default_quantization,container=default_container)
         return cls.from_file(converted_model,None,session_config,lora_paths,verbose)
     
+# Hack to make the quantization type enum hashable
+_APPENDIX_MAP = {
+    QuantizationType.Q4_0.__repr__(): "q4_0",
+    QuantizationType.Q4_1.__repr__(): "q4_1",
+    QuantizationType.Q5_0.__repr__(): "q5_0",
+    QuantizationType.Q5_1.__repr__(): "q5_1",
+    QuantizationType.Q8_0.__repr__(): "q8_0",
+}
+
 class AutoQuantizer():
     """
     Utility to quantize models, without having to specify the model type.
     """
     @staticmethod
     def quantize(model_file:Union[str,os.PathLike],target_path:Optional[Union[str,os.PathLike]]=None,quantization:QuantizationType=QuantizationType.Q4_0,container:ContainerType=ContainerType.GGJT)->Union[str,os.PathLike]:
         metadata=AutoModel.load_metadata(model_file)
@@ -347,40 +366,39 @@
 
         if target_path is None:
             target_path = os.path.dirname(model_file)
             
         def build_target_name()->str:
             output_path = pathlib.Path(target_path)
             if output_path.is_file():
-                return output_path
+                return str(output_path)
             else:
                 output_path.mkdir(parents=True,exist_ok=True)
                 model_path = pathlib.Path(model_file)
                 appendix = ""
-                if  quantization == QuantizationType.Q4_0:
-                    appendix += "-q4_0"
-                elif quantization == QuantizationType.Q4_1:
-                    appendix += "-q4_1"
+
+                if quantization.__repr__() in _APPENDIX_MAP:
+                    appendix += f"-{_APPENDIX_MAP[quantization.__repr__()]}"
 
                 if container == ContainerType.GGJT:
                     appendix += "-ggjt"
             
                 filename = model_path.stem.replace("-f16","") + appendix + model_path.suffix
                 return str(output_path / filename)
 
         target_file = build_target_name()
         if pathlib.Path(target_file).exists():
             logging.warning(f"Target file '{target_file}' already exists, skipping quantization")
             return target_file
         
         logging.info(f"Quantizing model '{model_file}' to '{target_file}'")
-        model_type.quantize(model_file,target_file,quantization,container)
+        model_type.quantize(str(model_file),target_file,quantization,container)
 
         metadata_file = pathlib.Path(target_file).with_suffix(".meta")
-        quantized_metadata = ModelMetadata(model=metadata.model,quantization=quantization,container=container,quantization_version=QuantizationVersions.V2)
+        quantized_metadata = ModelMetadata(model=metadata.model,quantization=quantization,container=container,quantization_version=CURRENT_QUANTIZATION_VERSION,base_model=metadata.base_model)
         quantized_metadata.add_hash(target_file)
         logging.info(f"Writing metadata file '{metadata_file}'")
-        metadata_file.write_text(json.dumps(quantized_metadata.serialize()))
+        metadata_file.write_text(json.dumps(quantized_metadata.serialize(),indent=4))
         logging.info(f"Finished quantizing model '{model_file}' to '{target_file}'")
         return target_file
```

### Comparing `llm_rs-0.2.6/llm_rs/base_model.py` & `llm_rs-0.2.7/llm_rs/base_model.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/config.pyi` & `llm_rs-0.2.7/llm_rs/config.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 class ContainerType(Enum):
     GGML=auto(),
     GGJT=auto(),
 
 class QuantizationType(Enum):
     Q4_0=auto(),
     Q4_1=auto(),
+    Q5_0=auto(),
+    Q5_1=auto(),
+    Q8_0=auto(),
     F16=auto(),
 
 class Precision(Enum):
     FP32=auto(),
     FP16=auto(),
     
 class GenerationConfig():
```

### Comparing `llm_rs-0.2.6/llm_rs/convert/auto_converter.py` & `llm_rs-0.2.7/llm_rs/convert/auto_converter.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/convert/models/_base.py` & `llm_rs-0.2.7/llm_rs/convert/models/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from transformers import AutoTokenizer,AutoModelForCausalLM,AutoConfig
 import os
 import struct
 from enum import Enum
 import logging
 import numpy as np
 from ...config import QuantizationType,ContainerType
-from ...auto import ModelMetadata, KnownModels
+from ...auto import ModelMetadata, KnownModels, QuantizationVersions
 import pathlib
 import json
 import torch
 
 GGML_MAGIC = 0x67676D6C
 GGMF_MAGIC = 0x67676D66
 GGJT_MAGIC = 0x67676a74
@@ -22,14 +22,15 @@
 
 class BaseAdapter(ABC):
     model_type:KnownModels=None
     file_magic:int=GGML_MAGIC
     version:int=1
 
     def  __init__(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None) -> None:
+        self.pretrained_model_name_or_path = pretrained_model_name_or_path
         self.config,self.tokenizer,self.model= self.load(pretrained_model_name_or_path,pretrained_tokenizer_name_or_path)
 
     @abstractmethod
     def load(self,pretrained_model_name_or_path:Union[str,os.PathLike],pretrained_tokenizer_name_or_path:Optional[Union[str,os.PathLike]]=None)->Tuple[AutoConfig,AutoTokenizer,AutoModelForCausalLM]:
         ...
 
     @abstractmethod
@@ -136,17 +137,18 @@
             self._write_vocabulary(out_file)
             self._write_weights(out_file)
             logging.info(f"Done converting model to GGML format. Saved to '{output_file}'")
 
         #Create the *.meta file needed for automatic loading
         metadata_file = pathlib.Path(output_file).with_suffix(".meta")
         metadata = ModelMetadata(
-            self.model_type,
-            QuantizationType.F16,
-            ContainerType.GGML
+            model = self.model_type,
+            quantization = QuantizationType.F16,
+            container = ContainerType.GGML,
+            quantization_version=QuantizationVersions.Not_Quantized,
+            base_model=str(self.pretrained_model_name_or_path),
             )
         metadata.add_hash(output_file)
         metadata_file.write_text(json.dumps(metadata.serialize(),indent=4))
         
         logging.info(f"Created metadata file at '{output_file}'")
-        return output_file
```

### Comparing `llm_rs-0.2.6/llm_rs/convert/models/bloom.py` & `llm_rs-0.2.7/llm_rs/convert/models/bloom.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/convert/models/gpt2.py` & `llm_rs-0.2.7/llm_rs/convert/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/convert/models/gptj.py` & `llm_rs-0.2.7/llm_rs/convert/models/gptj.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/convert/models/gptneox.py` & `llm_rs-0.2.7/llm_rs/convert/models/gptneox.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/convert/models/llama.py` & `llm_rs-0.2.7/llm_rs/convert/models/llama.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/convert/models/mpt.py` & `llm_rs-0.2.7/llm_rs/convert/models/mpt.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/langchain/langchain.py` & `llm_rs-0.2.7/llm_rs/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/models.pyi` & `llm_rs-0.2.7/llm_rs/models.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/repository.py` & `llm_rs-0.2.7/llm_rs/repository.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/llm_rs/results.pyi` & `llm_rs-0.2.7/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/pyproject.toml` & `llm_rs-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/src/configs.rs` & `llm_rs-0.2.7/src/configs.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/src/lib.rs` & `llm_rs-0.2.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/src/model_base.rs` & `llm_rs-0.2.7/src/model_base.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/src/quantize.rs` & `llm_rs-0.2.7/src/quantize.rs`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 }
 
 #[pyclass]
 #[derive(Clone, Copy, Debug, PartialEq)]
 pub enum QuantizationType {
     Q4_0,
     Q4_1,
+    Q5_0,
+    Q5_1,
+    Q8_0,
     F16,
 }
 
 pub fn _quantize<M: llm::KnownModel + 'static>(
     source: PathBuf,
     destination: PathBuf,
     container: ContainerType,
@@ -34,14 +37,17 @@
         ContainerType::GGML => ggml::format::SaveContainerType::Ggml,
         ContainerType::GGJT => ggml::format::SaveContainerType::GgjtV3,
     };
 
     let quantization = match quantization {
         QuantizationType::Q4_0 => Ok(ggml::Type::Q4_0),
         QuantizationType::Q4_1 => Ok(ggml::Type::Q4_1),
+        QuantizationType::Q5_0 => Ok(ggml::Type::Q5_0),
+        QuantizationType::Q5_1 => Ok(ggml::Type::Q5_1),
+        QuantizationType::Q8_0 => Ok(ggml::Type::Q8_0),
         QuantizationType::F16 => Err(QuantizeError::UnsupportedElementType {
             element_type: ggml::Type::F16,
         }),
     }?;
 
     let mut source = BufReader::new(std::fs::File::open(source)?);
     let mut destination = BufWriter::new(std::fs::File::create(destination)?);
```

### Comparing `llm_rs-0.2.6/src/results.rs` & `llm_rs-0.2.7/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/src/stopwords.rs` & `llm_rs-0.2.7/src/stopwords.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.6/Cargo.lock` & `llm_rs-0.2.7/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "aho-corasick"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bitflags"
@@ -48,24 +57,24 @@
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "ggml"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "ggml-sys",
  "thiserror",
 ]
 
 [[package]]
 name = "ggml-sys"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "half"
 version = "2.2.1"
@@ -86,102 +95,103 @@
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "llm"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "llm-base",
  "llm-bloom",
  "llm-gpt2",
  "llm-gptj",
  "llm-gptneox",
  "llm-llama",
  "llm-mpt",
  "serde",
 ]
 
 [[package]]
 name = "llm-base"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "bytemuck",
  "ggml",
  "half",
  "memmap2",
  "partial_sort",
  "rand",
+ "regex",
  "serde",
  "serde_bytes",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-bloom"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gpt2"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptj"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptneox"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "bytemuck",
  "llm-base",
  "serde",
 ]
 
 [[package]]
 name = "llm-llama"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "bytemuck",
  "llm-base",
  "rand",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-mpt"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#5cb475ad5aa76488a289666cb1c278f0cdf79de2"
+source = "git+https://github.com/rustformers/llm.git#8ba7a0b1b5f40724f07a2fc06c3a15a541861be8"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.2.6"
+version = "0.2.7"
 dependencies = [
  "ggml",
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
@@ -196,20 +206,23 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+
+[[package]]
+name = "memchr"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
 version = "0.5.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
@@ -380,14 +393,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "regex"
+version = "1.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
```

### Comparing `llm_rs-0.2.6/PKG-INFO` & `llm_rs-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: llm-rs
-Version: 0.2.6
+Version: 0.2.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: blake3
 Requires-Dist: huggingface-hub >= 0.14.1
+Requires-Dist: langchain; extra == 'langchain'
 Requires-Dist: transformers >= 4.29.0; extra == 'convert'
 Requires-Dist: sentencepiece >= 0.1.99; extra == 'convert'
 Requires-Dist: torch >= 2.0.0; extra == 'convert'
 Requires-Dist: accelerate >= 0.19.0; extra == 'convert'
 Requires-Dist: tqdm; extra == 'convert'
 Requires-Dist: einops >= 0.6.1; extra == 'convert'
-Requires-Dist: langchain; extra == 'langchain'
-Provides-Extra: convert
 Provides-Extra: langchain
+Provides-Extra: convert
 License-File: LICENSE
 Summary: Unofficial python bindings for llm-rs. 🐍❤️🦀
 Keywords: LLM,Transformers
 Author: Lukas Kreussel
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/LLukas22/llm-rs-python
 Project-URL: documentation, https://llukas22.github.io/llm-rs-python/
+Project-URL: repository, https://github.com/LLukas22/llm-rs-python
 
 # llm-rs-python: Python Bindings for Rust's llm Library
 
 Welcome to `llm-rs`, an unofficial Python interface for the Rust-based [llm](https://github.com/rustformers/llm) library, made possible through [PyO3](https://github.com/PyO3/pyo3). Our package combines the convenience of Python with the performance of Rust to offer an efficient tool for your machine learning projects. 🐍❤️🦀
 
 With `llm-rs`, you can operate a variety of Large Language Models (LLMs) including LLama and GPT-NeoX directly on your CPU.
```

