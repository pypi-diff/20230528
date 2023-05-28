# Comparing `tmp/openschema-0.6.dev2-py3-none-any.whl.zip` & `tmp/openschema-0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14655 bytes, number of entries: 12
--rw-r--r--  2.0 unx      836 b- defN 20-Feb-02 00:00 openschema/__init__.py
+Zip file size: 14591 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      831 b- defN 20-Feb-02 00:00 openschema/__init__.py
 -rw-r--r--  2.0 unx      944 b- defN 20-Feb-02 00:00 openschema/kaggle/__init__.py
 -rw-r--r--  2.0 unx     3069 b- defN 20-Feb-02 00:00 openschema/kaggle/_avazu.py
 -rw-r--r--  2.0 unx     2732 b- defN 20-Feb-02 00:00 openschema/kaggle/_titanic.py
 -rw-r--r--  2.0 unx     1010 b- defN 20-Feb-02 00:00 openschema/sklearn/__init__.py
 -rw-r--r--  2.0 unx     6768 b- defN 20-Feb-02 00:00 openschema/sklearn/_breast_cancer.py
 -rw-r--r--  2.0 unx     2458 b- defN 20-Feb-02 00:00 openschema/sklearn/_iris.py
-?rw-r--r--  2.0 unx     3783 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      124 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/licenses/NOTICE
-?rw-r--r--  2.0 unx     1026 b- defN 20-Feb-02 00:00 openschema-0.6.dev2.dist-info/RECORD
-12 files, 34195 bytes uncompressed, 12921 bytes compressed:  62.2%
+?rw-r--r--  2.0 unx     3778 b- defN 20-Feb-02 00:00 openschema-0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 openschema-0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openschema-0.7.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      124 b- defN 20-Feb-02 00:00 openschema-0.7.dist-info/licenses/NOTICE
+?rw-r--r--  2.0 unx     1001 b- defN 20-Feb-02 00:00 openschema-0.7.dist-info/RECORD
+12 files, 34160 bytes uncompressed, 12907 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: openschema/sklearn/_breast_cancer.py
 Comment: 
 
 Filename: openschema/sklearn/_iris.py
 Comment: 
 
-Filename: openschema-0.6.dev2.dist-info/METADATA
+Filename: openschema-0.7.dist-info/METADATA
 Comment: 
 
-Filename: openschema-0.6.dev2.dist-info/WHEEL
+Filename: openschema-0.7.dist-info/WHEEL
 Comment: 
 
-Filename: openschema-0.6.dev2.dist-info/licenses/LICENSE
+Filename: openschema-0.7.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: openschema-0.6.dev2.dist-info/licenses/NOTICE
+Filename: openschema-0.7.dist-info/licenses/NOTICE
 Comment: 
 
-Filename: openschema-0.6.dev2.dist-info/RECORD
+Filename: openschema-0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openschema/__init__.py

```diff
@@ -15,8 +15,8 @@
 # specific language governing permissions and limitations
 # under the License.
 
 """
 Schema catalog.
 """
 
-__version__ = '0.6.dev2'
+__version__ = '0.7'
```

## Comparing `openschema-0.6.dev2.dist-info/METADATA` & `openschema-0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openschema
-Version: 0.6.dev2
+Version: 0.7
 Summary: Programmatic catalog of public dataset schemas.
 Project-URL: Source, https://github.com/formlio/openschema/
 Project-URL: Documentation, https://openschema.readthedocs.io/
 Project-URL: Issues, https://github.com/formlio/openschema/issues/
 Maintainer-email: ForML Development Team <info@forml.io>
 License: Apache License 2.0
 License-File: LICENSE
```

## Comparing `openschema-0.6.dev2.dist-info/licenses/LICENSE` & `openschema-0.7.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

