# Comparing `tmp/jupytercards-2.5.3.tar.gz` & `tmp/jupytercards-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.5.3.tar", last modified: Fri May 19 14:03:02 2023, max compression
+gzip compressed data, was "jupytercards-2.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jupytercards-2.5.3.tar` & `jupytercards-2.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.5.3/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.5.3/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.5.3/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     4210 2023-05-17 20:46:04.470697 jupytercards-2.5.3/README.md
--rw-r--r--   0        0        0    28114 2023-05-12 13:16:37.861910 jupytercards-2.5.3/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.5.3/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.5.3/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.5.3/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      657 2023-05-19 14:01:51.403060 jupytercards-2.5.3/jupytercards/__init__.py
--rw-r--r--   0        0        0     9737 2023-05-19 14:00:07.262578 jupytercards-2.5.3/jupytercards/dynamic.py
--rw-r--r--   0        0        0    10291 2023-05-17 20:41:22.769979 jupytercards-2.5.3/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.5.3/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.5.3/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 jupytercards-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.5.4/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.5.4/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.5.4/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     4210 2023-05-17 20:46:04.470697 jupytercards-2.5.4/README.md
+-rw-r--r--   0        0        0    28114 2023-05-12 13:16:37.861910 jupytercards-2.5.4/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.5.4/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.5.4/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.5.4/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      657 2023-05-28 20:19:35.850403 jupytercards-2.5.4/jupytercards/__init__.py
+-rw-r--r--   0        0        0     9737 2023-05-19 14:00:07.262578 jupytercards-2.5.4/jupytercards/dynamic.py
+-rw-r--r--   0        0        0    10291 2023-05-17 20:41:22.769979 jupytercards-2.5.4/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4216 2023-05-28 20:04:15.394179 jupytercards-2.5.4/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.5.4/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 jupytercards-2.5.4/PKG-INFO
```

### Comparing `jupytercards-2.5.3/.gitignore` & `jupytercards-2.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/LICENSE` & `jupytercards-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/Markdown-flashcards.ipynb` & `jupytercards-2.5.4/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/README.md` & `jupytercards-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/example.ipynb` & `jupytercards-2.5.4/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/extractdefinitions.py` & `jupytercards-2.5.4/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/flashcards.gif` & `jupytercards-2.5.4/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/jupytercards/__init__.py` & `jupytercards-2.5.4/jupytercards/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.5.3'
+__version__ = '2.5.4'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.5.3/jupytercards/dynamic.py` & `jupytercards-2.5.4/jupytercards/dynamic.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/jupytercards/flashcards.js` & `jupytercards-2.5.4/jupytercards/flashcards.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/jupytercards/styles.css` & `jupytercards-2.5.4/jupytercards/styles.css`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 .next {
     color: var(--rich-black-fogra-39);
     cursor:pointer;
     font-size: 1.5em;
     /*left:90%; */
     margin-left: 70%;
-    width: 100pt;
+    width: 55pt;
     height: 22pt;
     opacity:0.3;
     position:relative; 
     top:-1em;
 }
 
 .next svg {
```

### Comparing `jupytercards-2.5.3/jupytercards/swiped-events.min.js` & `jupytercards-2.5.4/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.5.3/PKG-INFO` & `jupytercards-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.5.3
+Version: 2.5.4
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

