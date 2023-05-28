# Comparing `tmp/talk_codebase-0.1.17.tar.gz` & `tmp/talk_codebase-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.17.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.18.tar", max compression
```

## Comparing `talk_codebase-0.1.17.tar` & `talk_codebase-0.1.18.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1236 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/README.md
--rw-r--r--   0        0        0      811 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1960 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/consts.py
--rw-r--r--   0        0        0     2318 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/llm.py
--rw-r--r--   0        0        0     1947 2023-05-27 14:30:36.778215 talk_codebase-0.1.17/talk_codebase/utils.py
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 talk_codebase-0.1.17/PKG-INFO
+-rw-r--r--   0        0        0     1236 2023-05-28 20:47:11.082286 talk_codebase-0.1.18/README.md
+-rw-r--r--   0        0        0      811 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1972 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2301 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1947 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 talk_codebase-0.1.18/PKG-INFO
```

### Comparing `talk_codebase-0.1.17/README.md` & `talk_codebase-0.1.18/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.17/pyproject.toml` & `talk_codebase-0.1.18/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.17"
+version = "0.1.18"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.17/talk_codebase/cli.py` & `talk_codebase-0.1.18/talk_codebase/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     try:
         config = get_config()
         api_key = config.get("api_key")
         model_name = config.get("model_name")
         if not (api_key and model_name):
             configure()
             chat(root_dir)
-        vector_store = create_vector_store(root_dir, api_key)
+        vector_store = create_vector_store(root_dir, api_key, model_name)
         loop(vector_store, api_key, model_name)
     except KeyboardInterrupt:
         print("\n🤖 Bye!")
     except Exception as e:
         if str(e) == "<empty message>":
             print("🤖 Please configure your API key.")
             configure()
```

### Comparing `talk_codebase-0.1.17/talk_codebase/consts.py` & `talk_codebase-0.1.18/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.17/talk_codebase/llm.py` & `talk_codebase-0.1.18/talk_codebase/llm.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,33 +9,32 @@
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.text_splitter import CharacterTextSplitter
 
 from talk_codebase.utils import StreamStdOut, load_files
 
 
-def calculate_cost(texts):
-    enc = tiktoken.get_encoding("cl100k_base")
+def calculate_cost(texts, model_name):
+    enc = tiktoken.encoding_for_model(model_name)
     all_text = ''.join([text.page_content for text in texts])
     tokens = enc.encode(all_text)
     token_count = len(tokens)
-    rate_per_thousand_tokens = 0.0004
-    cost = (token_count / 1000) * rate_per_thousand_tokens
+    cost = (token_count / 1000) * 0.0004
     return cost
 
 
-def create_vector_store(root_dir, openai_api_key):
+def create_vector_store(root_dir, openai_api_key, model_name):
     docs = load_files(root_dir)
     if len(docs) == 0:
         print("✘ No documents found")
         exit(0)
     text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
     texts = text_splitter.split_documents(docs)
 
-    cost = calculate_cost(docs)
+    cost = calculate_cost(docs, model_name)
     approve = questionary.select(
         f"Creating a vector store for {len(docs)} documents will cost ~${cost:.5f}. Do you want to continue?",
         choices=[
             {"name": "Yes", "value": True},
             {"name": "No", "value": False},
         ]
     ).ask()
```

### Comparing `talk_codebase-0.1.17/talk_codebase/utils.py` & `talk_codebase-0.1.18/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.17/PKG-INFO` & `talk_codebase-0.1.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.17
+Version: 0.1.18
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

