# Comparing `tmp/sciform-0.6.0.tar.gz` & `tmp/sciform-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciform-0.6.0.tar", last modified: Sat May 27 21:45:10 2023, max compression
+gzip compressed data, was "sciform-0.6.1.tar", last modified: Sat May 27 22:09:18 2023, max compression
```

## Comparing `sciform-0.6.0.tar` & `sciform-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 21:45:10.314568 sciform-0.6.0/
--rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.6.0/LICENSE
--rw-rw-rw-   0        0        0    30674 2023-05-27 21:45:10.313074 sciform-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    30306 2023-05-27 07:11:38.000000 sciform-0.6.0/README.md
--rw-rw-rw-   0        0        0      589 2023-05-27 07:16:40.000000 sciform-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 21:45:10.314568 sciform-0.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 21:45:10.234326 sciform-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 21:45:10.285353 sciform-0.6.0/src/sciform/
--rw-rw-rw-   0        0        0       84 2023-05-27 21:42:56.000000 sciform-0.6.0/src/sciform/__init__.py
--rw-rw-rw-   0        0        0    16402 2023-05-27 21:42:44.000000 sciform-0.6.0/src/sciform/format_spec.py
--rw-rw-rw-   0        0        0     6226 2023-05-27 21:42:44.000000 sciform-0.6.0/src/sciform/format_utils.py
--rw-rw-rw-   0        0        0     2373 2023-05-26 18:40:38.000000 sciform-0.6.0/src/sciform/grouping.py
--rw-rw-rw-   0        0        0     4111 2023-05-27 21:42:44.000000 sciform-0.6.0/src/sciform/modes.py
--rw-rw-rw-   0        0        0     2258 2023-05-27 21:42:44.000000 sciform-0.6.0/src/sciform/prefix.py
--rw-rw-rw-   0        0        0     6664 2023-05-27 21:42:44.000000 sciform-0.6.0/src/sciform/sfloat.py
--rw-rw-rw-   0        0        0     3592 2023-05-27 06:34:06.000000 sciform-0.6.0/src/sciform/unc_format.py
-drwxrwxrwx   0        0        0        0 2023-05-27 21:45:10.310338 sciform-0.6.0/src/sciform.egg-info/
--rw-rw-rw-   0        0        0    30674 2023-05-27 21:45:10.000000 sciform-0.6.0/src/sciform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-05-27 21:45:10.000000 sciform-0.6.0/src/sciform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 21:45:10.000000 sciform-0.6.0/src/sciform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 21:45:10.000000 sciform-0.6.0/src/sciform.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 21:45:10.311796 sciform-0.6.0/tests/
--rw-rw-rw-   0        0        0    18672 2023-05-27 21:42:44.000000 sciform-0.6.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.232853 sciform-0.6.1/
+-rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0    32842 2023-05-27 22:09:18.232853 sciform-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    32474 2023-05-27 22:08:11.000000 sciform-0.6.1/README.md
+-rw-rw-rw-   0        0        0      589 2023-05-27 07:16:40.000000 sciform-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 22:09:18.232853 sciform-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.203997 sciform-0.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.220342 sciform-0.6.1/src/sciform/
+-rw-rw-rw-   0        0        0       84 2023-05-27 22:08:47.000000 sciform-0.6.1/src/sciform/__init__.py
+-rw-rw-rw-   0        0        0    16402 2023-05-27 21:42:44.000000 sciform-0.6.1/src/sciform/format_spec.py
+-rw-rw-rw-   0        0        0     6226 2023-05-27 21:42:44.000000 sciform-0.6.1/src/sciform/format_utils.py
+-rw-rw-rw-   0        0        0     2373 2023-05-26 18:40:38.000000 sciform-0.6.1/src/sciform/grouping.py
+-rw-rw-rw-   0        0        0     4111 2023-05-27 21:42:44.000000 sciform-0.6.1/src/sciform/modes.py
+-rw-rw-rw-   0        0        0     2258 2023-05-27 21:42:44.000000 sciform-0.6.1/src/sciform/prefix.py
+-rw-rw-rw-   0        0        0     6996 2023-05-27 21:58:23.000000 sciform-0.6.1/src/sciform/sfloat.py
+-rw-rw-rw-   0        0        0     3592 2023-05-27 06:34:06.000000 sciform-0.6.1/src/sciform/unc_format.py
+drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.230852 sciform-0.6.1/src/sciform.egg-info/
+-rw-rw-rw-   0        0        0    32842 2023-05-27 22:09:18.000000 sciform-0.6.1/src/sciform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-05-27 22:09:18.000000 sciform-0.6.1/src/sciform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 22:09:18.000000 sciform-0.6.1/src/sciform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 22:09:18.000000 sciform-0.6.1/src/sciform.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.231853 sciform-0.6.1/tests/
+-rw-rw-rw-   0        0        0    18672 2023-05-27 21:42:44.000000 sciform-0.6.1/tests/test.py
```

### Comparing `sciform-0.6.0/LICENSE` & `sciform-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sciform-0.6.0/PKG-INFO` & `sciform-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: sciform
-Version: 0.6.0
-Summary: A package for formatting floats into scientific formatted strings.
-Author-email: Justin Gerber <justin.gerber48@gmail.com>
-Project-URL: Homepage, https://github.com/jagerber48/sciform
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sciform
 
 This package is used to format floats into scientific presentation 
 formats. Features include fixed point, and decimal and binary scientific 
 and engineering notations. Where possible, formatting follows documented 
 standards such as those published by [BIPM](https://www.bipm.org/en/) or 
 [IEC](https://iec.ch/homepage).
@@ -211,23 +201,63 @@
 
 - `f'{sfloat(12.4e+06):rp}'` gives `'12 M`'
 - `f'{sfloat(1024*2**10):bp'` gives `1 Mi`
 
 
 # Configuration options (forthcoming)
 
-Forthcoming features to improve ease of configuration:
-- Function-based (as opposed to string formatting/`__format__` based) 
-  formatting.
-- Ability to set module or class level defaults for each FSML term to 
-  avoid repetitive, verbose format specifications.
-- Class-based API for storing default configurations?
-- Optional registration of new prefixes, notably `c`, `d`, `da`, and `h` which 
-  are recognized SI prefixes for 10<sup>-2</sup>, 10<sup>-1</sup>, 
-  10<sup>+1</sup> and 10<sup>+2</sup> respectively.
+It is possible to modify the global default configuration for `sciform`
+to avoid repetition of verbose (and difficult-to-parse-for-humans) 
+format specification strings. 
+
+The global defaults are stored in the `FMT_SPEC_GLOBAL_DEFAULTS` 
+`FormatSpec` object.
+When a call is made to format an `sfloat`, any parameters extracted from
+the format specification string are used for the formatting, while any 
+parameters not supplied are extracted from the global defaults object.
+
+The global configuration object can be permanently modified using the 
+`update_global_defaults()` function and `kwargs` corresponding to the 
+parameters the default configuration options the user would like to
+update (TODO: Documentation of acceptable `kwargs`). 
+The user can also pass in an entirely new replacement `FormatSpec`
+object to use as the new global configuration object.
+In this case any `kwargs` passed in will be used to update this new
+configuration object after it has replaced the old one.
+
+The global configuration object can also be temporarily modified using 
+the `GlobalDefaultsContext` context decorator. 
+Similarly, the user can pass in `kwargs` to modify the existing 
+configuration object as well as an entirely new configuration object. 
+Within the scope of the context manager the new global configuration 
+will be used, but when the context manager scope exits, the original 
+configuration will be restored.
+
+Modifying the global configuration allows the user to modify the mapping
+between exponents and SI or IEC prefixes.
+In particular, it is possible to include the `c` SI prefix (e.g. 
+1 cm = 10<sup>-2</sup> m) using the `include_c` kwarg as well as to
+include all of the `c`, `d`, `da`, and `h` SI prefixes corresponding to
+10<sup>-2</sup>, 10<sup>-1</sup>, 10<sup>+1</sup>, and 10<sup>+2</sup>
+respectively using the `include_small_si_prefixes` kwarg.
+
+The user can format floats directly using the `format_float` function 
+and passing in an explicitly defined `FormatSpec` object. In the future
+a function allowing users to format floats using kwargs directly will be
+included.
+
+In the future, configuration may be added for persistant class- and
+instance-level default configuration options. However, it needs to be
+decided how configuration will be shared between the different levels.
+For example, if an `sfloat` object is instantiated which does not 
+specify behavior for the `prefix` field, but then the `prefix` field at
+the global level is modified, should this `sfloat` instance adopt the
+new global config?
+Also, how should config conflicts be managed?
+One idea is to resolve conflicts by deferring to the parent config.
 
 
 # Value + uncertainty formatting (forthcoming)
 
 One of (if not the) most important use cases for scientific formatting
 is formatting a value together with its specified uncertainty, e.g.
 `84.3 +/- 0.2`. The ability to format pairs of floats as
```

### Comparing `sciform-0.6.0/README.md` & `sciform-0.6.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: sciform
+Version: 0.6.1
+Summary: A package for formatting floats into scientific formatted strings.
+Author-email: Justin Gerber <justin.gerber48@gmail.com>
+Project-URL: Homepage, https://github.com/jagerber48/sciform
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sciform
 
 This package is used to format floats into scientific presentation 
 formats. Features include fixed point, and decimal and binary scientific 
 and engineering notations. Where possible, formatting follows documented 
 standards such as those published by [BIPM](https://www.bipm.org/en/) or 
 [IEC](https://iec.ch/homepage).
@@ -201,23 +211,63 @@
 
 - `f'{sfloat(12.4e+06):rp}'` gives `'12 M`'
 - `f'{sfloat(1024*2**10):bp'` gives `1 Mi`
 
 
 # Configuration options (forthcoming)
 
-Forthcoming features to improve ease of configuration:
-- Function-based (as opposed to string formatting/`__format__` based) 
-  formatting.
-- Ability to set module or class level defaults for each FSML term to 
-  avoid repetitive, verbose format specifications.
-- Class-based API for storing default configurations?
-- Optional registration of new prefixes, notably `c`, `d`, `da`, and `h` which 
-  are recognized SI prefixes for 10<sup>-2</sup>, 10<sup>-1</sup>, 
-  10<sup>+1</sup> and 10<sup>+2</sup> respectively.
+It is possible to modify the global default configuration for `sciform`
+to avoid repetition of verbose (and difficult-to-parse-for-humans) 
+format specification strings. 
+
+The global defaults are stored in the `FMT_SPEC_GLOBAL_DEFAULTS` 
+`FormatSpec` object.
+When a call is made to format an `sfloat`, any parameters extracted from
+the format specification string are used for the formatting, while any 
+parameters not supplied are extracted from the global defaults object.
+
+The global configuration object can be permanently modified using the 
+`update_global_defaults()` function and `kwargs` corresponding to the 
+parameters the default configuration options the user would like to
+update (TODO: Documentation of acceptable `kwargs`). 
+The user can also pass in an entirely new replacement `FormatSpec`
+object to use as the new global configuration object.
+In this case any `kwargs` passed in will be used to update this new
+configuration object after it has replaced the old one.
+
+The global configuration object can also be temporarily modified using 
+the `GlobalDefaultsContext` context decorator. 
+Similarly, the user can pass in `kwargs` to modify the existing 
+configuration object as well as an entirely new configuration object. 
+Within the scope of the context manager the new global configuration 
+will be used, but when the context manager scope exits, the original 
+configuration will be restored.
+
+Modifying the global configuration allows the user to modify the mapping
+between exponents and SI or IEC prefixes.
+In particular, it is possible to include the `c` SI prefix (e.g. 
+1 cm = 10<sup>-2</sup> m) using the `include_c` kwarg as well as to
+include all of the `c`, `d`, `da`, and `h` SI prefixes corresponding to
+10<sup>-2</sup>, 10<sup>-1</sup>, 10<sup>+1</sup>, and 10<sup>+2</sup>
+respectively using the `include_small_si_prefixes` kwarg.
+
+The user can format floats directly using the `format_float` function 
+and passing in an explicitly defined `FormatSpec` object. In the future
+a function allowing users to format floats using kwargs directly will be
+included.
+
+In the future, configuration may be added for persistant class- and
+instance-level default configuration options. However, it needs to be
+decided how configuration will be shared between the different levels.
+For example, if an `sfloat` object is instantiated which does not 
+specify behavior for the `prefix` field, but then the `prefix` field at
+the global level is modified, should this `sfloat` instance adopt the
+new global config?
+Also, how should config conflicts be managed?
+One idea is to resolve conflicts by deferring to the parent config.
 
 
 # Value + uncertainty formatting (forthcoming)
 
 One of (if not the) most important use cases for scientific formatting
 is formatting a value together with its specified uncertainty, e.g.
 `84.3 +/- 0.2`. The ability to format pairs of floats as
```

### Comparing `sciform-0.6.0/pyproject.toml` & `sciform-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciform-0.6.0/src/sciform/format_spec.py` & `sciform-0.6.1/src/sciform/format_spec.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.0/src/sciform/format_utils.py` & `sciform-0.6.1/src/sciform/format_utils.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.0/src/sciform/grouping.py` & `sciform-0.6.1/src/sciform/grouping.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.0/src/sciform/modes.py` & `sciform-0.6.1/src/sciform/modes.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.0/src/sciform/prefix.py` & `sciform-0.6.1/src/sciform/prefix.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.0/src/sciform/sfloat.py` & `sciform-0.6.1/src/sciform/sfloat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from copy import copy
 from math import isfinite
+from typing import Optional
 
 from sciform.modes import (FillMode, GroupingSeparator, DecimalSeparator)
 from sciform.format_spec import (parse_format_spec, FormatSpec,
                                  update_global_defaults,
                                  get_global_defaults)
 from sciform.format_utils import (get_mantissa_exp_base, get_exp_str,
                                   get_top_and_bottom_digit,
@@ -161,20 +162,26 @@
         return self.to_sfloat(super().__sub__(x))
 
     def __truediv__(self, x: float) -> 'sfloat':
         return self.to_sfloat(super().__truediv__(x))
 
 
 class GlobalDefaultsContext:
-    def __init__(self, **kwargs):
+    def __init__(self,
+                 replacement_format_spec: Optional[FormatSpec] = None,
+                 **kwargs):
+        self.replacement_format_spec = replacement_format_spec
         self.kwargs = kwargs
         self.initial_global_defaults = None
 
     def __enter__(self):
         self.initial_global_defaults = copy(get_global_defaults())
-        new_defaults = FormatSpec.from_template(
-            template=self.initial_global_defaults,
-            **self.kwargs)
-        update_global_defaults(new_defaults)
+        if self.replacement_format_spec is None:
+            new_defaults = FormatSpec.from_template(
+                template=self.initial_global_defaults,
+                **self.kwargs)
+        else:
+            new_defaults = self.replacement_format_spec
+        update_global_defaults(new_defaults, **self.kwargs)
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         update_global_defaults(self.initial_global_defaults)
```

### Comparing `sciform-0.6.0/src/sciform/unc_format.py` & `sciform-0.6.1/src/sciform/unc_format.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.0/src/sciform.egg-info/PKG-INFO` & `sciform-0.6.1/src/sciform.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciform
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package for formatting floats into scientific formatted strings.
 Author-email: Justin Gerber <justin.gerber48@gmail.com>
 Project-URL: Homepage, https://github.com/jagerber48/sciform
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -211,23 +211,63 @@
 
 - `f'{sfloat(12.4e+06):rp}'` gives `'12 M`'
 - `f'{sfloat(1024*2**10):bp'` gives `1 Mi`
 
 
 # Configuration options (forthcoming)
 
-Forthcoming features to improve ease of configuration:
-- Function-based (as opposed to string formatting/`__format__` based) 
-  formatting.
-- Ability to set module or class level defaults for each FSML term to 
-  avoid repetitive, verbose format specifications.
-- Class-based API for storing default configurations?
-- Optional registration of new prefixes, notably `c`, `d`, `da`, and `h` which 
-  are recognized SI prefixes for 10<sup>-2</sup>, 10<sup>-1</sup>, 
-  10<sup>+1</sup> and 10<sup>+2</sup> respectively.
+It is possible to modify the global default configuration for `sciform`
+to avoid repetition of verbose (and difficult-to-parse-for-humans) 
+format specification strings. 
+
+The global defaults are stored in the `FMT_SPEC_GLOBAL_DEFAULTS` 
+`FormatSpec` object.
+When a call is made to format an `sfloat`, any parameters extracted from
+the format specification string are used for the formatting, while any 
+parameters not supplied are extracted from the global defaults object.
+
+The global configuration object can be permanently modified using the 
+`update_global_defaults()` function and `kwargs` corresponding to the 
+parameters the default configuration options the user would like to
+update (TODO: Documentation of acceptable `kwargs`). 
+The user can also pass in an entirely new replacement `FormatSpec`
+object to use as the new global configuration object.
+In this case any `kwargs` passed in will be used to update this new
+configuration object after it has replaced the old one.
+
+The global configuration object can also be temporarily modified using 
+the `GlobalDefaultsContext` context decorator. 
+Similarly, the user can pass in `kwargs` to modify the existing 
+configuration object as well as an entirely new configuration object. 
+Within the scope of the context manager the new global configuration 
+will be used, but when the context manager scope exits, the original 
+configuration will be restored.
+
+Modifying the global configuration allows the user to modify the mapping
+between exponents and SI or IEC prefixes.
+In particular, it is possible to include the `c` SI prefix (e.g. 
+1 cm = 10<sup>-2</sup> m) using the `include_c` kwarg as well as to
+include all of the `c`, `d`, `da`, and `h` SI prefixes corresponding to
+10<sup>-2</sup>, 10<sup>-1</sup>, 10<sup>+1</sup>, and 10<sup>+2</sup>
+respectively using the `include_small_si_prefixes` kwarg.
+
+The user can format floats directly using the `format_float` function 
+and passing in an explicitly defined `FormatSpec` object. In the future
+a function allowing users to format floats using kwargs directly will be
+included.
+
+In the future, configuration may be added for persistant class- and
+instance-level default configuration options. However, it needs to be
+decided how configuration will be shared between the different levels.
+For example, if an `sfloat` object is instantiated which does not 
+specify behavior for the `prefix` field, but then the `prefix` field at
+the global level is modified, should this `sfloat` instance adopt the
+new global config?
+Also, how should config conflicts be managed?
+One idea is to resolve conflicts by deferring to the parent config.
 
 
 # Value + uncertainty formatting (forthcoming)
 
 One of (if not the) most important use cases for scientific formatting
 is formatting a value together with its specified uncertainty, e.g.
 `84.3 +/- 0.2`. The ability to format pairs of floats as
```

### Comparing `sciform-0.6.0/tests/test.py` & `sciform-0.6.1/tests/test.py`

 * *Files identical despite different names*

