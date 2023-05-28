# Comparing `tmp/bs4_web_scraper-0.1.1.tar.gz` & `tmp/bs4_web_scraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs4_web_scraper-0.1.1.tar", last modified: Sat May 27 19:21:37 2023, max compression
+gzip compressed data, was "bs4_web_scraper-0.1.2.tar", last modified: Sun May 28 18:50:27 2023, max compression
```

## Comparing `bs4_web_scraper-0.1.1.tar` & `bs4_web_scraper-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 19:21:37.715564 bs4_web_scraper-0.1.1/
--rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0    19379 2023-05-27 19:21:37.712561 bs4_web_scraper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    18039 2023-05-27 19:11:56.000000 bs4_web_scraper-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 19:21:37.532407 bs4_web_scraper-0.1.1/bs4_web_scraper/
--rw-rw-rw-   0        0        0     3635 2023-05-27 19:20:08.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/__init__.py
--rw-rw-rw-   0        0        0    41404 2023-05-27 13:07:58.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/base.py
--rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/exceptions.py
--rw-rw-rw-   0        0        0    12777 2023-05-23 09:26:13.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/file_handler.py
--rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/logging.py
--rw-rw-rw-   0        0        0     4858 2023-05-27 19:09:12.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/request_limiter.py
--rw-rw-rw-   0        0        0    39119 2023-05-27 19:20:26.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/scraper.py
--rw-rw-rw-   0        0        0    22737 2023-05-27 12:41:04.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/translate.py
--rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.1/bs4_web_scraper/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 19:21:37.704508 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/
--rw-rw-rw-   0        0        0    19379 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-27 19:21:37.000000 bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1731 2023-05-27 19:19:47.000000 bs4_web_scraper-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 19:21:37.715564 bs4_web_scraper-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 18:50:27.829218 bs4_web_scraper-0.1.2/
+-rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0    19798 2023-05-28 18:50:27.829218 bs4_web_scraper-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18458 2023-05-28 18:46:31.000000 bs4_web_scraper-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 18:50:27.644941 bs4_web_scraper-0.1.2/bs4_web_scraper/
+-rw-rw-rw-   0        0        0     3635 2023-05-28 18:48:55.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/__init__.py
+-rw-rw-rw-   0        0        0    41852 2023-05-28 18:29:56.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/base.py
+-rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/exceptions.py
+-rw-rw-rw-   0        0        0    12777 2023-05-23 09:26:13.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/file_handler.py
+-rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/logging.py
+-rw-rw-rw-   0        0        0     4858 2023-05-27 19:09:12.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/request_limiter.py
+-rw-rw-rw-   0        0        0    39596 2023-05-28 18:47:14.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/scraper.py
+-rw-rw-rw-   0        0        0    22737 2023-05-27 12:41:04.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/translate.py
+-rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:50:27.821211 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/
+-rw-rw-rw-   0        0        0    19798 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1731 2023-05-28 18:49:10.000000 bs4_web_scraper-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 18:50:27.829218 bs4_web_scraper-0.1.2/setup.cfg
```

### Comparing `bs4_web_scraper-0.1.1/LICENSE.md` & `bs4_web_scraper-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.1/PKG-INFO` & `bs4_web_scraper-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs4_web_scraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A web scraper based on the BeautifulSoup4 library and translators package.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/bs4_web_scraper
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/bs4_web_scraper/issues
 Project-URL: Repository, https://github.com/ti-oluwa/bs4_web_scraper
 Keywords: web scraper,bs4,beautifulsoup4,web scraping,web scraping with python,web scraping with bs4,web scraping with beautifulsoup4,web scraping with translation,web scraping with translation to other languages,web scraping with translation to other languages with python,web scraping with translation to other languages with bs4,web scraping with translation to other languages with beautifulsoup4,web scraping with translation to other languages with python and bs4,web scraping with translation to other languages with python and beautifulsoup4
@@ -292,37 +292,42 @@
     "https://www.example.com/download/example1.mkv",
     "https://www.example.com/download/example2.mkv",
     "https://www.example.com/download/example3.mkv",
     "https://www.example.com/download/example4.mkv",
     "https://www.example.com/download/example5.mkv",
 ]
 
-bs4_scraper.download_urls(urls=urls, save_to="downloads")
+bs4_scraper.download_urls(urls=urls, save_to="downloads", fast_download=True)
 
 ```
-The define what each file should be saved as, you can pass the `save_as` alongside the url as a dictionary - `urls` becomes a list of dictionaries, as parameter to the `download_urls` method. The following example shows how to download multiple files from a web page and save them with different names
+To define what each file should be saved as, you can pass the `save_as` alongside the url as a dictionary - `urls` becomes a list of dictionaries, as parameter to the `download_urls` method. The following example shows how to download multiple files from a web page and save them with different names
 
 ```python
 
 urls = [
     {
         "url": "https://www.example.com/download/example1.mkv",
-        "save_as": "example1.mkv"
+        "save_as": "example_1.mkv"
     },
     {
         "url": "https://www.example.com/download/example2.mkv",
-        "save_as": "example2.mkv"
+        "save_as": "example_2.mkv"
     },
     {
         "url": "https://www.example.com/download/example3.mkv",
-        "save_as": "example3.mkv"
+        "save_as": "example_3.mkv",
+        "save_to": "./downloads2/" 
+        # This will be treated as an absolute path and will not be saved in `self.base_storage_dir`. 
+        # This file will be saved in its own directory(determined by the path given).
     },
+    # You can also add a normal string url. This will we saved as 'example4.mkv' by default.
+    "https://www.example.com/download/example4.mkv", 
 ]
 
-bs4_scraper.download_urls(urls=urls, save_to="downloads")
+bs4_scraper.download_urls(urls=urls, save_to="downloads", fast_download=True)
 
 ```
 
 #### `find_urls`
 
 This method is used to get all resource related attribute(url or link) on elements that match a given tag name. This method only works for tags that have the `src` or `href` attribute. The following example shows how to find all urls on the `img` elements in a web page:
```

### Comparing `bs4_web_scraper-0.1.1/README.md` & `bs4_web_scraper-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -273,37 +273,42 @@
     "https://www.example.com/download/example1.mkv",
     "https://www.example.com/download/example2.mkv",
     "https://www.example.com/download/example3.mkv",
     "https://www.example.com/download/example4.mkv",
     "https://www.example.com/download/example5.mkv",
 ]
 
-bs4_scraper.download_urls(urls=urls, save_to="downloads")
+bs4_scraper.download_urls(urls=urls, save_to="downloads", fast_download=True)
 
 ```
-The define what each file should be saved as, you can pass the `save_as` alongside the url as a dictionary - `urls` becomes a list of dictionaries, as parameter to the `download_urls` method. The following example shows how to download multiple files from a web page and save them with different names
+To define what each file should be saved as, you can pass the `save_as` alongside the url as a dictionary - `urls` becomes a list of dictionaries, as parameter to the `download_urls` method. The following example shows how to download multiple files from a web page and save them with different names
 
 ```python
 
 urls = [
     {
         "url": "https://www.example.com/download/example1.mkv",
-        "save_as": "example1.mkv"
+        "save_as": "example_1.mkv"
     },
     {
         "url": "https://www.example.com/download/example2.mkv",
-        "save_as": "example2.mkv"
+        "save_as": "example_2.mkv"
     },
     {
         "url": "https://www.example.com/download/example3.mkv",
-        "save_as": "example3.mkv"
+        "save_as": "example_3.mkv",
+        "save_to": "./downloads2/" 
+        # This will be treated as an absolute path and will not be saved in `self.base_storage_dir`. 
+        # This file will be saved in its own directory(determined by the path given).
     },
+    # You can also add a normal string url. This will we saved as 'example4.mkv' by default.
+    "https://www.example.com/download/example4.mkv", 
 ]
 
-bs4_scraper.download_urls(urls=urls, save_to="downloads")
+bs4_scraper.download_urls(urls=urls, save_to="downloads", fast_download=True)
 
 ```
 
 #### `find_urls`
 
 This method is used to get all resource related attribute(url or link) on elements that match a given tag name. This method only works for tags that have the `src` or `href` attribute. The following example shows how to find all urls on the `img` elements in a web page:
```

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/__init__.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 __date__ = '27-05-2023'
 __author__ = 'ti-oluwa'
 __doc__ = 'A web scraper that uses BeautifulSoup4 to scrape web pages and can translate them to__ other languages.'
 __license__ = 'MIT'
 __title__ = 'bs4_web_scraper'
 __url__ = 'https://github.com/ti-oluwa/bs4_web_scraper'
 __description__ = 'A web scraper that uses BeautifulSoup4 to scrape web pages and can translates them to other languages.'
```

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/base.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 DESCRIPTION: ::
     This module contains the BS4BaseScraper class which is the base class for creating scraper subclasses.
 """
 
+from os.path import isabs
 from typing import IO, Any, Dict, List
 import requests
 import os
 import random
 import time
 import json
 import math
@@ -588,15 +589,15 @@
         try:
             if os.path.isabs(storage_path):
                 if os.path.isdir(storage_path):
                     file_path = f"{storage_path}\{filename}"
                 else:
                     file_path = storage_path   
             else:
-                file_path = f"{self.base_storage_dir}\{storage_path}\{filename}"
+                file_path = os.path.normpath(f"{self.base_storage_dir}\{storage_path}\{filename}")
                 
             file_hdl = FileHandler(file_path, encoding, exists_ok=True, allow_any=True)
 
             # Translate content if necessary
             if translate and (self.translate_to and file_hdl.filetype in ['xhtml', 'htm', 'shtml', 'html', 'xml']):
                 content = self.translator.translate_markup(content, target_lang=self.translate_to)
 
@@ -614,15 +615,16 @@
 
         Args:
         * `url_obj` (Url): Url object to be parsed.
         * `remove_str` (str): string to be removed from the path. Defaults to None.
         '''
         url_path = url_obj.path or ''
         url_path = url_path.replace(remove_str, '') if remove_str else url_path
-        return url_path.replace('/', '\\')
+        path = os.path.normpath(url_path.replace('/', '\\'))
+        return path
 
 
     def get_rra_by_tag_name(self, tag_name: str) -> str | None:
         '''
         Return the tag attribute that contains the src url/path.
 
         Returns None if tag name is not recognizable.
@@ -639,22 +641,22 @@
             src = 'href'
         return src
         
 
     def download_url(self, url: str, save_as: str | None = None, save_to: str | None = None, overwrite: bool = False,
                         check_ext: bool = True, unique_if_query_params: bool = False):
         '''
-        Download file from the given url. Saves the file in a storage path in `self.base_storage_dir`.
+        Download file from the given url. Saves the file in a storage path in `self.base_storage_dir` if `save_to` is not an absolute path.
 
         Returns the FileHandler object for the downloaded file if downloaded or already existing else None.
 
         Args::
         * url (str): Url to be downloaded.
         * save_as Optional[str]: Name of the file to be downloaded or name with which the file should be saved.
-        * save_to Optional[str]: Path to the directory where the file should be saved in `self.base_storage_dir`.
+        * save_to Optional[str]: Absolute path or path to the directory where the file should be saved in `self.base_storage_dir`.
         * overwrite (bool, optional): Whether to overwrite the file if it already exists. Defaults to False.
         * check_ext (bool, optional): Whether to check for extension in the url and use it for filename validation. Defaults to True.
         * unique_if_query_params (bool, optional): Whether to add a unique string to the filename if the url has query parameters. Defaults to False.
         
         #### NOTE::
         * If `save_as` is not provided, the filename will be extracted from the url.
         * If `save_to` is not provided, then `save_to` will automatically be the url path.
@@ -689,36 +691,42 @@
                 raise ValueError('Invalid extension! `save_as` extension does not match the extension in the url.')
             filename = f"{save_as_name}{save_as_ext}"
 
         if not filename:
             raise ValueError('`filename` seems to be empty. Please check the url "%s" or provide a `save_as` name.' % url)
 
         response = None
-        file_storage_path = save_to.replace('/', '\\').strip() if save_to is not None else save_to
-        # check if element src has query params
+        file_storage_path = save_to.replace('/', '\\').strip() if save_to else save_to
+        file_storage_path = os.path.abspath(file_storage_path) if file_storage_path and file_storage_path.startswith('.') else file_storage_path
+        # check if url has query params
         has_query_params = bool(url_obj.query)
         if file_storage_path is None:
-            file_storage_path = self.parse_storage_path_from_Url(url_obj, remove_str=f"{url_based_name}{url_based_ext}")
-            # Clean up storage path
-            file_storage_path = file_storage_path.removeprefix('\\').removesuffix('\\')        
-                
+            file_storage_path = self.parse_storage_path_from_Url(url_obj, remove_str=f"{url_based_name}{url_based_ext}")  
+            file_storage_path = file_storage_path.removeprefix('\\').removesuffix('\\')    
+   
         if has_query_params and (url_obj.query not in self.url_query_params.keys()):
             if unique_if_query_params is True:
                 filename = utils.generate_unique_filename(filename)
                 
         if has_query_params and (url_obj.query in self.url_query_params.keys()):
             file_hdl: FileHandler = self.url_query_params[url_obj.query]
             return file_hdl
-            
+
         if not has_query_params or (url_obj.query not in self.url_query_params.keys()):
+            if os.path.isabs(file_storage_path):
+                full_path = f'{file_storage_path}/{filename}'
+                os.makedirs(os.path.dirname(full_path), exist_ok=True)
+            else:
+                full_path = f'{self.base_storage_dir}\{file_storage_path}\{filename}'
+            full_path = os.path.normpath(full_path)
             # check if file already exists
-            if os.path.exists(f'{self.base_storage_dir}\{file_storage_path}\{filename}') is False:
+            if os.path.exists(full_path) is False:
                 response = self.get(url_obj.url)
             else:
-                file_hdl = FileHandler(f'{self.base_storage_dir}\{file_storage_path}\{filename}', exists_ok=True, allow_any=True)
+                file_hdl = FileHandler(full_path, exists_ok=True, allow_any=True)
                 if overwrite is True:
                     file_hdl.delete_file()
                     response = self.get(url_obj.url)
                 else:
                     return file_hdl
 
         if response:
```

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/exceptions.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/exceptions.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/file_handler.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/file_handler.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/logging.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/logging.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/request_limiter.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/request_limiter.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/scraper.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,64 +198,75 @@
             self.log(f"SCRAPING COMPLETED IN {(time_taken / 60):.2f} MINUTE{'S'[:round(time_taken / 60)^1]}\n")
         else:
             self.log(f"SCRAPING COMPLETED IN {time_taken:.2f} SECOND{'S'[:round(time_taken)^1]}\n")
 
         return None
 
     
-    def download_urls(self, urls: Iterable[Dict[str, str]], save_to: str | None = None, overwrite: bool = False,
+    def download_urls(self, urls: Iterable[Dict[str, str]] | Iterable[str], save_to: str | None = None, overwrite: bool = False,
                         check_ext: bool = True, fast_download: bool = False, unique_if_query_params: bool = False):
         '''
         Download files from the given urls using the `download_url` method. Saves the files in a storage path in `self.base_storage_dir`.
 
         Returns the storage path of the downloaded files.
 
         Args:
-            - urls (List[Dict[str, str]]): List of urls to be downloaded. The url in the list should be of type dict[str, str].
+            - urls (Iterable[Dict[str, str]] | Iterable[str]): List of urls to be downloaded. The url in the list can be of type str or dict[str, str].
             - save_to Optional[str]: Path to the directory where the file should be saved in `self.base_storage_dir`.
             - overwrite (bool, optional): Whether to overwrite existing files. Defaults to False.
             - check_ext (bool, optional): Whether to check for extension in the url and use it for filename validation. Defaults to True.
             Check the doc string of `download_url` for more info on setting this value.
             - unique_if_query_params (bool, optional): Whether to generate a unique filename if the any of the urls has query params. Defaults to False.
             - fast_download (bool, optional): Whether to download the urls in parallel. Defaults to False. 
             If the number or urls exceed 200 then fast download wont be used to avoid sending high frequency requests to the server.
 
         #### Example Usage: ::
             >>> urls = [
-                    {'url': 'https://www.example.com/', 'save_as': 'site.html'},
-                    {'url': 'https://www.example.com/image2.jpg', 'save_as': ''},
-                    {'url': 'https://www.example.com/image3.jpg', 'save_as': 'image3.jpg'},
+                    {
+                        'url': 'https://www.example.com/', 
+                        'save_as': 'site.html',
+                    },
+                    'https://www.example.com/image2.jpg',
+                    {
+                        'url': 'https://www.example.com/image3.jpg', 
+                        'save_as': 'image3.jpg', 
+                        'save_to': './jpeg-downloads/',
+                    },
                 ]
             >>> bs4_scraper.download_urls(urls=urls, save_to='images', fast_download=True)
         ''' 
-
+        for index, url in enumerate(urls):
+            if isinstance(url, str):
+                urls[index] = {'url': url}
         urls = list(filter(lambda url: isinstance(url, dict) and any(url), urls))
-
         if len(urls) < 1:
             raise ValueError("No valid url was found in `urls`")
 
         results = []
         params = {
             'save_to': save_to, 'overwrite': overwrite, 
             'check_ext': check_ext, 'unique_if_query_params': unique_if_query_params
         }
-        urls_download_params = map(lambda dict: {**params, **dict}, urls)
-
+        urls_download_params = list(map(lambda dict: {**params, **dict}, urls))
         if fast_download and len(urls) <= 200:
             self.log("FAST DOWNLOAD STARTED...\n")
             with ThreadPoolExecutor() as executor:
                 values = executor.map(lambda kwargs: self.download_url(**kwargs), urls_download_params)
             results.extend(values)
 
         elif fast_download and len(urls) > 200:
             self.logger.log_warning("CANNOT USE FAST DOWNLOAD! TOO MANY URLS. FALLING BACK TO NORMAL DOWNLOAD.\n")
             self.log("DOWNLOADS STARTED...")
             values = map(lambda kwargs: self.download_url(**kwargs), urls_download_params)
             results.extend(values)
 
+        else:
+            for kwargs in urls_download_params:
+                results.append(self.download_url(**kwargs))
+
         if results:
             self.log("DOWNLOADS FINISHED!\n")
         else:
             self.log("NOTHING DOWNLOADED!\n")
         return results
```

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/translate.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/translate.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper/utils.py` & `bs4_web_scraper-0.1.2/bs4_web_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.1/bs4_web_scraper.egg-info/PKG-INFO` & `bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs4-web-scraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A web scraper based on the BeautifulSoup4 library and translators package.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/bs4_web_scraper
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/bs4_web_scraper/issues
 Project-URL: Repository, https://github.com/ti-oluwa/bs4_web_scraper
 Keywords: web scraper,bs4,beautifulsoup4,web scraping,web scraping with python,web scraping with bs4,web scraping with beautifulsoup4,web scraping with translation,web scraping with translation to other languages,web scraping with translation to other languages with python,web scraping with translation to other languages with bs4,web scraping with translation to other languages with beautifulsoup4,web scraping with translation to other languages with python and bs4,web scraping with translation to other languages with python and beautifulsoup4
@@ -292,37 +292,42 @@
     "https://www.example.com/download/example1.mkv",
     "https://www.example.com/download/example2.mkv",
     "https://www.example.com/download/example3.mkv",
     "https://www.example.com/download/example4.mkv",
     "https://www.example.com/download/example5.mkv",
 ]
 
-bs4_scraper.download_urls(urls=urls, save_to="downloads")
+bs4_scraper.download_urls(urls=urls, save_to="downloads", fast_download=True)
 
 ```
-The define what each file should be saved as, you can pass the `save_as` alongside the url as a dictionary - `urls` becomes a list of dictionaries, as parameter to the `download_urls` method. The following example shows how to download multiple files from a web page and save them with different names
+To define what each file should be saved as, you can pass the `save_as` alongside the url as a dictionary - `urls` becomes a list of dictionaries, as parameter to the `download_urls` method. The following example shows how to download multiple files from a web page and save them with different names
 
 ```python
 
 urls = [
     {
         "url": "https://www.example.com/download/example1.mkv",
-        "save_as": "example1.mkv"
+        "save_as": "example_1.mkv"
     },
     {
         "url": "https://www.example.com/download/example2.mkv",
-        "save_as": "example2.mkv"
+        "save_as": "example_2.mkv"
     },
     {
         "url": "https://www.example.com/download/example3.mkv",
-        "save_as": "example3.mkv"
+        "save_as": "example_3.mkv",
+        "save_to": "./downloads2/" 
+        # This will be treated as an absolute path and will not be saved in `self.base_storage_dir`. 
+        # This file will be saved in its own directory(determined by the path given).
     },
+    # You can also add a normal string url. This will we saved as 'example4.mkv' by default.
+    "https://www.example.com/download/example4.mkv", 
 ]
 
-bs4_scraper.download_urls(urls=urls, save_to="downloads")
+bs4_scraper.download_urls(urls=urls, save_to="downloads", fast_download=True)
 
 ```
 
 #### `find_urls`
 
 This method is used to get all resource related attribute(url or link) on elements that match a given tag name. This method only works for tags that have the `src` or `href` attribute. The following example shows how to find all urls on the `img` elements in a web page:
```

### Comparing `bs4_web_scraper-0.1.1/pyproject.toml` & `bs4_web_scraper-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bs4_web_scraper"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "A web scraper based on the BeautifulSoup4 library and translators package."
```

