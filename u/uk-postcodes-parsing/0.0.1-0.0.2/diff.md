# Comparing `tmp/uk_postcodes_parsing-0.0.1.tar.gz` & `tmp/uk_postcodes_parsing-0.0.2.tar.gz`

## Comparing `uk_postcodes_parsing-0.0.1.tar` & `uk_postcodes_parsing-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/tests/tests.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/LICENSE
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/tests/tests.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.2/PKG-INFO
```

### Comparing `uk_postcodes_parsing-0.0.1/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.1/src/uk_postcodes_parsing/fix.py` & `uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/fix.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.1/src/uk_postcodes_parsing/postcode_utils.py` & `uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/postcode_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,50 +31,38 @@
 def to_normalised(postcode: str) -> Union[str, None]:
     outcode = to_outcode(postcode)
     if outcode is None:
         return None
     incode = to_incode(postcode)
     return None if incode is None else f'{outcode} {incode}'
 
-
 def to_outcode(postcode: str) -> Union[str, None]:
     if not is_valid(postcode):
         return None
     return re.sub(INCODE_REGEX, '', sanitize(postcode))
 
 def to_incode(postcode: str) -> Union[str, None]:
     if not is_valid(postcode):
         return
     incode = re.findall(INCODE_REGEX, sanitize(postcode))
     return incode[0] if incode else None
 
 def to_area(postcode: str) -> Union[str, None]:
-    """
-    Returns a correctly formatted area given a postcode
-
-    Args:
-        postcode: The postcode to get the area of
-
-    Returns:
-        The area, or `None` if the postcode is invalid
-    """
-
     if not is_valid(postcode):
         return None
     area = re.findall(AREA_REGEX, sanitize(postcode))
     return area[0] if area else None
 
 def to_sector(postcode: str) -> Union[str, None]:
     outcode = to_outcode(postcode)
     if outcode is None:
         return None
     incode = to_incode(postcode)
     return None if incode is None else f'{outcode} {incode[0]}'
 
-
 def to_unit(postcode: str) -> Union[str, None]:
     if not is_valid(postcode):
         return None
     unit = re.findall(UNIT_REGEX, sanitize(postcode))
     return unit[0] if unit else None
 
 def to_district(postcode):
```

### Comparing `uk_postcodes_parsing-0.0.1/src/uk_postcodes_parsing/ukpostcode.py` & `uk_postcodes_parsing-0.0.2/src/uk_postcodes_parsing/ukpostcode.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from typing import Union, List
 
 from uk_postcodes_parsing.postcode_utils import *
 from uk_postcodes_parsing.fix import fix
 
 logging.basicConfig(level=logging.DEBUG)
-logger = logging.getLogger('ukpostcode')
+logger = logging.getLogger('uk-postcodes-parsing')
 
 # Test for a valid postcode embedded in text
 POSTCODE_CORPUS_REGEX = re.compile(r'[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}', re.I)
 FIXABLE_POSTCODE_CORPUS_REGEX = re.compile("[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}")
 
 def _parse(postcode: str) -> dict:
     if not is_valid(postcode):
```

### Comparing `uk_postcodes_parsing-0.0.1/tests/tests.py` & `uk_postcodes_parsing-0.0.2/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ukpostcodes.fix import fix
-from ukpostcodes.ukpostcode import parse_from_corpus, Postcode
+from uk_postcodes_parsing.fix import fix
+from uk_postcodes_parsing.ukpostcode import parse_from_corpus, Postcode
 
 #TODO - covert to actual tests
 
 def test_fix():
     # Trims postcode
     assert fix(" SW1A 2AA ") == "SW1A 2AA"
     # Upper case
```

### Comparing `uk_postcodes_parsing-0.0.1/.gitignore` & `uk_postcodes_parsing-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.1/LICENSE` & `uk_postcodes_parsing-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.1/pyproject.toml` & `uk_postcodes_parsing-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uk_postcodes_parsing"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Anirudh Gangwal", email="angangwa@amazon.com" },
 ]
 description = "A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `uk_postcodes_parsing-0.0.1/PKG-INFO` & `uk_postcodes_parsing-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 Metadata-Version: 2.1
 Name: uk_postcodes_parsing
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP.
 Project-URL: Homepage, https://github.com/anirudhgangwal/ukpostcodes
 Project-URL: Bug Tracker, https://github.com/anirudhgangwal/ukpostcodes/issues
 Author-email: Anirudh Gangwal <angangwa@amazon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# ukpostcodes
-
-NOTE: pending improvements / tests.
+# uk-postcodes-parsing
 
 A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP.
 
-Example usage:
+Install:
 
 ```bash
-git clone https://github.com/anirudhgangwal/ukpostcodes.git
-cd ukpostcodes
-pip install .
+pip install uk-postcodes-parsing
 ``` 
 
-```python
-from ukpostcodes import parse_from_corpus
+## Usage
 
-corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
+- Parsing text to get a list of postcodes.
 
-postcodes = parse_from_corpus(corpus)
-print(postcodes)
+```python
+>>> from uk_postcodes_parsing.ukpostcode import parse_from_corpus, Postcode
+>>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
+>>> postcodes = parse_from_corpus(corpus)
+INFO:uk-postcodes-parsing:Found 2 postcodes in corpus
+>>> print(postcodes)
+[Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(original='e34ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
 ```
 
-Output
+- Optional auto-correct: Attempt correcting common mistakes in postcodes such as reading "O" and "0" and vice-versa.
 
+```python
+>>> from uk_postcodes_parsing.ukpostcode import parse_from_corpus, Postcode
+>>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
+>>> postcodes = parse_from_corpus(corpus, attempt_fix=True)
+INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
+INFO:uk-postcodes-parsing:Found 3 postcodes in corpus
 ```
-INFO:ukpostcode:Found 3 postcodes in corpus
+
+- Parsing
+
+```python
+>>> parse("EC1r 1ub")
+Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
+>>> parse("EH16 50Y", attempt_fix=True)
 INFO:ukpostcode:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
-[Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(original='e34ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS'), Postcode(original='eh16 50y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')]
+Postcode(original='eh16 50y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
+```
+
+- Fixing
+
+```python
+>>> from uk_postcodes_parsing.fix import fix
+>>> fix("0W1 OAA") 
+OW1 0AA
 ```
```

