# Comparing `tmp/rising_plugin-0.0.5.tar.gz` & `tmp/rising_plugin-0.0.6.tar.gz`

## Comparing `rising_plugin-0.0.5.tar` & `rising_plugin-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/.idea/RisingPlugin.iml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/csv_embed.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/image_embedding.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/phone.csv
--rw-r--r--   0        0        0   283637 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/phone.json
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/pinecone_engine.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/risingplugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/common/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/src/rising_plugin/common/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/LICENSE
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 rising_plugin-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/RisingPlugin.iml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/csv_embed.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/image_embedding.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/phone.csv
+-rw-r--r--   0        0        0   283637 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/phone.json
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/pinecone_engine.py
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/risingplugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/common/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/common/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/LICENSE
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/PKG-INFO
```

### Comparing `rising_plugin-0.0.5/.idea/workspace.xml` & `rising_plugin-0.0.6/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.5/.idea/inspectionProfiles/Project_Default.xml` & `rising_plugin-0.0.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.5/src/rising_plugin/csv_embed.py` & `rising_plugin-0.0.6/src/rising_plugin/csv_embed.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.5/src/rising_plugin/image_embedding.py` & `rising_plugin-0.0.6/src/rising_plugin/image_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from langchain.embeddings.openai import OpenAIEmbeddings
 
 from .common.utils import OPENAI_API_KEY, PINECONE_NAMESPACE, PINECONE_INDEX_NAME
-from pinecone_engine import (
+from .pinecone_engine import (
     init_pinecone,
     get_pinecone_index_namespace,
 )
 
 
 def get_embeddings():
     return OpenAIEmbeddings(openai_api_key=OPENAI_API_KEY)
```

### Comparing `rising_plugin-0.0.5/src/rising_plugin/phone.csv` & `rising_plugin-0.0.6/src/rising_plugin/phone.csv`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.5/src/rising_plugin/phone.json` & `rising_plugin-0.0.6/src/rising_plugin/phone.json`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.5/src/rising_plugin/pinecone_engine.py` & `rising_plugin-0.0.6/src/rising_plugin/pinecone_engine.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.5/src/rising_plugin/risingplugin.py` & `rising_plugin-0.0.6/src/rising_plugin/risingplugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from firebase_admin import storage
 
 from .common.utils import (
     OPENAI_API_KEY,
     FIREBASE_STORAGE_ROOT,
     COMMAND_SMS_INDEXS,
 )
-from image_embedding import (
+from .image_embedding import (
     query_image_text,
     get_prompt_image_with_message,
 )
 
 def getCompletion(query, model="gpt-3.5-turbo", uuid="", image_search=True,):
     llm = ChatOpenAI(model_name=model, temperature=0, openai_api_key=OPENAI_API_KEY)
     chain = load_qa_chain(llm, chain_type="stuff")
```

### Comparing `rising_plugin-0.0.5/LICENSE` & `rising_plugin-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.5/pyproject.toml` & `rising_plugin-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rising_plugin"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Thomas Richardson", email="thomasr37oss@gmail.com" },
 ]
 description = "It is a plugin for Rising GPT"
 readme = "README.md"
 dependencies = [
     "langchain >= 0.0.148",
```

### Comparing `rising_plugin-0.0.5/PKG-INFO` & `rising_plugin-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rising_plugin
-Version: 0.0.5
+Version: 0.0.6
 Summary: It is a plugin for Rising GPT
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Thomas Richardson <thomasr37oss@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

