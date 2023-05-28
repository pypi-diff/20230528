# Comparing `tmp/sword2vec-3.2.6.tar.gz` & `tmp/sword2vec-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sword2vec-3.2.6.tar", last modified: Sat May 27 08:10:33 2023, max compression
+gzip compressed data, was "sword2vec-3.2.7.tar", last modified: Sun May 28 13:30:36 2023, max compression
```

## Comparing `sword2vec-3.2.6.tar` & `sword2vec-3.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:10:33.262539 sword2vec-3.2.6/
--rw-rw-rw-   0        0        0     1097 2023-05-27 04:27:08.000000 sword2vec-3.2.6/LICENSE
--rw-rw-rw-   0        0        0     2952 2023-05-27 08:10:33.260540 sword2vec-3.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2475 2023-05-27 06:27:03.000000 sword2vec-3.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 08:10:33.262539 sword2vec-3.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1284 2023-05-27 07:58:11.000000 sword2vec-3.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:10:33.230537 sword2vec-3.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:10:33.241539 sword2vec-3.2.6/src/sword2vec/
--rw-rw-rw-   0        0        0      163 2023-05-27 06:14:31.000000 sword2vec-3.2.6/src/sword2vec/__init__.py
--rw-rw-rw-   0        0        0     6369 2023-05-27 07:00:04.000000 sword2vec-3.2.6/src/sword2vec/preprocessor.py
--rw-rw-rw-   0        0        0    14071 2023-05-27 07:00:54.000000 sword2vec-3.2.6/src/sword2vec/word2vec.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:10:33.258547 sword2vec-3.2.6/src/sword2vec.egg-info/
--rw-rw-rw-   0        0        0     2952 2023-05-27 08:10:33.000000 sword2vec-3.2.6/src/sword2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-27 08:10:33.000000 sword2vec-3.2.6/src/sword2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:10:33.000000 sword2vec-3.2.6/src/sword2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-27 08:10:33.000000 sword2vec-3.2.6/src/sword2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 08:10:33.000000 sword2vec-3.2.6/src/sword2vec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 13:30:36.274640 sword2vec-3.2.7/
+-rw-rw-rw-   0        0        0     1097 2023-05-27 04:27:08.000000 sword2vec-3.2.7/LICENSE
+-rw-rw-rw-   0        0        0     2952 2023-05-28 13:30:36.273639 sword2vec-3.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2475 2023-05-27 06:27:03.000000 sword2vec-3.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 13:30:36.275641 sword2vec-3.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1284 2023-05-28 13:30:31.000000 sword2vec-3.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 13:30:36.173058 sword2vec-3.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 13:30:36.236637 sword2vec-3.2.7/src/sword2vec/
+-rw-rw-rw-   0        0        0      163 2023-05-27 06:14:31.000000 sword2vec-3.2.7/src/sword2vec/__init__.py
+-rw-rw-rw-   0        0        0     6369 2023-05-27 07:00:04.000000 sword2vec-3.2.7/src/sword2vec/preprocessor.py
+-rw-rw-rw-   0        0        0    14358 2023-05-28 13:29:46.000000 sword2vec-3.2.7/src/sword2vec/word2vec.py
+drwxrwxrwx   0        0        0        0 2023-05-28 13:30:36.270638 sword2vec-3.2.7/src/sword2vec.egg-info/
+-rw-rw-rw-   0        0        0     2952 2023-05-28 13:30:36.000000 sword2vec-3.2.7/src/sword2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-28 13:30:36.000000 sword2vec-3.2.7/src/sword2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 13:30:36.000000 sword2vec-3.2.7/src/sword2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-28 13:30:36.000000 sword2vec-3.2.7/src/sword2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-28 13:30:36.000000 sword2vec-3.2.7/src/sword2vec.egg-info/top_level.txt
```

### Comparing `sword2vec-3.2.6/LICENSE` & `sword2vec-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sword2vec-3.2.6/PKG-INFO` & `sword2vec-3.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sword2vec
-Version: 3.2.6
+Version: 3.2.7
 Summary: A simple skipgram word2vec implementations
 Home-page: https://github.com/aziyan99/sword2vec
 Author: Raja Azian
 Author-email: rajaazian08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sword2vec-3.2.6/README.md` & `sword2vec-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sword2vec-3.2.6/setup.py` & `sword2vec-3.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 extensions = [
     Extension("sword2vec.helpers", [os.path.join(basdir, "src/sword2vec/helpers.pyx")])
 ]
 
 
 setup(
     name="sword2vec",
-    version="3.2.6",
+    version="3.2.7",
     author="Raja Azian",
     author_email="rajaazian08@gmail.com",
     description="A simple skipgram word2vec implementations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aziyan99/sword2vec",
     classifiers=[
```

### Comparing `sword2vec-3.2.6/src/sword2vec/preprocessor.py` & `sword2vec-3.2.7/src/sword2vec/preprocessor.py`

 * *Files identical despite different names*

### Comparing `sword2vec-3.2.6/src/sword2vec/word2vec.py` & `sword2vec-3.2.7/src/sword2vec/word2vec.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.INFO)
 
 import datetime
 import time
 import gzip
 import gc
 import pickle
+import pickletools
 from . import helpers
 
 np.random.seed(1)
 
 
 class SkipGramWord2Vec:
     """
@@ -217,52 +218,56 @@
         """
         Predicts the most probable words given a target word.
 
         Parameters:
         - word (str): The target word for prediction.
         - topn (int): The number of top words to return. Default is 2.
         """
-        word = word.lower()
-        center_vec = [0] * len(self.word_to_idx)
-        center_vec[self.word_to_idx[word]] = 1
-
-        out, _, _ = helpers.forward_pass(center_vec, self.w1, self.w2)
-        most_likely_idxs = np.array(out).argsort()[-topn:][::-1]
-        return [self.idx_to_word[w] for w in most_likely_idxs]
+        try:
+            word = word.lower()
+            center_vec = [0] * len(self.word_to_idx)
+            center_vec[self.word_to_idx[word]] = 1
+
+            out, _, _ = helpers.forward_pass(center_vec, self.w1, self.w2)
+            most_likely_idxs = np.array(out).argsort()[-topn:][::-1]
+            return [self.idx_to_word[w] for w in most_likely_idxs]
+        except KeyError:
+            logging.warning(f"{word}'s unknown.")
 
     def search_similar_words(self, word, topn=10):
         """
         Searches for the most similar words to the given word based on learned word embeddings.
 
         Parameters:
         - word (str): The word to search for similar words.
         - topn (int): The number of top similar words to return. Default is 10.
         """
-        try:
+        similar_words = {}
+        if self.word_to_idx.get(word):
             word_embedding = self.w1[self.word_to_idx[word]]
             word_embeddings = self.w1
 
             similarities = []
             for embedding in word_embeddings:
                 similarity = helpers.cosine_similarity(word_embedding, embedding)
                 similarities.append(similarity)
 
             similarities = np.array(similarities)
 
             # Get the indices of the most similar words (excluding the search word)
             similar_word_indices = similarities.argsort()[-(topn + 1) : -1][::-1]
 
             # Create a dictionary of {word: score} pairs
-            similar_words = {}
             for idx in similar_word_indices:
                 similar_words[self.idx_to_word[idx]] = similarities[idx]
 
             return similar_words
-        except KeyError:
+        else:
             logging.warning(f"{word}'s unknown.")
+            return similar_words
 
     def save_model(self, filename=None):
         """
         Saves the trained model to a pickle file.
 
         Parameters:
         - filename (str): The name of the file to save the model. If not provided, a timestamped filename will be used.
@@ -313,15 +318,16 @@
             "w2": self.w2,
             "history": self.history,
             "matrix": self.matrix,
             "vocabulary": self.vocabulary,
         }
 
         with gzip.open(filename, "wb") as file:
-            pickle.dump(model_data, file, protocol=-1)
+            optimized_pickled = pickletools.optimize(pickle.dumps(model_data))
+            file.write(optimized_pickled)
 
     @staticmethod
     def load_model(filename):
         """
         Loads a saved model from a pickle file.
 
         Parameters:
@@ -363,15 +369,16 @@
 
         Returns:
         - model (SkipGramWord2Vec): The loaded SkipGramWord2Vec model.
         """
         try:
             logging.info("| Load compressed model")
             with gzip.open(filename, "rb") as file:
-                model_data = pickle.load(file)
+                p = pickle.Unpickler(file=file)
+                model_data = p.load()
 
             model = SkipGramWord2Vec(
                 window_size=model_data["window_size"],
                 learning_rate=model_data["learning_rate"],
                 embedding_dim=model_data["embedding_dim"],
                 epochs=model_data["epochs"],
             )
```

### Comparing `sword2vec-3.2.6/src/sword2vec.egg-info/PKG-INFO` & `sword2vec-3.2.7/src/sword2vec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sword2vec
-Version: 3.2.6
+Version: 3.2.7
 Summary: A simple skipgram word2vec implementations
 Home-page: https://github.com/aziyan99/sword2vec
 Author: Raja Azian
 Author-email: rajaazian08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

