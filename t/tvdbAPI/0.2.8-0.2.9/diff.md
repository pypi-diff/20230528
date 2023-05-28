# Comparing `tmp/tvdbAPI-0.2.8.tar.gz` & `tmp/tvdbAPI-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdbAPI-0.2.8.tar", last modified: Fri Jan 14 01:56:14 2022, max compression
+gzip compressed data, was "tvdbAPI-0.2.9.tar", last modified: Sun Sep  4 05:14:13 2022, max compression
```

## Comparing `tvdbAPI-0.2.8.tar` & `tvdbAPI-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-01-14 01:56:14.844160 tvdbAPI-0.2.8/
--rw-rw-rw-   0        0        0     1076 2021-02-17 22:49:45.000000 tvdbAPI-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      775 2022-01-14 01:56:14.844160 tvdbAPI-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      336 2021-02-17 22:49:45.000000 tvdbAPI-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2022-01-14 01:56:14.844160 tvdbAPI-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      884 2022-01-14 01:54:09.000000 tvdbAPI-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-14 01:56:14.843159 tvdbAPI-0.2.8/tvdbAPI.egg-info/
--rw-rw-rw-   0        0        0      775 2022-01-14 01:56:14.000000 tvdbAPI-0.2.8/tvdbAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2022-01-14 01:56:14.000000 tvdbAPI-0.2.8/tvdbAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-14 01:56:14.000000 tvdbAPI-0.2.8/tvdbAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-01-14 01:56:14.000000 tvdbAPI-0.2.8/tvdbAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-01-14 01:56:14.000000 tvdbAPI-0.2.8/tvdbAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10466 2022-01-14 01:31:10.000000 tvdbAPI-0.2.8/tvdbAPI.py
+drwxrwxrwx   0        0        0        0 2022-09-04 05:14:13.924407 tvdbAPI-0.2.9/
+-rw-rw-rw-   0        0        0     1076 2021-02-17 22:49:45.000000 tvdbAPI-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      754 2022-09-04 05:14:13.923908 tvdbAPI-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2021-02-17 22:49:45.000000 tvdbAPI-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-09-04 05:14:13.924407 tvdbAPI-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      884 2022-09-04 05:06:40.000000 tvdbAPI-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-04 05:14:13.922907 tvdbAPI-0.2.9/tvdbAPI.egg-info/
+-rw-rw-rw-   0        0        0      754 2022-09-04 05:14:13.000000 tvdbAPI-0.2.9/tvdbAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2022-09-04 05:14:13.000000 tvdbAPI-0.2.9/tvdbAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-04 05:14:13.000000 tvdbAPI-0.2.9/tvdbAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2022-09-04 05:14:13.000000 tvdbAPI-0.2.9/tvdbAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-09-04 05:14:13.000000 tvdbAPI-0.2.9/tvdbAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10466 2022-09-04 05:06:26.000000 tvdbAPI-0.2.9/tvdbAPI.py
```

### Comparing `tvdbAPI-0.2.8/LICENSE` & `tvdbAPI-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tvdbAPI-0.2.8/setup.py` & `tvdbAPI-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     longDescription = f.read()
 
 # with open(path.join(here, 'requirements.txt')) as f:
 #     requirements = f.read().split('\n')
 
 setup(
     name="tvdbAPI",
-    version="0.2.8",
+    version="0.2.9",
     author="Kevin Riehl",
     author_email="kevinriehl@gmail.com",
     description="Python Module for accessing the TVDB API",
     long_description=longDescription,
     long_description_content_type="text/markdown",
     py_modules=['tvdbAPI'],
     install_requires=['requests >= 2.22.0', 'sanction >= 0.4.1'],
```

### Comparing `tvdbAPI-0.2.8/tvdbAPI.py` & `tvdbAPI-0.2.9/tvdbAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         if not self.__authorized:
             self._authorize()
         id = self._getShowID(name, accuracy)
         if id == -1:
             raise InvalidShowID("Show was not found, please try again")
         return self._getActors(id)
 
-    def getImages(self, name, imageType = "series", accuracy = 0.8):
+    def getImages(self, name, imageType = "poster", accuracy = 0.8):
         """Grabs the urls for the images of the show based on the type you have selected. Default grabs 'series' image urls,
         and returns them in a list.
         
         Arguments:
             name {String} -- The name of the show.
         
         Keyword Arguments:
```

