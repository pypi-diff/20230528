# Comparing `tmp/usellm-0.0.3.tar.gz` & `tmp/usellm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usellm-0.0.3.tar", last modified: Sat May 27 19:44:30 2023, max compression
+gzip compressed data, was "usellm-0.0.4.tar", last modified: Sun May 28 06:20:29 2023, max compression
```

## Comparing `usellm-0.0.3.tar` & `usellm-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 19:44:30.789788 usellm-0.0.3/
--rw-r--r--   0 jovian     (501) staff       (20)     1063 2023-05-10 15:34:43.000000 usellm-0.0.3/LICENSE
--rw-r--r--   0 jovian     (501) staff       (20)      172 2023-05-27 19:44:30.789639 usellm-0.0.3/PKG-INFO
--rw-r--r--   0 jovian     (501) staff       (20)     3476 2023-05-27 19:44:21.000000 usellm-0.0.3/README.md
--rw-r--r--   0 jovian     (501) staff       (20)       38 2023-05-27 19:44:30.789826 usellm-0.0.3/setup.cfg
--rw-r--r--   0 jovian     (501) staff       (20)      282 2023-05-27 19:44:21.000000 usellm-0.0.3/setup.py
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 19:44:30.788654 usellm-0.0.3/usellm/
--rw-r--r--   0 jovian     (501) staff       (20)       90 2023-05-27 17:31:49.000000 usellm-0.0.3/usellm/__init__.py
--rw-r--r--   0 jovian     (501) staff       (20)     3628 2023-05-27 19:44:21.000000 usellm-0.0.3/usellm/use_llm.py
--rw-r--r--   0 jovian     (501) staff       (20)       72 2023-05-27 17:32:05.000000 usellm-0.0.3/usellm/utils.py
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-27 19:44:30.789487 usellm-0.0.3/usellm.egg-info/
--rw-r--r--   0 jovian     (501) staff       (20)      172 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/PKG-INFO
--rw-r--r--   0 jovian     (501) staff       (20)      228 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/SOURCES.txt
--rw-r--r--   0 jovian     (501) staff       (20)        1 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/dependency_links.txt
--rw-r--r--   0 jovian     (501) staff       (20)       17 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/requires.txt
--rw-r--r--   0 jovian     (501) staff       (20)        7 2023-05-27 19:44:30.000000 usellm-0.0.3/usellm.egg-info/top_level.txt
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-28 06:20:29.374226 usellm-0.0.4/
+-rw-r--r--   0 jovian     (501) staff       (20)     1063 2023-05-10 15:34:43.000000 usellm-0.0.4/LICENSE
+-rw-r--r--   0 jovian     (501) staff       (20)      172 2023-05-28 06:20:29.374075 usellm-0.0.4/PKG-INFO
+-rw-r--r--   0 jovian     (501) staff       (20)     3476 2023-05-27 19:44:21.000000 usellm-0.0.4/README.md
+-rw-r--r--   0 jovian     (501) staff       (20)       38 2023-05-28 06:20:29.374264 usellm-0.0.4/setup.cfg
+-rw-r--r--   0 jovian     (501) staff       (20)      283 2023-05-28 06:16:44.000000 usellm-0.0.4/setup.py
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-28 06:20:29.373064 usellm-0.0.4/usellm/
+-rw-r--r--   0 jovian     (501) staff       (20)       90 2023-05-27 17:31:49.000000 usellm-0.0.4/usellm/__init__.py
+-rw-r--r--   0 jovian     (501) staff       (20)     3633 2023-05-28 06:16:38.000000 usellm-0.0.4/usellm/use_llm.py
+-rw-r--r--   0 jovian     (501) staff       (20)       72 2023-05-27 17:32:05.000000 usellm-0.0.4/usellm/utils.py
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-28 06:20:29.373906 usellm-0.0.4/usellm.egg-info/
+-rw-r--r--   0 jovian     (501) staff       (20)      172 2023-05-28 06:20:29.000000 usellm-0.0.4/usellm.egg-info/PKG-INFO
+-rw-r--r--   0 jovian     (501) staff       (20)      228 2023-05-28 06:20:29.000000 usellm-0.0.4/usellm.egg-info/SOURCES.txt
+-rw-r--r--   0 jovian     (501) staff       (20)        1 2023-05-28 06:20:29.000000 usellm-0.0.4/usellm.egg-info/dependency_links.txt
+-rw-r--r--   0 jovian     (501) staff       (20)       17 2023-05-28 06:20:29.000000 usellm-0.0.4/usellm.egg-info/requires.txt
+-rw-r--r--   0 jovian     (501) staff       (20)        7 2023-05-28 06:20:29.000000 usellm-0.0.4/usellm.egg-info/top_level.txt
```

### Comparing `usellm-0.0.3/LICENSE` & `usellm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `usellm-0.0.3/README.md` & `usellm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `usellm-0.0.3/usellm/use_llm.py` & `usellm-0.0.4/usellm/use_llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,32 +46,32 @@
 class Options:
     def __init__(
         self,
         messages: Optional[List[Message]] = [],
         stream: Optional[bool] = None,
         template: Optional[str] = None,
         inputs: Optional[dict] = None,
-        prompt:Optional[str] = None,
-        n:Optional[int] = None,
-        size:Optional[str] = None
+        prompt: Optional[str] = None,
+        n: Optional[int] = None,
+        size: Optional[str] = None
     ):
         self.messages = messages
         self.stream = stream
         self.template = template
         self.inputs = inputs
         self.prompt = prompt
         self.n = n
         self.size = size
 
 
 class UseLLM:
     def __init__(self, service_url: str):
         self.service_url = service_url
 
-    def chat(self, options: Options) -> None:
+    def chat(self, options: Options) -> Message:
         if options.stream:
             raise Exception("Streaming is not supported")
 
         data = json.dumps(
             {
                 "messages": [msg.to_dict() for msg in options.messages],
                 "stream": options.stream,
@@ -96,25 +96,23 @@
             elif "choices" not in json_response:
                 raise Exception(
                     "Unexpected response: {}".format(json_response))
             else:
                 message = json_response["choices"][0]["message"]
                 return Message(role=message["role"], content=message["content"])
 
-
-
-    def generate_image(self, options: Options) -> None:
+    def generate_image(self, options: Options) -> GenerateImageResponse:
 
         if options.prompt is None:
             raise Exception('Prompt is required')
-        
+
         no_of_images = options.n
         if no_of_images is None:
             no_of_images = 1
-        
+
         image_size = options.size
         if image_size is None:
             image_size = '256x256'
 
         data = json.dumps(
             {
                 "prompt": options.prompt,
```

