# Comparing `tmp/tooltime-0.2.8.tar.gz` & `tmp/tooltime-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooltime-0.2.8.tar", last modified: Sun Oct  9 17:47:34 2022, max compression
+gzip compressed data, was "tooltime-0.2.9.tar", last modified: Wed Apr 26 04:38:41 2023, max compression
```

## Comparing `tooltime-0.2.8.tar` & `tooltime-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       87 2022-05-27 02:46:06.474595 tooltime-0.2.8/.gitignore
--rw-r--r--   0        0        0    11358 2021-11-05 04:11:12.321652 tooltime-0.2.8/LICENSE
--rw-r--r--   0        0        0    22195 2022-08-24 18:13:18.229924 tooltime-0.2.8/README.md
--rw-r--r--   0        0        0      449 2022-05-27 02:44:39.190898 tooltime-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1085 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timefrequency_tests/test_timefrequency_convert.py
--rw-r--r--   0        0        0      466 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timefrequency_tests/test_timefrequency_identify.py
--rw-r--r--   0        0        0      645 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timelength_tests/test_timelength_convert.py
--rw-r--r--   0        0        0      637 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timelength_tests/test_timelength_identify.py
--rw-r--r--   0        0        0      646 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timeperiod_tests/test_timeperiod_convert.py
--rw-r--r--   0        0        0      443 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timeperiod_tests/test_timeperiod_identify.py
--rw-r--r--   0        0        0     5517 2021-11-29 03:28:17.062899 tooltime-0.2.8/tests/timeperiod_tests/test_timeperiod_overlap.py
--rw-r--r--   0        0        0     1871 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timeperiod_tests/test_timeperiod_standard.py
--rw-r--r--   0        0        0      833 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timestamp_tests/test_timestamp_convert.py
--rw-r--r--   0        0        0      433 2021-11-05 04:11:12.321652 tooltime-0.2.8/tests/timestamp_tests/test_timestamp_identify.py
--rw-r--r--   0        0        0     1361 2022-06-26 07:31:05.865119 tooltime-0.2.8/tests/timestamp_tests/test_timestamp_samples.py
--rw-r--r--   0        0        0      275 2022-10-09 17:47:02.469950 tooltime-0.2.8/tooltime/__init__.py
--rw-r--r--   0        0        0      135 2021-11-05 04:11:12.321652 tooltime-0.2.8/tooltime/exceptions.py
--rw-r--r--   0        0        0        0 2021-11-29 04:01:32.849600 tooltime-0.2.8/tooltime/py.typed
--rw-r--r--   0        0        0     7755 2022-08-26 16:40:37.326601 tooltime-0.2.8/tooltime/spec.py
--rw-r--r--   0        0        0      150 2021-11-27 21:20:23.212535 tooltime-0.2.8/tooltime/timefrequency_utils/__init__.py
--rw-r--r--   0        0        0     4625 2022-05-08 16:50:10.025359 tooltime-0.2.8/tooltime/timefrequency_utils/timefrequency_convert.py
--rw-r--r--   0        0        0     4204 2022-05-08 16:41:33.771235 tooltime-0.2.8/tooltime/timefrequency_utils/timefrequency_crud.py
--rw-r--r--   0        0        0     2166 2022-05-08 16:31:37.209642 tooltime-0.2.8/tooltime/timefrequency_utils/timefrequency_identify.py
--rw-r--r--   0        0        0     2160 2022-05-08 16:53:17.968935 tooltime-0.2.8/tooltime/timefrequency_utils/timefrequency_resolution.py
--rw-r--r--   0        0        0      133 2021-11-27 21:21:51.972263 tooltime-0.2.8/tooltime/timelength_utils/__init__.py
--rw-r--r--   0        0        0    17633 2022-07-22 21:19:09.144561 tooltime-0.2.8/tooltime/timelength_utils/timelength_convert.py
--rw-r--r--   0        0        0     4203 2022-07-18 23:50:14.575209 tooltime-0.2.8/tooltime/timelength_utils/timelength_crud.py
--rw-r--r--   0        0        0     3909 2022-02-09 07:03:49.861277 tooltime-0.2.8/tooltime/timelength_utils/timelength_identify.py
--rw-r--r--   0        0        0     2606 2022-07-22 21:16:33.105059 tooltime-0.2.8/tooltime/timelength_utils/timelength_units.py
--rw-r--r--   0        0        0      207 2021-11-27 21:23:46.647915 tooltime-0.2.8/tooltime/timeperiod_utils/__init__.py
--rw-r--r--   0        0        0     3483 2022-02-11 20:25:12.140218 tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_convert.py
--rw-r--r--   0        0        0     4271 2022-02-11 20:25:12.140218 tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_crud.py
--rw-r--r--   0        0        0     1686 2022-02-09 07:03:31.757008 tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_identify.py
--rw-r--r--   0        0        0      982 2022-02-11 20:25:12.140218 tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_introspect.py
--rw-r--r--   0        0        0     4201 2021-11-29 03:32:46.233313 tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_overlap.py
--rw-r--r--   0        0        0     6619 2022-06-26 06:57:17.745693 tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_standard.py
--rw-r--r--   0        0        0      196 2022-06-26 07:26:03.032221 tooltime-0.2.8/tooltime/timestamp_utils/__init__.py
--rw-r--r--   0        0        0     1571 2021-11-27 22:47:33.075315 tooltime-0.2.8/tooltime/timestamp_utils/datetime_utils.py
--rw-r--r--   0        0        0    19164 2022-09-17 22:26:50.727673 tooltime-0.2.8/tooltime/timestamp_utils/timestamp_convert.py
--rw-r--r--   0        0        0     3938 2022-10-06 18:10:42.618837 tooltime-0.2.8/tooltime/timestamp_utils/timestamp_crud.py
--rw-r--r--   0        0        0     4788 2022-08-26 16:37:01.493328 tooltime-0.2.8/tooltime/timestamp_utils/timestamp_identify.py
--rw-r--r--   0        0        0     5796 2022-05-08 16:53:40.480861 tooltime-0.2.8/tooltime/timestamp_utils/timestamp_introspect.py
--rw-r--r--   0        0        0     8624 2022-09-06 17:05:52.229888 tooltime-0.2.8/tooltime/timestamp_utils/timestamp_samples.py
--rw-r--r--   0        0        0    22589 1970-01-01 00:00:00.000000 tooltime-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-05 23:32:11.424170 tooltime-0.2.9/.gitignore
+-rw-r--r--   0        0        0    11358 2023-04-05 23:32:11.424335 tooltime-0.2.9/LICENSE
+-rw-r--r--   0        0        0    22195 2023-04-05 23:32:11.424541 tooltime-0.2.9/README.md
+-rw-r--r--   0        0        0      449 2023-04-05 23:32:11.424657 tooltime-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1085 2023-04-05 23:32:11.424881 tooltime-0.2.9/tests/timefrequency_tests/test_timefrequency_convert.py
+-rw-r--r--   0        0        0      466 2023-04-05 23:32:11.424997 tooltime-0.2.9/tests/timefrequency_tests/test_timefrequency_identify.py
+-rw-r--r--   0        0        0      645 2023-04-05 23:32:11.425181 tooltime-0.2.9/tests/timelength_tests/test_timelength_convert.py
+-rw-r--r--   0        0        0      637 2023-04-05 23:32:11.425295 tooltime-0.2.9/tests/timelength_tests/test_timelength_identify.py
+-rw-r--r--   0        0        0      646 2023-04-05 23:32:11.425443 tooltime-0.2.9/tests/timeperiod_tests/test_timeperiod_convert.py
+-rw-r--r--   0        0        0      443 2023-04-05 23:32:11.425538 tooltime-0.2.9/tests/timeperiod_tests/test_timeperiod_identify.py
+-rw-r--r--   0        0        0     5517 2023-04-05 23:32:11.425662 tooltime-0.2.9/tests/timeperiod_tests/test_timeperiod_overlap.py
+-rw-r--r--   0        0        0     1871 2023-04-05 23:32:11.425771 tooltime-0.2.9/tests/timeperiod_tests/test_timeperiod_standard.py
+-rw-r--r--   0        0        0      833 2023-04-05 23:32:11.425918 tooltime-0.2.9/tests/timestamp_tests/test_timestamp_convert.py
+-rw-r--r--   0        0        0      433 2023-04-05 23:32:11.426015 tooltime-0.2.9/tests/timestamp_tests/test_timestamp_identify.py
+-rw-r--r--   0        0        0     1361 2023-04-05 23:32:11.426120 tooltime-0.2.9/tests/timestamp_tests/test_timestamp_samples.py
+-rw-r--r--   0        0        0      275 2023-04-26 04:38:16.705669 tooltime-0.2.9/tooltime/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-05 23:32:11.426409 tooltime-0.2.9/tooltime/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-05 23:32:11.426462 tooltime-0.2.9/tooltime/py.typed
+-rw-r--r--   0        0        0     7755 2023-04-05 23:32:11.426614 tooltime-0.2.9/tooltime/spec.py
+-rw-r--r--   0        0        0      150 2023-04-05 23:32:11.426787 tooltime-0.2.9/tooltime/timefrequency_utils/__init__.py
+-rw-r--r--   0        0        0     4625 2023-04-05 23:32:11.426917 tooltime-0.2.9/tooltime/timefrequency_utils/timefrequency_convert.py
+-rw-r--r--   0        0        0     4204 2023-04-05 23:32:11.427026 tooltime-0.2.9/tooltime/timefrequency_utils/timefrequency_crud.py
+-rw-r--r--   0        0        0     2166 2023-04-05 23:32:11.427129 tooltime-0.2.9/tooltime/timefrequency_utils/timefrequency_identify.py
+-rw-r--r--   0        0        0     2160 2023-04-05 23:32:11.427267 tooltime-0.2.9/tooltime/timefrequency_utils/timefrequency_resolution.py
+-rw-r--r--   0        0        0      133 2023-04-05 23:32:11.427425 tooltime-0.2.9/tooltime/timelength_utils/__init__.py
+-rw-r--r--   0        0        0    17840 2023-04-09 05:51:08.825045 tooltime-0.2.9/tooltime/timelength_utils/timelength_convert.py
+-rw-r--r--   0        0        0     4217 2023-04-09 05:52:58.565067 tooltime-0.2.9/tooltime/timelength_utils/timelength_crud.py
+-rw-r--r--   0        0        0     3909 2023-04-05 23:32:11.427834 tooltime-0.2.9/tooltime/timelength_utils/timelength_identify.py
+-rw-r--r--   0        0        0     2606 2023-04-05 23:32:11.427945 tooltime-0.2.9/tooltime/timelength_utils/timelength_units.py
+-rw-r--r--   0        0        0      207 2023-04-05 23:32:11.428104 tooltime-0.2.9/tooltime/timeperiod_utils/__init__.py
+-rw-r--r--   0        0        0     3487 2023-04-09 05:44:51.022272 tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_convert.py
+-rw-r--r--   0        0        0     4362 2023-04-09 05:45:44.248575 tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_crud.py
+-rw-r--r--   0        0        0     1686 2023-04-05 23:32:11.428441 tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_identify.py
+-rw-r--r--   0        0        0      999 2023-04-09 05:43:55.971778 tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_introspect.py
+-rw-r--r--   0        0        0     4257 2023-04-09 05:43:27.710953 tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_overlap.py
+-rw-r--r--   0        0        0     9328 2023-04-09 06:40:33.537612 tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_standard.py
+-rw-r--r--   0        0        0      196 2023-04-05 23:32:11.428928 tooltime-0.2.9/tooltime/timestamp_utils/__init__.py
+-rw-r--r--   0        0        0     1590 2023-04-05 23:52:53.708053 tooltime-0.2.9/tooltime/timestamp_utils/datetime_utils.py
+-rw-r--r--   0        0        0    19248 2023-04-09 05:42:52.541860 tooltime-0.2.9/tooltime/timestamp_utils/timestamp_convert.py
+-rw-r--r--   0        0        0     4001 2023-04-09 05:49:31.111568 tooltime-0.2.9/tooltime/timestamp_utils/timestamp_crud.py
+-rw-r--r--   0        0        0     4788 2023-04-05 23:32:11.429422 tooltime-0.2.9/tooltime/timestamp_utils/timestamp_identify.py
+-rw-r--r--   0        0        0     5800 2023-04-09 05:52:19.443612 tooltime-0.2.9/tooltime/timestamp_utils/timestamp_introspect.py
+-rw-r--r--   0        0        0     8624 2023-04-05 23:32:11.429685 tooltime-0.2.9/tooltime/timestamp_utils/timestamp_samples.py
+-rw-r--r--   0        0        0    22589 1970-01-01 00:00:00.000000 tooltime-0.2.9/PKG-INFO
```

### Comparing `tooltime-0.2.8/LICENSE` & `tooltime-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/README.md` & `tooltime-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tests/timefrequency_tests/test_timefrequency_convert.py` & `tooltime-0.2.9/tests/timefrequency_tests/test_timefrequency_convert.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tests/timelength_tests/test_timelength_convert.py` & `tooltime-0.2.9/tests/timelength_tests/test_timelength_convert.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tests/timelength_tests/test_timelength_identify.py` & `tooltime-0.2.9/tests/timelength_tests/test_timelength_identify.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tests/timeperiod_tests/test_timeperiod_convert.py` & `tooltime-0.2.9/tests/timeperiod_tests/test_timeperiod_convert.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tests/timeperiod_tests/test_timeperiod_overlap.py` & `tooltime-0.2.9/tests/timeperiod_tests/test_timeperiod_overlap.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tests/timeperiod_tests/test_timeperiod_standard.py` & `tooltime-0.2.9/tests/timeperiod_tests/test_timeperiod_standard.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tests/timestamp_tests/test_timestamp_convert.py` & `tooltime-0.2.9/tests/timestamp_tests/test_timestamp_convert.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tests/timestamp_tests/test_timestamp_samples.py` & `tooltime-0.2.9/tests/timestamp_tests/test_timestamp_samples.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/spec.py` & `tooltime-0.2.9/tooltime/spec.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timefrequency_utils/timefrequency_convert.py` & `tooltime-0.2.9/tooltime/timefrequency_utils/timefrequency_convert.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timefrequency_utils/timefrequency_crud.py` & `tooltime-0.2.9/tooltime/timefrequency_utils/timefrequency_crud.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timefrequency_utils/timefrequency_identify.py` & `tooltime-0.2.9/tooltime/timefrequency_utils/timefrequency_identify.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timefrequency_utils/timefrequency_resolution.py` & `tooltime-0.2.9/tooltime/timefrequency_utils/timefrequency_resolution.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timelength_utils/timelength_convert.py` & `tooltime-0.2.9/tooltime/timelength_utils/timelength_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ) -> spec.TimelengthTimedelta:
     ...
 
 
 def convert_timelength(
     timelength: spec.Timelength,
     to_representation: spec.TimelengthRepresentation,
-    from_representation: typing.Optional[spec.TimelengthRepresentation] = None,
+    from_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.Timelength:
     """convert Timelength to a new representation
 
     ## Inputs
     - timelength: Timelength
     - to_representation: str of Timelength representation of input timelength
     - from_representation: str of target Timelength representation
@@ -147,15 +147,15 @@
 #
 # # functions with target representation specified
 #
 
 
 def timelength_to_seconds(
     timelength: spec.Timelength,
-    from_representation: spec.TimelengthRepresentation = None,
+    from_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.TimelengthSeconds:
     """convert Timelength to TimelengthSeconds
 
     ## Inputs
     - timelength: Timelength
     - from_representation: str representation name of input timelength
 
@@ -167,15 +167,15 @@
         to_representation='TimelengthSeconds',
         from_representation=from_representation,
     )
 
 
 def timelength_to_seconds_precise(
     timelength: spec.Timelength,
-    from_representation: spec.TimelengthRepresentation = None,
+    from_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.TimelengthSecondsPrecise:
     """convert Timelength to TimelengthSecondsPrecise
 
     ## Inputs
     - timelength: Timelength
     - from_representation: str representation name of input timelength
 
@@ -187,15 +187,15 @@
         to_representation='TimelengthSecondsPrecise',
         from_representation=from_representation,
     )
 
 
 def timelength_to_label(
     timelength: spec.Timelength,
-    from_representation: spec.TimelengthRepresentation = None,
+    from_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.TimelengthLabel:
     """convert Timelength to TimelengthLabel
 
     ## Inputs
     - timelength: Timelength
     - from_representation: str representation name of input timelength
 
@@ -207,15 +207,15 @@
         to_representation='TimelengthLabel',
         from_representation=from_representation,
     )
 
 
 def timelength_to_phrase(
     timelength: spec.Timelength,
-    from_representation: spec.TimelengthRepresentation = None,
+    from_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.TimelengthPhrase:
     """convert Timelength to TimelengthPhrase
 
     ## Inputs
     - timelength: Timelength
     - from_representation: str representation name of input timelength
 
@@ -227,15 +227,15 @@
         to_representation='TimelengthPhrase',
         from_representation=from_representation,
     )
 
 
 def timelength_to_clock(
     timelength: spec.Timelength,
-    from_representation: spec.TimelengthRepresentation = None,
+    from_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.TimelengthClock:
     """convert Timelength to TimelengthClock
 
     ## Inputs
     - timelength: Timelength
     - from_representation: str representation name of input timelength
 
@@ -247,15 +247,15 @@
         to_representation='TimelengthClock',
         from_representation=from_representation,
     )
 
 
 def timelength_to_clock_phrase(
     timelength: spec.Timelength,
-    from_representation: spec.TimelengthRepresentation = None,
+    from_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.TimelengthClockPhrase:
     """convert Timelength to TimelengthClockPhrase
 
     ## Inputs
     - timelength: Timelength
     - from_representation: str representation name of input timelength
 
@@ -267,15 +267,15 @@
         to_representation='TimelengthClockPhrase',
         from_representation=from_representation,
     )
 
 
 def timelength_to_timedelta(
     timelength: spec.Timelength,
-    from_representation: spec.TimelengthRepresentation = None,
+    from_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.TimelengthTimedelta:
     """convert Timelength to TimelengthTimedelta
 
     ## Inputs
     - timelength: Timelength
     - from_representation: str representation name of input timelength
 
@@ -293,16 +293,16 @@
 # # specific conversion functions, from seconds
 #
 
 
 def timelength_seconds_to_label(
     timelength_seconds: spec.TimelengthSecondsRaw,
     base_only: bool = False,
-    fuzzy_tolerance: typing.SupportsFloat = None,
-    base_unit: str = None,
+    fuzzy_tolerance: typing.SupportsFloat | None = None,
+    base_unit: str | None = None,
 ) -> spec.TimelengthLabel:
     """convert seconds to TimelengthLabel
 
     - matches integer multiples of base units
         - see get_base_units() for base units
 
     ## Inputs
@@ -550,19 +550,22 @@
 # # special conversions
 #
 
 
 def timelength_to_pandas_timelength(
     timelength: spec.Timelength,
 ) -> spec.TimelengthPandas:
+    if isinstance(timelength, str) and timelength.endswith('w'):
+        number = int(timelength[:-1])
+        timelength = str(7 * number) + 'd'
     timelength_label = timelength_to_label(timelength)
-    number = timelength_label[:-1]
+    number_str = timelength_label[:-1]
     unit_name = timelength_units.unit_letters_to_names()[timelength_label[-1]]
     pandas_unit = timelength_units.get_english_to_pandas_units()[unit_name]
-    return number + pandas_unit
+    return number_str + pandas_unit
 
 
 def timelength_to_numerical(timelength: spec.Timelength) -> int | float:
     seconds_precise = timelength_to_seconds_precise(timelength)
     if math.isclose(seconds_precise, int(seconds_precise)):
         return int(seconds_precise)
     else:
```

### Comparing `tooltime-0.2.8/tooltime/timelength_utils/timelength_crud.py` & `tooltime-0.2.9/tooltime/timelength_utils/timelength_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     precise: bool = False,
 ) -> spec.TimelengthSecondsPrecise:
     ...
 
 
 def get_age(
     timestamp: spec.Timestamp,
-    to_representation: spec.TimelengthRepresentation = None,
+    to_representation: spec.TimelengthRepresentation | None = None,
     *,
     precise: bool = False,
 ) -> spec.Timelength:
     now = time.time()
     if not precise:
         now = int(now)
         seconds: int | float = now - timestamp_utils.timestamp_to_seconds(
@@ -57,15 +57,15 @@
     else:
         seconds = now - timestamp_utils.timestamp_to_seconds_precise(timestamp)
     return create_timelength(seconds, to_representation=to_representation)
 
 
 def create_timelength(
     seconds: spec.TimelengthSecondsRaw,
-    to_representation: spec.TimelengthRepresentation = None,
+    to_representation: spec.TimelengthRepresentation | None = None,
 ) -> spec.Timelength:
     """create Timelength
 
     ## Inputs
     - seconds: int or float seconds
     - to_reprsentation: str name of Timelength representation
```

### Comparing `tooltime-0.2.8/tooltime/timelength_utils/timelength_identify.py` & `tooltime-0.2.9/tooltime/timelength_utils/timelength_identify.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timelength_utils/timelength_units.py` & `tooltime-0.2.9/tooltime/timelength_utils/timelength_units.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_convert.py` & `tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ) -> spec.TimeperiodMap:
     ...
 
 
 def convert_timeperiod(
     timeperiod: spec.Timeperiod,
     to_representation: spec.TimeperiodRepresentation,
-    from_representation: typing.Optional[spec.TimeperiodRepresentation] = None,
+    from_representation: spec.TimeperiodRepresentation | None = None,
 ) -> spec.Timeperiod:
     """convert Timeperiod to a new representation
 
     ## Inputs
     - timeperiod: Timeperiod
     - to_representation: str of Timeperiod representation of input timeperiod
     - from_representation: str of target Timeperiod representation
@@ -63,15 +63,15 @@
         raise Exception(
             'unknown timeperiod representation: ' + str(to_representation)
         )
 
 
 def timeperiod_to_pair(
     timeperiod: spec.Timeperiod,
-    from_representation: spec.TimeperiodRepresentation = None,
+    from_representation: spec.TimeperiodRepresentation | None = None,
 ) -> spec.TimeperiodPair:
     """convert Timeperiod to TimeperiodPair
 
     ## Inputs
     - timeperiod: Timeperiod
     - from_representation: str representation name of input timeperiod
 
@@ -90,15 +90,15 @@
         raise Exception(
             'unknown Timeperiod representation: ' + str(from_representation)
         )
 
 
 def timeperiod_to_map(
     timeperiod: spec.Timeperiod,
-    from_representation: spec.TimeperiodRepresentation = None,
+    from_representation: spec.TimeperiodRepresentation | None = None,
 ) -> spec.TimeperiodMap:
     """convert Timeperiod to TimeperiodMap
 
     ## Inputs
     - timeperiod: Timeperiod
     - from_representation: str representation name of input timeperiod
```

### Comparing `tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_crud.py` & `tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_crud.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from .. import spec
 from .. import timestamp_utils
 from .. import timelength_utils
 from . import timeperiod_identify
 
 
 def create_timeperiod(
-    start: spec.Timestamp = None,
-    end: spec.Timestamp = None,
-    length: spec.Timelength = None,
-    to_representation: spec.TimeperiodRepresentation = None,
+    start: spec.Timestamp | None = None,
+    end: spec.Timestamp | None = None,
+    length: spec.Timelength | None = None,
+    to_representation: spec.TimeperiodRepresentation | None = None,
 ) -> spec.Timeperiod:
     """create Timeperiod
 
     ## Inputs
     - start: Timestamp
     - end: Timestamp
     - length: Timelength
@@ -37,17 +37,17 @@
     else:
         raise Exception(
             'unknown timeperiod representation: ' + str(to_representation)
         )
 
 
 def create_timeperiod_pair(
-    start: spec.Timestamp = None,
-    end: spec.Timestamp = None,
-    length: spec.Timelength = None,
+    start: spec.Timestamp | None = None,
+    end: spec.Timestamp | None = None,
+    length: spec.Timelength | None = None,
 ) -> spec.TimeperiodPair:
     """create Timeperiod with representation TimeperiodPair
 
     ## Inputs
     - start: Timestamp
     - end: Timestamp
     - length: Timelength
@@ -56,17 +56,17 @@
     - TimeperiodPair
     """
     start, end = compute_start_end(start=start, end=end, length=length)
     return (start, end)
 
 
 def create_timeperiod_map(
-    start: spec.Timestamp = None,
-    end: spec.Timestamp = None,
-    length: spec.Timelength = None,
+    start: spec.Timestamp | None = None,
+    end: spec.Timestamp | None = None,
+    length: spec.Timelength | None = None,
 ) -> spec.TimeperiodMap:
     """create Timeperiod with representation TimeperiodMap
 
     ## Inputs
     - start: Timestamp
     - end: Timestamp
     - length: Timelength
@@ -75,17 +75,17 @@
     - TimeperiodMap
     """
     start, end = compute_start_end(start=start, end=end, length=length)
     return {'start': start, 'end': end}
 
 
 def compute_start_end(
-    start: spec.Timestamp = None,
-    end: spec.Timestamp = None,
-    length: spec.Timelength = None,
+    start: spec.Timestamp | None = None,
+    end: spec.Timestamp | None = None,
+    length: spec.Timelength | None = None,
 ) -> tuple[typing.Union[int, float], typing.Union[int, float]]:
     """return start and end given two of start, end, and length
 
     ## Inputs
     - start: Timestamp
     - end: Timestamp
     - length: Timelength
```

### Comparing `tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_identify.py` & `tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_identify.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_introspect.py` & `tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_introspect.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .. import timestamp_utils
 from . import timeperiod_convert
 
 
 def print_timeperiod(
     timeperiod: spec.Timeperiod,
     timestamp_representation: spec.TimestampRepresentation = 'TimestampLabel',
-    print_kwargs: dict[str, typing.Any] = None,
+    print_kwargs: typing.Mapping[str, typing.Any] | None = None,
 ) -> None:
     """print Timeperiod
 
     ## Inputs
     - timeperiod: Timeperiod
     - timestamp_representation: str name of Timestamp representation to print
     - print_kwargs: kwargs passed to print()
```

### Comparing `tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_overlap.py` & `tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_overlap.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,22 +45,22 @@
         if end > max_end:
             max_end = end
     return (min_start, max_end)
 
 
 def create_overlapping_timeperiod(
     timeperiod: spec.Timeperiod,
-    trim_start_relative: typing.SupportsFloat = None,
-    trim_end_relative: typing.SupportsFloat = None,
-    trim_start_absolute: spec.Timelength = None,
-    trim_end_absolute: spec.Timelength = None,
-    extend_start_relative: typing.SupportsFloat = None,
-    extend_end_relative: typing.SupportsFloat = None,
-    extend_start_absolute: spec.Timelength = None,
-    extend_end_absolute: spec.Timelength = None,
+    trim_start_relative: typing.SupportsFloat | None = None,
+    trim_end_relative: typing.SupportsFloat | None = None,
+    trim_start_absolute: spec.Timelength | None = None,
+    trim_end_absolute: spec.Timelength | None = None,
+    extend_start_relative: typing.SupportsFloat | None = None,
+    extend_end_relative: typing.SupportsFloat | None = None,
+    extend_start_absolute: spec.Timelength | None = None,
+    extend_end_absolute: spec.Timelength | None = None,
 ) -> spec.Timeperiod:
     """create copy of timeperiod with start or end trimmed or extended
 
     - can trim or end by relative or absolute amount
 
     ## Inputs
     - timeperiod: Timeperiod
```

### Comparing `tooltime-0.2.8/tooltime/timeperiod_utils/timeperiod_standard.py` & `tooltime-0.2.9/tooltime/timeperiod_utils/timeperiod_standard.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import math
 import typing
 
 from .. import spec
 from .. import timelength_utils
 from .. import timestamp_utils
 
+if typing.TYPE_CHECKING:
+    import polars as pl
+
 
 def get_standard_timeperiod(
-    timelength_label: spec.TimelengthLabel = None,
+    timelength_label: spec.TimelengthLabel | None = None,
     *,
     block_unit: typing.Optional[spec.DatetimeUnit] = None,
     block_size: typing.Optional[int] = None,
     timestamp: typing.Optional[spec.Timestamp] = None,
     include_start: bool = True,
     include_end: bool = False,
     boundary_unit: spec.DatetimeUnit = 'second',
@@ -47,14 +50,18 @@
 
     if (timelength_label is not None) and (block_unit is not None):
         raise Exception('must specify either timelength_label or block_unit')
     elif (timelength_label is None) and (block_unit is not None):
         if block_size is None:
             block_size = 1
     elif (timelength_label is not None) and (block_unit is None):
+        if timelength_label.endswith('w'):
+            number = int(timelength_label[:-1])
+            timelength_label = str(7 * number) + 'd'
+
         block_size = int(timelength_label[:-1])
         unit_letters_to_names = (
             timelength_utils.datetime_unit_letters_to_names()
         )
         block_unit = unit_letters_to_names[timelength_label[-1]]
     elif (timelength_label is None) and (block_unit is None):
         raise Exception()
@@ -82,14 +89,17 @@
     # compute to_datetime
     if block_unit == 'month':
         # datetime.timedelta does not support months
         to_month_raw = from_datetime.month + block_size
         to_month = to_month_raw % 12
         to_year = from_datetime.year + math.floor(to_month_raw / 12)
         to_datetime = from_datetime.replace(month=to_month, year=to_year)
+    elif block_unit == 'year':
+        to_year = from_datetime.year + block_size
+        to_datetime = from_datetime.replace(year=to_year)
     else:
         block_timedelta = datetime.timedelta(**{(block_unit + 's'): block_size})
         to_datetime = from_datetime + block_timedelta
 
     # trim boundaries
     if not include_start:
         timedelta = datetime.timedelta(**{(boundary_unit + 's'): 1})
@@ -171,15 +181,97 @@
                 interval_size
             ),
             include_end=True,
         )
         date_range_kwargs['end'] = timeperiod['end'] * 1000000000
 
     # create intervals
-    import pandas as pd
+    import pandas as pd  # type: ignore
 
     intervals = pd.date_range(**date_range_kwargs)
 
     # extract timestamps
     timestamps = [int(interval.timestamp()) for interval in intervals]
 
     return timestamps
+
+
+def get_interval_df(
+    interval_size: spec.Timelength,
+    start_time: typing.Optional[spec.Timestamp] = None,
+    end_time: typing.Optional[spec.Timestamp] = None,
+    n_intervals: typing.Optional[int] = None,
+    window_size: typing.Optional[spec.Timelength] = None,
+) -> pl.DataFrame:
+
+    import polars as pl
+
+    # create standard timestamps
+    timestamps = get_standard_intervals(
+        interval_size=interval_size,
+        start_time=start_time,
+        end_time=end_time,
+        n_intervals=n_intervals,
+        window_size=window_size,
+    )
+    start_timestamps = [time for time in timestamps[:-1]]
+    end_timestamps = [time - 1 for time in timestamps[1:]]
+
+    # create labels
+    if interval_size == "1M":
+        labels = [
+            timestamp_utils.timestamp_to_iso_pretty(timestamp)[:7]
+            for timestamp in start_timestamps
+        ]
+    elif interval_size == "1d":
+        labels = [
+            timestamp_utils.timestamp_to_iso_pretty(timestamp)[:10]
+            for timestamp in start_timestamps
+        ]
+    elif interval_size == "1y":
+        labels = [
+            timestamp_utils.timestamp_to_iso_pretty(timestamp)[:4]
+            for timestamp in start_timestamps
+        ]
+    else:
+        labels = [
+            timestamp_utils.timestamp_to_iso_pretty(timestamp)
+            for timestamp in start_timestamps
+        ]
+
+    # create dataframe
+    df = pl.DataFrame(
+        {
+            "label": labels,
+            "start_timestamp": start_timestamps,
+            "end_timestamp": end_timestamps,
+        }
+    )
+
+    # compute middle timestamp
+    df = df.with_columns(
+        ((pl.col("end_timestamp") + pl.col("start_timestamp")) / 2)
+        .round(0)
+        .cast(pl.Int64)
+        .alias("middle_timestamp"),
+    )
+
+    # create iso_pretty timestamps
+    df = df.with_columns(
+        pl.col("start_timestamp")
+        .apply(timestamp_utils.timestamp_to_iso_pretty)
+        .alias("start_iso"),
+        pl.col("end_timestamp")
+        .apply(timestamp_utils.timestamp_to_iso_pretty)
+        .alias("end_iso"),
+        pl.col("middle_timestamp")
+        .apply(timestamp_utils.timestamp_to_iso_pretty)
+        .alias("middle_iso"),
+    )
+
+    # compute duration
+    df = df.with_columns(
+        (pl.col("end_timestamp") - pl.col("start_timestamp") + 1).alias("duration"),
+    )
+
+    return df
+
```

### Comparing `tooltime-0.2.8/tooltime/timestamp_utils/datetime_utils.py` & `tooltime-0.2.9/tooltime/timestamp_utils/datetime_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,10 +52,11 @@
     lowest_values = {
         'month': 1,
         'day': 1,
         'hour': 0,
         'minute': 0,
         'second': 0,
         'microsecond': 0,
+        'year': 0,
     }
     return lowest_values[datetime_unit]
```

### Comparing `tooltime-0.2.8/tooltime/timestamp_utils/timestamp_convert.py` & `tooltime-0.2.9/tooltime/timestamp_utils/timestamp_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 #
 # # functions with target representation specified
 #
 
 
 def timestamp_to_seconds(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampSeconds:
     """convert timestamp to TimestampSeconds
 
     ## Inputs
     - timestamp: Timestamp
     - from_representation: str representation name of input timestamp
 
@@ -234,15 +234,15 @@
         to_representation='TimestampSeconds',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_seconds_precise(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampSecondsPrecise:
     """convert timestamp to TimestampSecondsPrecise
 
     ## Inputs
     - timestamp: Timestamp
     - from_representation: str representation name of input timestamp
 
@@ -254,15 +254,15 @@
         to_representation='TimestampSecondsPrecise',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_label(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampLabel:
     """convert timestamp to TimestampLabel
 
     ## Inputs
     - timestamp: Timestamp
     - from_representation: str representation name of input timestamp
 
@@ -274,15 +274,15 @@
         to_representation='TimestampLabel',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_iso(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampISO:
     """convert timestamp to TimestampISO
 
     ## Inputs
     - timestamp: Timestamp
     - from_representation: str representation name of input timestamp
 
@@ -294,15 +294,15 @@
         to_representation='TimestampISO',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_iso_pretty(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampISOPretty:
     """convert timestamp to TimestampISOPretty
 
     ## Inputs
     - timestamp: Timestamp
     - from_representation: str representation name of input timestamp
 
@@ -314,15 +314,15 @@
         to_representation='TimestampISOPretty',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_date(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampDate:
     """convert timestamp to TimestampDate
 
     ## Inputs
     - timestamp: Timestamp
     - from_representation: str representation name of input timestamp
 
@@ -334,15 +334,15 @@
         to_representation='TimestampDate',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_year(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampYear:
     """convert timestamp to TimestampYear
 
     ## Inputs
     - timestamp: Timestamp
     - from_representation: str representation name of input timestamp
 
@@ -354,15 +354,15 @@
         to_representation='TimestampYear',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_datetime(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampDatetime:
     """convert timestamp to TimestampDatetime
 
     ## Inputs
     - timestamp: Timestamp
     - from_representation: str representation name of input timestamp
 
@@ -374,48 +374,48 @@
         to_representation='TimestampDatetime',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_date_compact(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampDateCompact:
     return convert_timestamp(
         timestamp,
         to_representation='TimestampDateCompact',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_month(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampMonth:
     return convert_timestamp(
         timestamp,
         to_representation='TimestampMonth',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_month_compact(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampMonthCompact:
     return convert_timestamp(
         timestamp,
         to_representation='TimestampMonthCompact',
         from_representation=from_representation,
     )
 
 
 def timestamp_to_seconds_string(
     timestamp: spec.Timestamp,
-    from_representation: spec.TimestampRepresentation = None,
+    from_representation: spec.TimestampRepresentation | None = None,
 ) -> spec.TimestampSecondsString:
     return convert_timestamp(
         timestamp,
         to_representation='TimestampSecondsString',
         from_representation=from_representation,
     )
```

### Comparing `tooltime-0.2.8/tooltime/timestamp_utils/timestamp_crud.py` & `tooltime-0.2.9/tooltime/timestamp_utils/timestamp_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def now(
     representation: spec.TimestampRepresentation = 'TimestampSeconds',
 ) -> spec.Timestamp:
     return create_timestamp(seconds=None, representation=representation)
 
 
 def create_timestamp(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
     representation: spec.TimestampRepresentation = 'TimestampSeconds',
 ) -> spec.Timestamp:
     """create Timestamp
 
     ## Inputs
     - seconds: int or float utc seconds
     - representation: str name of Timestamp representation
@@ -37,58 +37,58 @@
     elif representation == 'TimestampDatetime':
         return create_timestamp_datetime(seconds=seconds)
     else:
         raise Exception('unknown representation: ' + str(representation))
 
 
 def create_timestamp_seconds(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
 ) -> spec.TimestampSeconds:
     """create Timestamp with representation TimestampSeconds"""
     if seconds is None:
         seconds = time.time()
     return int(float(seconds))
 
 
 def create_timestamp_seconds_precise(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
 ) -> spec.TimestampSecondsPrecise:
     """create Timestamp with representation TimestampSecondsPrecise"""
     if seconds is None:
         seconds = time.time()
     return float(seconds)
 
 
 def create_timestamp_label(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
 ) -> spec.TimestampLabel:
     """create Timestamp with representation TimestampLabel"""
     if seconds is None:
         seconds = time.time()
     return timestamp_convert.timestamp_seconds_to_label(seconds)
 
 
 def create_timestamp_iso(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
 ) -> spec.TimestampISO:
     """create Timestamp with representation TimestampISO"""
     if seconds is None:
         seconds = time.time()
     return timestamp_convert.timestamp_seconds_to_iso(seconds)
 
 
 def create_timestamp_iso_pretty(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
 ) -> spec.TimestampISOPretty:
     """create Timestamp with representation TimestampISOPretty"""
     return create_timestamp_iso(seconds).replace('T', ' ')
 
 
 def create_timestamp_date(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
 ) -> spec.TimestampDate:
     """create Timestamp with representation TimestampDate
 
     does not round to nearest date, takes floor of seconds to previous date
     """
     import datetime
 
@@ -102,15 +102,15 @@
     year = dt.year
     month = dt.month
     day = dt.day
     return str(year) + '-' + ('%.02d' % month) + '-' + ('%.02d' % day)
 
 
 def create_timestamp_year(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
 ) -> spec.TimestampYear:
     """create Timestamp with representation TimestampDate
 
     does not round to nearest year, takes floor of seconds to previous year
     """
     import datetime
 
@@ -121,13 +121,13 @@
             float(seconds), tz=datetime.timezone.utc
         )
 
     return str(dt.year)
 
 
 def create_timestamp_datetime(
-    seconds: typing.SupportsFloat = None,
+    seconds: typing.SupportsFloat | None = None,
 ) -> spec.TimestampDatetime:
     """create Timestamp with representation TimestampDatetime"""
     if seconds is None:
         seconds = time.time()
     return timestamp_convert.timestamp_seconds_to_datetime(seconds)
```

### Comparing `tooltime-0.2.8/tooltime/timestamp_utils/timestamp_identify.py` & `tooltime-0.2.9/tooltime/timestamp_utils/timestamp_identify.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/tooltime/timestamp_utils/timestamp_introspect.py` & `tooltime-0.2.9/tooltime/timestamp_utils/timestamp_introspect.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,18 +71,18 @@
         summary['n_outliers'] = n_outliers
 
     return summary
 
 
 def print_timestamp_summary(
     *,
-    timestamps: typing.List[spec.Timestamp] = None,
-    summary: typing.Optional[spec.TimestampSummary] = None,
-    indent: typing.Optional[str] = None,
-    print_kwargs: dict[str, typing.Any] = None
+    timestamps: typing.List[spec.Timestamp] | None = None,
+    summary: spec.TimestampSummary | None = None,
+    indent: str | None = None,
+    print_kwargs: typing.Mapping[str, typing.Any] | None = None
 ) -> None:
     """print summary of timestamps
 
     - specify either timestamps or summary
     - timestamps should be ordered
         - todo: do not require ordering
```

### Comparing `tooltime-0.2.8/tooltime/timestamp_utils/timestamp_samples.py` & `tooltime-0.2.9/tooltime/timestamp_utils/timestamp_samples.py`

 * *Files identical despite different names*

### Comparing `tooltime-0.2.8/PKG-INFO` & `tooltime-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooltime
-Version: 0.2.8
+Version: 0.2.9
 Summary: tooltime makes it easy to create and convert representations of time
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: numpy ; extra == "full"
 Requires-Dist: pandas ; extra == "full"
 Project-URL: Source, https://github.com/sslivkoff/tooltime
```

