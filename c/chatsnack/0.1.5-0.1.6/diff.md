# Comparing `tmp/chatsnack-0.1.5.tar.gz` & `tmp/chatsnack-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatsnack-0.1.5.tar", max compression
+gzip compressed data, was "chatsnack-0.1.6.tar", max compression
```

## Comparing `chatsnack-0.1.5.tar` & `chatsnack-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3795 2023-04-15 22:05:43.794976 chatsnack-0.1.5/chatsnack/__init__.py
--rw-r--r--   0        0        0     8609 2023-05-13 02:00:34.040960 chatsnack-0.1.5/chatsnack/aiwrapper.py
--rw-r--r--   0        0        0     1498 2023-04-09 18:26:53.563580 chatsnack-0.1.5/chatsnack/asynchelpers.py
--rw-r--r--   0        0        0     4542 2023-05-12 21:47:45.298231 chatsnack-0.1.5/chatsnack/chat/__init__.py
--rw-r--r--   0        0        0     6844 2023-04-29 03:01:10.662761 chatsnack-0.1.5/chatsnack/chat/mixin_messages.py
--rw-r--r--   0        0        0     5326 2023-05-12 15:23:39.491102 chatsnack-0.1.5/chatsnack/chat/mixin_params.py
--rw-r--r--   0        0        0    11266 2023-05-12 23:17:34.321113 chatsnack-0.1.5/chatsnack/chat/mixin_query.py
--rw-r--r--   0        0        0     3345 2023-04-23 15:02:14.751611 chatsnack-0.1.5/chatsnack/chat/mixin_serialization.py
--rw-r--r--   0        0        0      929 2023-04-09 15:02:47.382274 chatsnack-0.1.5/chatsnack/defaults.py
--rw-r--r--   0        0        0     1306 2023-04-09 15:11:16.782131 chatsnack-0.1.5/chatsnack/fillings.py
--rw-r--r--   0        0        0       25 2023-04-09 16:04:20.190406 chatsnack-0.1.5/chatsnack/packs/__init__.py
--rw-r--r--   0        0        0    19461 2023-04-14 02:01:22.528095 chatsnack-0.1.5/chatsnack/packs/default_packs/ChatsnackHelper.yml
--rw-r--r--   0        0        0      762 2023-04-14 02:00:30.545934 chatsnack-0.1.5/chatsnack/packs/default_packs/Chester.yml
--rw-r--r--   0        0        0      811 2023-04-14 01:57:06.309659 chatsnack-0.1.5/chatsnack/packs/default_packs/Confectioner.yml
--rw-r--r--   0        0        0      889 2023-04-14 01:57:06.272212 chatsnack-0.1.5/chatsnack/packs/default_packs/Data.yml
--rw-r--r--   0        0        0      736 2023-04-14 01:57:06.293264 chatsnack-0.1.5/chatsnack/packs/default_packs/Jane.yml
--rw-r--r--   0        0        0      905 2023-04-14 01:57:06.327853 chatsnack-0.1.5/chatsnack/packs/default_packs/Jolly.yml
--rw-r--r--   0        0        0     1244 2023-04-23 18:55:56.684760 chatsnack-0.1.5/chatsnack/packs/default_packs/Summarizer.yml
--rw-r--r--   0        0        0     2877 2023-05-03 23:27:38.108990 chatsnack-0.1.5/chatsnack/packs/module_help_vendor.py
--rw-r--r--   0        0        0     4028 2023-04-20 15:50:28.683064 chatsnack-0.1.5/chatsnack/packs/snackpacks.py
--rw-r--r--   0        0        0     1229 2023-04-06 15:39:54.021402 chatsnack-0.1.5/chatsnack/txtformat.py
--rw-r--r--   0        0        0     3976 2023-04-20 00:41:01.746999 chatsnack-0.1.5/chatsnack/yamlformat.py
--rw-r--r--   0        0        0     1091 2023-04-14 18:33:08.190283 chatsnack-0.1.5/LICENSE
--rw-r--r--   0        0        0     1030 2023-05-13 02:02:04.638312 chatsnack-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     9186 2023-04-29 00:10:57.640242 chatsnack-0.1.5/README.md
--rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 chatsnack-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3795 2023-04-15 22:05:43.794976 chatsnack-0.1.6/chatsnack/__init__.py
+-rw-r--r--   0        0        0    10772 2023-05-28 00:42:51.456671 chatsnack-0.1.6/chatsnack/aiwrapper.py
+-rw-r--r--   0        0        0     1498 2023-04-09 18:26:53.563580 chatsnack-0.1.6/chatsnack/asynchelpers.py
+-rw-r--r--   0        0        0     4737 2023-05-24 19:12:12.474715 chatsnack-0.1.6/chatsnack/chat/__init__.py
+-rw-r--r--   0        0        0     6844 2023-04-29 03:01:10.662761 chatsnack-0.1.6/chatsnack/chat/mixin_messages.py
+-rw-r--r--   0        0        0     6080 2023-05-26 23:20:36.198540 chatsnack-0.1.6/chatsnack/chat/mixin_params.py
+-rw-r--r--   0        0        0    11473 2023-05-26 19:48:45.244560 chatsnack-0.1.6/chatsnack/chat/mixin_query.py
+-rw-r--r--   0        0        0     3345 2023-05-24 21:40:51.429802 chatsnack-0.1.6/chatsnack/chat/mixin_serialization.py
+-rw-r--r--   0        0        0      929 2023-04-09 15:02:47.382274 chatsnack-0.1.6/chatsnack/defaults.py
+-rw-r--r--   0        0        0     1306 2023-04-09 15:11:16.782131 chatsnack-0.1.6/chatsnack/fillings.py
+-rw-r--r--   0        0        0       25 2023-04-09 16:04:20.190406 chatsnack-0.1.6/chatsnack/packs/__init__.py
+-rw-r--r--   0        0        0    19461 2023-04-14 02:01:22.528095 chatsnack-0.1.6/chatsnack/packs/default_packs/ChatsnackHelper.yml
+-rw-r--r--   0        0        0      762 2023-04-14 02:00:30.545934 chatsnack-0.1.6/chatsnack/packs/default_packs/Chester.yml
+-rw-r--r--   0        0        0      811 2023-04-14 01:57:06.309659 chatsnack-0.1.6/chatsnack/packs/default_packs/Confectioner.yml
+-rw-r--r--   0        0        0      889 2023-04-14 01:57:06.272212 chatsnack-0.1.6/chatsnack/packs/default_packs/Data.yml
+-rw-r--r--   0        0        0      736 2023-04-14 01:57:06.293264 chatsnack-0.1.6/chatsnack/packs/default_packs/Jane.yml
+-rw-r--r--   0        0        0      905 2023-04-14 01:57:06.327853 chatsnack-0.1.6/chatsnack/packs/default_packs/Jolly.yml
+-rw-r--r--   0        0        0     1244 2023-04-23 18:55:56.684760 chatsnack-0.1.6/chatsnack/packs/default_packs/Summarizer.yml
+-rw-r--r--   0        0        0     2877 2023-05-03 23:27:38.108990 chatsnack-0.1.6/chatsnack/packs/module_help_vendor.py
+-rw-r--r--   0        0        0     4028 2023-04-20 15:50:28.683064 chatsnack-0.1.6/chatsnack/packs/snackpacks.py
+-rw-r--r--   0        0        0     1229 2023-04-06 15:39:54.021402 chatsnack-0.1.6/chatsnack/txtformat.py
+-rw-r--r--   0        0        0     3976 2023-04-20 00:41:01.746999 chatsnack-0.1.6/chatsnack/yamlformat.py
+-rw-r--r--   0        0        0     1091 2023-04-14 18:33:08.190283 chatsnack-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1030 2023-05-28 00:54:26.275409 chatsnack-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9186 2023-04-29 00:10:57.640242 chatsnack-0.1.6/README.md
+-rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 chatsnack-0.1.6/PKG-INFO
```

### Comparing `chatsnack-0.1.5/chatsnack/__init__.py` & `chatsnack-0.1.6/chatsnack/__init__.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/aiwrapper.py` & `chatsnack-0.1.6/chatsnack/aiwrapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 import json
 import time
 from loguru import logger
 from functools import wraps
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
 
+if os.getenv("OPENAI_API_BASE") is not None:
+    openai.api_base = os.getenv("OPENAI_API_BASE")
+
+if os.getenv("OPENAI_API_VERSION") is not None:
+    openai.api_version = os.getenv("OPENAI_API_VERSION")
+
+if os.getenv("OPENAI_API_TYPE") is not None:
+    # e.g. 'azure'
+    openai.api_type = os.getenv("OPENAI_API_TYPE")
+
 async def set_api_key(api_key):
     openai.api_key = api_key
 
 # decorator to retry API calls
 def retryAPI_a(exception, tries=4, delay=3, backoff=2):
     """Retry calling the decorated function using an exponential backoff.
     :param Exception exception: the exception to check. may be a tuple of
@@ -64,95 +74,124 @@
                     mdelay *= backoff
             return f(*args, **kwargs)
         return f_retry  # true decorator
     return deco_retry
 
 # openai
 @retryAPI_a(openai.error.RateLimitError, tries=3, delay=2, backoff=2)
-async def _chatcompletion(prompt, engine="gpt-3.5-turbo", max_tokens=None, temperature=0.7, top_p=1, stop=None, presence_penalty=0, frequency_penalty=0, n=1, stream=False, user=None):
+async def _chatcompletion(prompt, engine="gpt-3.5-turbo", max_tokens=None, temperature=0.7, top_p=1, stop=None, presence_penalty=0, frequency_penalty=0, n=1, stream=False, user=None, deployment=None, api_type=None, api_base=None, api_version=None, api_key_env=None):
     if user is None:
         user = "_not_set"
     # prompt will be in JSON format, let us translate it to a python list
     # if the prompt is a list already, we will just use it as is
     if isinstance(prompt, list):
         messages = prompt
     else:
         messages = json.loads(prompt)
     logger.trace("""Chat Query:
     Prompt: {0}
     Model: {2}, Max Tokens: {3}, Stop: {5}, Temperature: {1}, Top-P: {4}, Presence Penalty {6}, Frequency Penalty: {7}, N: {8}, Stream: {9}, User: {10}
     """,prompt, temperature, engine, max_tokens, top_p, stop, presence_penalty, frequency_penalty, n, stream, user)
+
+    additional_args = {}
+    if deployment is not None:
+        additional_args["deployment_id"] = deployment
+    if api_key_env is not None:
+        additional_args["api_key"] = os.getenv(api_key_env)           
+    if stream is None:
+        stream = False
+
     response = await openai.ChatCompletion.acreate(model=engine,
                                             messages=messages,
                                             max_tokens=max_tokens,
                                             temperature=temperature,
                                             top_p=top_p,
                                             presence_penalty=presence_penalty,
                                             frequency_penalty=frequency_penalty,
                                             stop=stop,
                                             n=n,
                                             stream=stream,
-                                            user=user)
+                                            user=user,
+                                            # NOTE: It's not documented, but the openai library allows you 
+                                            #       to pass these api_ parameters rather than depending on
+                                            #       the environment variables
+                                            api_type=api_type, api_base=api_base, api_version=api_version, 
+                                            **additional_args)
     logger.trace("OpenAI Completion Result: {0}".format(response))
     return response
 
 @retryAPI(openai.error.RateLimitError, tries=3, delay=2, backoff=2)
-def _chatcompletion_s(prompt, engine="gpt-3.5-turbo", max_tokens=None, temperature=0.7, top_p=1, stop=None, presence_penalty=0, frequency_penalty=0, n=1, stream=False, user=None):
+def _chatcompletion_s(prompt, engine="gpt-3.5-turbo", max_tokens=None, temperature=0.7, top_p=1, stop=None, presence_penalty=0, frequency_penalty=0, n=1, stream=False, user=None, deployment=None, api_type=None, api_base=None, api_version=None, api_key_env=None):
     if user is None:
         user = "_not_set"
     # prompt will be in JSON format, let us translate it to a python list
     # if the prompt is a list already, we will just use it as is
     if isinstance(prompt, list):
         messages = prompt
     else:
         messages = json.loads(prompt)
-    logger.trace("""Chat Query:
+    logger.debug("""Chat Query:
     Prompt: {0}
     Model: {2}, Max Tokens: {3}, Stop: {5}, Temperature: {1}, Top-P: {4}, Presence Penalty {6}, Frequency Penalty: {7}, N: {8}, Stream: {9}, User: {10}
     """,prompt, temperature, engine, max_tokens, top_p, stop, presence_penalty, frequency_penalty, n, stream, user)
+    additional_args = {}
+    if deployment is not None:
+        additional_args["deployment_id"] = deployment
+    if api_key_env is not None:
+        additional_args["api_key"] = os.getenv(api_key_env)   
+    if stream is None:
+        stream = False
     response = openai.ChatCompletion.create(model=engine,
                                             messages=messages,
                                             max_tokens=max_tokens,
                                             temperature=temperature,
                                             top_p=top_p,
                                             presence_penalty=presence_penalty,
                                             frequency_penalty=frequency_penalty,
                                             stop=stop,
                                             n=n,
                                             stream=stream,
-                                            user=user)
+                                            user=user, 
+                                            # NOTE: It's not documented, but the openai library allows you 
+                                            #       to pass these api_ parameters rather than depending on
+                                            #       the environment variables
+                                            api_type=api_type, api_base=api_base, api_version=api_version, 
+                                            **additional_args)
+    # revert them back to what they were
     logger.trace("OpenAI Completion Result: {0}".format(response))
     return response
 
 def _trimmed_fetch_chat_response(resp, n):
     if n == 1:
         return resp.choices[0].message.content.strip()
     else:
         logger.trace('_trimmed_fetch_response :: returning {0} responses from ChatGPT'.format(n))
         texts = []
         for idx in range(0, n):
             texts.append(resp.choices[idx].message.content.strip())
         return texts
 
 # ChatGPT
-async def cleaned_chat_completion(prompt, engine="gpt-3.5-turbo", max_tokens=None, temperature=0.7, top_p=1, stop=None, presence_penalty=0, frequency_penalty=0, n=1, stream=False, user=None, **ignored):
+async def cleaned_chat_completion(prompt, engine="gpt-3.5-turbo", max_tokens=None, temperature=0.7, top_p=1, stop=None, presence_penalty=0, frequency_penalty=0, n=1, stream=False, user=None, **additional_args):
     '''
     Wrapper for OpenAI API chat completion. Returns whitespace trimmed result from ChatGPT.
     '''
+    # ignore any additional_args which are None
+    additional_args = {k: v for k, v in additional_args.items() if v is not None}
     resp = await _chatcompletion(prompt,
                             engine=engine,
                             max_tokens=max_tokens,
                             temperature=temperature,
                             top_p=top_p,
                             presence_penalty=presence_penalty,
                             frequency_penalty=frequency_penalty,
                             stop=stop,
                             n=n,
                             stream=stream,
-                            user=user)
+                            user=user, **additional_args)
 
     return _trimmed_fetch_chat_response(resp, n)
 
 # TODO: Add back support for content classification (i.e. is this text NSFW?)
 # TODO: Consider adding support for other local language models
 
 # Structure of this code is based on some methods from github.com/OthersideAI/chronology
```

### Comparing `chatsnack-0.1.5/chatsnack/asynchelpers.py` & `chatsnack-0.1.6/chatsnack/asynchelpers.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/chat/__init__.py` & `chatsnack-0.1.6/chatsnack/chat/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                         if we get two args, the first is the name and the second is the system message
 
         :param kwargs: (keyword arguments are as follows)
         :param name: the name of the chat prompt (optional, defaults to _ChatPrompt-<date>-<uuid>)
         :param params: the engine parameters (optional, defaults to None)
         :param messages: the messages (optional, defaults to [])
         :param system: the initial system message (optional, defaults to None)
+        :param engine: the engine name (optional, defaults to None, will overwrite params if specified)
         """
 
         # get name from kwargs, if it's there
         if "name" in kwargs:
             self.name = kwargs["name"]
         else:
             # if we get two args, the first is the name and the second is the system message
@@ -68,14 +69,17 @@
         
         if "messages" in kwargs:
             self.messages = kwargs["messages"]
         else:
             # get the default from the dataclass fields and use that
             self.messages = self.__dataclass_fields__["messages"].default_factory()
 
+        if "engine" in kwargs:
+            self.engine = kwargs["engine"]
+            
         if "system" in kwargs:
             self.system_message = kwargs["system"]
         else:
             if len(args) == 1:
                 # if we only get one args, we'll assume it's the system message
                 self.system_message = args[0]
             elif len(args) == 2:
```

### Comparing `chatsnack-0.1.5/chatsnack/chat/mixin_messages.py` & `chatsnack-0.1.6/chatsnack/chat/mixin_messages.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/chat/mixin_params.py` & `chatsnack-0.1.6/chatsnack/chat/mixin_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,23 +15,34 @@
     top_p: Optional[float] = None  #: Controls the proportion of tokens considered for response generation. A value of 1.0 considers all tokens, lower values (e.g., 0.9) restrict the token set.
     n: Optional[int] = None  #: Number of responses to generate for each prompt.
     stream: Optional[bool] = None  #: If True, responses are streamed as they are generated. (not implemented yet)
     stop: Optional[List[str]] = None  #: List of strings that, if encountered, stop the generation of a response.
     max_tokens: Optional[int] = None  #: Maximum number of tokens allowed in a generated response.
     presence_penalty: Optional[float] = None  #: Penalty applied to tokens based on presence in the input.
     frequency_penalty: Optional[float] = None  #: Penalty applied to tokens based on their frequency in the response.
+
+    # Azure-specific parameters
+    deployment: Optional[str] = None  #: The deployment ID to use for this request (e.g. for Azure)
+    api_type: Optional[str] = None  #: The API type to use for this request (e.g. 'azure' or 'azure_ad')
+    api_base: Optional[str] = None  #: The base URL to use for this request (e.g. for Azure)
+    api_version: Optional[str] = None  #: The API version to use for this request (e.g. for Azure)
+    api_key_env: Optional[str] = None  #: The environment variable name to use for the API key (e.g. for Azure)
+    
     response_pattern: Optional[str] = None # regex pattern to capture subset of response to return (ignore the rest)
 
     def _get_non_none_params(self):
-        """ Returns a dictionary of non-None parameters """
+        """ Returns a dictionary of non-None parameters for the OpenAI API"""
         # get a list of dataclass fields
         fields = [field.name for field in self.__dataclass_fields__.values()]
         out = {field: getattr(self, field) for field in fields if getattr(self, field) is not None}
         if "engine" not in out or len(out["engine"]) < 2:
             out["engine"] = "gpt-3.5-turbo"
+        # TODO response_pattern maybe should live elsewhere but for now just exclude it for the API
+        if "response_pattern" in out:
+            del out["response_pattern"]
         return out
 
 
 # Define the Chat Configuration mixin
 class ChatParamsMixin:
     # make an engine property that allows set/get
     @property
```

### Comparing `chatsnack-0.1.5/chatsnack/chat/mixin_query.py` & `chatsnack-0.1.6/chatsnack/chat/mixin_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,21 @@
                     last_assistant_message = message["assistant"]
             # filter the response if we have a pattern
             last_assistant_message = self.filter_by_pattern(last_assistant_message)
         else:
             last_assistant_message = self._response_so_far
         return last_assistant_message
 
+    def __str__(self):
+        """ Returns the most recent response from the chat prompt ⭐"""
+        if self.response is None:
+            return ""
+        else:
+            return self.response
+
     def __call__(self, usermsg=None, **additional_vars) -> object:
         """ Executes the query as-is and returns a Chat object with the response, shortcut for Chat.chat()"""
         if usermsg is not None:
             additional_vars["__user"] = usermsg
         return self.chat(**additional_vars)
  
     def ask(self, usermsg=None, **additional_vars) -> str:
```

### Comparing `chatsnack-0.1.5/chatsnack/chat/mixin_serialization.py` & `chatsnack-0.1.6/chatsnack/chat/mixin_serialization.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/defaults.py` & `chatsnack-0.1.6/chatsnack/defaults.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/fillings.py` & `chatsnack-0.1.6/chatsnack/fillings.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/default_packs/ChatsnackHelper.yml` & `chatsnack-0.1.6/chatsnack/packs/default_packs/ChatsnackHelper.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/default_packs/Chester.yml` & `chatsnack-0.1.6/chatsnack/packs/default_packs/Chester.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/default_packs/Confectioner.yml` & `chatsnack-0.1.6/chatsnack/packs/default_packs/Confectioner.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/default_packs/Data.yml` & `chatsnack-0.1.6/chatsnack/packs/default_packs/Data.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/default_packs/Jane.yml` & `chatsnack-0.1.6/chatsnack/packs/default_packs/Jane.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/default_packs/Jolly.yml` & `chatsnack-0.1.6/chatsnack/packs/default_packs/Jolly.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/default_packs/Summarizer.yml` & `chatsnack-0.1.6/chatsnack/packs/default_packs/Summarizer.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/module_help_vendor.py` & `chatsnack-0.1.6/chatsnack/packs/module_help_vendor.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/packs/snackpacks.py` & `chatsnack-0.1.6/chatsnack/packs/snackpacks.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/txtformat.py` & `chatsnack-0.1.6/chatsnack/txtformat.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/chatsnack/yamlformat.py` & `chatsnack-0.1.6/chatsnack/yamlformat.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/LICENSE` & `chatsnack-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/pyproject.toml` & `chatsnack-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "chatsnack"
-version = "0.1.5"
+version = "0.1.6"
 description = "chatsnack is the easiest Python library for rapid development with OpenAI's ChatGPT API. It provides an intuitive interface for creating and managing chat-based prompts and responses, making it convenient to build complex, interactive conversations with AI."
 authors = ["Mattie Casper"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 datafiles = "^2.0"
 python-dotenv = "^1.0.0"
 loguru = "^0.6.0"
 nest-asyncio = "^1.5.6"
-openai = "^0.27.2"
+openai = "^0.27.6"
 Flask = {version = "^2.1", optional = true}
 questionary = {version = "^1.10.0", optional = true}
 rich = {version = "^13.3.2", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 pytest-asyncio = "^0.21.0"
```

### Comparing `chatsnack-0.1.5/README.md` & `chatsnack-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.5/PKG-INFO` & `chatsnack-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatsnack
-Version: 0.1.5
+Version: 0.1.6
 Summary: chatsnack is the easiest Python library for rapid development with OpenAI's ChatGPT API. It provides an intuitive interface for creating and managing chat-based prompts and responses, making it convenient to build complex, interactive conversations with AI.
 License: MIT
 Author: Mattie Casper
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Provides-Extra: flask
 Provides-Extra: questionary
 Provides-Extra: rich
 Requires-Dist: Flask (>=2.1,<3.0) ; extra == "flask" or extra == "examples"
 Requires-Dist: datafiles (>=2.0,<3.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
-Requires-Dist: openai (>=0.27.2,<0.28.0)
+Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0) ; extra == "questionary" or extra == "examples"
 Requires-Dist: rich (>=13.3.2,<14.0.0) ; extra == "rich" or extra == "examples"
 Description-Content-Type: text/markdown
 
 # chatsnack
```

