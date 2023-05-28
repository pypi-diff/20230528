# Comparing `tmp/rising_plugin-0.0.2.tar.gz` & `tmp/rising_plugin-0.0.3.tar.gz`

## Comparing `rising_plugin-0.0.2.tar` & `rising_plugin-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/src/rising_plugin/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/src/rising_plugin/csv_embed.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/src/rising_plugin/image_embedding.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/src/rising_plugin/phone.csv
--rw-r--r--   0        0        0   283637 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/src/rising_plugin/phone.json
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/src/rising_plugin/pinecone_engine.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/src/rising_plugin/risingplugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/README.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 rising_plugin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/RisingPlugin.iml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/__init__.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/csv_embed.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/image_embedding.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/phone.csv
+-rw-r--r--   0        0        0   283637 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/phone.json
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/pinecone_engine.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/risingplugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/common/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/src/rising_plugin/common/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/LICENSE
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 rising_plugin-0.0.3/PKG-INFO
```

### Comparing `rising_plugin-0.0.2/src/rising_plugin/csv_embed.py` & `rising_plugin-0.0.3/src/rising_plugin/csv_embed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 
 from langchain.document_loaders.csv_loader import CSVLoader
 from langchain.embeddings.openai import OpenAIEmbeddings
 import json
 
-OPENAI_API_KEY = os.environ["OPENAI_API_KEY"]
+from src.rising_plugin.common.utils import OPENAI_API_KEY
 
 
 def csv_embed():
-    loader = CSVLoader(file_path="src/langchain/phone.csv", encoding="utf8")
+    loader = CSVLoader(file_path="src/langchain_plugin/phone.csv", encoding="utf8")
     data = loader.load()
     embeddings = OpenAIEmbeddings(openai_api_key=OPENAI_API_KEY)
 
     result = list()
     for t in data:
         query_result = embeddings.embed_query(t.page_content)
         result.append(query_result)
-    with open("src/langchain/phone.json", "w") as outfile:
+    with open("src/langchain_plugin/phone.json", "w") as outfile:
         json.dump(result, outfile, indent=2)
 
 
 if __name__ == "__main__":
     csv_embed()
```

### Comparing `rising_plugin-0.0.2/src/rising_plugin/image_embedding.py` & `rising_plugin-0.0.3/src/rising_plugin/image_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from langchain.embeddings.openai import OpenAIEmbeddings
 
-from src.common.utils import OPENAI_API_KEY, PINECONE_NAMESPACE, PINECONE_INDEX_NAME
-from src.langchain.pinecone_engine import (
+from src.rising_plugin.common.utils import OPENAI_API_KEY, PINECONE_NAMESPACE, PINECONE_INDEX_NAME
+from src.rising_plugin.pinecone_engine import (
     init_pinecone,
     get_pinecone_index_namespace,
 )
 
 
 def get_embeddings():
     return OpenAIEmbeddings(openai_api_key=OPENAI_API_KEY)
```

### Comparing `rising_plugin-0.0.2/src/rising_plugin/phone.csv` & `rising_plugin-0.0.3/src/rising_plugin/phone.csv`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.2/src/rising_plugin/phone.json` & `rising_plugin-0.0.3/src/rising_plugin/phone.json`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.2/src/rising_plugin/pinecone_engine.py` & `rising_plugin-0.0.3/src/rising_plugin/pinecone_engine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # initialize pinecone
 import pinecone
 
-from src.common.utils import (
+from src.rising_plugin.common.utils import (
     PINECONE_KEY,
     PINECONE_ENV,
     PINECONE_INDEX_NAME,
     PINECONE_NAMESPACE,
 )
 
 DIMENSION = 1536
```

### Comparing `rising_plugin-0.0.2/src/rising_plugin/risingplugin.py` & `rising_plugin-0.0.3/src/rising_plugin/risingplugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,30 +10,26 @@
 from langchain.chains.question_answering import load_qa_chain
 from langchain.docstore.document import Document
 import openai
 
 import replicate
 from firebase_admin import storage
 
-from src.common.utils import (
+from src.rising_plugin.common.utils import (
     OPENAI_API_KEY,
     FIREBASE_STORAGE_ROOT,
-    GPT_MODEL,
     COMMAND_SMS_INDEXS,
 )
-from src.langchain.image_embedding import (
+from src.rising_plugin.image_embedding import (
     query_image_text,
     get_prompt_image_with_message,
 )
-from src.model.chat_response_model import ChatResponseModel
-from src.service.llm.base import Message
 
-
-def getCompletion(query, uuid="", image_search=True):
-    llm = ChatOpenAI(model_name=GPT_MODEL, temperature=0, openai_api_key=OPENAI_API_KEY)
+def getCompletion(query, model="gpt-3.5-turbo", uuid="", image_search=True,):
+    llm = ChatOpenAI(model_name=model, temperature=0, openai_api_key=OPENAI_API_KEY)
     chain = load_qa_chain(llm, chain_type="stuff")
 
     with open("src/langchain/phone.json", "r") as infile:
         data = json.load(infile)
     embeddings = OpenAIEmbeddings(openai_api_key=OPENAI_API_KEY)
 
     query_result = embeddings.embed_query(query)
@@ -116,17 +112,15 @@
       'content': 'The 2020 World Series was played in Arlington, Texas at the Globe Life Field, which was the new home stadium for the Texas Rangers.'},
     'finish_reason': 'stop',
     'index': 0
    }
   ]
 }
 """
-
-
-def handle_chat_completion(messages: List[Message], model: str) -> ChatResponseModel:
+def handle_chat_completion(messages: Any, model: str) -> Any:
     openai.api_key = OPENAI_API_KEY
 
     response = openai.ChatCompletion.create(
         model=model,
         messages=messages,
     )
-    return ChatResponseModel(response)
+    return response
```

### Comparing `rising_plugin-0.0.2/LICENSE` & `rising_plugin-0.0.3/LICENSE`

 * *Files identical despite different names*

