# Comparing `tmp/act4e_mcdp-0.5.0-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 37442 bytes, number of entries: 15
--rw-r--r--  2.0 unx      387 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
+Zip file size: 39260 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      424 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
 -rw-r--r--  2.0 unx    67896 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
 -rw-r--r--  2.0 unx      571 b- defN 80-Jan-01 00:00 act4e_mcdp/download.py
--rw-r--r--  2.0 unx    10246 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
+-rw-r--r--  2.0 unx    10772 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
 -rw-r--r--  2.0 unx     3281 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_dp.py
+-rw-r--r--  2.0 unx     4931 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_dp_queries.py
 -rw-r--r--  2.0 unx     3924 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_mcdp.py
 -rw-r--r--  2.0 unx     4656 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
 -rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 act4e_mcdp/posets.py
 -rw-r--r--  2.0 unx    11916 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
--rw-r--r--  2.0 unx     7934 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
--rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      164 b- defN 80-Jan-01 00:00 act4e_mcdp-0.5.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1216 b- defN 16-Jan-01 00:00 act4e_mcdp-0.5.0.dist-info/RECORD
-15 files, 114430 bytes uncompressed, 35438 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx     7955 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1308 b- defN 16-Jan-01 00:00 act4e_mcdp-0.6.0.dist-info/RECORD
+16 files, 120098 bytes uncompressed, 37110 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: act4e_mcdp/loading.py
 Comment: 
 
 Filename: act4e_mcdp/main_solve_dp.py
 Comment: 
 
+Filename: act4e_mcdp/main_solve_dp_queries.py
+Comment: 
+
 Filename: act4e_mcdp/main_solve_mcdp.py
 Comment: 
 
 Filename: act4e_mcdp/nameddps.py
 Comment: 
 
 Filename: act4e_mcdp/posets.py
@@ -27,20 +30,20 @@
 
 Filename: act4e_mcdp/py.typed
 Comment: 
 
 Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
-Filename: act4e_mcdp-0.5.0.dist-info/METADATA
+Filename: act4e_mcdp-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.5.0.dist-info/WHEEL
+Filename: act4e_mcdp-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.5.0.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.5.0.dist-info/RECORD
+Filename: act4e_mcdp-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/__init__.py

```diff
@@ -13,7 +13,8 @@
 from .main_solve_mcdp import *
 from .main_solve_dp import *
 from .solution_interface import *
 from .nameddps import *
 from .primitivedps import *
 from .posets import *
 from .download import *
+from .main_solve_dp_queries import *
```

## act4e_mcdp/loading.py

```diff
@@ -13,15 +13,14 @@
     NodeResource,
     SimpleWrap,
 )
 from .posets import FinitePoset, Numbers, Poset, PosetProduct
 from .primitivedps import (
     AmbientConversion,
     CatalogueDP,
-    M_Res_DivideConstant_DP,
     Constant,
     DPLoop2,
     DPSeries,
     EntryInfo,
     IdentityDP,
     JoinNDP,
     Limit,
@@ -30,23 +29,25 @@
     M_Fun_AddConstant_DP,
     M_Fun_AddMany_DP,
     M_Fun_MultiplyConstant_DP,
     M_Fun_MultiplyMany_DP,
     M_Power_DP,
     M_Res_AddConstant_DP,
     M_Res_AddMany_DP,
+    M_Res_DivideConstant_DP,
     M_Res_MultiplyConstant_DP,
     M_Res_MultiplyMany_DP,
     MeetNDualDP,
     Mux,
     ParallelDP,
     PrimitiveDP,
     UnitConversion,
     ValueFromPoset,
 )
+from .solution_interface import Interval, LowerSet, UpperSet
 
 loaders = {}
 
 __all__ = [
     "load_repr1",
     "loader_for",
     "parse_yaml_value",
@@ -349,14 +350,33 @@
     elements = ob["elements"]
     relations = ob["relations"]
     relations = set(tuple(x) for x in relations)
     elements = set(elements)
     return FinitePoset(elements=elements, relations=relations)
 
 
+@loader_for("Interval")
+def load_Interval(ob: dict):
+    pessimistic = load_repr1(ob["pessimistic"])
+    optimistic = load_repr1(ob["optimistic"])
+    return Interval(pessimistic=pessimistic, optimistic=optimistic)
+
+
+@loader_for("LowerSet")
+def load_LowerSet(ob: dict):
+    maximals = ob["maximals"]
+    return LowerSet(maximals=maximals)
+
+
+@loader_for("UpperSet")
+def load_UpperSet(ob: dict):
+    minimals = ob["minimals"]
+    return UpperSet(minimals=minimals)
+
+
 @loader_for("Numbers")
 def load_Numbers(ob: dict):
     bottom = Decimal(ob["bottom"])
     top = Decimal(ob["top"])
     units = ob.get("units", "")
     step = Decimal(ob.get("step", 0))
     return Numbers(bottom=bottom, top=top, step=step, units=units)
```

## act4e_mcdp/solution_interface.py

```diff
@@ -18,32 +18,32 @@
 
 @dataclass
 class UpperSet(Generic[X]):
     """
     Describes a finitely-supported **upper set** of elements of type X.
 
     Attributes:
-        minima: A list of elements of type X, which are the minimal elements of the set.
+        minimals: A list of elements of type X, which are the minimal elements of the set.
 
     """
 
-    minima: list[X]
+    minimals: list[X]
 
 
 @dataclass
 class LowerSet(Generic[X]):
     """
     Describes a finitely-supported **lower set** of elements of type X.
 
     Attributes:
-        maxima: A list of elements of type X, which are the minimal elements of the set.
+        maximals: A list of elements of type X, which are the minimal elements of the set.
 
     """
 
-    maxima: list[X]
+    maximals: list[X]
 
 
 @dataclass(kw_only=True)
 class Interval(Generic[X]):
     """
     Describes an optimistic-pessimistic interval for a quantity of type X.
 
@@ -70,15 +70,15 @@
         self,
         dp: PrimitiveDP,
         functionality_needed: object,
         /,
         resolution_optimistic: int = 0,
         resolution_pessimistic: int = 0,
     ) -> Interval[UpperSet[object]]:
-        """
+        r"""
 
         Solves the problem of finding the minimal resources needed to satisfy a given functional requirement.
 
         The problem is defined by a DP and a query. The model is a DP, and the query is an
         object that belongs to the poset $\F$ of the functionalities of the DP.
 
         The solution is an interval of upper sets (of objects of $\R$).
@@ -115,17 +115,20 @@
             assert result.pessimistic == result.optimistic == UpperSet(['a'])
 
         ```
 
         Parameters:
             dp: A design problem.
             functionality_needed: The functionality needed.
-            resolution_optimistic: An integer returning the resolution of the optimistic answer, to be used
-            in the case of DPs that are not computable.
-            resolution_pessimistic: Same thing, for the pessimistic answer.
+            resolution_optimistic: An integer returning the resolution of the optimistic answer, to
+                be used in the case of DPs that are not computable.
+
+            resolution_pessimistic: Same for the pessimistic answer.
+
+
 
         Returns:
 
             An interval of upper sets.
         """
         raise NotImplementedError
 
@@ -142,16 +145,16 @@
         Solves the problem of finding the maximal functionality that can be provided with a given budget of
         resources.
         It is the dual of solve_dp_FixFunMinRes.
 
         Parameters:
             dp: A design problem.
             resource_budget: The resources available.
-            resolution_optimistic: An integer returning the resolution of the optimistic answer, to be used
-            in the case of DPs that are not computable.
+            resolution_optimistic: An integer returning the resolution of the optimistic answer,
+                to be used in the case of DPs that are not computable.
             resolution_pessimistic: Same thing, for the pessimistic answer.
 
         Returns:
 
             An interval of lower sets.
         """
 
@@ -220,16 +223,16 @@
             assert list(result.minima) == [{'r1': 'a'}]
         ```
 
 
         Parameters:
             graph: The model of the problem.
             functionality_needed: The functionality needed (key-value dictionary).
-            resolution_optimistic: An integer returning the resolution of the optimistic answer, to be used
-            in the case of DPs that are not computable.
+            resolution_optimistic: An integer returning the resolution of the optimistic answer,
+                to be used in the case of DPs that are not computable.
             resolution_pessimistic: Same thing, for the pessimistic answer.
 
         Returns:
 
             An interval of upper sets.
 
         """
@@ -264,16 +267,16 @@
             assert list(result.maxima) == [{}]
 
         ```
 
         Parameters:
             graph: The model of the problem.
             resources_budget: The maximum budget that we have (key-value dictionary).
-            resolution_optimistic: An integer returning the resolution of the optimistic answer, to be used
-            in the case of DPs that are not computable.
+            resolution_optimistic: An integer returning the resolution of the optimistic answer,
+                to be used in the case of DPs that are not computable.
             resolution_pessimistic: Same thing, for the pessimistic answer.
 
         Returns:
 
              An interval of lower sets.
```

## Comparing `act4e_mcdp-0.5.0.dist-info/RECORD` & `act4e_mcdp-0.6.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-act4e_mcdp/__init__.py,sha256=d9ADT_wi7QyptWco7RLEWJdmUyqhvqIXxvOY7qnM1q8,387
+act4e_mcdp/__init__.py,sha256=GQsby_cbaGnIexdyFinnY6jVbCNIvaqBNwyEjsVvUjk,424
 act4e_mcdp/autogen_packed_test_data.py,sha256=Iadf_CeH5_iFkDPJWFATFzLRM_FImr7fg2yN7lDYsVg,67896
 act4e_mcdp/download.py,sha256=fXm46ISIYvpFjouSMB0l0XLuJWw5CxZSpgi-fvmxMGA,571
-act4e_mcdp/loading.py,sha256=4ksOXLlFLKjxcBuJYvB6QgKGGf8YAT4tKOSfYeL1WHY,10246
+act4e_mcdp/loading.py,sha256=qfT0Rz_PUZ50mfxjSyoCanH_JLd8DZt4WuTMf0FSY3w,10772
 act4e_mcdp/main_solve_dp.py,sha256=qq6hdqu0LBLjK-1gJyayFhHsGFd0vvbHMgR4PVTWKYo,3281
+act4e_mcdp/main_solve_dp_queries.py,sha256=P-npPcV0D_NfwUtmOnMRLRy4Ihq-Xiko5zMAnArNWPw,4931
 act4e_mcdp/main_solve_mcdp.py,sha256=zOAJhpY2S2E_P_c_UXkS4bMB40FxohF4iDMZlfRS-q0,3924
 act4e_mcdp/nameddps.py,sha256=knysGfVrbeilCg9gX4B7S-b8JcuwbfFJN-WMxgCBrXo,4656
 act4e_mcdp/posets.py,sha256=7iijB7waZd3nTyK-_eNBR6YZOWhcTUYtKqCm7irpFKE,1790
 act4e_mcdp/primitivedps.py,sha256=dfA15BwI43XJQMx6OLf2rTu31TWnHcnpIKUaDPxc3r0,11916
 act4e_mcdp/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-act4e_mcdp/solution_interface.py,sha256=sYW2lddJ7NesUDVW-WdSMQ_BElCQIK6MxALQY_dIJCw,7934
-act4e_mcdp-0.5.0.dist-info/METADATA,sha256=YvT51akYxkY0e6fkVlHTJbDGvkFI1toYE_gLZflxmb8,361
-act4e_mcdp-0.5.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-act4e_mcdp-0.5.0.dist-info/entry_points.txt,sha256=rtFkJmTGnQcebzyd-LQ-lyrbP1hJ1FtkJ9E4W5niq3o,164
-act4e_mcdp-0.5.0.dist-info/RECORD,,
+act4e_mcdp/solution_interface.py,sha256=ZXjfYHep9JNFukgCJfgs5smqrwazsXmkJU9Da4LIQsg,7955
+act4e_mcdp-0.6.0.dist-info/METADATA,sha256=fNbevVXlLzw6xGVJcCE9viftxg16BKihHIlejYhebqE,361
+act4e_mcdp-0.6.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+act4e_mcdp-0.6.0.dist-info/entry_points.txt,sha256=cFH3w3DzczOms0kJedGgJfIn3m4Ip6dqqlcFy5dRWWI,225
+act4e_mcdp-0.6.0.dist-info/RECORD,,
```

