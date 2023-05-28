# Comparing `tmp/kaioretry-0.9.2.tar.gz` & `tmp/kaioretry-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaioretry-0.9.2.tar", max compression
+gzip compressed data, was "kaioretry-0.9.3.tar", max compression
```

## Comparing `kaioretry-0.9.2.tar` & `kaioretry-0.9.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    26526 2023-01-15 22:50:34.820830 kaioretry-0.9.2/LICENSE
--rw-r--r--   0        0        0     1594 2023-02-08 22:29:16.723125 kaioretry-0.9.2/README.md
--rw-r--r--   0        0        0     4982 2023-05-19 21:19:35.001878 kaioretry-0.9.2/kaioretry/__init__.py
--rw-r--r--   0        0        0     8113 2023-02-25 20:58:24.581309 kaioretry-0.9.2/kaioretry/context.py
--rw-r--r--   0        0        0     9876 2023-05-19 20:11:56.069743 kaioretry-0.9.2/kaioretry/decorator.py
--rw-r--r--   0        0        0        0 2023-05-19 21:06:43.593979 kaioretry-0.9.2/kaioretry/py.typed
--rw-r--r--   0        0        0     1453 2023-05-19 20:11:56.070743 kaioretry-0.9.2/kaioretry/types.py
--rw-r--r--   0        0        0     1178 2023-05-19 21:19:34.932878 kaioretry-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2704 1970-01-01 00:00:00.000000 kaioretry-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-01-15 22:50:34.820830 kaioretry-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1594 2023-02-08 22:29:16.723125 kaioretry-0.9.3/README.md
+-rw-r--r--   0        0        0     4985 2023-05-28 09:42:38.333240 kaioretry-0.9.3/kaioretry/__init__.py
+-rw-r--r--   0        0        0     8116 2023-05-28 09:40:31.637139 kaioretry-0.9.3/kaioretry/context.py
+-rw-r--r--   0        0        0     9876 2023-05-28 09:40:42.599065 kaioretry-0.9.3/kaioretry/decorator.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:06:43.593979 kaioretry-0.9.3/kaioretry/py.typed
+-rw-r--r--   0        0        0     1465 2023-05-28 09:34:43.823942 kaioretry-0.9.3/kaioretry/types.py
+-rw-r--r--   0        0        0     1178 2023-05-28 09:42:38.272241 kaioretry-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2704 1970-01-01 00:00:00.000000 kaioretry-0.9.3/PKG-INFO
```

### Comparing `kaioretry-0.9.2/LICENSE` & `kaioretry-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kaioretry-0.9.2/README.md` & `kaioretry-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `kaioretry-0.9.2/kaioretry/__init__.py` & `kaioretry-0.9.3/kaioretry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import logging
 import random
 
 from typing import Awaitable, cast
 from collections.abc import Callable
 
 from .types import Exceptions, NonNegative, Number, Jitter, \
-    FuncParam, FuncRetVal, UpdateDelayF, RetryDecorator, JitterTuple
+    FuncParam, FuncRetVal, UpdateDelayFunc, RetryDecorator, JitterTuple
 from .context import Context
 from .decorator import Retry
 
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 
 RETRY_PARAMS_DOCSTRING = """
     :param exceptions: exceptions classes that will trigger another
         try. Other exceptions raised by the decorated function will
         not trigger a retry. The value of the exceptions parameters
         can be either an :py:class:`Exception` class or a
```

### Comparing `kaioretry-0.9.2/kaioretry/context.py` & `kaioretry-0.9.3/kaioretry/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 import asyncio
 import logging
 import uuid
 
 from typing import cast, Awaitable, Any, TypeVar
 from collections.abc import Callable, Generator, AsyncGenerator
 
-from .types import NonNegative, Number, UpdateDelayF
+from .types import NonNegative, Number, UpdateDelayFunc
 
 
 SleepRetVal = TypeVar('SleepRetVal', None, Awaitable[None])
 SleepF = Callable[[Number], SleepRetVal]
 
 
 class _ContextIterator:
```

### Comparing `kaioretry-0.9.2/kaioretry/decorator.py` & `kaioretry-0.9.3/kaioretry/decorator.py`

 * *Files identical despite different names*

### Comparing `kaioretry-0.9.2/kaioretry/types.py` & `kaioretry-0.9.3/kaioretry/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from typing_extensions import Protocol
 
 # Protocols do not have public methods. This module will not define any
 # otherwise valid class.
 # pylint: disable=too-few-public-methods
 
 
-ExceptionT: TypeAlias = type[BaseException]
-ExceptionList: TypeAlias = tuple[ExceptionT, ...]
-Exceptions: TypeAlias = ExceptionList | ExceptionT
+ExceptionType: TypeAlias = type[BaseException]
+ExceptionList: TypeAlias = tuple[ExceptionType, ...]
+Exceptions: TypeAlias = ExceptionList | ExceptionType
 
 
 Number: TypeAlias = int | float
 
 
 # Until better implementation.
 NonNegative: TypeAlias = Number   # >= 0
@@ -32,15 +32,15 @@
 
 FuncParam = ParamSpec('FuncParam')
 FuncRetVal = TypeVar('FuncRetVal')
 
 Function: TypeAlias = Callable[..., Any]
 
 
-UpdateDelayF: TypeAlias = Callable[[NonNegative], NonNegative]
+UpdateDelayFunc: TypeAlias = Callable[[NonNegative], NonNegative]
 
 
 class RetryDecorator(Protocol):
     """Retry Decorator Type"""
     def __call__(self,
                  exceptions: Exceptions = Exception, tries: int = -1, *,
                  delay: NonNegative = 0, backoff: Number = 1,
```

### Comparing `kaioretry-0.9.2/pyproject.toml` & `kaioretry-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaioretry"
-version = "0.9.2"
+version = "0.9.3"
 description = "All in one retry and aioretry decorators"
 authors = ["Damien Nadé <anvil.github+kaioretry@livna.org>"]
 license = "LGPL-2.1-or-later"
 repository = "https://github.com/Anvil/kaioretry/"
 readme = "README.md"
 keywords = ["retry", "decorator", "asyncio"]
 documentation = "https://kaioretry.readthedocs.io/en/latest/"
```

### Comparing `kaioretry-0.9.2/PKG-INFO` & `kaioretry-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaioretry
-Version: 0.9.2
+Version: 0.9.3
 Summary: All in one retry and aioretry decorators
 Home-page: https://github.com/Anvil/kaioretry/
 License: LGPL-2.1-or-later
 Keywords: retry,decorator,asyncio
 Author: Damien Nadé
 Author-email: anvil.github+kaioretry@livna.org
 Requires-Python: >=3.10,<4.0
```

