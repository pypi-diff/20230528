# Comparing `tmp/taipan_di-0.0.1.tar.gz` & `tmp/taipan_di-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipan_di-0.0.1.tar", max compression
+gzip compressed data, was "taipan_di-0.0.2.tar", max compression
```

## Comparing `taipan_di-0.0.1.tar` & `taipan_di-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-05-24 15:05:15.988156 taipan_di-0.0.1/LICENSE
--rw-r--r--   0        0        0     2894 2023-05-24 15:05:15.988156 taipan_di-0.0.1/README.md
--rw-r--r--   0        0        0     1004 2023-05-24 15:05:15.988156 taipan_di-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      110 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/__init__.py
--rw-r--r--   0        0        0       21 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/__version__.py
--rw-r--r--   0        0        0       55 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/classes/__init__.py
--rw-r--r--   0        0        0     2557 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/classes/dependency_collection.py
--rw-r--r--   0        0        0      676 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/classes/dependency_container.py
--rw-r--r--   0        0        0      703 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/classes/dependency_provider.py
--rw-r--r--   0        0        0     3651 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/classes/instanciate_service.py
--rw-r--r--   0        0        0       83 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/classes/scopes/__init__.py
--rw-r--r--   0        0        0      644 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/classes/scopes/factory_scope.py
--rw-r--r--   0        0        0      781 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/classes/scopes/singleton_scope.py
--rw-r--r--   0        0        0      204 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/errors/__init__.py
--rw-r--r--   0        0        0       38 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/errors/taipan_error.py
--rw-r--r--   0        0        0      105 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/errors/taipan_injection_error.py
--rw-r--r--   0        0        0      100 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/errors/taipan_type_error.py
--rw-r--r--   0        0        0      108 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/errors/taipan_unregistered_error.py
--rw-r--r--   0        0        0      157 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/interfaces/__init__.py
--rw-r--r--   0        0        0      938 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/interfaces/base_dependency_container.py
--rw-r--r--   0        0        0      614 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/interfaces/base_dependency_provider.py
--rw-r--r--   0        0        0      519 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/interfaces/base_scope.py
--rw-r--r--   0        0        0        0 2023-05-24 15:05:15.988156 taipan_di-0.0.1/taipan_di/py.typed
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 taipan_di-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-28 19:09:58.108375 taipan_di-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2894 2023-05-28 19:09:58.108375 taipan_di-0.0.2/README.md
+-rw-r--r--   0        0        0     1025 2023-05-28 19:09:58.108375 taipan_di-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/__version__.py
+-rw-r--r--   0        0        0       55 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/__init__.py
+-rw-r--r--   0        0        0     2832 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/dependency_collection.py
+-rw-r--r--   0        0        0      676 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/dependency_container.py
+-rw-r--r--   0        0        0      703 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/dependency_provider.py
+-rw-r--r--   0        0        0     3651 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/instanciate_service.py
+-rw-r--r--   0        0        0       83 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/scopes/__init__.py
+-rw-r--r--   0        0        0      686 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/scopes/factory_scope.py
+-rw-r--r--   0        0        0      800 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/classes/scopes/singleton_scope.py
+-rw-r--r--   0        0        0      204 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/taipan_error.py
+-rw-r--r--   0        0        0      105 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/taipan_injection_error.py
+-rw-r--r--   0        0        0      100 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/taipan_type_error.py
+-rw-r--r--   0        0        0      108 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/errors/taipan_unregistered_error.py
+-rw-r--r--   0        0        0      157 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/interfaces/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/interfaces/base_dependency_container.py
+-rw-r--r--   0        0        0      614 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/interfaces/base_dependency_provider.py
+-rw-r--r--   0        0        0      519 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/interfaces/base_scope.py
+-rw-r--r--   0        0        0        0 2023-05-28 19:09:58.108375 taipan_di-0.0.2/taipan_di/py.typed
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 taipan_di-0.0.2/PKG-INFO
```

### Comparing `taipan_di-0.0.1/LICENSE` & `taipan_di-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.1/README.md` & `taipan_di-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.1/pyproject.toml` & `taipan_di-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Taipan-DI"
-version = "0.0.1"
+version = "0.0.2"
 description = "Truly Amazing Inversion of control Python library Analogous to .Net's DI"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["taipan", "dependency injection", "dependency", "python"]
 
@@ -18,14 +18,15 @@
 ]
 
 include = ["taipan_di/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.6.0"
+typeguard = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 black = "^23.3.0"
 mypy = "^1.3.0"
```

### Comparing `taipan_di-0.0.1/taipan_di/classes/dependency_collection.py` & `taipan_di-0.0.2/taipan_di/classes/dependency_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Callable, Type, TypeVar
 
 from taipan_di.interfaces import BaseDependencyProvider
 from taipan_di.errors import TaipanTypeError
+from typeguard import check_type
 
 from .dependency_container import DependencyContainer
 from .instanciate_service import instanciate_service
 from .scopes import FactoryScope, SingletonScope
 
 
 T = TypeVar("T")
@@ -27,43 +28,51 @@
     def register_singleton_instance(self, type: Type[T], instance: T) -> None:
         self._assert_instance_type(instance, type)
 
         creator = lambda provider: instance
         self.register_singleton_creator(type, creator)
 
     def register_singleton(
-        self, interface_type: Type[T], implementation_type: Type[U]
+        self, interface_type: Type[T], implementation_type: Type[U] = None
     ) -> None:
+        if implementation_type is None:
+            implementation_type = interface_type
+            
         self._assert_implementation_derives_interface(implementation_type, interface_type)
 
         creator = lambda provider: instanciate_service(implementation_type, provider)
         self.register_singleton_creator(interface_type, creator)
 
     def register_factory_creator(
         self, type: Type[T], creator: Callable[[BaseDependencyProvider], T]
     ) -> None:
         service = FactoryScope(creator)
         self._container.register(type, service)
 
     def register_factory(
-        self, interface_type: Type[T], implementation_type: Type[U]
+        self, interface_type: Type[T], implementation_type: Type[U] = None
     ) -> None:
+        if implementation_type is None:
+            implementation_type = interface_type
+            
         self._assert_implementation_derives_interface(implementation_type, interface_type)
 
         creator = lambda provider: instanciate_service(implementation_type, provider)
         self.register_factory_creator(interface_type, creator)
 
     def build(self) -> BaseDependencyProvider:
         return self._container.build()
 
     # Private methods
 
     def _assert_instance_type(self, instance: Any, type: Type) -> None:
-        if not isinstance(instance, type):
-            raise TaipanTypeError("Provided instance is not of type %s", str(type))
+        try:
+            check_type(instance, type)
+        except:
+            raise TaipanTypeError(f"Provided instance is not of type {str(type)}")
 
     def _assert_implementation_derives_interface(
         self, implementation_type: Type[U], interface_type: Type[T]
     ) -> None:
         if not issubclass(implementation_type, interface_type):
             raise TaipanTypeError(
                 "Implementation type %s must derive from interface type %s",
```

### Comparing `taipan_di-0.0.1/taipan_di/classes/dependency_container.py` & `taipan_di-0.0.2/taipan_di/classes/dependency_container.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.1/taipan_di/classes/dependency_provider.py` & `taipan_di-0.0.2/taipan_di/classes/dependency_provider.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.1/taipan_di/classes/instanciate_service.py` & `taipan_di-0.0.2/taipan_di/classes/instanciate_service.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.1/taipan_di/classes/scopes/factory_scope.py` & `taipan_di-0.0.2/taipan_di/classes/scopes/factory_scope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Any, Callable, Type, TypeVar, cast
+from typeguard import check_type
 
 from taipan_di.interfaces import BaseDependencyProvider, BaseScope
 from taipan_di.errors import TaipanTypeError
 
 T = TypeVar("T")
 
 class FactoryScope(BaseScope):
     def __init__(self, creator: Callable[[BaseDependencyProvider], Any]) -> None:
         self._creator = creator
 
     def get_instance(self, type: Type[T], container: BaseDependencyProvider) -> T:
         instance = self._creator(container)
-
-        if not isinstance(instance, type):
-            raise TaipanTypeError("Created instance is not of type %s", str(type))
-
-        result = cast(T, instance)
-        return result
+        
+        try:
+            result = check_type(instance, type)
+            return result
+        except:
+            raise TaipanTypeError(f"Created instance is not of type {str(type)}")
```

### Comparing `taipan_di-0.0.1/taipan_di/classes/scopes/singleton_scope.py` & `taipan_di-0.0.2/taipan_di/classes/scopes/singleton_scope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Any, Callable, Type, TypeVar, cast
 
 from taipan_di.interfaces import BaseDependencyProvider, BaseScope
 from taipan_di.errors import TaipanTypeError
+from typeguard import check_type
 
 T = TypeVar("T")
 
 class SingletonScope(BaseScope):
     def __init__(self, creator: Callable[[BaseDependencyProvider], Any]) -> None:
         self._creator = creator
         self._memoized_instance = None
 
     def get_instance(self, type: Type[T], container: BaseDependencyProvider) -> T:
         if self._memoized_instance is None:
             self._memoized_instance = self._creator(container)
 
-        if not isinstance(self._memoized_instance, type):
-            raise TaipanTypeError("Registered instance is not of type %s", str(type))
-
-        result = cast(T, self._memoized_instance)
-        return result
+        try:
+            result = check_type(self._memoized_instance, type)
+            return result
+        except:
+            raise TaipanTypeError(f"Registered instance is not of type {str(type)}")
```

### Comparing `taipan_di-0.0.1/taipan_di/interfaces/base_dependency_container.py` & `taipan_di-0.0.2/taipan_di/interfaces/base_dependency_container.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.1/taipan_di/interfaces/base_dependency_provider.py` & `taipan_di-0.0.2/taipan_di/interfaces/base_dependency_provider.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.1/taipan_di/interfaces/base_scope.py` & `taipan_di-0.0.2/taipan_di/interfaces/base_scope.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.1/PKG-INFO` & `taipan_di-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: taipan-di
-Version: 0.0.1
+Version: 0.0.2
 Summary: Truly Amazing Inversion of control Python library Analogous to .Net's DI
 Home-page: https://github.com/Billuc/Taipan-DI
 License: MIT
 Keywords: taipan,dependency injection,dependency,python
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: typeguard (>=4.0.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.6.0,<5.0.0)
 Project-URL: Documentation, https://github.com/Billuc/Taipan-DI
 Project-URL: Repository, https://github.com/Billuc/Taipan-DI
 Description-Content-Type: text/markdown
 
 # Taipan-DI
```

