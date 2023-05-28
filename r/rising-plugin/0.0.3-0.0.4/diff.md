# Comparing `tmp/rising_plugin-0.0.3.tar.gz` & `tmp/rising_plugin-0.0.4.tar.gz`

## Comparing `rising_plugin-0.0.3.tar` & `rising_plugin-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/RisingPlugin.iml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/__init__.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/csv_embed.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/image_embedding.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/phone.csv
--rw-r--r--   0        0        0   283637 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/phone.json
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/pinecone_engine.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/risingplugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/common/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/common/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/LICENSE
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/.idea/RisingPlugin.iml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/csv_embed.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/image_embedding.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/phone.csv
+-rw-r--r--   0        0        0   283637 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/phone.json
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/pinecone_engine.py
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/risingplugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/common/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/src/rising_plugin/common/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/LICENSE
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 rising_plugin-0.0.4/PKG-INFO
```

### Comparing `rising_plugin-0.0.3/.idea/workspace.xml` & `rising_plugin-0.0.4/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `rising_plugin-0.0.3/.idea/workspace.xml` & `rising_plugin-0.0.4/.idea/workspace.xml`

```diff
@@ -96,15 +96,15 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="a286c75f-6878-46cb-a44d-a341ea83c212" name="Changes" comment=""/>
       <created>1685296306253</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685296306253</updated>
       <workItem from="1685296307822" duration="2522000"/>
-      <workItem from="1685299570603" duration="5408000"/>
+      <workItem from="1685299570603" duration="5732000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `rising_plugin-0.0.3/.idea/inspectionProfiles/Project_Default.xml` & `rising_plugin-0.0.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.3/src/rising_plugin/csv_embed.py` & `rising_plugin-0.0.4/src/rising_plugin/csv_embed.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from langchain.document_loaders.csv_loader import CSVLoader
 from langchain.embeddings.openai import OpenAIEmbeddings
 import json
 
-from src.rising_plugin.common.utils import OPENAI_API_KEY
+from common.utils import OPENAI_API_KEY
 
 
 def csv_embed():
     loader = CSVLoader(file_path="src/langchain_plugin/phone.csv", encoding="utf8")
     data = loader.load()
     embeddings = OpenAIEmbeddings(openai_api_key=OPENAI_API_KEY)
```

### Comparing `rising_plugin-0.0.3/src/rising_plugin/image_embedding.py` & `rising_plugin-0.0.4/src/rising_plugin/image_embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from langchain.embeddings.openai import OpenAIEmbeddings
 
-from src.rising_plugin.common.utils import OPENAI_API_KEY, PINECONE_NAMESPACE, PINECONE_INDEX_NAME
-from src.rising_plugin.pinecone_engine import (
+from common.utils import OPENAI_API_KEY, PINECONE_NAMESPACE, PINECONE_INDEX_NAME
+from pinecone_engine import (
     init_pinecone,
     get_pinecone_index_namespace,
 )
 
 
 def get_embeddings():
     return OpenAIEmbeddings(openai_api_key=OPENAI_API_KEY)
```

### Comparing `rising_plugin-0.0.3/src/rising_plugin/phone.csv` & `rising_plugin-0.0.4/src/rising_plugin/phone.csv`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.3/src/rising_plugin/phone.json` & `rising_plugin-0.0.4/src/rising_plugin/phone.json`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.3/src/rising_plugin/pinecone_engine.py` & `rising_plugin-0.0.4/src/rising_plugin/pinecone_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # initialize pinecone
 import pinecone
 
-from src.rising_plugin.common.utils import (
+from common.utils import (
     PINECONE_KEY,
     PINECONE_ENV,
     PINECONE_INDEX_NAME,
     PINECONE_NAMESPACE,
 )
 
 DIMENSION = 1536
```

### Comparing `rising_plugin-0.0.3/src/rising_plugin/risingplugin.py` & `rising_plugin-0.0.4/src/rising_plugin/risingplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from langchain.chains.question_answering import load_qa_chain
 from langchain.docstore.document import Document
 import openai
 
 import replicate
 from firebase_admin import storage
 
-from src.rising_plugin.common.utils import (
+from common.utils import (
     OPENAI_API_KEY,
     FIREBASE_STORAGE_ROOT,
     COMMAND_SMS_INDEXS,
 )
 from src.rising_plugin.image_embedding import (
     query_image_text,
     get_prompt_image_with_message,
```

### Comparing `rising_plugin-0.0.3/LICENSE` & `rising_plugin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.3/pyproject.toml` & `rising_plugin-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rising_plugin"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Thomas Richardson", email="thomasr37oss@gmail.com" },
 ]
 description = "It is a plugin for Rising GPT"
 readme = "README.md"
 dependencies = [
     "langchain >= 0.0.148",
```

### Comparing `rising_plugin-0.0.3/PKG-INFO` & `rising_plugin-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rising_plugin
-Version: 0.0.3
+Version: 0.0.4
 Summary: It is a plugin for Rising GPT
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Thomas Richardson <thomasr37oss@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

