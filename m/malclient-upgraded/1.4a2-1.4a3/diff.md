# Comparing `tmp/malclient-upgraded-1.4a2.tar.gz` & `tmp/malclient-upgraded-1.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malclient-upgraded-1.4a2.tar", last modified: Fri May 26 01:30:33 2023, max compression
+gzip compressed data, was "malclient-upgraded-1.4a3.tar", last modified: Sun May 28 00:19:16 2023, max compression
```

## Comparing `malclient-upgraded-1.4a2.tar` & `malclient-upgraded-1.4a3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-26 01:30:33.058825 malclient-upgraded-1.4a2/
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1087 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a2/LICENSE
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4721 2023-05-26 01:30:33.058825 malclient-upgraded-1.4a2/PKG-INFO
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4233 2023-05-26 00:21:49.000000 malclient-upgraded-1.4a2/README.md
-drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-26 01:30:33.025213 malclient-upgraded-1.4a2/malclient/
-drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-26 01:30:33.048213 malclient-upgraded-1.4a2/malclient/Datamodels/
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      105 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a2/malclient/Datamodels/__init__.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7420 2022-11-22 17:28:58.000000 malclient-upgraded-1.4a2/malclient/Datamodels/enums.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    15855 2023-05-26 01:28:26.000000 malclient-upgraded-1.4a2/malclient/Datamodels/fields.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    13483 2023-05-26 01:28:26.000000 malclient-upgraded-1.4a2/malclient/Datamodels/models.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1275 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a2/malclient/Datamodels/pagination.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       77 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a2/malclient/__init__.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     8789 2023-05-26 00:17:31.000000 malclient-upgraded-1.4a2/malclient/anime.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3336 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a2/malclient/boards.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7808 2023-05-25 22:05:50.000000 malclient-upgraded-1.4a2/malclient/client.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     2068 2023-01-22 22:26:02.000000 malclient-upgraded-1.4a2/malclient/exceptions.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3849 2022-11-22 20:46:54.000000 malclient-upgraded-1.4a2/malclient/manga.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    12218 2022-11-22 20:47:13.000000 malclient-upgraded-1.4a2/malclient/my_list.py
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     6527 2023-05-26 01:28:26.000000 malclient-upgraded-1.4a2/malclient/request_handler.py
-drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-26 01:30:33.057826 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4721 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/PKG-INFO
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      594 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/SOURCES.txt
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        1 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/dependency_links.txt
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       18 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/requires.txt
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       10 2023-05-26 01:30:32.000000 malclient-upgraded-1.4a2/malclient_upgraded.egg-info/top_level.txt
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      148 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a2/pyproject.toml
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       79 2023-05-26 01:30:33.059825 malclient-upgraded-1.4a2/setup.cfg
--rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      889 2023-05-26 01:30:16.000000 malclient-upgraded-1.4a2/setup.py
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-28 00:19:16.215516 malclient-upgraded-1.4a3/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1087 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a3/LICENSE
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4721 2023-05-28 00:19:16.215516 malclient-upgraded-1.4a3/PKG-INFO
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4233 2023-05-26 00:21:49.000000 malclient-upgraded-1.4a3/README.md
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-28 00:19:16.166338 malclient-upgraded-1.4a3/malclient/
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-28 00:19:16.204489 malclient-upgraded-1.4a3/malclient/Datamodels/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      105 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a3/malclient/Datamodels/__init__.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7420 2022-11-22 17:28:58.000000 malclient-upgraded-1.4a3/malclient/Datamodels/enums.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    16448 2023-05-28 00:14:04.000000 malclient-upgraded-1.4a3/malclient/Datamodels/fields.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    13617 2023-05-28 00:08:31.000000 malclient-upgraded-1.4a3/malclient/Datamodels/models.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     1275 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a3/malclient/Datamodels/pagination.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       77 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a3/malclient/__init__.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     8789 2023-05-26 00:17:31.000000 malclient-upgraded-1.4a3/malclient/anime.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3336 2022-11-08 19:51:57.000000 malclient-upgraded-1.4a3/malclient/boards.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     7850 2023-05-28 00:01:51.000000 malclient-upgraded-1.4a3/malclient/client.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     2068 2023-01-22 22:26:02.000000 malclient-upgraded-1.4a3/malclient/exceptions.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      832 2023-05-28 00:14:04.000000 malclient-upgraded-1.4a3/malclient/industry.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     3849 2022-11-22 20:46:54.000000 malclient-upgraded-1.4a3/malclient/manga.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)    12218 2022-11-22 20:47:13.000000 malclient-upgraded-1.4a3/malclient/my_list.py
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     6527 2023-05-26 01:28:26.000000 malclient-upgraded-1.4a3/malclient/request_handler.py
+drwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        0 2023-05-28 00:19:16.214515 malclient-upgraded-1.4a3/malclient_upgraded.egg-info/
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)     4721 2023-05-28 00:19:16.000000 malclient-upgraded-1.4a3/malclient_upgraded.egg-info/PKG-INFO
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      616 2023-05-28 00:19:16.000000 malclient-upgraded-1.4a3/malclient_upgraded.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)        1 2023-05-28 00:19:16.000000 malclient-upgraded-1.4a3/malclient_upgraded.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       18 2023-05-28 00:19:16.000000 malclient-upgraded-1.4a3/malclient_upgraded.egg-info/requires.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       10 2023-05-28 00:19:16.000000 malclient-upgraded-1.4a3/malclient_upgraded.egg-info/top_level.txt
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      148 2022-11-08 15:30:53.000000 malclient-upgraded-1.4a3/pyproject.toml
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)       79 2023-05-28 00:19:16.217515 malclient-upgraded-1.4a3/setup.cfg
+-rwxrwxrwx   0 gruzin    (1000) gruzin    (1000)      889 2023-05-28 00:18:31.000000 malclient-upgraded-1.4a3/setup.py
```

### Comparing `malclient-upgraded-1.4a2/LICENSE` & `malclient-upgraded-1.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/PKG-INFO` & `malclient-upgraded-1.4a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malclient-upgraded
-Version: 1.4a2
+Version: 1.4a3
 Summary: Modified and rewritten using modern models version of James Fotherby malclient
 Home-page: https://github.com/ModerNews/MAL-API-Client-Upgraded
 Author: ModerNews
 Author-email: polski.gruzin.biz@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mal-api-client-upgraded.readthedocs.io
 Platform: UNKNOWN
```

### Comparing `malclient-upgraded-1.4a2/README.md` & `malclient-upgraded-1.4a3/README.md`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient/Datamodels/enums.py` & `malclient-upgraded-1.4a3/malclient/Datamodels/enums.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient/Datamodels/fields.py` & `malclient-upgraded-1.4a3/malclient/Datamodels/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from types import MethodType, MethodWrapperType, BuiltinFunctionType
 from typing import Union
 
-__all__ = ['Fields', 'AuthorFields', 'ListStatusFields', 'UserFields', "CharacterFields"]
+__all__ = ['Fields', 'AuthorFields', 'ListStatusFields', 'UserFields', "CharacterFields", 'PersonFields']
 
 
 class FieldsBase(object):
     """
     Base class for all Field classes
     """
     def __init__(self, **kwargs):
@@ -365,14 +365,25 @@
         return self._animeography
 
     @animeography.setter
     def animeography(self, value: Fields):
         self._animeography: Fields = self._generate_subclass(Fields, value)
 
 
+class PersonFields(FieldsBase):
+    def __init__(self, **kwargs):
+        self.id: bool = kwargs.get("id", True)
+        self.first_name: bool = kwargs.get("first_name", True)
+        self.last_name: bool = kwargs.get("last_name", True)
+        self.alternative_names: bool = kwargs.get("alternative_names", False)
+        self.num_favorites: bool = kwargs.get("num_favorites", False)
+        self.main_picture: bool = kwargs.get("main_picture", False)
+        self.birthday: bool = kwargs.get("birthday", False)
+        self.more: bool = kwargs.get("more", False)
+
 # Deprecated - This serves no purpose, you can't specify fields for this parameter
 # class AnimeStatisticsFields(FieldsBase):
 #     def __init__(self, **kwargs):
 #         self.num_items_watching: bool = kwargs.get("num_items_watching", False)
 #         self.num_items_completed: bool = kwargs.get("num_items_completed", False)
 #         self.num_items_on_hold: bool = kwargs.get("num_items_on_hold", False)
 #         self.num_items_dropped: bool = kwargs.get("num_items_dropped", False)
```

### Comparing `malclient-upgraded-1.4a2/malclient/Datamodels/models.py` & `malclient-upgraded-1.4a3/malclient/Datamodels/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .pagination import PagedResult
 from .fields import Fields
 from ..exceptions import NotFound
 
 __all__ = ['Asset', 'Node', 'AnimeSeason', 'Genre', 'Studio', 'Broadcast', 'Statistics', 'Relation', 'Recommendation',
            'MyMangaListStatus', 'MyAnimeListStatus', 'AnimeObject', 'MangaObject', 'UserAnimeStatistics', "User",
            'ForumTopicDetail', 'ForumTopic', 'ForumCategory', 'ForumAuthor', 'ForumPoll', 'ForumPollOption',
-           'ForumPost', 'ForumBoard', 'ForumSubboard', 'Character']
+           'ForumPost', 'ForumBoard', 'ForumSubboard', 'Character', 'Person']
 
 
 class MALBaseModel(BaseModel):
     """
     Helper model class used to generate all models used by this API
     """
 
@@ -489,18 +489,23 @@
     However it always contains role field, which represents role given to character in anime.
 
     This object is only available in Character object.
     """
     role: Optional[str]
 
 
-class Character(MALBaseModel):
-    id: int
+class Character(PersonBase):
     role: Optional[str]
-    first_name: Optional[str]
-    last_name: Optional[str]
-    alternative_name: Optional[list[str]]
+    alternative_name: Optional[str]
     main_picture: Optional[Asset]
     biography: Optional[str]
     pictures: Optional[list[Asset]]
     animeography: Optional[list[Animeography]]
     num_favorites: Optional[int]
+
+
+class Person(PersonBase):
+    alternative_names: Optional[list[str]]
+    num_favorites: Optional[int]
+    main_picture: Optional[Asset]
+    birthday: Optional[datetime.date]
+    more: Optional[str]
```

### Comparing `malclient-upgraded-1.4a2/malclient/Datamodels/pagination.py` & `malclient-upgraded-1.4a3/malclient/Datamodels/pagination.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient/anime.py` & `malclient-upgraded-1.4a3/malclient/anime.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient/boards.py` & `malclient-upgraded-1.4a3/malclient/boards.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient/client.py` & `malclient-upgraded-1.4a3/malclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional
 import platform
 
 from .request_handler import APICaller
 from .anime import Anime
 from .my_list import MyList
 from .manga import Manga
+from .industry import Industry
 from .exceptions import AuthorizationError
 from .boards import Boards
 
 __all__ = ['Client', 'setup_logging', 'generate_authorization_url', 'fetch_token_schema_2']
 
 
 def generate_authorization_url(client_id: str, *,
@@ -74,15 +75,15 @@
         format = "%(levelname)s | %(asctime)s | %(message)s"
     now = datetime.datetime.now()
     if filename is None:
         filename = f"malclient_log_{now.strftime('%Y-%m-%d_%H-%M')}.log"
     logging.basicConfig(filename=filename, level=log_level, format=format)
 
 
-class Client(Anime, Manga, MyList, Boards):
+class Client(Anime, Manga, MyList, Boards, Industry):
     """
 
     Base class for interacting with MyAnimeList REST API
 
     :ivar client_id: string containing client_id obtained from [client configuration on MAL](https://myanimelist.net/apiconfig)
     :ivar access_token: string containing access token obtained through OAuth2
     :ivar refresh_token: string containing refresh token obtained through OAuth2
```

### Comparing `malclient-upgraded-1.4a2/malclient/exceptions.py` & `malclient-upgraded-1.4a3/malclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient/manga.py` & `malclient-upgraded-1.4a3/malclient/manga.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient/my_list.py` & `malclient-upgraded-1.4a3/malclient/my_list.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient/request_handler.py` & `malclient-upgraded-1.4a3/malclient/request_handler.py`

 * *Files identical despite different names*

### Comparing `malclient-upgraded-1.4a2/malclient_upgraded.egg-info/PKG-INFO` & `malclient-upgraded-1.4a3/malclient_upgraded.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malclient-upgraded
-Version: 1.4a2
+Version: 1.4a3
 Summary: Modified and rewritten using modern models version of James Fotherby malclient
 Home-page: https://github.com/ModerNews/MAL-API-Client-Upgraded
 Author: ModerNews
 Author-email: polski.gruzin.biz@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mal-api-client-upgraded.readthedocs.io
 Platform: UNKNOWN
```

### Comparing `malclient-upgraded-1.4a2/malclient_upgraded.egg-info/SOURCES.txt` & `malclient-upgraded-1.4a3/malclient_upgraded.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 malclient/__init__.py
 malclient/anime.py
 malclient/boards.py
 malclient/client.py
 malclient/exceptions.py
+malclient/industry.py
 malclient/manga.py
 malclient/my_list.py
 malclient/request_handler.py
 malclient/Datamodels/__init__.py
 malclient/Datamodels/enums.py
 malclient/Datamodels/fields.py
 malclient/Datamodels/models.py
```

### Comparing `malclient-upgraded-1.4a2/setup.py` & `malclient-upgraded-1.4a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="malclient-upgraded",
-    version="1.4a2",
+    version="1.4a3",
     author="ModerNews",
     author_email="polski.gruzin.biz@gmail.com",
     description=
     "Modified and rewritten using modern models version of James Fotherby malclient",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ModerNews/MAL-API-Client-Upgraded",
```

