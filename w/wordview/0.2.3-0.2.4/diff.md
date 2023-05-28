# Comparing `tmp/wordview-0.2.3.tar.gz` & `tmp/wordview-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.2.3.tar", max compression
+gzip compressed data, was "wordview-0.2.4.tar", max compression
```

## Comparing `wordview-0.2.3.tar` & `wordview-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      742 2023-05-18 09:41:49.907167 wordview-0.2.3/CHANGES.rst
--rw-r--r--   0        0        0     1074 2022-06-16 16:46:04.846999 wordview-0.2.3/LICENSE
--rw-r--r--   0        0        0     4601 2023-05-18 07:47:52.026224 wordview-0.2.3/README.rst
--rw-r--r--   0        0        0      873 2023-05-18 09:41:53.859877 wordview-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      151 2022-06-16 16:46:04.892361 wordview-0.2.3/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-03-30 15:57:29.123003 wordview-0.2.3/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-02-19 17:09:47.466124 wordview-0.2.3/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-03-31 14:18:45.152428 wordview-0.2.3/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-02-24 14:54:27.524967 wordview-0.2.3/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-03-02 08:17:36.835194 wordview-0.2.3/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       84 2023-01-11 13:24:40.126952 wordview-0.2.3/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-01-24 17:56:38.022613 wordview-0.2.3/wordview/mwes/am.py
--rw-r--r--   0        0        0     5305 2023-05-10 15:53:47.791178 wordview-0.2.3/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     6711 2023-05-10 15:53:47.792472 wordview-0.2.3/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-03-08 15:49:42.676986 wordview-0.2.3/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-04-20 12:24:54.167225 wordview-0.2.3/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-03-27 11:57:05.780678 wordview-0.2.3/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11986 2023-05-18 09:32:55.382122 wordview-0.2.3/wordview/text_analysis/core.py
--rw-r--r--   0        0        0   938013 2022-12-31 16:48:35.212911 wordview-0.2.3/wordview/text_analysis/lid.176.ftz
--rw-r--r--   0        0        0     8399 2023-05-18 09:32:55.382826 wordview-0.2.3/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5489 1970-01-01 00:00:00.000000 wordview-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-05-28 14:55:33.259579 wordview-0.2.4/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2022-06-16 16:46:04.846999 wordview-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4638 2023-05-28 14:58:06.375929 wordview-0.2.4/README.rst
+-rw-r--r--   0        0        0      877 2023-05-28 14:51:21.658364 wordview-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-05-28 13:04:33.316548 wordview-0.2.4/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-03-30 15:57:29.123003 wordview-0.2.4/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-02-19 17:09:47.466124 wordview-0.2.4/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-03-31 14:18:45.152428 wordview-0.2.4/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-02-24 14:54:27.524967 wordview-0.2.4/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-03-02 08:17:36.835194 wordview-0.2.4/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       85 2023-05-28 13:04:33.317278 wordview-0.2.4/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-28 10:30:16.290129 wordview-0.2.4/wordview/mwes/am.py
+-rw-r--r--   0        0        0     8698 2023-05-28 10:30:16.291853 wordview-0.2.4/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-05-28 10:30:16.292732 wordview-0.2.4/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-03-08 15:49:42.676986 wordview-0.2.4/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-04-20 12:24:54.167225 wordview-0.2.4/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-05-28 13:04:33.317988 wordview-0.2.4/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11805 2023-05-28 10:30:16.293548 wordview-0.2.4/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8399 2023-05-19 15:06:13.517119 wordview-0.2.4/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 wordview-0.2.4/setup.py
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.2.4/PKG-INFO
```

### Comparing `wordview-0.2.3/LICENSE` & `wordview-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.2.3/README.rst` & `wordview-0.2.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-Wordview
-########
+Wordview (Work In Progress)
+###########################
 
 |PyPI version|
 
 |Python 3.9|
 
-
 Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
 Wordview's Python API is open-source and available under the `MIT
 license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
 offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
 more information about this framework.
 
 |text_analysis_cover|
```

### Comparing `wordview-0.2.3/pyproject.toml` & `wordview-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "wordview"
-version = "0.2.3"
+version = "0.2.4"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
-fasttext = "0.9.2"
+python = ">=3.9,<3.11"
+langdetect = ">=1.0.9"
 pandas = "2.0.1"
 scikit-learn = "1.2.2"
 scipy = "1.10.0"
 nltk = "3.6.6"
 tqdm = "4.62.3"
 wordcloud = "1.9.1.1"
 plotly = "5.5.0"
@@ -23,15 +23,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3.0.0"
 pytest = ">=7.1"
 pytest-cov = ">=3.0.0"
 ipython = ">=8.4.0"
 sphinx = ">=v6.1.3"
-sphinx-rtd-theme= "1.2.0"
+sphinx-rtd-theme= "1.2.1"
 
 [tool.poetry.scripts]
 script_download = "wordview.bin.downloads:download_nltk_req"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wordview-0.2.3/wordview/anomaly/gaussianize.py` & `wordview-0.2.4/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.3/wordview/anomaly/normaldist.py` & `wordview-0.2.4/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.3/wordview/clustering/cluster.py` & `wordview-0.2.4/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.3/wordview/mwes/am.py` & `wordview-0.2.4/wordview/mwes/am.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Dict, List
 import math
+from typing import Dict, List
 
 
 def calculate_pmi(
     compound_dict: dict,
     word_dic: dict,
     num_words: int,
     normalize: bool = False,
```

### Comparing `wordview-0.2.3/wordview/mwes/mwe.py` & `wordview-0.2.4/wordview/mwes/mwe.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
+import re
+from collections import Counter
 from pathlib import Path
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 import pandas
+import tqdm
 from nltk import word_tokenize
 
 from wordview import logger
 from wordview.mwes.am import calculate_am
-from wordview.mwes.mwe_utils import get_counts
+from wordview.mwes.mwe_utils import get_pos_tags, is_alphanumeric_latinscript_multigram
 
 
 class MWE(object):
     """
     Represents a Multiword Expression.
     """
 
     def __init__(
         self,
         df: pandas.DataFrame,
         text_column: str,
-        mwe_types: List[str] = ["NC"],
+        mwe_types: list[str] = ["NC"],
         tokenize=False,
     ) -> None:
         """Initialize a new MWE object with the given df, text_column and mwe_types.
 
         Args:
             df (pandas.DataFram): DataFrame with a text_column that contains the corpus.
             text_column (str): Specifies the column of DataFrame where text data resides.
@@ -31,14 +34,18 @@
             tokenize (bool): Tokenize the content of `df[text_column]`.
 
         Returns:
             None
         """
         self.df = df
         self.text_column = text_column
+        if not mwe_types:
+            raise ValueError("mwe_types is empty.")
+        if not isinstance(mwe_types, list):
+            raise TypeError("mwe_types is not a list.")
         for mt in mwe_types:
             if mt not in ["NC", "JNC"]:
                 raise ValueError(f"{mt} type is not recognized.")
         self.mwe_types = mwe_types
         if tokenize:
             logger.info(
                 '"tokenize" flag set to True. This might lead to a slow instantiation.'
@@ -80,68 +87,69 @@
                 logger.error(f"Could not tokenize and join tokens in {t}: \n {E} ")
 
         if float(num_pass) / float(len(tests)) < 0.8:
             logger.warning(
                 f"It seems that the content of {self.text_column} in the input data frame is not (fully) tokenized.\nThis can lead to poor results. Consider re-instantiating your MWE instance with 'tokenize' flag set to True.\nNote that this might lead to a slower instantiation."
             )
 
-    def build_counts(self, counts_filename: str = "") -> Union[None, Dict]:  # type: ignore
+    def build_counts(self, counts_filename: Optional[str] = None) -> Optional[Dict]:
         """Create various count files to be used by downstream methods
         by calling wordview.mwes.mwe_utils.
 
         Args:
             counts_filename (str): Filename for storing counts.
 
         Returns:
             None when no counts_filename is provided, otherwise res which is a dictionary of counts.
         """
         logger.info("Creating counts...")
-        res = get_counts(
-            df=self.df, text_column=self.text_column, mwe_types=self.mwe_types
-        )
+        res = self.get_counts()
         if not counts_filename:
             return res
         else:
             try:
                 with open(counts_filename, "w") as file:
                     json.dump(res, file)
             except Exception as e:
                 logger.error(e)
                 raise e
+            return None
 
     def extract_mwes(
         self,
         am: str = "pmi",
-        mwes_filename: str = "",
-        counts_filename: str = "",
-        counts: Dict = {},
-    ) -> Dict:
+        mwes_filename: Optional[str] = None,
+        counts_filename: Optional[str] = None,
+        counts: Optional[dict] = None,
+    ) -> dict:
         """
         Extract MWEs from counts_filename with respect to the association measure specified by `am`.
 
         Args:
             am (str): The association measure to be used. Can be any of [pmi, npmi]
             mwes_filename (str): File for storing MWEs. Defaults to None.
             counts_filename (str): File to read counts from.
 
         Returns:
             Dictionary of MWEs.
         """
         if counts:
             count_data = counts
-        else:
+        elif counts_filename is not None:
             try:
                 with open(counts_filename, "r") as file:
                     count_data = json.load(file)
             except Exception as e:
                 logger.error(e)
                 logger.error(
                     "Counts must be provided either via input argument `counts` or `counts_filename`. Argument `counts` is not specified and it seems like there was an error reading the counts from `counts_filename`."
                 )
                 raise e
+        else:
+            raise ValueError("Either 'counts' or 'counts_filename' must be provided.")
 
         logger.info(f"Extracting {self.mwe_types} based on {am}")
         mwe_am_dict = calculate_am(
             count_data=count_data, am=am, mwe_types=self.mwe_types
         )
         if mwes_filename:
             try:
@@ -150,7 +158,85 @@
             except Exception as e:
                 logger.error(e)
                 raise e
             finally:
                 return mwe_am_dict
         else:
             return mwe_am_dict
+
+    def get_counts(self) -> Dict:
+        """Read a corpus in pandas.DataFrame format and generates all counts necessary for calculating AMs.
+
+        Args:
+            None
+
+        Returns:
+            res: Dictionary of mwe_types to dictionary of individual mwe within that type and their count.
+                E.g. {'NC':{'climate change': 10, 'brain drain': 3}, 'JNC': {'black sheep': 3, 'red flag': 2}}
+        """
+        res: Dict = {}
+        for mt in self.mwe_types:
+            res[mt] = {}
+        res["WORDS"] = {}
+        for sent in tqdm.tqdm(self.df[self.text_column]):
+            tokens = sent.split(" ")
+            word_count_dict = Counter(tokens)
+            for k, v in word_count_dict.items():
+                if k in res["WORDS"]:
+                    res["WORDS"][k] += v
+                else:
+                    res["WORDS"][k] = v
+            for mt in self.mwe_types:
+                mwes_count_dic = self.extract_mwes_from_sent(tokens, mwe_type=mt)
+                for k, v in mwes_count_dic.items():
+                    if k in res[mt]:
+                        res[mt][k] += v
+                    else:
+                        res[mt][k] = v
+        return res
+
+    def extract_mwes_from_sent(self, tokens: list[str], mwe_type: str) -> Dict:
+        """Extract two-word noun compounds from tokenized input.
+
+        Args:
+            tokens: A tokenized sentence, i.e. list of tokens.
+            type: Type of MWE. Any of ['NC', 'JNC'].
+
+        Returns:
+            mwes_count_dic: Dictionary of compounds to their count.
+        """
+        if not isinstance(tokens, list):
+            raise TypeError(
+                f'Input argument "tokens" must be a list of string. Currently it is of type {type(tokens)} \
+                with a value of: {tokens}.'
+            )
+        if len(tokens) == 0:
+            return {}
+        mwes = []
+        postag_tokens: list[tuple[str, str]] = get_pos_tags(tokens)
+        w1_pos_tags = []
+        w2_pos_tags = []
+        if mwe_type == "NC":
+            w1_pos_tags = ["NN", "NNS"]
+            w2_pos_tags = ["NN", "NNS"]
+        elif mwe_type == "JNC":
+            w1_pos_tags = ["JJ"]
+            w2_pos_tags = ["NN", "NNS"]
+        for i in range(len(postag_tokens) - 1):
+            w1 = postag_tokens[i]
+            if w1[1] not in w1_pos_tags:
+                continue
+            else:
+                w2 = postag_tokens[i + 1]
+                if not is_alphanumeric_latinscript_multigram(
+                    w1[0]
+                ) or not is_alphanumeric_latinscript_multigram(w2[0]):
+                    continue
+                if w2[1] in w2_pos_tags:
+                    if i + 2 < len(postag_tokens):
+                        w3 = postag_tokens[i + 2]
+                        if w3 not in ["NN", "NNS"]:
+                            mwes.append(w1[0] + " " + w2[0])
+                    else:
+                        mwes.append(w1[0] + " " + w2[0])
+        mwes_count_dic = Counter(mwes)
+        return mwes_count_dic
```

### Comparing `wordview-0.2.3/wordview/preprocessing/cleaning.py` & `wordview-0.2.4/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.3/wordview/text_analysis/core.py` & `wordview-0.2.4/wordview/text_analysis/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-import os
 import string
 import time
 from statistics import median
 from typing import Any, Dict, List, Tuple
 
-import fasttext
 import nltk
 import numpy as np
 import pandas
 import pandas as pd
 import plotly
 import plotly.graph_objs as go
+from langdetect import detect
 from nltk.corpus import stopwords
-
-plotly.graph_objects.Figure
 from plotly.subplots import make_subplots
 from tqdm import tqdm
 from wordcloud import WordCloud, get_single_color_func
 
 from wordview import logger
 
-here = os.path.dirname(os.path.abspath(__file__))
-ftmodel = fasttext.load_model(os.path.join(here, "lid.176.ftz"))
-
 
 def plotly_wordcloud(
     token_count_dic: dict, settings: Dict = {"color": "deepskyblue", "max_words": 100}
 ) -> plotly.graph_objects.Scattergl:
     """Create a world cloud trace for plotly.
 
     Args:
@@ -258,15 +252,15 @@
     NNs: Dict[str, int] = {}
     JJs: Dict[str, int] = {}
     Vs: Dict[str, int] = {}
     languages = set()
 
     logger.info("Processing text in %s column of the input DataFrame..." % text_col)
     for text in tqdm(df[text_col]):
-        ls = ftmodel.predict(text)[0][0].replace("__label__", "").upper()
+        ls = detect(text).upper()
         languages.update([ls])
         try:
             tokens = text.lower().split(" ")
             doc_lengths.append(len(tokens))
             if skip_stopwords_punc:
                 tokens = [
                     t for t in tokens if t not in stop_words and t not in punctuations
```

### Comparing `wordview-0.2.3/wordview/text_analysis/wrapper.py` & `wordview-0.2.4/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.2.3/PKG-INFO` & `wordview-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.2.3
+Version: 0.2.4
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fasttext (==0.9.2)
+Requires-Dist: langdetect (>=1.0.9)
 Requires-Dist: nltk (==3.6.6)
 Requires-Dist: pandas (==2.0.1)
 Requires-Dist: plotly (==5.5.0)
 Requires-Dist: scikit-learn (==1.2.2)
 Requires-Dist: scipy (==1.10.0)
 Requires-Dist: sentence-transformers (==2.2.2)
 Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: tqdm (==4.62.3)
 Requires-Dist: wordcloud (==1.9.1.1)
 Description-Content-Type: text/x-rst
 
-Wordview
-########
+Wordview (Work In Progress)
+###########################
 
 |PyPI version|
 
 |Python 3.9|
 
-
 Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
 Wordview's Python API is open-source and available under the `MIT
 license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
 offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
 more information about this framework.
 
 |text_analysis_cover|
```

