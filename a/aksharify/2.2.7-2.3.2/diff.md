# Comparing `tmp/aksharify-2.2.7.tar.gz` & `tmp/aksharify-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.2.7.tar", last modified: Sun May 21 16:11:40 2023, max compression
+gzip compressed data, was "aksharify-2.3.2.tar", last modified: Sun May 28 05:44:09 2023, max compression
```

## Comparing `aksharify-2.2.7.tar` & `aksharify-2.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 16:11:40.617824 aksharify-2.2.7/
--rw-rw-rw-   0        0        0     1094 2023-05-09 13:06:55.000000 aksharify-2.2.7/LICENSE.md
--rw-rw-rw-   0        0        0     4709 2023-05-21 16:11:40.616203 aksharify-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4193 2023-05-11 14:40:43.000000 aksharify-2.2.7/README.md
--rw-rw-rw-   0        0        0      622 2023-05-21 16:09:15.000000 aksharify-2.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 16:11:40.618964 aksharify-2.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 16:11:40.552981 aksharify-2.2.7/src/
--rw-rw-rw-   0        0        0        0 2023-05-09 16:00:52.000000 aksharify-2.2.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 16:11:40.612457 aksharify-2.2.7/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4709 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-21 16:11:40.000000 aksharify-2.2.7/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3203 2023-05-21 16:03:49.000000 aksharify-2.2.7/src/aksharify.py
+drwxrwxrwx   0        0        0        0 2023-05-28 05:44:09.853717 aksharify-2.3.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.3.2/LICENSE.md
+-rw-rw-rw-   0        0        0     4874 2023-05-28 05:44:09.849695 aksharify-2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.3.2/README.md
+-rw-rw-rw-   0        0        0      622 2023-05-28 05:42:56.000000 aksharify-2.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 05:44:09.855740 aksharify-2.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 05:44:09.785028 aksharify-2.3.2/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.3.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 05:44:09.847176 aksharify-2.3.2/src/aksharify.egg-info/
+-rw-rw-rw-   0        0        0     4874 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-28 05:44:09.000000 aksharify-2.3.2/src/aksharify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4705 2023-05-28 05:34:29.000000 aksharify-2.3.2/src/aksharify.py
```

### Comparing `aksharify-2.2.7/LICENSE.md` & `aksharify-2.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.2.7/PKG-INFO` & `aksharify-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.2.7
+Version: 2.3.2
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
+[![PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
 
 <br />
 
 <!-- ABOUT THE PROJECT -->
 ## About the module
 
 The inspiration for this module came from a Numberphile video called "The Trinity Hall Prime," which I first saw in high school days. It motivated me to explore the possibilities of such a prime number. I created a Python module that uses a predetermined character set to turn photos into ASCII art. It manipulates images using the PIL package, transforming them to grayscale before mapping pixel values to ASCII letters. Users can change the character set to get different effects.
@@ -129,7 +130,8 @@
 [stars-url]: https://github.com/primepatel/Aksharify/stargazers
 [issues-shield]: https://img.shields.io/github/issues/primepatel/Aksharify.svg?style=for-the-badge
 [issues-url]: https://github.com/primepatel/Aksharify/issues
 [license-shield]: https://img.shields.io/github/license/primepatel/Aksharify.svg?style=for-the-badge
 [license-url]: https://github.com/primepatel/Aksharify/blob/master/LICENSE.txt
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://linkedin.com/in/primepatel
+[Downloads-shield]: https://img.shields.io/pypi/dm/aksharify?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.2.7 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.3.2 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
 shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+[license-shield]][license-url] [![LinkedIn][linkedin-shield]][linkedin-url] [!
+[PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
+
  ## About the module The inspiration for this module came from a Numberphile
 video called "The Trinity Hall Prime," which I first saw in high school days.
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
@@ -51,8 +53,9 @@
 Aksharify/stargazers [issues-shield]: https://img.shields.io/github/issues/
 primepatel/Aksharify.svg?style=for-the-badge [issues-url]: https://github.com/
 primepatel/Aksharify/issues [license-shield]: https://img.shields.io/github/
 license/primepatel/Aksharify.svg?style=for-the-badge [license-url]: https://
 github.com/primepatel/Aksharify/blob/master/LICENSE.txt [linkedin-shield]:
 https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-
 badge&logo=linkedin&colorB=555 [linkedin-url]: https://linkedin.com/in/
-primepatel
+primepatel [Downloads-shield]: https://img.shields.io/pypi/dm/
+aksharify?style=for-the-badge
```

### Comparing `aksharify-2.2.7/README.md` & `aksharify-2.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
+[![PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
 
 <br />
 
 <!-- ABOUT THE PROJECT -->
 ## About the module
 
 The inspiration for this module came from a Numberphile video called "The Trinity Hall Prime," which I first saw in high school days. It motivated me to explore the possibilities of such a prime number. I created a Python module that uses a predetermined character set to turn photos into ASCII art. It manipulates images using the PIL package, transforming them to grayscale before mapping pixel values to ASCII letters. Users can change the character set to get different effects.
@@ -114,8 +115,9 @@
 [stars-shield]: https://img.shields.io/github/stars/primepatel/Aksharify.svg?style=for-the-badge
 [stars-url]: https://github.com/primepatel/Aksharify/stargazers
 [issues-shield]: https://img.shields.io/github/issues/primepatel/Aksharify.svg?style=for-the-badge
 [issues-url]: https://github.com/primepatel/Aksharify/issues
 [license-shield]: https://img.shields.io/github/license/primepatel/Aksharify.svg?style=for-the-badge
 [license-url]: https://github.com/primepatel/Aksharify/blob/master/LICENSE.txt
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-[linkedin-url]: https://linkedin.com/in/primepatel
+[linkedin-url]: https://linkedin.com/in/primepatel
+[Downloads-shield]: https://img.shields.io/pypi/dm/aksharify?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
  # __Aksharify__ [![Contributors][contributors-shield]][contributors-url] [!
 [Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+url] [![LinkedIn][linkedin-shield]][linkedin-url] [![PyPI - Downloads]
+[Downloads-shield]](https://pypistats.org/packages/aksharify)
  ## About the module The inspiration for this module came from a Numberphile
 video called "The Trinity Hall Prime," which I first saw in high school days.
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
@@ -44,8 +45,9 @@
 Aksharify/stargazers [issues-shield]: https://img.shields.io/github/issues/
 primepatel/Aksharify.svg?style=for-the-badge [issues-url]: https://github.com/
 primepatel/Aksharify/issues [license-shield]: https://img.shields.io/github/
 license/primepatel/Aksharify.svg?style=for-the-badge [license-url]: https://
 github.com/primepatel/Aksharify/blob/master/LICENSE.txt [linkedin-shield]:
 https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-
 badge&logo=linkedin&colorB=555 [linkedin-url]: https://linkedin.com/in/
-primepatel
+primepatel [Downloads-shield]: https://img.shields.io/pypi/dm/
+aksharify?style=for-the-badge
```

### Comparing `aksharify-2.2.7/pyproject.toml` & `aksharify-2.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aksharify"
-version = "2.2.7"
+version = "2.3.2"
 authors = [
     {name="Prime Patel", email = "primespatel@gmail.com"}
 ]
 description = "Ascii art module"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `aksharify-2.2.7/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.3.2/src/aksharify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.2.7
+Version: 2.3.2
 Summary: Ascii art module
 Author-email: Prime Patel <primespatel@gmail.com>
 Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
+[![PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
 
 <br />
 
 <!-- ABOUT THE PROJECT -->
 ## About the module
 
 The inspiration for this module came from a Numberphile video called "The Trinity Hall Prime," which I first saw in high school days. It motivated me to explore the possibilities of such a prime number. I created a Python module that uses a predetermined character set to turn photos into ASCII art. It manipulates images using the PIL package, transforming them to grayscale before mapping pixel values to ASCII letters. Users can change the character set to get different effects.
@@ -129,7 +130,8 @@
 [stars-url]: https://github.com/primepatel/Aksharify/stargazers
 [issues-shield]: https://img.shields.io/github/issues/primepatel/Aksharify.svg?style=for-the-badge
 [issues-url]: https://github.com/primepatel/Aksharify/issues
 [license-shield]: https://img.shields.io/github/license/primepatel/Aksharify.svg?style=for-the-badge
 [license-url]: https://github.com/primepatel/Aksharify/blob/master/LICENSE.txt
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://linkedin.com/in/primepatel
+[Downloads-shield]: https://img.shields.io/pypi/dm/aksharify?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.2.7 Summary: Ascii art module
+Metadata-Version: 2.1 Name: aksharify Version: 2.3.2 Summary: Ascii art module
 Author-email: Prime Patel
 gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
 Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
 shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+[license-shield]][license-url] [![LinkedIn][linkedin-shield]][linkedin-url] [!
+[PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
+
  ## About the module The inspiration for this module came from a Numberphile
 video called "The Trinity Hall Prime," which I first saw in high school days.
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
@@ -51,8 +53,9 @@
 Aksharify/stargazers [issues-shield]: https://img.shields.io/github/issues/
 primepatel/Aksharify.svg?style=for-the-badge [issues-url]: https://github.com/
 primepatel/Aksharify/issues [license-shield]: https://img.shields.io/github/
 license/primepatel/Aksharify.svg?style=for-the-badge [license-url]: https://
 github.com/primepatel/Aksharify/blob/master/LICENSE.txt [linkedin-shield]:
 https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-
 badge&logo=linkedin&colorB=555 [linkedin-url]: https://linkedin.com/in/
-primepatel
+primepatel [Downloads-shield]: https://img.shields.io/pypi/dm/
+aksharify?style=for-the-badge
```

