# Comparing `tmp/phasellm-0.0.6.tar.gz` & `tmp/phasellm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasellm-0.0.6.tar", last modified: Mon May  8 17:55:53 2023, max compression
+gzip compressed data, was "phasellm-0.0.7.tar", last modified: Sun May 28 04:11:42 2023, max compression
```

## Comparing `phasellm-0.0.6.tar` & `phasellm-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 17:55:53.150623 phasellm-0.0.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-05-08 17:39:29.000000 phasellm-0.0.6/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-05-08 17:55:53.150623 phasellm-0.0.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-05-08 17:39:29.000000 phasellm-0.0.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 17:55:53.150623 phasellm-0.0.6/phasellm/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      653 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5152 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/agents.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4802 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/eval.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3015 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16699 2023-05-08 17:39:29.000000 phasellm-0.0.6/phasellm/llms.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 17:55:53.150623 phasellm-0.0.6/phasellm.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      126 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-08 17:55:53.000000 phasellm-0.0.6/phasellm.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-08 17:55:53.150623 phasellm-0.0.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1167 2023-05-08 17:39:29.000000 phasellm-0.0.6/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-28 04:11:42.374458 phasellm-0.0.7/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1083 2023-05-23 17:50:05.000000 phasellm-0.0.7/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-05-28 04:11:42.374458 phasellm-0.0.7/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4999 2023-05-23 17:50:05.000000 phasellm-0.0.7/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-28 04:11:42.374458 phasellm-0.0.7/phasellm/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      653 2023-05-23 17:50:05.000000 phasellm-0.0.7/phasellm/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5152 2023-05-23 17:50:05.000000 phasellm-0.0.7/phasellm/agents.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4802 2023-05-23 17:50:05.000000 phasellm-0.0.7/phasellm/eval.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4372 2023-05-23 17:50:05.000000 phasellm-0.0.7/phasellm/exceptions.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    17411 2023-05-28 02:53:32.000000 phasellm-0.0.7/phasellm/llms.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-28 04:11:42.374458 phasellm-0.0.7/phasellm.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      739 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      282 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      126 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        9 2023-05-28 04:11:42.000000 phasellm-0.0.7/phasellm.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       38 2023-05-28 04:11:42.374458 phasellm-0.0.7/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1167 2023-05-28 02:47:44.000000 phasellm-0.0.7/setup.py
```

### Comparing `phasellm-0.0.6/LICENSE` & `phasellm-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.6/PKG-INFO` & `phasellm-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.6
+Version: 0.0.7
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.6/README.md` & `phasellm-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,18 +48,18 @@
 anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
 cohere_api_key = os.getenv("COHERE_API_KEY")
 ```
 
 We're going to set up the *Evaluator*, which takes two LLM model outputs and decides which one is better for the objective at hand.
 
 ```python
-from phasellm.eval import GPT35Evaluator
+from phasellm.eval import GPTEvaluator
 
-# We'll use GPT-3.5 as the evaluator.
-e = GPT35Evaluator(openai_api_key)
+# We'll use GPT-3.5 as the evaluator (default for GPTEvaluator).
+e = GPTEvaluator(openai_api_key)
 ```
 
 Now it's time to set up the experiment. In this case, we'll set up an `objective` which describes what we're trying to achieve with our chatbot. We'll also provide 5 examples of starting chats that we've seen with our users.
 
 ```python
 # Our objective.
 objective = "We're building a chatbot to discuss a user's travel preferences and provide advice."
```

### Comparing `phasellm-0.0.6/phasellm/__init__.py` & `phasellm-0.0.7/phasellm/__init__.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.6/phasellm/agents.py` & `phasellm-0.0.7/phasellm/agents.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.6/phasellm/eval.py` & `phasellm-0.0.7/phasellm/eval.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.6/phasellm/llms.py` & `phasellm-0.0.7/phasellm/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     def __init__(self, apikey, model="claude-v1"):
         self.apikey = apikey
         self.model = model
 
     def __repr__(self):
         return f"ClaudeWrapper(model={self.model})"
     
-    def complete_chat(self, messages, append_role=None):
+    def complete_chat(self, messages, append_role="Assistant:"):
         """
         Completes chat with Claude. Since Claude doesn't support a chat interface via API, we mimick the chat via the a prompt.
         """
 
         r_headers = {"X-API-Key":self.apikey, "Accept":"application/json"}
 
         prompt_text = _clean_messages_to_prompt(messages)
@@ -476,14 +476,29 @@
 
     def _append_message(self, role, message):
         """
         Saves a message to the chatbot's message queue.
         """
         self.messages.append({"role":role, "content":message})
 
+    def resend(self):
+        """
+        If the last message in the messages stack (i.e. array of role and content pairs) is from the user, it will resend the message and return the response. It's similar to erasing the last message in the stack and resending the last user message to the chat model.
+
+        This is useful if a model has errored out or if you are building a broader messages stack outside of the actual chatbot.
+        """
+
+        last_message = self.messages.pop()
+        if last_message['role'] == 'user':
+            response = self.chat(last_message['content'])
+            return response
+        else:
+            self.messages.append(last_message)
+            return None 
+
     def chat(self, message):
         """
         Chats with the chatbot.
         """
         self._append_message('user', message)
         response = self.llm.complete_chat(self.messages, "assistant")
         self._append_message('assistant', response)
```

### Comparing `phasellm-0.0.6/phasellm.egg-info/PKG-INFO` & `phasellm-0.0.7/phasellm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.6
+Version: 0.0.7
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
```

### Comparing `phasellm-0.0.6/setup.py` & `phasellm-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 DESCRIPTION = "Wrappers for common large langugae models (LLMs) with support for evaluation."
 
 LONG_DESCRIPTION = "PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use."
 
 setup(
     name="phasellm",
```

