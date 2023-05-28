# Comparing `tmp/newsapi-python-client-0.2.3.tar.gz` & `tmp/newsapi-python-client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newsapi-python-client-0.2.3.tar", last modified: Sun May 28 11:02:19 2023, max compression
+gzip compressed data, was "newsapi-python-client-0.2.4.tar", last modified: Sun May 28 12:19:45 2023, max compression
```

## Comparing `newsapi-python-client-0.2.3.tar` & `newsapi-python-client-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:02:19.021592 newsapi-python-client-0.2.3/
--rw-rw-rw-   0        0        0     1086 2023-05-27 16:50:04.000000 newsapi-python-client-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     3099 2023-05-28 11:02:19.021328 newsapi-python-client-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2244 2023-05-27 16:50:04.000000 newsapi-python-client-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 11:02:19.002281 newsapi-python-client-0.2.3/newsApi/
--rw-rw-rw-   0        0        0        0 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:02:19.005253 newsapi-python-client-0.2.3/newsApi/models/
--rw-rw-rw-   0        0        0        0 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/models/__init__.py
--rw-rw-rw-   0        0        0     4344 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/models/request.py
--rw-rw-rw-   0        0        0     2240 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/models/response.py
--rw-rw-rw-   0        0        0     1438 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.3/newsApi/service.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:02:19.019283 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/
--rw-rw-rw-   0        0        0     3099 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 11:02:18.000000 newsapi-python-client-0.2.3/newsapi_python_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 11:02:19.021592 newsapi-python-client-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1323 2023-05-28 11:02:15.000000 newsapi-python-client-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:19:45.391820 newsapi-python-client-0.2.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-27 16:50:04.000000 newsapi-python-client-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2969 2023-05-28 12:19:45.390822 newsapi-python-client-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2114 2023-05-28 12:18:47.000000 newsapi-python-client-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 12:19:45.377760 newsapi-python-client-0.2.4/newsApi/
+-rw-rw-rw-   0        0        0        0 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.4/newsApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:19:45.381290 newsapi-python-client-0.2.4/newsApi/models/
+-rw-rw-rw-   0        0        0        0 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.4/newsApi/models/__init__.py
+-rw-rw-rw-   0        0        0     4344 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.4/newsApi/models/request.py
+-rw-rw-rw-   0        0        0     2240 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.4/newsApi/models/response.py
+-rw-rw-rw-   0        0        0     1438 2023-05-28 11:01:27.000000 newsapi-python-client-0.2.4/newsApi/service.py
+drwxrwxrwx   0        0        0        0 2023-05-28 12:19:45.389936 newsapi-python-client-0.2.4/newsapi_python_client.egg-info/
+-rw-rw-rw-   0        0        0     2969 2023-05-28 12:19:45.000000 newsapi-python-client-0.2.4/newsapi_python_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-28 12:19:45.000000 newsapi-python-client-0.2.4/newsapi_python_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 12:19:45.000000 newsapi-python-client-0.2.4/newsapi_python_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-28 12:19:45.000000 newsapi-python-client-0.2.4/newsapi_python_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 12:19:45.000000 newsapi-python-client-0.2.4/newsapi_python_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 12:19:45.391820 newsapi-python-client-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1323 2023-05-28 12:19:08.000000 newsapi-python-client-0.2.4/setup.py
```

### Comparing `newsapi-python-client-0.2.3/LICENSE` & `newsapi-python-client-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.3/PKG-INFO` & `newsapi-python-client-0.2.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newsapi-python-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python client to interact with News API from NewApi.org
 Home-page: https://github.com/roachseb/NewsAPI-Python-Client
 Author: Roach Sebastien
 Author-email: sebastien.r.r@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,84 +16,79 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+Based on the updated structure of your library, here's a revised README:
+
 # NewsAPI Python Client
 
 ## Description
 
-This project provides a Python client for accessing the NewsAPI. It aims to make it easier for developers to integrate news searching capabilities into their applications. Whether you are building a news aggregation service, a stock trading platform that needs financial news, or a social media app that needs to show relevant news to users, this library is for you.
+This project provides a Python client for accessing the NewsAPI. It simplifies the process of integrating news search capabilities into your applications. Whether you're building a news aggregation service, a stock trading platform that needs financial news, or a social media app that wants to display relevant news to users, this library is here to assist.
 
 ## Features
 
-- Simple and intuitive Python interface to the NewsAPI.
-- Uses the `requests` library for making HTTP requests.
-- Object-oriented models for request and response data.
+- Intuitive Python interface for NewsAPI.
+- Leverages the `requests` library for HTTP requests.
+- Employs an object-oriented model for both requests and responses.
 - Supports all parameters of the NewsAPI, including advanced search queries and filtering.
-- Built with flexibility and extensibility in mind, allowing developers to customize it according to their needs.
+- Designed for flexibility and extensibility, allowing for customization as needed.
 
 ## Installation
 
 ```bash
 pip install newsapi-python-client
 ```
 
 ## Usage
-Create a secrets.json file in the base directory of the project with the following structure:
 
-```json
-{
-    "NEWS_API_KEY": "YOUR_NEWS_API_KEY"
-}
+First, you need to initialize the `NewsAPIService` with your NewsAPI key.
+
+```python
+import os
+from newsApi.service import NewsAPIService  
+
+news_api_service = NewsAPIService(os.environ.get('NEWS_API_KEY'))
 ```
 
+Then you can use the service to make requests. Here is an example for retrieving news about finance:
+
 ```python
-from services.news_service import get_finance_news
-from models.request_model import RequestModel
+from newsApi.models.request import EverythingRequestModel
 
-request_model = RequestModel(
+request_model = EverythingRequestModel(
     q='finance',
-    searchIn='title,content',
-    sources='source1,source2',
-    domains='domain1.com,domain2.com',
-    excludeDomains='excludedomain1.com,excludedomain2.com',
-    from_param='2023-05-01T00:00:00',
-    to='2023-05-27T23:59:59',
-    language='en',
-    sortBy='popularity',
-    pageSize=100,
-    page=1
 )
 
-response_model = get_finance_news(request_model)
+response = news_api_service.everything(request_model)
 
-for article in response_model.articles:
+for article in response.articles:
     print(f"Title: {article.title}")
     print(f"URL: {article.url}")
     print("---")
 ```
 
-Note: Remember to replace placeholder values in the `RequestModel` with actual values.
+Note: Remember to replace placeholder values in the `EverythingRequestModel` with actual values.
 
 ## Requirements
 
 - Python 3.6 or later
 - `requests` package
 
 ## Future Plans
 
-- Improve error handling and validation.
-- Add more examples and use cases.
-- Create more comprehensive documentation.
+- Enhance error handling and validation.
+- Include more examples and use cases.
+- Develop comprehensive documentation.
 
 ## Contributing
 
-We welcome contributions from the community. Please refer to the CONTRIBUTING.md file for more details.
+Contributions from the community are welcome. Please refer to the CONTRIBUTING.md file for more details.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `newsapi-python-client-0.2.3/README.md` & `newsapi-python-client-0.2.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,70 @@
+Based on the updated structure of your library, here's a revised README:
+
 # NewsAPI Python Client
 
 ## Description
 
-This project provides a Python client for accessing the NewsAPI. It aims to make it easier for developers to integrate news searching capabilities into their applications. Whether you are building a news aggregation service, a stock trading platform that needs financial news, or a social media app that needs to show relevant news to users, this library is for you.
+This project provides a Python client for accessing the NewsAPI. It simplifies the process of integrating news search capabilities into your applications. Whether you're building a news aggregation service, a stock trading platform that needs financial news, or a social media app that wants to display relevant news to users, this library is here to assist.
 
 ## Features
 
-- Simple and intuitive Python interface to the NewsAPI.
-- Uses the `requests` library for making HTTP requests.
-- Object-oriented models for request and response data.
+- Intuitive Python interface for NewsAPI.
+- Leverages the `requests` library for HTTP requests.
+- Employs an object-oriented model for both requests and responses.
 - Supports all parameters of the NewsAPI, including advanced search queries and filtering.
-- Built with flexibility and extensibility in mind, allowing developers to customize it according to their needs.
+- Designed for flexibility and extensibility, allowing for customization as needed.
 
 ## Installation
 
 ```bash
 pip install newsapi-python-client
 ```
 
 ## Usage
-Create a secrets.json file in the base directory of the project with the following structure:
 
-```json
-{
-    "NEWS_API_KEY": "YOUR_NEWS_API_KEY"
-}
+First, you need to initialize the `NewsAPIService` with your NewsAPI key.
+
+```python
+import os
+from newsApi.service import NewsAPIService  
+
+news_api_service = NewsAPIService(os.environ.get('NEWS_API_KEY'))
 ```
 
+Then you can use the service to make requests. Here is an example for retrieving news about finance:
+
 ```python
-from services.news_service import get_finance_news
-from models.request_model import RequestModel
+from newsApi.models.request import EverythingRequestModel
 
-request_model = RequestModel(
+request_model = EverythingRequestModel(
     q='finance',
-    searchIn='title,content',
-    sources='source1,source2',
-    domains='domain1.com,domain2.com',
-    excludeDomains='excludedomain1.com,excludedomain2.com',
-    from_param='2023-05-01T00:00:00',
-    to='2023-05-27T23:59:59',
-    language='en',
-    sortBy='popularity',
-    pageSize=100,
-    page=1
 )
 
-response_model = get_finance_news(request_model)
+response = news_api_service.everything(request_model)
 
-for article in response_model.articles:
+for article in response.articles:
     print(f"Title: {article.title}")
     print(f"URL: {article.url}")
     print("---")
 ```
 
-Note: Remember to replace placeholder values in the `RequestModel` with actual values.
+Note: Remember to replace placeholder values in the `EverythingRequestModel` with actual values.
 
 ## Requirements
 
 - Python 3.6 or later
 - `requests` package
 
 ## Future Plans
 
-- Improve error handling and validation.
-- Add more examples and use cases.
-- Create more comprehensive documentation.
+- Enhance error handling and validation.
+- Include more examples and use cases.
+- Develop comprehensive documentation.
 
 ## Contributing
 
-We welcome contributions from the community. Please refer to the CONTRIBUTING.md file for more details.
+Contributions from the community are welcome. Please refer to the CONTRIBUTING.md file for more details.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `newsapi-python-client-0.2.3/newsApi/models/request.py` & `newsapi-python-client-0.2.4/newsApi/models/request.py`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.3/newsApi/models/response.py` & `newsapi-python-client-0.2.4/newsApi/models/response.py`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.3/newsApi/service.py` & `newsapi-python-client-0.2.4/newsApi/service.py`

 * *Files identical despite different names*

### Comparing `newsapi-python-client-0.2.3/newsapi_python_client.egg-info/PKG-INFO` & `newsapi-python-client-0.2.4/newsapi_python_client.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newsapi-python-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python client to interact with News API from NewApi.org
 Home-page: https://github.com/roachseb/NewsAPI-Python-Client
 Author: Roach Sebastien
 Author-email: sebastien.r.r@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,84 +16,79 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+Based on the updated structure of your library, here's a revised README:
+
 # NewsAPI Python Client
 
 ## Description
 
-This project provides a Python client for accessing the NewsAPI. It aims to make it easier for developers to integrate news searching capabilities into their applications. Whether you are building a news aggregation service, a stock trading platform that needs financial news, or a social media app that needs to show relevant news to users, this library is for you.
+This project provides a Python client for accessing the NewsAPI. It simplifies the process of integrating news search capabilities into your applications. Whether you're building a news aggregation service, a stock trading platform that needs financial news, or a social media app that wants to display relevant news to users, this library is here to assist.
 
 ## Features
 
-- Simple and intuitive Python interface to the NewsAPI.
-- Uses the `requests` library for making HTTP requests.
-- Object-oriented models for request and response data.
+- Intuitive Python interface for NewsAPI.
+- Leverages the `requests` library for HTTP requests.
+- Employs an object-oriented model for both requests and responses.
 - Supports all parameters of the NewsAPI, including advanced search queries and filtering.
-- Built with flexibility and extensibility in mind, allowing developers to customize it according to their needs.
+- Designed for flexibility and extensibility, allowing for customization as needed.
 
 ## Installation
 
 ```bash
 pip install newsapi-python-client
 ```
 
 ## Usage
-Create a secrets.json file in the base directory of the project with the following structure:
 
-```json
-{
-    "NEWS_API_KEY": "YOUR_NEWS_API_KEY"
-}
+First, you need to initialize the `NewsAPIService` with your NewsAPI key.
+
+```python
+import os
+from newsApi.service import NewsAPIService  
+
+news_api_service = NewsAPIService(os.environ.get('NEWS_API_KEY'))
 ```
 
+Then you can use the service to make requests. Here is an example for retrieving news about finance:
+
 ```python
-from services.news_service import get_finance_news
-from models.request_model import RequestModel
+from newsApi.models.request import EverythingRequestModel
 
-request_model = RequestModel(
+request_model = EverythingRequestModel(
     q='finance',
-    searchIn='title,content',
-    sources='source1,source2',
-    domains='domain1.com,domain2.com',
-    excludeDomains='excludedomain1.com,excludedomain2.com',
-    from_param='2023-05-01T00:00:00',
-    to='2023-05-27T23:59:59',
-    language='en',
-    sortBy='popularity',
-    pageSize=100,
-    page=1
 )
 
-response_model = get_finance_news(request_model)
+response = news_api_service.everything(request_model)
 
-for article in response_model.articles:
+for article in response.articles:
     print(f"Title: {article.title}")
     print(f"URL: {article.url}")
     print("---")
 ```
 
-Note: Remember to replace placeholder values in the `RequestModel` with actual values.
+Note: Remember to replace placeholder values in the `EverythingRequestModel` with actual values.
 
 ## Requirements
 
 - Python 3.6 or later
 - `requests` package
 
 ## Future Plans
 
-- Improve error handling and validation.
-- Add more examples and use cases.
-- Create more comprehensive documentation.
+- Enhance error handling and validation.
+- Include more examples and use cases.
+- Develop comprehensive documentation.
 
 ## Contributing
 
-We welcome contributions from the community. Please refer to the CONTRIBUTING.md file for more details.
+Contributions from the community are welcome. Please refer to the CONTRIBUTING.md file for more details.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `newsapi-python-client-0.2.3/setup.py` & `newsapi-python-client-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='newsapi-python-client',
-    version='0.2.3',
+    version='0.2.4',
     url='https://github.com/roachseb/NewsAPI-Python-Client',
     author='Roach Sebastien',
     author_email='sebastien.r.r@hotmail.com',
     packages=find_packages(exclude=['tests*']),
     install_requires=[
         'requests',
         'dataclasses;python_version<"3.7"'
```

