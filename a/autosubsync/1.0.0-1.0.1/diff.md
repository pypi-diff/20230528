# Comparing `tmp/autosubsync-1.0.0-py2.py3-none-any.whl.zip` & `tmp/autosubsync-1.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 16712 bytes, number of entries: 17
--rw-r--r--  2.0 unx     2533 b- defN 18-Oct-03 18:34 trained-model.bin
--rw-r--r--  2.0 unx     3321 b- defN 20-Sep-14 15:24 autosubsync/preprocessing.py
--rw-r--r--  2.0 unx     2503 b- defN 18-Sep-29 13:24 autosubsync/quality_of_fit.py
--rw-r--r--  2.0 unx     5132 b- defN 19-Mar-11 20:48 autosubsync/srt_io.py
--rw-r--r--  2.0 unx      150 b- defN 18-Sep-30 15:45 autosubsync/__init__.py
--rw-r--r--  2.0 unx     5735 b- defN 19-Mar-11 17:32 autosubsync/main.py
--rw-r--r--  2.0 unx     6027 b- defN 18-Oct-03 18:16 autosubsync/features.py
--rw-r--r--  2.0 unx     2315 b- defN 18-Sep-30 16:13 autosubsync/trained_logistic_regression.py
--rw-r--r--  2.0 unx     3776 b- defN 19-Mar-11 19:59 autosubsync/find_transform.py
--rw-r--r--  2.0 unx     3110 b- defN 18-Sep-30 16:13 autosubsync/model.py
--rw-r--r--  2.0 unx      340 b- defN 20-Sep-14 15:31 autosubsync-1.0.0.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx       63 b- defN 20-Sep-14 15:31 autosubsync-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1126 b- defN 20-Sep-14 15:31 autosubsync-1.0.0.dist-info/metadata.json
--rw-r--r--  2.0 unx       12 b- defN 20-Sep-14 15:31 autosubsync-1.0.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx      110 b- defN 20-Sep-14 15:31 autosubsync-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     1206 b- defN 20-Sep-14 15:31 autosubsync-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx     1448 b- defN 20-Sep-14 15:31 autosubsync-1.0.0.dist-info/RECORD
-17 files, 38907 bytes uncompressed, 14352 bytes compressed:  63.1%
+Zip file size: 16873 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     2533 b- defN 21-Mar-03 02:11 trained-model.bin
+-rw-rw-r--  2.0 unx      150 b- defN 21-Mar-03 02:10 autosubsync/__init__.py
+-rw-rw-r--  2.0 unx     6027 b- defN 21-Mar-03 02:10 autosubsync/features.py
+-rw-rw-r--  2.0 unx     3773 b- defN 23-May-28 20:36 autosubsync/find_transform.py
+-rw-r--r--  2.0 unx     5735 b- defN 21-Mar-03 02:10 autosubsync/main.py
+-rw-rw-r--  2.0 unx     3110 b- defN 21-Mar-03 02:10 autosubsync/model.py
+-rw-r--r--  2.0 unx      932 b- defN 21-Mar-03 02:10 autosubsync/predict.py
+-rw-rw-r--  2.0 unx     3318 b- defN 23-May-28 20:36 autosubsync/preprocessing.py
+-rw-rw-r--  2.0 unx     2503 b- defN 21-Mar-03 02:10 autosubsync/quality_of_fit.py
+-rw-rw-r--  2.0 unx     5132 b- defN 21-Mar-03 02:10 autosubsync/srt_io.py
+-rw-r--r--  2.0 unx     2315 b- defN 21-Mar-03 02:10 autosubsync/trained_logistic_regression.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-28 20:40 autosubsync-1.0.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1114 b- defN 23-May-28 20:40 autosubsync-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-28 20:40 autosubsync-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-May-28 20:40 autosubsync-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-May-28 20:40 autosubsync-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1408 b- defN 23-May-28 20:40 autosubsync-1.0.1.dist-info/RECORD
+17 files, 39305 bytes uncompressed, 14559 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -1,52 +1,52 @@
 Filename: trained-model.bin
 Comment: 
 
-Filename: autosubsync/preprocessing.py
+Filename: autosubsync/__init__.py
 Comment: 
 
-Filename: autosubsync/quality_of_fit.py
+Filename: autosubsync/features.py
 Comment: 
 
-Filename: autosubsync/srt_io.py
+Filename: autosubsync/find_transform.py
 Comment: 
 
-Filename: autosubsync/__init__.py
+Filename: autosubsync/main.py
 Comment: 
 
-Filename: autosubsync/main.py
+Filename: autosubsync/model.py
 Comment: 
 
-Filename: autosubsync/features.py
+Filename: autosubsync/predict.py
 Comment: 
 
-Filename: autosubsync/trained_logistic_regression.py
+Filename: autosubsync/preprocessing.py
 Comment: 
 
-Filename: autosubsync/find_transform.py
+Filename: autosubsync/quality_of_fit.py
 Comment: 
 
-Filename: autosubsync/model.py
+Filename: autosubsync/srt_io.py
 Comment: 
 
-Filename: autosubsync-1.0.0.dist-info/DESCRIPTION.rst
+Filename: autosubsync/trained_logistic_regression.py
 Comment: 
 
-Filename: autosubsync-1.0.0.dist-info/entry_points.txt
+Filename: autosubsync-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: autosubsync-1.0.0.dist-info/metadata.json
+Filename: autosubsync-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: autosubsync-1.0.0.dist-info/top_level.txt
+Filename: autosubsync-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: autosubsync-1.0.0.dist-info/WHEEL
+Filename: autosubsync-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: autosubsync-1.0.0.dist-info/METADATA
+Filename: autosubsync-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: autosubsync-1.0.0.dist-info/RECORD
+Filename: autosubsync-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autosubsync/preprocessing.py

```diff
@@ -27,15 +27,15 @@
     if sample_rate < warning_threshold:
         # probably never happens but checking anyway
         sys.stderr.write('warning: low sound sample rate %d Hz\n' % sample_rate)
 
     return samples, sample_rate, data_range
 
 def build_sub_vec(subs, sample_rate, n, sub_filter=None):
-    subvec = np.zeros(n, np.bool)
+    subvec = np.zeros(n, bool)
     to_index = lambda x: int(sample_rate*x)
     for line in subs:
         if sub_filter is not None and not sub_filter(line.text): continue
         subvec[to_index(line.begin):to_index(line.end)] = 1
     return subvec
 
 def import_subs(srt_filename, sample_rate, n, **kwargs):
```

## autosubsync/find_transform.py

```diff
@@ -11,15 +11,15 @@
     # sklearn.roc_auc_score but this is faster to compute
     labels = labels == 1
     return (np.sum(probs[labels]) + np.sum(1.0 - probs[~labels]))/float(len(labels))
 
 def sub_score_transform(y_true, y_probs, func):
     y_true = np.array(list(y_true))
     n = len(y_true)
-    shifted_indices = np.round(func(np.arange(n)*frame_secs)/frame_secs).astype(np.int)
+    shifted_indices = np.round(func(np.arange(n)*frame_secs)/frame_secs).astype(int)
     y_shift = y_true*0
     valid_indices = (shifted_indices >= 0) & (shifted_indices < n)
     y_shift[shifted_indices[valid_indices]] = y_true[valid_indices]
 
     missed_fraction = np.sum(y_true[~valid_indices])
     penalty_factor = 1.0 - missed_fraction / float(n)
```

## Comparing `autosubsync-1.0.0.dist-info/METADATA` & `autosubsync-1.0.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-Metadata-Version: 2.0
+Metadata-Version: 2.1
 Name: autosubsync
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automatically synchronize subtitles with audio
 Home-page: https://github.com/oseiskar/autosubsync
 Author: Otto Seiskari
 License: MIT
 Keywords: subtitles syncrhonization srt ffmpeg
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Multimedia
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Provides-Extra: test
-Provides-Extra: dev
 Requires-Dist: numpy
 Requires-Dist: pysoundfile
 Provides-Extra: dev
-Requires-Dist: pandas; extra == 'dev'
-Requires-Dist: sklearn; extra == 'dev'
-Provides-Extra: test
-Requires-Dist: nose; extra == 'test'
+Requires-Dist: pandas ; extra == 'dev'
+Requires-Dist: scikit-learn ; extra == 'dev'
 
 Automatically synchronize SRT subtitles with audio.
 Requires ffmpeg (``sudo apt-get install ffmepg``)::
 
   autosubsync [input movie] [input subtitles] [output subs]
 
   # for example
```

