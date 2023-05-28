# Comparing `tmp/newsapi-python-client-0.2.2.tar.gz` & `tmp/newsapi-python-client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newsapi-python-client-0.2.2.tar", last modified: Sat May 27 10:38:28 2023, max compression
+gzip compressed data, was "newsapi-python-client-0.2.3.tar", last modified: Sun May 28 11:02:19 2023, max compression
```

## Comparing `newsapi-python-client-0.2.2.tar` & `newsapi-python-client-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:38:28.029616 newsapi-python-client-0.2.2/
--rw-rw-rw-   0        0        0     1086 2023-05-27 09:04:11.000000 newsapi-python-client-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     3099 2023-05-27 10:38:28.029616 newsapi-python-client-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2244 2023-05-27 10:37:45.000000 newsapi-python-client-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 10:38:28.013615 newsapi-python-client-0.2.2/models/
--rw-rw-rw-   0        0        0        0 2023-05-27 09:05:25.000000 newsapi-python-client-0.2.2/models/__init__.py
--rw-rw-rw-   0        0        0     1580 2023-05-27 09:32:29.000000 newsapi-python-client-0.2.2/models/request_model.py
--rw-rw-rw-   0        0        0     1699 2023-05-27 09:31:28.000000 newsapi-python-client-0.2.2/models/response_model.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:38:28.025617 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/
--rw-rw-rw-   0        0        0     3099 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-27 10:38:27.000000 newsapi-python-client-0.2.2/newsapi_python_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 10:38:28.027615 newsapi-python-client-0.2.2/services/
--rw-rw-rw-   0        0        0        0 2023-05-27 09:13:02.000000 newsapi-python-client-0.2.2/services/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-05-27 09:30:02.000000 newsapi-python-client-0.2.2/services/news_service.py
--rw-rw-rw-   0        0        0       42 2023-05-27 10:38:28.029616 newsapi-python-client-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1323 2023-05-27 10:38:22.000000 newsapi-python-client-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:02:19.021592 newsapi-python-client-0.2.3/
+-rw-rw-rw-   0        0        0     1086 2023-05-27 16:50:04.000000 newsapi-python-client-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3099 2023-05-28 11:02:19.021328 newsapi-python-client-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2244 2023-05-27 16:50:04.000000 newsapi-python-client-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 11:02:19.002281 newsapi-python-client-0.2.3/newsApi/
+-rw-rw-rw-   0        0        0        0 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:02:19.005253 newsapi-python-client-0.2.3/newsApi/models/
+-rw-rw-rw-   0        0        0        0 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/models/__init__.py
+-rw-rw-rw-   0        0        0     4344 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/models/request.py
+-rw-rw-rw-   0        0        0     2240 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/models/response.py
+-rw-rw-rw-   0        0        0     1438 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/service.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:02:19.019283 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/
+-rw-rw-rw-   0        0        0     3099 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 11:02:19.021592 newsapi-python-client-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1323 2023-05-28 11:02:15.000000 newsapi-python-client-0.2.3/setup.py
```

### Comparing `newsapi-python-client-0.2.2/LICENSE` & `newsapi-python-client-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.2/PKG-INFO` & `newsapi-python-client-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newsapi-python-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python client to interact with News API from NewApi.org
 Home-page: https://github.com/roachseb/NewsAPI-Python-Client
 Author: Roach Sebastien
 Author-email: sebastien.r.r@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `newsapi-python-client-0.2.2/README.md` & `newsapi-python-client-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.2/models/response_model.py` & `newsapi-python-client-0.2.3/newsApi/models/response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,84 @@
-from dataclasses import dataclass
 from typing import List, Optional
+import dataclasses
 
-@dataclass
+
+@dataclasses.dataclass
 class Source:
-    id: Optional[str]
+    id: str
     name: str
 
-    @classmethod
-    def from_dict(cls, data: dict) -> 'Source':
-        return cls(id=data.get('id'), name=data['name'])
 
-@dataclass
+@dataclasses.dataclass
 class Article:
     source: Source
     author: Optional[str]
     title: str
     description: Optional[str]
     url: str
     urlToImage: Optional[str]
     publishedAt: str
     content: Optional[str]
 
     @classmethod
-    def from_dict(cls, data: dict) -> 'Article':
-        source = Source.from_dict(data['source'])
+    def from_dict(cls, data: dict) -> "Article":
         return cls(
-            source=source,
-            author=data.get('author'),
-            title=data['title'],
-            description=data.get('description'),
-            url=data['url'],
-            urlToImage=data.get('urlToImage'),
-            publishedAt=data['publishedAt'],
-            content=data.get('content')
+            source=Source(**data.get("source", {})),
+            author=data.get("author"),
+            title=data.get("title"),
+            description=data.get("description"),
+            url=data.get("url"),
+            urlToImage=data.get("urlToImage"),
+            publishedAt=data.get("publishedAt"),
+            content=data.get("content"),
         )
 
 
-@dataclass
-class ResponseModel:
-    """
-    A data class that represents the response from News API.
+@dataclasses.dataclass
+class TopHeadlinesResponseModel:
+    status: str
+    totalResults: int
+    articles: List[Article]
+
+    @classmethod
+    def from_dict(cls, data: dict) -> "TopHeadlinesResponseModel":
+        articles = [Article.from_dict(article) for article in data.get("articles", [])]
+        return cls(
+            status=data.get("status", ""),
+            totalResults=data.get("totalResults", 0),
+            articles=articles,
+        )
+
 
-    Attributes:
-        - status (str): If the request was successful or not. Options: ok, error.
-        - totalResults (int): The total number of results available for your request.
-        - articles (List[Article]): The results of the request.
-    """
+@dataclasses.dataclass
+class ResponseModel:
     status: str
+
+    @classmethod
+    def from_dict(cls, data: dict) -> "ResponseModel":
+        raise NotImplementedError()
+
+
+@dataclasses.dataclass
+class EverythingResponseModel(ResponseModel):
     totalResults: int
     articles: List[Article]
 
     @classmethod
-    def from_dict(cls, data: dict) -> 'ResponseModel':
-        articles = [Article.from_dict(article) for article in data['articles']]
+    def from_dict(cls, data: dict) -> "EverythingResponseModel":
+        articles = [Article.from_dict(article) for article in data["articles"]]
+        return cls(
+            status=data["status"], totalResults=data["totalResults"], articles=articles
+        )
+
+
+@dataclasses.dataclass
+class SourcesResponseModel(ResponseModel):
+    sources: List[Source]
+
+    @classmethod
+    def from_dict(cls, data: dict) -> "SourcesResponseModel":
+        sources = [Source(**source) for source in data.get("sources", [])]
         return cls(
-            status=data['status'],
-            totalResults=data['totalResults'],
-            articles=articles
+            status=data["status"],
+            sources=sources,
         )
```

### Comparing `newsapi-python-client-0.2.2/newsapi_python_client.egg-info/PKG-INFO` & `newsapi-python-client-0.2.3/newsapi_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newsapi-python-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python client to interact with News API from NewApi.org
 Home-page: https://github.com/roachseb/NewsAPI-Python-Client
 Author: Roach Sebastien
 Author-email: sebastien.r.r@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `newsapi-python-client-0.2.2/setup.py` & `newsapi-python-client-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='newsapi-python-client',
-    version='0.2.2',
+    version='0.2.3',
     url='https://github.com/roachseb/NewsAPI-Python-Client',
     author='Roach Sebastien',
     author_email='sebastien.r.r@hotmail.com',
     packages=find_packages(exclude=['tests*']),
     install_requires=[
         'requests',
         'dataclasses;python_version<"3.7"'
```

