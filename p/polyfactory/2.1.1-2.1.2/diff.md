# Comparing `tmp/polyfactory-2.1.1.tar.gz` & `tmp/polyfactory-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.1.1.tar", max compression
+gzip compressed data, was "polyfactory-2.1.2.tar", max compression
```

## Comparing `polyfactory-2.1.1.tar` & `polyfactory-2.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1092 2023-05-17 19:31:53.700877 polyfactory-2.1.1/LICENSE
--rw-r--r--   0        0        0     9082 2023-05-17 19:31:53.700877 polyfactory-2.1.1/README.md
--rw-r--r--   0        0        0      425 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/__init__.py
--rw-r--r--   0        0        0      642 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    30193 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2757 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1603 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2193 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0     7552 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1471 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     2939 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3328 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/fields.py
--rw-r--r--   0        0        0     1191 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/py.typed
--rw-r--r--   0        0        0     2890 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3401 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     2807 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1838 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13431 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0     3845 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0     3635 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-05-17 19:31:53.704877 polyfactory-2.1.1/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6030 2023-05-17 19:31:53.704877 polyfactory-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    11105 1970-01-01 00:00:00.000000 polyfactory-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-28 07:11:11.577643 polyfactory-2.1.2/LICENSE
+-rw-r--r--   0        0        0     9429 2023-05-28 07:11:11.577643 polyfactory-2.1.2/README.md
+-rw-r--r--   0        0        0      425 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    30734 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2757 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1603 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2193 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0     7552 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1471 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     2939 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3328 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/fields.py
+-rw-r--r--   0        0        0     1191 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/py.typed
+-rw-r--r--   0        0        0     2890 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3401 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     2807 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1838 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13431 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0     3845 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0     3635 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6185 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6030 2023-05-28 07:11:11.581643 polyfactory-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11250 1970-01-01 00:00:00.000000 polyfactory-2.1.2/PKG-INFO
```

### Comparing `polyfactory-2.1.1/LICENSE` & `polyfactory-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/README.md` & `polyfactory-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors-)
 
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 <!-- markdownlint-restore -->
 
 Polyfactory is a simple and powerful mock data generation library, based around type
@@ -102,22 +102,25 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/guacs"><img src="https://avatars.githubusercontent.com/u/126393040?v=4?s=100" width="100px;" alt="guacs"/><br /><sub><b>guacs</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=guacs" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `polyfactory-2.1.1/polyfactory/constants.py` & `polyfactory-2.1.2/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/decorators.py` & `polyfactory-2.1.2/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/exceptions.py` & `polyfactory-2.1.2/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/factories/base.py` & `polyfactory-2.1.2/polyfactory/factories/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from ipaddress import (
     IPv4Address,
     IPv4Interface,
     IPv4Network,
     IPv6Address,
     IPv6Interface,
     IPv6Network,
+    ip_address,
+    ip_network,
+    ip_interface,
 )
 from os.path import realpath
 from pathlib import Path
 from random import Random
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -408,27 +411,27 @@
             list: cls.__faker__.pylist,
             set: cls.__faker__.pyset,
             frozenset: lambda: frozenset(cls.__faker__.pylist()),
             deque: lambda: deque(cls.__faker__.pylist()),
             # standard library objects
             Path: lambda: Path(realpath(__file__)),
             Decimal: cls.__faker__.pydecimal,
-            UUID: cls.__faker__.uuid4,
+            UUID: lambda: UUID(cls.__faker__.uuid4()),
             # datetime
             datetime: cls.__faker__.date_time_between,
             date: cls.__faker__.date_this_decade,
-            time: cls.__faker__.time,
+            time: cls.__faker__.time_object,
             timedelta: cls.__faker__.time_delta,
             # ip addresses
-            IPv4Address: cls.__faker__.ipv4,
-            IPv4Interface: cls.__faker__.ipv4,
-            IPv4Network: lambda: cls.__faker__.ipv4(network=True),
-            IPv6Address: cls.__faker__.ipv6,
-            IPv6Interface: cls.__faker__.ipv6,
-            IPv6Network: lambda: cls.__faker__.ipv6(network=True),
+            IPv4Address: lambda: ip_address(cls.__faker__.ipv4()),
+            IPv4Interface: lambda: ip_interface(cls.__faker__.ipv4()),
+            IPv4Network: lambda: ip_network(cls.__faker__.ipv4(network=True)),
+            IPv6Address: lambda: ip_address(cls.__faker__.ipv6()),
+            IPv6Interface: lambda: ip_interface(cls.__faker__.ipv6()),
+            IPv6Network: lambda: ip_network(cls.__faker__.ipv6(network=True)),
             # types
             Callable: _create_generic_fn,
             Counter: lambda: Counter(cls.__faker__.pystr()),
             **_create_pydantic_type_map(cls),
         }
 
     @classmethod
@@ -525,25 +528,35 @@
                 pattern=constraints.get("pattern"),
             )
 
         if (
             is_safe_subclass(annotation, set)
             or is_safe_subclass(annotation, list)
             or is_safe_subclass(annotation, frozenset)
+            or is_safe_subclass(annotation, tuple)
         ):
-            result = handle_constrained_collection(
-                collection_type=list if is_safe_subclass(annotation, list) else set,  # pyright: ignore
+            collection_type: type[list] | type[set] | type[tuple] | type[frozenset]
+            if is_safe_subclass(annotation, list):
+                collection_type = list
+            elif is_safe_subclass(annotation, set):
+                collection_type = set
+            elif is_safe_subclass(annotation, tuple):
+                collection_type = tuple
+            else:
+                collection_type = frozenset
+
+            return handle_constrained_collection(
+                collection_type=collection_type,  # type: ignore
                 factory=cls,
                 field_meta=field_meta.children[0] if field_meta.children else field_meta,
                 item_type=constraints.get("item_type"),
                 max_items=constraints.get("max_length"),
                 min_items=constraints.get("min_length"),
                 unique_items=constraints.get("unique_items", False),
             )
-            return frozenset(result) if is_safe_subclass(annotation, frozenset) else result
 
         if is_safe_subclass(annotation, date):
             return handle_constrained_date(
                 faker=cls.__faker__,
                 ge=cast("Any", constraints.get("ge")),
                 gt=cast("Any", constraints.get("gt")),
                 le=cast("Any", constraints.get("le")),
@@ -576,15 +589,15 @@
         if is_literal(annotation=unwrapped_annotation) and (literal_args := get_args(unwrapped_annotation)):
             return cls.__random__.choice(literal_args)
 
         if isinstance(unwrapped_annotation, EnumMeta):
             return cls.__random__.choice(list(unwrapped_annotation))  # pyright: ignore
 
         if field_meta.constraints and (
-            unwrapped_annotation in (float, int, Decimal, str, list, tuple, set, frozenset)
+            unwrapped_annotation in (float, int, Decimal, bytes, str, list, tuple, set, frozenset, date)
             or unwrapped_annotation not in cls.get_provider_map()
         ):
             return cls.get_constrained_field_value(annotation=unwrapped_annotation, field_meta=field_meta)
 
         if BaseFactory.is_factory_type(annotation=unwrapped_annotation):
             return cls._get_or_create_factory(model=unwrapped_annotation).build(
                 **(field_build_parameters if isinstance(field_build_parameters, Mapping) else {})
```

### Comparing `polyfactory-2.1.1/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.1.2/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.1.2/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.1.2/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.1.2/polyfactory/factories/pydantic_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.1.2/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/field_meta.py` & `polyfactory-2.1.2/polyfactory/field_meta.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/fields.py` & `polyfactory-2.1.2/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/persistence.py` & `polyfactory-2.1.2/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/pytest_plugin.py` & `polyfactory-2.1.2/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/utils/helpers.py` & `polyfactory-2.1.2/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/utils/predicates.py` & `polyfactory-2.1.2/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/value_generators/complex_types.py` & `polyfactory-2.1.2/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.1.2/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.1.2/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.1.2/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.1.2/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/value_generators/primitives.py` & `polyfactory-2.1.2/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/polyfactory/value_generators/regex.py` & `polyfactory-2.1.2/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.1/pyproject.toml` & `polyfactory-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.1.1"
+version = "2.1.2"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
```

### Comparing `polyfactory-2.1.1/PKG-INFO` & `polyfactory-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.1.1
+Version: 2.1.2
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: dataclasses,factory,faker,mock,pydantic,pytest,litestar,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -19,18 +19,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: beanie
@@ -69,15 +65,15 @@
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors-)
 
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 <!-- markdownlint-restore -->
 
 Polyfactory is a simple and powerful mock data generation library, based around type
@@ -149,22 +145,25 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/guacs"><img src="https://avatars.githubusercontent.com/u/126393040?v=4?s=100" width="100px;" alt="guacs"/><br /><sub><b>guacs</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=guacs" title="Code">💻</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

