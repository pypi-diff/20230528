# Comparing `tmp/muutils-0.3.9.tar.gz` & `tmp/muutils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muutils-0.3.9.tar", max compression
+gzip compressed data, was "muutils-0.4.0.tar", max compression
```

## Comparing `muutils-0.3.9.tar` & `muutils-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,37 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.3.9/LICENSE
--rw-r--r--   0        0        0       22 2023-04-18 18:13:20.205838 muutils-0.3.9/muutils/__init__.py
--rw-r--r--   0        0        0     3910 2023-03-24 22:25:29.757321 muutils-0.3.9/muutils/_wip/dataclass_validator.py
--rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.3.9/muutils/_wip/experiments.ipynb
--rw-r--r--   0        0        0     5835 2023-03-24 22:25:29.757321 muutils-0.3.9/muutils/_wip/gptdataset.py
--rw-r--r--   0        0        0    23453 2023-03-24 22:25:29.758323 muutils-0.3.9/muutils/_wip/json_serialize_old.py
--rw-r--r--   0        0        0     3286 2023-03-24 22:25:29.758323 muutils-0.3.9/muutils/_wip/lazy_externals.py
--rw-r--r--   0        0        0     9214 2023-03-24 22:25:29.759320 muutils-0.3.9/muutils/_wip/newargparser.py
--rw-r--r--   0        0        0     7414 2023-03-24 22:25:29.760323 muutils-0.3.9/muutils/_wip/torch_util_old.py
--rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.3.9/muutils/dictmagic.py
--rw-r--r--   0        0        0     1613 2023-03-06 19:25:21.018548 muutils-0.3.9/muutils/group_equiv.py
--rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.3.9/muutils/json_serialize/__init__.py
--rw-r--r--   0        0        0     6090 2023-04-18 18:13:20.206840 muutils-0.3.9/muutils/json_serialize/array.py
--rw-r--r--   0        0        0    10989 2023-04-18 18:13:20.207837 muutils-0.3.9/muutils/json_serialize/dataclass_factories.py
--rw-r--r--   0        0        0     8906 2023-04-15 04:06:05.294628 muutils-0.3.9/muutils/json_serialize/json_serialize.py
--rw-r--r--   0        0        0    15787 2023-04-18 18:13:20.209838 muutils-0.3.9/muutils/json_serialize/serializable_dataclass.py
--rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.3.9/muutils/json_serialize/util.py
--rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.3.9/muutils/jsonlines.py
--rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.3.9/muutils/logger/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.3.9/muutils/logger/exception_context.py
--rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.3.9/muutils/logger/headerfuncs.py
--rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.3.9/muutils/logger/log_util.py
--rw-r--r--   0        0        0    10669 2023-03-24 22:25:29.766326 muutils-0.3.9/muutils/logger/logger.py
--rw-r--r--   0        0        0     3796 2023-03-24 22:25:29.767323 muutils-0.3.9/muutils/logger/loggingstream.py
--rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.3.9/muutils/logger/simplelogger.py
--rw-r--r--   0        0        0     2488 2023-03-24 22:25:29.769322 muutils-0.3.9/muutils/logger/timing.py
--rw-r--r--   0        0        0     2231 2023-03-24 22:25:29.770322 muutils-0.3.9/muutils/misc.py
--rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.3.9/muutils/py.typed
--rw-r--r--   0        0        0     8778 2023-03-24 22:25:29.771346 muutils-0.3.9/muutils/statcounter.py
--rw-r--r--   0        0        0     6322 2023-03-30 07:34:00.609964 muutils-0.3.9/muutils/sysinfo.py
--rw-r--r--   0        0        0    10118 2023-04-18 18:13:20.210838 muutils-0.3.9/muutils/tensor_utils.py
--rw-r--r--   0        0        0      139 2023-03-24 22:25:29.773320 muutils-0.3.9/muutils/zanj/__init__.py
--rw-r--r--   0        0        0     1469 2023-03-25 05:30:53.722117 muutils-0.3.9/muutils/zanj/externals.py
--rw-r--r--   0        0        0    12685 2023-04-18 18:13:20.211838 muutils-0.3.9/muutils/zanj/loading.py
--rw-r--r--   0        0        0     4151 2023-03-30 19:44:39.207720 muutils-0.3.9/muutils/zanj/readme.md
--rw-r--r--   0        0        0     8153 2023-04-18 18:13:20.212838 muutils-0.3.9/muutils/zanj/serializing.py
--rw-r--r--   0        0        0     8681 2023-04-06 20:15:44.284139 muutils-0.3.9/muutils/zanj/torchutil.py
--rw-r--r--   0        0        0     7755 2023-04-18 18:13:20.213837 muutils-0.3.9/muutils/zanj/zanj.py
--rw-r--r--   0        0        0      967 2023-04-18 18:13:20.214835 muutils-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     1575 2023-02-16 09:10:54.612163 muutils-0.3.9/README.md
--rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 muutils-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.4.0/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-28 05:49:08.534162 muutils-0.4.0/muutils/__init__.py
+-rw-r--r--   0        0        0     3910 2023-03-24 22:25:29.757321 muutils-0.4.0/muutils/_wip/dataclass_validator.py
+-rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.4.0/muutils/_wip/experiments.ipynb
+-rw-r--r--   0        0        0     5835 2023-03-24 22:25:29.757321 muutils-0.4.0/muutils/_wip/gptdataset.py
+-rw-r--r--   0        0        0    23453 2023-03-24 22:25:29.758323 muutils-0.4.0/muutils/_wip/json_serialize_old.py
+-rw-r--r--   0        0        0     3286 2023-03-24 22:25:29.758323 muutils-0.4.0/muutils/_wip/lazy_externals.py
+-rw-r--r--   0        0        0     9214 2023-03-24 22:25:29.759320 muutils-0.4.0/muutils/_wip/newargparser.py
+-rw-r--r--   0        0        0     7414 2023-03-24 22:25:29.760323 muutils-0.4.0/muutils/_wip/torch_util_old.py
+-rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.4.0/muutils/dictmagic.py
+-rw-r--r--   0        0        0     1613 2023-03-06 19:25:21.018548 muutils-0.4.0/muutils/group_equiv.py
+-rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.4.0/muutils/json_serialize/__init__.py
+-rw-r--r--   0        0        0     6272 2023-05-20 23:35:42.047282 muutils-0.4.0/muutils/json_serialize/array.py
+-rw-r--r--   0        0        0    10989 2023-04-18 18:13:20.207837 muutils-0.4.0/muutils/json_serialize/dataclass_factories.py
+-rw-r--r--   0        0        0     9048 2023-05-20 23:35:42.048268 muutils-0.4.0/muutils/json_serialize/json_serialize.py
+-rw-r--r--   0        0        0    16919 2023-05-28 05:49:08.535171 muutils-0.4.0/muutils/json_serialize/serializable_dataclass.py
+-rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.4.0/muutils/json_serialize/util.py
+-rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.4.0/muutils/jsonlines.py
+-rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.4.0/muutils/logger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.4.0/muutils/logger/exception_context.py
+-rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.4.0/muutils/logger/headerfuncs.py
+-rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.4.0/muutils/logger/log_util.py
+-rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.4.0/muutils/logger/logger.py
+-rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.4.0/muutils/logger/loggingstream.py
+-rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.4.0/muutils/logger/simplelogger.py
+-rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.4.0/muutils/logger/timing.py
+-rw-r--r--   0        0        0     2607 2023-05-17 07:31:29.361724 muutils-0.4.0/muutils/misc.py
+-rw-r--r--   0        0        0    12374 2023-05-17 07:31:29.362725 muutils-0.4.0/muutils/nbutils/convert_ipynb_to_script.py
+-rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.4.0/muutils/nbutils/print_tex.py
+-rw-r--r--   0        0        0     3573 2023-05-17 07:31:29.363723 muutils-0.4.0/muutils/nbutils/run_notebook_tests.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.4.0/muutils/py.typed
+-rw-r--r--   0        0        0     7753 2023-05-28 05:49:08.539161 muutils-0.4.0/muutils/statcounter.py
+-rw-r--r--   0        0        0     6322 2023-03-30 07:34:00.609964 muutils-0.4.0/muutils/sysinfo.py
+-rw-r--r--   0        0        0    10235 2023-05-28 05:49:08.540162 muutils-0.4.0/muutils/tensor_utils.py
+-rw-r--r--   0        0        0      991 2023-05-28 05:49:08.541168 muutils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2260 2023-05-28 05:49:08.532163 muutils-0.4.0/README.md
+-rw-r--r--   0        0        0     3090 1970-01-01 00:00:00.000000 muutils-0.4.0/PKG-INFO
```

### Comparing `muutils-0.3.9/LICENSE` & `muutils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/_wip/dataclass_validator.py` & `muutils-0.4.0/muutils/_wip/dataclass_validator.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/_wip/experiments.ipynb` & `muutils-0.4.0/muutils/_wip/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/_wip/gptdataset.py` & `muutils-0.4.0/muutils/_wip/gptdataset.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/_wip/json_serialize_old.py` & `muutils-0.4.0/muutils/_wip/json_serialize_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/_wip/lazy_externals.py` & `muutils-0.4.0/muutils/_wip/lazy_externals.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/_wip/newargparser.py` & `muutils-0.4.0/muutils/_wip/newargparser.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/_wip/torch_util_old.py` & `muutils-0.4.0/muutils/_wip/torch_util_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/dictmagic.py` & `muutils-0.4.0/muutils/dictmagic.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/group_equiv.py` & `muutils-0.4.0/muutils/group_equiv.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/json_serialize/__init__.py` & `muutils-0.4.0/muutils/json_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/json_serialize/array.py` & `muutils-0.4.0/muutils/json_serialize/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,18 @@
             arr, typing.Sequence
         ), f"invalid list format: {type(arr) = }\n{arr = }"
 
         return np.array(arr)
     elif array_mode == "external":
         # assume ZANJ has taken care of it
         assert isinstance(arr, typing.Mapping)
+        if "data" not in arr:
+            raise KeyError(
+                f"invalid external array, expected key 'data', got keys: '{list(arr.keys())}' and arr: {arr}"
+            )
         return arr["data"]
     elif array_mode == "zero_dim":
         assert isinstance(arr, typing.Mapping)
         data = np.array(arr["data"])
         if tuple(arr["shape"]) != tuple(data.shape):
             raise ValueError(f"invalid shape: {arr}")
         return data
```

### Comparing `muutils-0.3.9/muutils/json_serialize/dataclass_factories.py` & `muutils-0.4.0/muutils/json_serialize/dataclass_factories.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/json_serialize/json_serialize.py` & `muutils-0.4.0/muutils/json_serialize/json_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,20 @@
             self, obj.detach().cpu(), path=path
         ),
         uid="torch.Tensor",
     ),
     SerializerHandler(
         check=lambda self, obj, path: str(type(obj))
         == "<class 'pandas.core.frame.DataFrame'>",
-        serialize_func=lambda self, obj, path: obj.to_dict(orient="records"),
+        serialize_func=lambda self, obj, path: dict(
+            __format__="pandas.DataFrame",
+            columns=obj.columns.tolist(),
+            data=obj.to_dict(orient="records"),
+            path=path,
+        ),
         uid="pandas.DataFrame",
     ),
     SerializerHandler(
         check=lambda self, obj, path: isinstance(obj, (set, list, tuple))
         or isinstance(obj, Iterable),
         serialize_func=lambda self, obj, path: [
             self.json_serialize(x, tuple(path) + (i,)) for i, x in enumerate(obj)
```

### Comparing `muutils-0.3.9/muutils/json_serialize/serializable_dataclass.py` & `muutils-0.4.0/muutils/json_serialize/serializable_dataclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         default: Any | dataclasses._MISSING_TYPE = dataclasses.MISSING,
         default_factory: Callable[[], Any]
         | dataclasses._MISSING_TYPE = dataclasses.MISSING,
         init: bool = True,
         repr: bool = True,
         hash: Optional[bool] = None,
         compare: bool = True,
+        # TODO: add field for custom comparator (such as serializing)
         metadata: types.MappingProxyType | None = None,
         kw_only: bool | dataclasses._MISSING_TYPE = dataclasses.MISSING,
         serialize: bool = True,
         serialization_fn: Optional[Callable[[Any], Any]] = None,
         loading_fn: Optional[Callable[[Any], Any]] = None,
         assert_type: bool = True,
     ):
@@ -188,15 +189,24 @@
 
 
     # TODO: there is some duplication here with register_loader_handler
     """
     global _zanj_loading_needs_import
 
     if _zanj_loading_needs_import:
-        from muutils.zanj.loading import LoaderHandler, register_loader_handler
+        try:
+            from zanj.loading import (  # type: ignore[import]
+                LoaderHandler,
+                register_loader_handler,
+            )
+        except ImportError:
+            warnings.warn(
+                "ZANJ not installed, cannot register serializable dataclass loader. ZANJ can be found at https://github.com/mivanit/ZANJ"
+            )
+            return
 
     _format: str = f"{cls.__name__}(SerializableDataclass)"
     lh: LoaderHandler = LoaderHandler(
         check=lambda json_item, path=None, z=None: (  # type: ignore
             isinstance(json_item, dict)
             and "__format__" in json_item
             and json_item["__format__"].startswith(_format)
@@ -227,73 +237,90 @@
 
     def __eq__(self, other: Any) -> bool:
         return dc_eq(self, other)
 
     def __hash__(self) -> int:
         return hash(json.dumps(self.serialize()))
 
-    def diff(self, other: "SerializableDataclass") -> dict[str, Any]:
+    def diff(
+        self, other: "SerializableDataclass", of_serialized: bool = False
+    ) -> dict[str, Any]:
         if type(self) != type(other):
             raise ValueError(
                 f"Instances must be of the same type, but got {type(self)} and {type(other)}"
             )
 
         diff_result: dict = {}
 
         if self == other:
             return diff_result
 
-        for field in dataclasses.fields(self):
+        if of_serialized:
+            ser_self: dict = self.serialize()
+            ser_other: dict = other.serialize()
+
+        for field in dataclasses.fields(self):  # type: ignore[arg-type]
             if not field.compare:
                 continue
 
             field_name: str = field.name
             self_value = getattr(self, field_name)
             other_value = getattr(other, field_name)
 
             if isinstance(self_value, SerializableDataclass) and isinstance(
                 other_value, SerializableDataclass
             ):
-                nested_diff: dict = self_value.diff(other_value)
+                nested_diff: dict = self_value.diff(
+                    other_value, of_serialized=of_serialized
+                )
                 if nested_diff:
                     diff_result[field_name] = nested_diff
             elif dataclasses.is_dataclass(self_value) and dataclasses.is_dataclass(
                 other_value
             ):
                 raise ValueError("Non-serializable dataclass is not supported")
             else:
-                if not array_safe_eq(self_value, other_value):
+                self_value_s = ser_self[field_name] if of_serialized else self_value
+                other_value_s = ser_other[field_name] if of_serialized else other_value
+                if not array_safe_eq(self_value_s, other_value_s):
                     diff_result[field_name] = {"self": self_value, "other": other_value}
 
         return diff_result
 
     def update_from_nested_dict(self, nested_dict: dict[str, Any]):
-        for field in dataclasses.fields(self):
+        for field in dataclasses.fields(self):  # type: ignore[arg-type]
             field_name: str = field.name
             self_value = getattr(self, field_name)
 
             if field_name in nested_dict:
                 if isinstance(self_value, SerializableDataclass):
                     self_value.update_from_nested_dict(nested_dict[field_name])
                 else:
                     setattr(self, field_name, nested_dict[field_name])
 
+    def __copy__(self) -> "SerializableDataclass":
+        return self.__class__.load(self.serialize())
+
+    def __deepcopy__(self, memo: dict) -> "SerializableDataclass":
+        return self.__class__.load(self.serialize())
+
 
 # Step 3: Create a custom serializable_dataclass decorator
 def serializable_dataclass(
     # this should be `_cls: Type[T] | None = None,` but mypy doesn't like it
     _cls=None,  # type: ignore
     *,
     init: bool = True,
     repr: bool = True,
     eq: bool = True,
     order: bool = False,
     unsafe_hash: bool = False,
     frozen: bool = False,
     properties_to_serialize: Optional[list[str]] = None,
+    register_handler: bool = True,
     **kwargs,
 ):
     # -> Union[Callable[[Type[T]], Type[T]], Type[T]]:
 
     if properties_to_serialize is None:
         _properties_to_serialize: list = list()
     else:
@@ -396,15 +423,15 @@
                         and hasattr(field_type_hint, "load")
                         and callable(field_type_hint.load)
                     ):
                         if isinstance(value, dict):
                             value = field_type_hint.load(value)
                         else:
                             raise ValueError(
-                                f"Cannot load value into {field_type_hint}, espected {type(value) = } to be a dict\n{value = }"
+                                f"Cannot load value into {field_type_hint}, expected {type(value) = } to be a dict\n{value = }"
                             )
 
                     if field.assert_type:
                         if field.name in ctor_kwargs:
                             assert isinstance(ctor_kwargs[field.name], field_type_hint)
 
                     ctor_kwargs[field.name] = value
@@ -415,15 +442,16 @@
         cls.serialize = serialize  # type: ignore[attr-defined]
         # type is `Callable[[dict], T]`
         cls.load = load  # type: ignore[attr-defined]
 
         cls.__eq__ = lambda self, other: dc_eq(self, other)  # type: ignore[assignment]
 
         # Register the class with ZANJ
-        zanj_register_loader_serializable_dataclass(cls)
+        if register_handler:
+            zanj_register_loader_serializable_dataclass(cls)
 
         return cls
 
     if _cls is None:
         return wrap
     else:
         return wrap(_cls)
```

### Comparing `muutils-0.3.9/muutils/json_serialize/util.py` & `muutils-0.4.0/muutils/json_serialize/util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/jsonlines.py` & `muutils-0.4.0/muutils/jsonlines.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/logger/exception_context.py` & `muutils-0.4.0/muutils/logger/exception_context.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/logger/headerfuncs.py` & `muutils-0.4.0/muutils/logger/headerfuncs.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/logger/log_util.py` & `muutils-0.4.0/muutils/logger/log_util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/logger/logger.py` & `muutils-0.4.0/muutils/logger/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                     "exception",
                     "exceptions",
                     "errors",
                 },
             )
 
         # check alias duplicates
-        alias_set: set[str] = set()
+        alias_set: set[str | None] = set()
         for stream in self._streams.values():
             for alias in stream.aliases:
                 if alias in alias_set:
                     raise ValueError(f"alias {alias} is already in use")
                 alias_set.add(alias)
 
         # add aliases
```

### Comparing `muutils-0.3.9/muutils/logger/loggingstream.py` & `muutils-0.4.0/muutils/logger/loggingstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             - if a fileIO type object, will write to that object
     - `default_level: int|None` default level for this stream
     - `default_contents: dict[str, Callable[[], Any]]` default contents for this stream
     - `last_msg: tuple[float, Any]|None` last message written to this stream (timestamp, message)
     """
 
     name: str | None
-    aliases: set[str] = field(default_factory=set)
+    aliases: set[str | None] = field(default_factory=set)
     file: str | bool | AnyIO | None = None
     default_level: int | None = None
     default_contents: dict[str, Callable[[], Any]] = field(default_factory=dict)
     handler: AnyIO | None = None
 
     # TODO: implement last-message caching
     # last_msg: tuple[float, Any]|None = None
@@ -71,15 +71,15 @@
                 raise ValueError(f"stream {self.name} has invalid handler {self.file}")
             # ignore type check because we know it has a .write() method,
             # assume the user knows what they're doing
             return self.file  # type: ignore
 
     def __post_init__(self):
         self.aliases = set(self.aliases)
-        if any(x.startswith("_") for x in self.aliases):
+        if any(x.startswith("_") for x in self.aliases if x is not None):
             raise ValueError(
                 "stream names or aliases cannot start with an underscore, sorry"
             )
         self.aliases.add(self.name)
         self.default_contents["_timestamp"] = time.time
         self.default_contents["_stream"] = lambda: self.name
         self.handler = self.make_handler()
```

### Comparing `muutils-0.3.9/muutils/logger/simplelogger.py` & `muutils-0.4.0/muutils/logger/simplelogger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/logger/timing.py` & `muutils-0.4.0/muutils/logger/timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import time
+from typing import Literal
 
 
 class TimerContext:
     """context manager for timing code"""
 
-    def __init__(self):
-        self.start_time: float = None
-        self.end_time: float = None
-        self.elapsed_time: float = None
+    def __init__(self) -> None:
+        self.start_time: float
+        self.end_time: float
+        self.elapsed_time: float
 
-    def __enter__(self):
+    def __enter__(self) -> "TimerContext":
         self.start_time = time.time()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type, exc_val, exc_tb) -> Literal[False]:
         self.end_time = time.time()
         self.elapsed_time = self.end_time - self.start_time
         return False
 
 
 def filter_time_str(time: str) -> str:
     """assuming format `h:mm:ss`, clips off the hours if its 0"""
```

### Comparing `muutils-0.3.9/muutils/statcounter.py` & `muutils-0.4.0/muutils/statcounter.py`

 * *Files 18% similar despite different names*

```diff
@@ -243,43 +243,7 @@
         std=_compute_err(counter.std(), np.std(arr)),
         min=_compute_err(counter.min(), np.min(arr)),
         q1=_compute_err(counter.percentile(0.25), np.percentile(arr, 25)),
         median=_compute_err(counter.median(), np.median(arr)),
         q3=_compute_err(counter.percentile(0.75), np.percentile(arr, 75)),
         max=_compute_err(counter.max(), np.max(arr)),
     )
-
-
-def _test_statscounter():
-    arrs: list[np.ndarray] = [
-        np.array([0, 1]),
-        np.array([1, 2]),
-        np.random.randint(0, 10, size=100),
-        np.random.randint(-5, 15, size=10),
-        np.array([-5, -4, -1, 1, 1, 3, 3, 5, 11, 12]),
-        np.random.randint(-5, 15, size=10000),
-        np.random.randint(0, 100, size=100),
-        np.random.randint(0, 1000, size=10000),
-    ]
-
-    for i, j in np.random.randint(1, 100, size=(50, 2)):
-        if i > j:
-            i, j = j, i
-
-        arrs.append(np.random.randint(i, j, size=1000))
-
-    import json
-
-    for a in arrs:
-        r = _compare_np_custom(a)
-
-        if any(x["diff"] > 0.00000000001 for x in r.values()):
-            print("!!!!!!!!!!!!!!!!!!!!")
-            print(f"errs for rantint array: {a.shape = } {np.min(a) =} {np.max(a) =}")
-            print(json.dumps(r, indent=2))
-        # s = StatCounter(a)
-        # print(s.total(), s)
-        # print(sorted(list(s.elements())))
-
-
-# if __name__ == '__main__':
-#     _test_statscounter()
```

### Comparing `muutils-0.3.9/muutils/sysinfo.py` & `muutils-0.4.0/muutils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `muutils-0.3.9/muutils/tensor_utils.py` & `muutils-0.4.0/muutils/tensor_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                     "cls.__doc__": cls.__doc__,
                     "params": params,
                     "type(params)": type(params),
                 }
             )
 
         @typing._tp_cache  # type: ignore
-        def __class_getitem__(cls, params):
+        def __class_getitem__(cls, params: str | tuple) -> type:
             # MyTensor["dim1 dim2"]
             if isinstance(params, str):
                 return default_jax_dtype[array_type, params]
 
             elif isinstance(params, tuple):
                 if len(params) != 2:
                     raise Exception(
@@ -111,16 +111,18 @@
                     elif legacy_mode == "warn":
                         warnings.warn(
                             f"legacy type annotation was used:\n{cls.param_info(params)}"
                         )
                     # MyTensor[("dim1", "dim2"), int]
                     shape_anot: list[str] = list()
                     for x in params[0]:
-                        if isinstance(x, (str, int)):
+                        if isinstance(x, str):
                             shape_anot.append(x)
+                        elif isinstance(x, int):
+                            shape_anot.append(str(x))
                         elif isinstance(x, tuple):
                             shape_anot.append("".join(str(y) for y in x))
                         else:
                             raise Exception(
                                 f"unexpected type for params:\n{cls.param_info(params)}"
                             )
```

### Comparing `muutils-0.3.9/pyproject.toml` & `muutils-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muutils"
-version = "0.3.9"
+version = "0.4.0"
 description = "A collection of miscellaneous python utilities"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -34,14 +34,15 @@
 
 [tool.pycln]
 all = true
 exclude = "_wip"
 
 [tool.isort]
 profile = "black"
+ignore_comments = false
 extend_skip = ["_wip"]
 
 [tool.black]
 extend-exclude = "_wip"
 
 [tool.mypy]
 exclude = ['_wip']
```

### Comparing `muutils-0.3.9/PKG-INFO` & `muutils-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muutils
-Version: 0.3.9
+Version: 0.4.0
 Summary: A collection of miscellaneous python utilities
 Home-page: https://github.com/mivanit/muutils
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,20 +21,27 @@
 Description-Content-Type: text/markdown
 
 
 
 `muutils`, stylized as "$\mu$utils" or "μutils", is a collection of miscellaneous python utilities, meant to be small and with ~~no~~ minimal dependencies outside of standard python.
 
 
-- [`json_serialize`](https://github.com/mivanit/muutils/tree/main/muutils/json_serialize.py) is a tool for serializing and loading arbitrary python objects into json
+- [`json_serialize`](https://github.com/mivanit/muutils/tree/main/muutils/json_serialize.py) is a tool for serializing and loading arbitrary python objects into json. plays nicely with [`ZANJ`](https://github.com/mivanit/ZANJ/)
 - [`statcounter`](https://github.com/mivanit/muutils/tree/main/muutils/statcounter.py) is an extension of `collections.Counter` that provides "smart" computation of stats (mean, variance, median, other percentiles) from the counter object without using `Counter.elements()`
+- `misc` contains a few utilities:
+	- `stable_hash()` uses `hashlib.sha256` to compute a hash of an object that is stable across runs of python
+	- `sanitize_fname()` takes any string and makes it only alphanumeric plus `-` and `_`
+	- `shorten_numerical_to_str()` turns numbers like `123456789` into `"123M"`
+	- a couple other things
+- [`nbutils`] (WIP) contains some utilities for working in notebooks (printing latex nicely) and also running notebooks as tests in CI by converting them to python scripts
+- [`tensor_utils`] contains minor utilities for working with pytorch tensors and numpy arrays. This needs to be moved into ZANJ, probably
 - [`group_equiv`](https://github.com/mivanit/muutils/tree/main/muutils/group_equiv.py) groups elements from a sequence according to a given equivalence relation, without assuming that the equivalence relation obeys the transitive property
 - [`logger`](https://github.com/mivanit/muutils/tree/main/muutils/logger.py) implements a logger with "streams" and a timer context manager
 - [`jsonlines`](https://github.com/mivanit/muutils/tree/main/muutils/jsonlines.py) extremely simple utility for reading/writing `jsonl` files
-- [`ZANJ`](https://github.com/mivanit/muutils/tree/main/muutils/zanj/zanj.py) is a WIP hdf5 alternative. This will probably be spun off into its own repo
+- [`ZANJ`](https://github.com/mivanit/ZANJ/) is a WIP hdf5 alternative. This ~~will probably be~~ has been spun off into its own repo
 
 There are a couple work-in-progress utilities in [`_wip`](https://github.com/mivanit/muutils/tree/main/muutils/_wip/) that aren't ready for anything, but nothing in this repo is suitable for production. Use at your own risk!
 
 
 # installation
 
 ```
```

