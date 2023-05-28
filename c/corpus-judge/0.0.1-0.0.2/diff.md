# Comparing `tmp/corpus_judge-0.0.1.tar.gz` & `tmp/corpus_judge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_judge-0.0.1.tar", max compression
+gzip compressed data, was "corpus_judge-0.0.2.tar", max compression
```

## Comparing `corpus_judge-0.0.1.tar` & `corpus_judge-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1491 2023-05-28 20:04:11.444523 corpus_judge-0.0.1/LICENSE
--rw-r--r--   0        0        0      250 2023-05-28 20:00:18.687607 corpus_judge-0.0.1/README.md
--rw-r--r--   0        0        0      139 2023-05-28 19:48:28.330357 corpus_judge-0.0.1/corpus_judge/__init__.py
--rw-r--r--   0        0        0     6741 2023-05-28 20:20:39.194238 corpus_judge-0.0.1/corpus_judge/justice_model.py
--rw-r--r--   0        0        0    11934 2023-05-28 20:13:51.190037 corpus_judge-0.0.1/corpus_judge/justice_name.py
--rw-r--r--   0        0        0     9632 2023-05-28 19:55:20.425045 corpus_judge-0.0.1/corpus_judge/justice_select.py
--rw-r--r--   0        0        0    45229 2023-05-28 19:46:46.811633 corpus_judge-0.0.1/corpus_judge/sc.yaml
--rw-r--r--   0        0        0     1227 2023-05-28 20:07:51.688457 corpus_judge-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 corpus_judge-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-28 20:04:11.444523 corpus_judge-0.0.2/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-28 20:00:18.687607 corpus_judge-0.0.2/README.md
+-rw-r--r--   0        0        0      153 2023-05-28 20:44:53.654068 corpus_judge-0.0.2/corpus_judge/__init__.py
+-rw-r--r--   0        0        0     6750 2023-05-28 20:43:59.813913 corpus_judge-0.0.2/corpus_judge/justice_model.py
+-rw-r--r--   0        0        0    11934 2023-05-28 20:13:51.190037 corpus_judge-0.0.2/corpus_judge/justice_name.py
+-rw-r--r--   0        0        0     9654 2023-05-28 20:45:49.114547 corpus_judge-0.0.2/corpus_judge/justice_select.py
+-rw-r--r--   0        0        0    45229 2023-05-28 19:46:46.811633 corpus_judge-0.0.2/corpus_judge/sc.yaml
+-rw-r--r--   0        0        0     1227 2023-05-28 20:44:13.923099 corpus_judge-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 corpus_judge-0.0.2/PKG-INFO
```

### Comparing `corpus_judge-0.0.1/LICENSE` & `corpus_judge-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.1/corpus_judge/justice_model.py` & `corpus_judge-0.0.2/corpus_judge/justice_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import datetime
+from pathlib import Path
 
 from dateutil.parser import parse
 from dateutil.relativedelta import relativedelta as rd
 from pydantic import Field, validator
 from sqlpyd import IndividualBio
 
 MAX_JUSTICE_AGE = 70  # 1987 Constitution
+JUSTICE_FILE = Path(__file__).parent / "sc.yaml"
 
 
 class Bio(IndividualBio):
     @classmethod
     def from_dict(cls, data: dict):
         sfx = data.pop("Suffix")
         return cls(
@@ -49,21 +51,19 @@
         >>> from sqlite_utils.db import Table
         >>> c = Connection(DatabasePath="test.db")
         >>> c.path_to_db.unlink(missing_ok=True) # tear down
         >>> table = c.create_table(Justice)
         >>> isinstance(table, Table)
         True
         >>> # See local file
-        >>> from pathlib import Path
-        >>> f = Path(__file__).parent / "sc.yaml"
-        >>> f.exists()
+        >>> JUSTICE_FILE.exists()
         True
         >>> # Can add all pydantic validated records from the local copy of justices to the database.
         >>> import yaml
-        >>> res = c.add_records(Justice, yaml.safe_load(f.read_bytes()))
+        >>> res = c.add_records(Justice, yaml.safe_load(JUSTICE_FILE.read_bytes()))
         >>> len(list(table.rows))
         194
         >>> c.path_to_db.unlink() # tear down
 
     The list of justices from the sc.yaml file are parsed through this model prior to being inserted
     into the database.
     """  # noqa: E501
```

### Comparing `corpus_judge-0.0.1/corpus_judge/justice_name.py` & `corpus_judge-0.0.2/corpus_judge/justice_name.py`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.1/corpus_judge/justice_select.py` & `corpus_judge-0.0.2/corpus_judge/justice_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,19 +49,19 @@
         """When selecting a ponente or voting members, create a candidate list of
         justices based on the `valid_date`.
 
         Examples:
             >>> import yaml
             >>> from pathlib import Path
             >>> from sqlpyd import Connection
-            >>> p = Path(__file__).parent / "sc.yaml"
+            >>> from corpus_judge import JUSTICE_FILE
             >>> c = Connection(DatabasePath="test.db")
             >>> c.path_to_db.unlink(missing_ok=True) # tear down
             >>> tbl = c.create_table(Justice)
-            >>> res = c.add_records(Justice, yaml.safe_load(p.read_bytes()))
+            >>> res = c.add_records(Justice, yaml.safe_load(JUSTICE_FILE.read_bytes()))
             >>> search = CandidateJustice(db=c.db, date_str='Dec. 1, 1995')
             >>> print(search.rows) # since start date is greater than target date, record is included
             [{'id': 137, 'surname': 'panganiban', 'alias': None, 'start_term': '1995-10-05', 'inactive_date': '2006-12-06', 'chief_date': '2005-12-20'}, {'id': 136, 'surname': 'hermosisima', 'alias': 'hermosisima jr.', 'start_term': '1995-01-10', 'inactive_date': '1997-10-18', 'chief_date': None}, {'id': 135, 'surname': 'francisco', 'alias': None, 'start_term': '1995-01-05', 'inactive_date': '1998-02-13', 'chief_date': None}, {'id': 134, 'surname': 'mendoza', 'alias': None, 'start_term': '1994-06-07', 'inactive_date': '2003-04-05', 'chief_date': None}, {'id': 133, 'surname': 'kapunan', 'alias': None, 'start_term': '1994-01-05', 'inactive_date': '2002-08-12', 'chief_date': None}, {'id': 132, 'surname': 'vitug', 'alias': None, 'start_term': '1993-06-28', 'inactive_date': '2004-07-15', 'chief_date': None}, {'id': 131, 'surname': 'puno', 'alias': None, 'start_term': '1993-06-28', 'inactive_date': '2010-05-17', 'chief_date': '2007-12-08'}, {'id': 128, 'surname': 'melo', 'alias': None, 'start_term': '1992-08-10', 'inactive_date': '2002-05-30', 'chief_date': None}, {'id': 127, 'surname': 'bellosillo', 'alias': None, 'start_term': '1992-03-03', 'inactive_date': '2003-11-13', 'chief_date': None}, {'id': 125, 'surname': 'romero', 'alias': None, 'start_term': '1991-10-21', 'inactive_date': '1999-08-01', 'chief_date': None}, {'id': 124, 'surname': 'davide', 'alias': 'davide jr.', 'start_term': '1991-01-24', 'inactive_date': '2005-12-20', 'chief_date': '1998-11-30'}, {'id': 123, 'surname': 'regalado', 'alias': None, 'start_term': '1988-07-29', 'inactive_date': '1998-10-13', 'chief_date': None}, {'id': 116, 'surname': 'padilla', 'alias': None, 'start_term': '1987-01-12', 'inactive_date': '1997-08-22', 'chief_date': None}, {'id': 115, 'surname': 'feliciano', 'alias': None, 'start_term': '1986-08-08', 'inactive_date': '1995-12-13', 'chief_date': None}, {'id': 112, 'surname': 'narvasa', 'alias': None, 'start_term': '1986-04-10', 'inactive_date': '1998-11-30', 'chief_date': '1991-12-08'}]
             >>> c.path_to_db.unlink() # tear down
 
         Returns:
             list[dict]: Filtered list of justices
@@ -139,19 +139,19 @@
     def detail(self) -> JusticeDetail | None:
         """Get object to match fields directly
 
         Examples:
             >>> import yaml
             >>> from pathlib import Path
             >>> from sqlpyd import Connection
-            >>> p = Path(__file__).parent / "sc.yaml"
+            >>> from corpus_judge import JUSTICE_FILE
             >>> c = Connection(DatabasePath="test.db")
             >>> c.path_to_db.unlink(missing_ok=True) # tear down
             >>> tbl = c.create_table(Justice)
-            >>> res = c.add_records(Justice, yaml.safe_load(p.read_bytes()))
+            >>> res = c.add_records(Justice, yaml.safe_load(JUSTICE_FILE.read_bytes()))
             >>> search = CandidateJustice(db=c.db, text='Panganiban, Acting Cj', date_str='Dec. 1, 1995')
             >>> print(search.detail)
             JusticeDetail(justice_id=137, raw_ponente='Panganiban', designation='J.', per_curiam=False)
             >>> c.path_to_db.unlink() # tear down
 
         Returns:
             JusticeDetail | None: Will subsequently be used in DecisionRow in a third-party library.
```

### Comparing `corpus_judge-0.0.1/corpus_judge/sc.yaml` & `corpus_judge-0.0.2/corpus_judge/sc.yaml`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.1/pyproject.toml` & `corpus_judge-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "corpus-judge"
 description = "Cleaning, setting Justices"
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/corpus-judge"
 documentation = "https://justmars.github.io/corpus-judge"
 classifiers = [
   "Programming Language :: Python :: 3.11",
```

### Comparing `corpus_judge-0.0.1/PKG-INFO` & `corpus_judge-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corpus-judge
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cleaning, setting Justices
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

