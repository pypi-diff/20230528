# Comparing `tmp/comicapi-2.2.1.tar.gz` & `tmp/comicapi-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicapi-2.2.1.tar", last modified: Sat Jan 22 10:28:14 2022, max compression
+gzip compressed data, was "comicapi-3.0.0.tar", last modified: Sun May 28 08:16:14 2023, max compression
```

## Comparing `comicapi-2.2.1.tar` & `comicapi-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 ozzie     (1000) ozzie     (1000)        0 2022-01-22 10:28:14.602615 comicapi-2.2.1/
--rw-rw-r--   0 ozzie     (1000) ozzie     (1000)      503 2022-01-22 10:28:14.602615 comicapi-2.2.1/PKG-INFO
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)      463 2021-01-17 08:56:41.000000 comicapi-2.2.1/README.md
-drwxrwxr-x   0 ozzie     (1000) ozzie     (1000)        0 2022-01-22 10:28:14.602615 comicapi-2.2.1/comicapi/
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)       47 2021-03-18 17:40:07.000000 comicapi-2.2.1/comicapi/__init__.py
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)     8405 2021-01-17 08:56:41.000000 comicapi-2.2.1/comicapi/comet.py
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)    41065 2022-01-22 10:22:43.000000 comicapi-2.2.1/comicapi/comicarchive.py
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)     4797 2021-01-17 08:56:41.000000 comicapi-2.2.1/comicapi/comicbookinfo.py
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)    10438 2021-01-17 08:56:41.000000 comicapi-2.2.1/comicapi/comicinfoxml.py
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)     9272 2021-01-17 08:56:41.000000 comicapi-2.2.1/comicapi/filenameparser.py
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)     9701 2021-01-17 08:56:41.000000 comicapi-2.2.1/comicapi/genericmetadata.py
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)     3453 2021-01-17 08:56:41.000000 comicapi-2.2.1/comicapi/issuestring.py
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)    13457 2021-01-17 08:56:41.000000 comicapi-2.2.1/comicapi/utils.py
-drwxrwxr-x   0 ozzie     (1000) ozzie     (1000)        0 2022-01-22 10:28:14.602615 comicapi-2.2.1/comicapi.egg-info/
--rw-rw-r--   0 ozzie     (1000) ozzie     (1000)      503 2022-01-22 10:28:14.000000 comicapi-2.2.1/comicapi.egg-info/PKG-INFO
--rw-rw-r--   0 ozzie     (1000) ozzie     (1000)      389 2022-01-22 10:28:14.000000 comicapi-2.2.1/comicapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ozzie     (1000) ozzie     (1000)        1 2022-01-22 10:28:14.000000 comicapi-2.2.1/comicapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ozzie     (1000) ozzie     (1000)       35 2022-01-22 10:28:14.000000 comicapi-2.2.1/comicapi.egg-info/requires.txt
--rw-rw-r--   0 ozzie     (1000) ozzie     (1000)        9 2022-01-22 10:28:14.000000 comicapi-2.2.1/comicapi.egg-info/top_level.txt
--rw-rw-r--   0 ozzie     (1000) ozzie     (1000)       38 2022-01-22 10:28:14.602615 comicapi-2.2.1/setup.cfg
--rw-r--r--   0 ozzie     (1000) ozzie     (1000)      734 2022-01-22 10:25:55.000000 comicapi-2.2.1/setup.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 08:16:14.605454 comicapi-3.0.0/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    11359 2023-05-28 07:28:44.000000 comicapi-3.0.0/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1306 2023-05-28 08:16:14.605454 comicapi-3.0.0/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      463 2023-05-04 16:45:48.000000 comicapi-3.0.0/README.md
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 08:16:14.605454 comicapi-3.0.0/comicapi/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       47 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7694 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/comet.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    44185 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/comicarchive.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4625 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/comicbookinfo.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    10401 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/comicinfoxml.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    10015 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/filenameparser.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    14912 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/genericmetadata.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3557 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/issuestring.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6381 2023-05-28 07:28:49.000000 comicapi-3.0.0/comicapi/utils.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 08:16:14.605454 comicapi-3.0.0/comicapi.egg-info/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1306 2023-05-28 08:16:14.000000 comicapi-3.0.0/comicapi.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      397 2023-05-28 08:16:14.000000 comicapi-3.0.0/comicapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2023-05-28 08:16:14.000000 comicapi-3.0.0/comicapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2023-05-28 08:16:14.000000 comicapi-3.0.0/comicapi.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        9 2023-05-28 08:16:14.000000 comicapi-3.0.0/comicapi.egg-info/top_level.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       38 2023-05-28 08:16:14.605454 comicapi-3.0.0/setup.cfg
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1443 2023-05-28 08:16:11.000000 comicapi-3.0.0/setup.py
```

### Comparing `comicapi-2.2.1/comicapi/comet.py` & `comicapi-3.0.0/comicapi/comet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,244 +1,226 @@
-"""
-A python class to encapsulate CoMet data
+"""A class to encapsulate CoMet data"""
 
-Copyright 2012-2014  Anthony Beville
+# Copyright 2012-2014 Anthony Beville
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import logging
 import xml.etree.ElementTree as ET
+
+from comicapi import utils
 from comicapi.genericmetadata import GenericMetadata
-import comicapi.utils
+
+logger = logging.getLogger(__name__)
 
 
 class CoMet:
 
-    writer_synonyms = ['writer', 'plotter', 'scripter']
-    penciller_synonyms = ['artist', 'penciller', 'penciler', 'breakdowns']
-    inker_synonyms = ['inker', 'artist', 'finishes']
-    colorist_synonyms = ['colorist', 'colourist', 'colorer', 'colourer']
-    letterer_synonyms = ['letterer']
-    cover_synonyms = ['cover', 'covers', 'coverartist', 'cover artist']
-    editor_synonyms = ['editor']
+    writer_synonyms = ["writer", "plotter", "scripter"]
+    penciller_synonyms = ["artist", "penciller", "penciler", "breakdowns"]
+    inker_synonyms = ["inker", "artist", "finishes"]
+    colorist_synonyms = ["colorist", "colourist", "colorer", "colourer"]
+    letterer_synonyms = ["letterer"]
+    cover_synonyms = ["cover", "covers", "coverartist", "cover artist"]
+    editor_synonyms = ["editor"]
 
-    def metadataFromString(self, string):
+    def metadata_from_string(self, string):
 
         tree = ET.ElementTree(ET.fromstring(string))
-        return self.convertXMLToMetadata(tree)
+        return self.convert_xml_to_metadata(tree)
 
-    def stringFromMetadata(self, metadata):
+    def string_from_metadata(self, metadata):
 
         header = '<?xml version="1.0" encoding="UTF-8"?>\n'
 
-        tree = self.convertMetadataToXML(self, metadata)
+        tree = self.convert_metadata_to_xml(metadata)
         return header + ET.tostring(tree.getroot())
 
-    def indent(self, elem, level=0):
-        # for making the XML output readable
-        i = "\n" + level * "  "
-        if len(elem):
-            if not elem.text or not elem.text.strip():
-                elem.text = i + "  "
-            if not elem.tail or not elem.tail.strip():
-                elem.tail = i
-            for elem in elem:
-                self.indent(elem, level + 1)
-            if not elem.tail or not elem.tail.strip():
-                elem.tail = i
-        else:
-            if level and (not elem.tail or not elem.tail.strip()):
-                elem.tail = i
-
-    def convertMetadataToXML(self, filename, metadata):
+    def convert_metadata_to_xml(self, metadata):
 
         # shorthand for the metadata
         md = metadata
 
         # build a tree structure
         root = ET.Element("comet")
-        root.attrib['xmlns:comet'] = "http://www.denvog.com/comet/"
-        root.attrib['xmlns:xsi'] = "http://www.w3.org/2001/XMLSchema-instance"
-        root.attrib[
-            'xsi:schemaLocation'] = "http://www.denvog.com http://www.denvog.com/comet/comet.xsd"
+        root.attrib["xmlns:comet"] = "http://www.denvog.com/comet/"
+        root.attrib["xmlns:xsi"] = "http://www.w3.org/2001/XMLSchema-instance"
+        root.attrib["xsi:schemaLocation"] = "http://www.denvog.com http://www.denvog.com/comet/comet.xsd"
 
         # helper func
         def assign(comet_entry, md_entry):
             if md_entry is not None:
-                ET.SubElement(root, comet_entry).text = u"{0}".format(md_entry)
+                ET.SubElement(root, comet_entry).text = str(md_entry)
 
         # title is manditory
         if md.title is None:
             md.title = ""
-        assign('title', md.title)
-        assign('series', md.series)
-        assign('issue', md.issue)  # must be int??
-        assign('volume', md.volume)
-        assign('description', md.comments)
-        assign('publisher', md.publisher)
-        assign('pages', md.pageCount)
-        assign('format', md.format)
-        assign('language', md.language)
-        assign('rating', md.maturityRating)
-        assign('price', md.price)
-        assign('isVersionOf', md.isVersionOf)
-        assign('rights', md.rights)
-        assign('identifier', md.identifier)
-        assign('lastMark', md.lastMark)
-        assign('genre', md.genre)  # TODO repeatable
+        assign("title", md.title)
+        assign("series", md.series)
+        assign("issue", md.issue)  # must be int??
+        assign("volume", md.volume)
+        assign("description", md.comments)
+        assign("publisher", md.publisher)
+        assign("pages", md.page_count)
+        assign("format", md.format)
+        assign("language", md.language)
+        assign("rating", md.maturity_rating)
+        assign("price", md.price)
+        assign("isVersionOf", md.is_version_of)
+        assign("rights", md.rights)
+        assign("identifier", md.identifier)
+        assign("lastMark", md.last_mark)
+        assign("genre", md.genre)  # TODO repeatable
 
         if md.characters is not None:
-            char_list = [c.strip() for c in md.characters.split(',')]
+            char_list = [c.strip() for c in md.characters.split(",")]
             for c in char_list:
-                assign('character', c)
+                assign("character", c)
 
         if md.manga is not None and md.manga == "YesAndRightToLeft":
-            assign('readingDirection', "rtl")
+            assign("readingDirection", "rtl")
 
-        date_str = ""
         if md.year is not None:
             date_str = str(md.year).zfill(4)
             if md.month is not None:
                 date_str += "-" + str(md.month).zfill(2)
-            assign('date', date_str)
+            assign("date", date_str)
 
-        assign('coverImage', md.coverImage)
+        assign("coverImage", md.cover_image)
 
-        #  loop thru credits, and build a list for each role that CoMet supports
+        # loop thru credits, and build a list for each role that CoMet supports
         for credit in metadata.credits:
 
-            if credit['role'].lower() in set(self.writer_synonyms):
-                ET.SubElement(root, 'writer').text = u"{0}".format(
-                    credit['person'])
-
-            if credit['role'].lower() in set(self.penciller_synonyms):
-                ET.SubElement(root, 'penciller').text = u"{0}".format(
-                    credit['person'])
-
-            if credit['role'].lower() in set(self.inker_synonyms):
-                ET.SubElement(root, 'inker').text = u"{0}".format(
-                    credit['person'])
-
-            if credit['role'].lower() in set(self.colorist_synonyms):
-                ET.SubElement(root, 'colorist').text = u"{0}".format(
-                    credit['person'])
-
-            if credit['role'].lower() in set(self.letterer_synonyms):
-                ET.SubElement(root, 'letterer').text = u"{0}".format(
-                    credit['person'])
-
-            if credit['role'].lower() in set(self.cover_synonyms):
-                ET.SubElement(root, 'coverDesigner').text = u"{0}".format(
-                    credit['person'])
-
-            if credit['role'].lower() in set(self.editor_synonyms):
-                ET.SubElement(root, 'editor').text = u"{0}".format(
-                    credit['person'])
+            if credit["role"].lower() in set(self.writer_synonyms):
+                ET.SubElement(root, "writer").text = str(credit["person"])
+
+            if credit["role"].lower() in set(self.penciller_synonyms):
+                ET.SubElement(root, "penciller").text = str(credit["person"])
+
+            if credit["role"].lower() in set(self.inker_synonyms):
+                ET.SubElement(root, "inker").text = str(credit["person"])
+
+            if credit["role"].lower() in set(self.colorist_synonyms):
+                ET.SubElement(root, "colorist").text = str(credit["person"])
+
+            if credit["role"].lower() in set(self.letterer_synonyms):
+                ET.SubElement(root, "letterer").text = str(credit["person"])
+
+            if credit["role"].lower() in set(self.cover_synonyms):
+                ET.SubElement(root, "coverDesigner").text = str(credit["person"])
+
+            if credit["role"].lower() in set(self.editor_synonyms):
+                ET.SubElement(root, "editor").text = str(credit["person"])
 
-        # self pretty-print
-        self.indent(root)
+        utils.indent(root)
 
         # wrap it in an ElementTree instance, and save as XML
         tree = ET.ElementTree(root)
         return tree
 
-    def convertXMLToMetadata(self, tree):
+    def convert_xml_to_metadata(self, tree):
 
         root = tree.getroot()
 
-        if root.tag != 'comet':
-            raise KeyError("Not a comet XML!")
+        if root.tag != "comet":
+            raise "1"
 
         metadata = GenericMetadata()
         md = metadata
 
         # Helper function
         def xlate(tag):
             node = root.find(tag)
             if node is not None:
                 return node.text
-            else:
-                return None
+            return None
 
-        md.series = xlate('series')
-        md.title = xlate('title')
-        md.issue = xlate('issue')
-        md.volume = xlate('volume')
-        md.comments = xlate('description')
-        md.publisher = xlate('publisher')
-        md.language = xlate('language')
-        md.format = xlate('format')
-        md.pageCount = xlate('pages')
-        md.maturityRating = xlate('rating')
-        md.price = xlate('price')
-        md.isVersionOf = xlate('isVersionOf')
-        md.rights = xlate('rights')
-        md.identifier = xlate('identifier')
-        md.lastMark = xlate('lastMark')
-        md.genre = xlate('genre')  # TODO - repeatable field
+        md.series = xlate("series")
+        md.title = xlate("title")
+        md.issue = xlate("issue")
+        md.volume = xlate("volume")
+        md.comments = xlate("description")
+        md.publisher = xlate("publisher")
+        md.language = xlate("language")
+        md.format = xlate("format")
+        md.page_count = xlate("pages")
+        md.maturity_rating = xlate("rating")
+        md.price = xlate("price")
+        md.is_version_of = xlate("isVersionOf")
+        md.rights = xlate("rights")
+        md.identifier = xlate("identifier")
+        md.last_mark = xlate("lastMark")
+        md.genre = xlate("genre")  # TODO - repeatable field
 
-        date = xlate('date')
+        date = xlate("date")
         if date is not None:
-            parts = date.split('-')
+            parts = date.split("-")
             if len(parts) > 0:
                 md.year = parts[0]
             if len(parts) > 1:
                 md.month = parts[1]
 
-        md.coverImage = xlate('coverImage')
+        md.cover_image = xlate("coverImage")
 
-        readingDirection = xlate('readingDirection')
-        if readingDirection is not None and readingDirection == "rtl":
+        reading_direction = xlate("readingDirection")
+        if reading_direction is not None and reading_direction == "rtl":
             md.manga = "YesAndRightToLeft"
 
         # loop for character tags
         char_list = []
         for n in root:
-            if n.tag == 'character':
+            if n.tag == "character":
                 char_list.append(n.text.strip())
-        md.characters = comicapi.utils.listToString(char_list)
+        md.characters = utils.list_to_string(char_list)
 
         # Now extract the credit info
         for n in root:
-            if (n.tag == 'writer' or n.tag == 'penciller' or n.tag == 'inker'
-                    or n.tag == 'colorist' or n.tag == 'letterer'
-                    or n.tag == 'editor'):
-                metadata.addCredit(n.text.strip(), n.tag.title())
+            if any(
+                [
+                    n.tag == "writer",
+                    n.tag == "penciller",
+                    n.tag == "inker",
+                    n.tag == "colorist",
+                    n.tag == "letterer",
+                    n.tag == "editor",
+                ]
+            ):
+                metadata.add_credit(n.text.strip(), n.tag.title())
 
-            if n.tag == 'coverDesigner':
-                metadata.addCredit(n.text.strip(), "Cover")
+            if n.tag == "coverDesigner":
+                metadata.add_credit(n.text.strip(), "Cover")
 
-        metadata.isEmpty = False
+        metadata.is_empty = False
 
         return metadata
 
     # verify that the string actually contains CoMet data in XML format
-    def validateString(self, string):
+    def validate_string(self, string):
         try:
             tree = ET.ElementTree(ET.fromstring(string))
             root = tree.getroot()
-            if root.tag != 'comet':
+            if root.tag != "comet":
                 raise Exception
         except:
             return False
 
         return True
 
-    def writeToExternalFile(self, filename, metadata):
+    def write_to_external_file(self, filename, metadata):
 
-        tree = self.convertMetadataToXML(self, metadata)
-        tree.write(filename, encoding='utf-8')
+        tree = self.convert_metadata_to_xml(metadata)
+        tree.write(filename, encoding="utf-8")
 
-    def readFromExternalFile(self, filename):
+    def read_from_external_file(self, filename):
 
         tree = ET.parse(filename)
-        return self.convertXMLToMetadata(tree)
+        return self.convert_xml_to_metadata(tree)
```

### Comparing `comicapi-2.2.1/comicapi/comicarchive.py` & `comicapi-3.0.0/comicapi/comicarchive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,328 +1,412 @@
-"""
-A python class to represent a single comic, be it file or folder of images
+"""A class to represent a single comic, be it file or folder of images"""
 
-Copyright 2012-2014  Anthony Beville
+# Copyright 2012-2014 Anthony Beville
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 
-import zipfile
-import tarfile
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import io
+import logging
 import os
+import platform
 import struct
+import subprocess
 import sys
 import tempfile
-import subprocess
-import platform
-import logging
+import time
+import zipfile
+import tarfile
+
+import natsort
+import py7zr
 
-from natsort import natsorted
 try:
     import rarfile
     rarsupport = True
 except (ImportError, SyntaxError):
     rarsupport = False
 
-import time
-
-from io import StringIO
 try:
     from PIL import Image
+
     pil_available = True
 except ImportError:
     pil_available = False
 
+from comicapi.comet import CoMet
+from comicapi.comicbookinfo import ComicBookInfo
+from comicapi.comicinfoxml import ComicInfoXml
+from comicapi.filenameparser import FileNameParser
+from comicapi.genericmetadata import GenericMetadata, PageType
+
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
+if not pil_available:
+    logger.exception("PIL unavalable")
 
 sys.path.insert(0, os.path.abspath("."))
 
-from comicapi.comicinfoxml import ComicInfoXml
-from comicapi.comicbookinfo import ComicBookInfo
-from comicapi.comet import CoMet
-from comicapi.genericmetadata import GenericMetadata, PageType
-from comicapi.filenameparser import FileNameParser
-
 
 class MetaDataStyle:
     CBI = 0
     CIX = 1
     COMET = 2
-    name = ['ComicBookLover', 'ComicRack', 'CoMet']
+    name = ["ComicBookLover", "ComicRack", "CoMet"]
 
 
-class ZipArchiver:
+class SevenZipArchiver:
+
+    """7Z implementation"""
+
     def __init__(self, path):
         self.path = path
 
-    def getArchiveComment(self):
-        zf = zipfile.ZipFile(self.path, 'r')
-        comment = zf.comment
-        zf.close()
-        return comment
-
-    def setArchiveComment(self, comment):
-        return self.writeZipComment(self.path, comment)
+    # @todo: Implement Comment?
+    def get_comment(self):
+        return ""
 
-    def readArchiveFile(self, archive_file):
-        zf = zipfile.ZipFile(self.path, 'r')
+    def set_comment(self, comment):
+        return False
 
+    def read_file(self, archive_file):
+        data = ""
         try:
-            data = zf.read(archive_file)
-        except zipfile.BadZipfile as e:
-            errMsg = u"bad zipfile [{0}]: {1} :: {2}".format(
-                e, self.path, archive_file)
-            logger.info(errMsg)
-            zf.close()
-            raise IOError
+            with py7zr.SevenZipFile(self.path, "r") as zf:
+                data = zf.read(archive_file)[archive_file].read()
+        except py7zr.Bad7zFile as e:
+            logger.error("bad 7zip file [%s]: %s :: %s", e, self.path, archive_file)
+            raise IOError from e
         except Exception as e:
-            zf.close()
-            errMsg = u"bad zipfile [{0}]: {1} :: {2}".format(
-                e, self.path, archive_file)
-            logger.info(errMsg)
-            raise IOError
-        finally:
-            zf.close()
+            logger.error("bad 7zip file [%s]: %s :: %s", e, self.path, archive_file)
+            raise IOError from e
+
         return data
 
-    def removeArchiveFile(self, archive_file):
+    def remove_file(self, archive_file):
         try:
-            self.rebuildZipFile([archive_file])
+            self.rebuild_zip_file([archive_file])
         except:
+            logger.exception("Failed to remove %s from 7zip archive", archive_file)
             return False
         else:
             return True
 
-    def writeArchiveFile(self, archive_file, data):
+    def write_file(self, archive_file, data):
         #  At the moment, no other option but to rebuild the whole
         #  zip archive w/o the indicated file. Very sucky, but maybe
         # another solution can be found
         try:
-            self.rebuildZipFile([archive_file])
+            files = self.get_filename_list()
+            if archive_file in files:
+                self.rebuild_zip_file([archive_file])
 
             # now just add the archive file as a new one
-            zf = zipfile.ZipFile(
-                self.path, mode='a', compression=zipfile.ZIP_DEFLATED)
-            zf.writestr(archive_file, data)
-            zf.close()
+            with py7zr.SevenZipFile(self.path, "a") as zf:
+                zf.writestr(data, archive_file)
             return True
         except:
+            logger.exception("Writing zip file failed")
             return False
 
-    def getArchiveFilenameList(self):
+    def get_filename_list(self):
         try:
-            zf = zipfile.ZipFile(self.path, 'r')
-            namelist = zf.namelist()
-            zf.close()
+            with py7zr.SevenZipFile(self.path, "r") as zf:
+                namelist = zf.getnames()
+
             return namelist
         except Exception as e:
-            errMsg = u"Unable to get zipfile list [{0}]: {1}".format(
-                e, self.path)
-            logger.info(errMsg)
+            logger.error("Unable to get 7zip file list [%s]: %s", e, self.path)
             return []
 
-    # zip helper func
-    def rebuildZipFile(self, exclude_list):
-
-        # this recompresses the zip archive, without the files in the exclude_list
-        # errMsg=u"Rebuilding zip {0} without {1}".format( self.path, exclude_list )
+    def rebuild_zip_file(self, exclude_list):
+        """Zip helper func
 
-        # generate temp file
+        This recompresses the zip archive, without the files in the exclude_list
+        """
         tmp_fd, tmp_name = tempfile.mkstemp(dir=os.path.dirname(self.path))
         os.close(tmp_fd)
 
-        zin = zipfile.ZipFile(self.path, 'r')
-        zout = zipfile.ZipFile(tmp_name, 'w')
-        for item in zin.infolist():
-            buffer = zin.read(item.filename)
-            if item.filename not in exclude_list:
-                zout.writestr(item, buffer)
+        try:
+            with py7zr.SevenZipFile(self.path, "r") as zin:
+                targets = [f for f in zin.getnames() if f not in exclude_list]
+            with py7zr.SevenZipFile(self.path, "r") as zin:
+                with py7zr.SevenZipFile(tmp_name, "w") as zout:
+                    for fname, bio in zin.read(targets).items():
+                        zout.writef(bio, fname)
+        except Exception:
+            logger.exception("Error rebuilding 7zip file: %s", self.path)
 
-        # preserve the old comment
-        zout.comment = zin.comment
+        # replace with the new file
+        os.remove(self.path)
+        os.rename(tmp_name, self.path)
+
+    def copy_from_archive(self, otherArchive):
+        """Replace the current zip with one copied from another archive"""
+        try:
+            with py7zr.SevenZipFile(self.path, "w") as zout:
+                for fname in otherArchive.get_filename_list():
+                    data = otherArchive.read_file(fname)
+                    if data is not None:
+                        zout.writestr(data, fname)
+        except Exception as e:
+            logger.exception("Error while copying to %s: %s", self.path, e)
+            return False
+        else:
+            return True
+
+
+class ZipArchiver:
+
+    """ZIP implementation"""
+
+    def __init__(self, path):
+        self.path = path
+
+    def get_comment(self):
+        with zipfile.ZipFile(self.path, "r") as zf:
+            comment = zf.comment
+        return comment
+
+    def set_comment(self, comment):
+        with zipfile.ZipFile(self.path, "a") as zf:
+            zf.comment = bytes(comment, "utf-8")
+        return True
 
-        zout.close()
-        zin.close()
+    def read_file(self, archive_file):
+        with zipfile.ZipFile(self.path, "r") as zf:
+
+            try:
+                data = zf.read(archive_file)
+            except zipfile.BadZipfile as e:
+                logger.error("bad zipfile [%s]: %s :: %s", e, self.path, archive_file)
+                raise IOError from e
+            except Exception as e:
+                logger.error("bad zipfile [%s]: %s :: %s", e, self.path, archive_file)
+                raise IOError from e
+        return data
+
+    def remove_file(self, archive_file):
+        try:
+            self.rebuild_zip_file([archive_file])
+        except:
+            logger.exception("Failed to remove %s from zip archive", archive_file)
+            return False
+        else:
+            return True
+
+    def write_file(self, archive_file, data):
+        #  At the moment, no other option but to rebuild the whole
+        #  zip archive w/o the indicated file. Very sucky, but maybe
+        # another solution can be found
+        try:
+            files = self.get_filename_list()
+            if archive_file in files:
+                self.rebuild_zip_file([archive_file])
+
+            # now just add the archive file as a new one
+            with zipfile.ZipFile(self.path, mode="a", allowZip64=True, compression=zipfile.ZIP_DEFLATED) as zf:
+                zf.writestr(archive_file, data)
+            return True
+        except Exception as e:
+            logger.error("writing zip file failed [%s]: %s", e, self.path)
+            return False
+
+    def get_filename_list(self):
+        try:
+            with zipfile.ZipFile(self.path, "r") as zf:
+                namelist = zf.namelist()
+            return namelist
+        except Exception as e:
+            logger.error("Unable to get zipfile list [%s]: %s", e, self.path)
+            return []
+
+    def rebuild_zip_file(self, exclude_list):
+        """Zip helper func
+
+        This recompresses the zip archive, without the files in the exclude_list
+        """
+        tmp_fd, tmp_name = tempfile.mkstemp(dir=os.path.dirname(self.path))
+        os.close(tmp_fd)
+
+        try:
+            with zipfile.ZipFile(self.path, "r") as zin:
+                with zipfile.ZipFile(tmp_name, "w", allowZip64=True) as zout:
+                    for item in zin.infolist():
+                        buffer = zin.read(item.filename)
+                        if item.filename not in exclude_list:
+                            zout.writestr(item, buffer)
+
+                    # preserve the old comment
+                    zout.comment = zin.comment
+        except Exception:
+            logger.exception("Error rebuilding zip file: %s", self.path)
 
         # replace with the new file
         os.remove(self.path)
         os.rename(tmp_name, self.path)
 
-    def writeZipComment(self, filename, comment):
+    def write_zip_comment(self, filename, comment):
         """
         This is a custom function for writing a comment to a zip file,
         since the built-in one doesn't seem to work on Windows and Mac OS/X
 
         Fortunately, the zip comment is at the end of the file, and it's
         easy to manipulate.  See this website for more info:
         see: http://en.wikipedia.org/wiki/Zip_(file_format)#Structure
         """
 
+        # get file size
         statinfo = os.stat(filename)
         file_length = statinfo.st_size
 
         try:
-            fo = open(filename, "r+b")
+            with open(filename, "r+b") as fo:
 
-            # the starting position, relative to EOF
-            pos = -4
-
-            found = False
-            value = bytearray()
+                # the starting position, relative to EOF
+                pos = -4
 
-            # walk backwards to find the "End of Central Directory" record
-            while (not found) and (-pos != file_length):
-                # seek, relative to EOF
-                fo.seek(pos, 2)
+                found = False
 
-                value = fo.read(4)
+                # walk backwards to find the "End of Central Directory" record
+                while (not found) and (-pos != file_length):
+                    # seek, relative to EOF
+                    fo.seek(pos, 2)
 
-                # look for the end of central directory signature
-                if bytearray(value) == bytearray([0x50, 0x4b, 0x05, 0x06]):
-                    found = True
-                else:
-                    # not found, step back another byte
-                    pos = pos - 1
-                # print pos,"{1} int: {0:x}".format(bytearray(value)[0], value)
+                    value = fo.read(4)
 
-            if found:
-
-                # now skip forward 20 bytes to the comment length word
-                pos += 20
-                fo.seek(pos, 2)
-
-                # Pack the length of the comment string
-                format = "H"  # one 2-byte integer
-                comment_length = struct.pack(
-                    format, len(comment))  # pack integer in a binary string
+                    # look for the end of central directory signature
+                    if bytearray(value) == bytearray([0x50, 0x4B, 0x05, 0x06]):
+                        found = True
+                    else:
+                        # not found, step back another byte
+                        pos = pos - 1
 
-                # write out the length
-                fo.write(comment_length)
-                fo.seek(pos + 2, 2)
+                if found:
 
-                # write out the comment itself
-                fo.write(comment)
-                fo.truncate()
-                fo.close()
-            else:
-                raise Exception('Failed to write comment to zip file!')
-        except:
+                    # now skip forward 20 bytes to the comment length word
+                    pos += 20
+                    fo.seek(pos, 2)
+
+                    # Pack the length of the comment string
+                    fmt = "H"  # one 2-byte integer
+                    comment_length = struct.pack(fmt, len(comment))  # pack integer in a binary string
+
+                    # write out the length
+                    fo.write(comment_length)
+                    fo.seek(pos + 2, 2)
+
+                    # write out the comment itself
+                    fo.write(bytes(comment))
+                    fo.truncate()
+                else:
+                    raise Exception("Failed to write comment to zip file!")
+        except Exception:
+            logger.exception("Writing comment to %s failed", filename)
             return False
         else:
             return True
 
-    def copyFromArchive(self, otherArchive):
-        # Replace the current zip with one copied from another archive
+    def copy_from_archive(self, other_archive):
+        """Replace the current zip with one copied from another archive"""
         try:
-            zout = zipfile.ZipFile(self.path, 'w')
-            for fname in otherArchive.getArchiveFilenameList():
-                data = otherArchive.readArchiveFile(fname)
-                if data is not None:
-                    zout.writestr(fname, data)
-            zout.close()
+            with zipfile.ZipFile(self.path, "w", allowZip64=True) as zout:
+                for fname in other_archive.get_filename_list():
+                    data = other_archive.read_file(fname)
+                    if data is not None:
+                        zout.writestr(fname, data)
 
             # preserve the old comment
-            comment = otherArchive.getArchiveComment()
+            comment = other_archive.get_comment()
             if comment is not None:
-                if not self.writeZipComment(self.path, comment):
+                if not self.write_zip_comment(self.path, comment):
                     return False
-        except Exception as e:
-            errMsg = u"Error while copying to {0}: {1}".format(self.path, e)
-            logger.info(errMsg)
+        except Exception:
+            logger.exception("Error while copying to %s", self.path)
             return False
         else:
             return True
 
 
 class TarArchiver:
+
+    """TAR implementation"""
+
     def __init__(self, path):
         self.path = path
 
-    def getArchiveComment(self):
+    def get_comment(self):
         tf = tarfile.TarFile(self.path, 'r')
         comment = tf.comment
         tf.close()
         return comment
 
-    def setArchiveComment(self, comment):
-        return self.writeTarComment(self.path, comment)
+    def set_comment(self, comment):
+        return self.write_tar_comment(self.path, comment)
 
-    def readArchiveFile(self, archive_file):
-        tf = tarfile.TarFile(self.path, 'r')
+    def read_file(self, archive_file):
+        with tarfile.TarFile(self.path, 'r') as tf:
 
-        try:
-            data = tf.extractfile(archive_file).read()
-        except tarfile.TarError as e:
-            errMsg = u"bad tarfile [{0}]: {1} :: {2}".format(
-                e, self.path, archive_file)
-            logger.info(errMsg)
-            tf.close()
-            raise IOError
-        except Exception as e:
-            tf.close()
-            errMsg = u"bad tarfile [{0}]: {1} :: {2}".format(
-                e, self.path, archive_file)
-            logger.info(errMsg)
-            raise IOError
-        finally:
-            tf.close()
+            try:
+                data = tf.extractfile(archive_file).read()
+            except tarfile.TarError as e:
+                logger.error("bad tarfile [%s]: %s :: %s", e, self.path, archive_file)
+                raise IOError from e
+            except Exception as e:
+                logger.error("bad tarfile [%s]: %s :: %s", e, self.path, archive_file)
+                raise IOError from e
         return data
 
-    def removeArchiveFile(self, archive_file):
+    def remove_file(self, archive_file):
         try:
-            self.rebuildTarFile([archive_file])
+            self.rebuild_tar_file([archive_file])
         except:
+            logger.exception("Failed to remove %s from tar archive", archive_file)
             return False
         else:
             return True
 
-    def writeArchiveFile(self, archive_file, data):
+    def write_file(self, archive_file, data):
         #  At the moment, no other option but to rebuild the whole
-        #  zip archive w/o the indicated file. Very sucky, but maybe
+        #  tar archive w/o the indicated file. Very sucky, but maybe
         # another solution can be found
         try:
-            self.rebuildTarFile([archive_file])
+            self.rebuild_tar_file([archive_file])
 
             # now just add the archive file as a new one
             tf = tarfile.Tarfile(
                 self.path, mode='a')
             tf.writestr(archive_file, data)
             tf.close()
             return True
-        except:
+        except Exception as e:
+            logger.error("writing tar file failed [%s]: %s", e, self.path)
             return False
 
-    def getArchiveFilenameList(self):
+    def get_filename_list(self):
         try:
-            tf = tarfile.TarFile(self.path, 'r')
-            namelist = tf.getnames()
-            tf.close()
+            with tarfile.TarFile(self.path, 'r') as tf:
+                namelist = tf.getnames()
             return namelist
         except Exception as e:
-            errMsg = u"Unable to get tarfile list [{0}]: {1}".format(
-                e, self.path)
-            logger.info(errMsg)
+            logger.error("Unable to get tarfile list [%s]: %s", e, self.path)
             return []
 
-    # zip helper func
-    def rebuildTarFile(self, exclude_list):
+    # tar helper func
+    def rebuild_tar_file(self, exclude_list):
 
-        # this recompresses the zip archive, without the files in the exclude_list
-        # errMsg=u"Rebuilding zip {0} without {1}".format( self.path, exclude_list )
+        # this recompresses the tar archive, without the files in the exclude_list
 
         # generate temp file
         tmp_fd, tmp_name = tempfile.mkstemp(dir=os.path.dirname(self.path))
         os.close(tmp_fd)
 
         tin = tarfile.TarFile(self.path, 'r')
         tout = tarfile.TarFile(tmp_name, 'w')
@@ -337,15 +421,15 @@
         tout.close()
         tin.close()
 
         # replace with the new file
         os.remove(self.path)
         os.rename(tmp_name, self.path)
 
-    def writeTarComment(self, filename, comment):
+    def write_tar_comment(self, filename, comment):
         """
         This is a custom function for writing a comment to a tar file,
         since the built-in one doesn't seem to work on Windows and Mac OS/X
         """
 
         statinfo = os.stat(filename)
         file_length = statinfo.st_size
@@ -390,580 +474,566 @@
 
                 # write out the comment itself
                 fo.write(comment)
                 fo.truncate()
                 fo.close()
             else:
                 raise Exception('Failed to write comment to tar file!')
-        except:
+        except Exception:
+            logger.exception("Writing comment to %s failed", filename)
             return False
         else:
             return True
 
-    def copyFromArchive(self, otherArchive):
+    def copy_from_archive(self, otherArchive):
         # Replace the current zip with one copied from another archive
         try:
             tout = tarfile.TarFile(self.path, 'w')
-            for fname in otherArchive.getArchiveFilenameList():
-                data = otherArchive.readArchiveFile(fname)
+            for fname in otherArchive.get_filename_list():
+                data = otherArchive.read_file(fname)
                 if data is not None:
                     tout.writestr(fname, data)
             tout.close()
 
             # preserve the old comment
-            comment = otherArchive.getArchiveComment()
+            comment = otherArchive.get_comment()
             if comment is not None:
-                if not self.writeTarComment(self.path, comment):
+                if not self.write_tar_comment(self.path, comment):
                     return False
         except Exception as e:
-            errMsg = u"Error while copying to {0}: {1}".format(self.path, e)
-            logger.info(errMsg)
+            logger.exception("Error while copying to [%s]: %s", self.path, e)
             return False
         else:
             return True
 
-# ------------------------------------------
-# RAR implementation
-
 
-if rarsupport:
-    class RarArchiver:
+class RarArchiver:
+    """RAR implementation"""
 
-        devnull = None
+    devnull = None
 
-        def __init__(self, path, rar_exe_path):
-            self.path = path
-            self.rar_exe_path = rar_exe_path
+    def __init__(self, path, rar_exe_path):
+        self.path = path
+        self.rar_exe_path = rar_exe_path
 
-            if RarArchiver.devnull is None:
-                RarArchiver.devnull = open(os.devnull, "w")
+        if RarArchiver.devnull is None:
+            RarArchiver.devnull = open(os.devnull, "bw")
 
-            # windows only, keeps the cmd.exe from popping up
-            if platform.system() == "Windows":
-                #    self.startupinfo = subprocess.STARTUPINFO()
-                #    self.startupinfo.dwFlags |= _subprocess.STARTF_USESHOWWINDOW
-                self.startupinfo = None
-            else:
-                self.startupinfo = None
+        # windows only, keeps the cmd.exe from popping up
+        if platform.system() == "Windows":
+            self.startupinfo = subprocess.STARTUPINFO()
+            self.startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        else:
+            self.startupinfo = None
 
-        def __del__(self):
-            # RarArchiver.devnull.close()
-            pass
-
-        def getArchiveComment(self):
-
-            rarc = self.getRARObj()
-            return rarc.comment
-
-        def setArchiveComment(self, comment):
-
-            if self.rar_exe_path is not None:
-                try:
-                    # write comment to temp file
-                    tmp_fd, tmp_name = tempfile.mkstemp()
-                    f = os.fdopen(tmp_fd, 'w+b')
-                    f.write(comment)
-                    f.close()
-
-                    working_dir = os.path.dirname(os.path.abspath(self.path))
-
-                    # use external program to write comment to Rar archive
-                    subprocess.call(
-                        [
-                            self.rar_exe_path, 'c', '-w' + working_dir, '-c-',
-                            '-z' + tmp_name, self.path
-                        ],
-                        startupinfo=self.startupinfo,
-                        stdout=RarArchiver.devnull)
+    def get_comment(self):
+        rarc = self.get_rar_obj()
+        return rarc.comment
 
-                    if platform.system() == "Darwin":
-                        time.sleep(1)
+    def set_comment(self, comment):
+        if self.rar_exe_path is not None:
+            try:
+                # write comment to temp file
+                tmp_fd, tmp_name = tempfile.mkstemp()
+                with os.fdopen(tmp_fd, "wb") as f:
+                    f.write(comment.encode("utf-8"))
+
+                working_dir = os.path.dirname(os.path.abspath(self.path))
+
+                # use external program to write comment to Rar archive
+                proc_args = [self.rar_exe_path, "c", "-w" + working_dir, "-c-", "-z" + tmp_name, self.path]
+                subprocess.call(
+                    proc_args,
+                    startupinfo=self.startupinfo,
+                    stdout=RarArchiver.devnull,
+                    stdin=RarArchiver.devnull,
+                    stderr=RarArchiver.devnull,
+                )
 
-                    os.remove(tmp_name)
-                except:
-                    return False
-                else:
-                    return True
-            else:
+                if platform.system() == "Darwin":
+                    time.sleep(1)
+                os.remove(tmp_name)
+            except Exception:
+                logger.exception("Failed to set a comment")
                 return False
+            else:
+                return True
+        else:
+            return False
 
-        def readArchiveFile(self, archive_file):
+    def read_file(self, archive_file):
 
-            # Make sure to escape brackets, since some funky stuff is going on
-            # underneath with "fnmatch"
+        rarc = self.get_rar_obj()
 
-            rarc = self.getRARObj()
+        tries = 0
+        while tries < 7:
+            try:
+                tries = tries + 1
+                data = rarc.open(archive_file).read()
+                entries = [(rarc.getinfo(archive_file), data)]
+
+                if entries[0][0].file_size != len(entries[0][1]):
+                    logger.info(
+                        "read_file(): [file is not expected size: %d vs %d]  %s:%s [attempt # %d]",
+                        entries[0][0].file_size,
+                        len(entries[0][1]),
+                        self.path,
+                        archive_file,
+                        tries,
+                    )
+                    continue
+            except (OSError, IOError) as e:
+                logger.error("read_file(): [%s]  %s:%s attempt #%d", e, self.path, archive_file, tries)
+                time.sleep(1)
+            except Exception as e:
+                logger.error(
+                    "Unexpected exception in read_file(): [%s] for %s:%s attempt #%d", e, self.path, archive_file, tries
+                )
+                break
 
-            tries = 0
-            while tries < 7:
-                try:
-                    tries = tries + 1
-                    data = rarc.read(archive_file)
-                    entries = [(rarc.getinfo(archive_file), data)]
-
-                    if entries[0][0].file_size != len(entries[0][1]):
-                        errMsg = u"readArchiveFile(): " \
-                                 u"[file is not expected size: {0} vs {1}]  {2}:{3} [attempt # {4}]\n".format(
-                            entries[0][0].file_size, len(entries[0][1]), self.path, archive_file, tries)
-                        logger.info(errMsg)
-                        continue
-
-                except (OSError, IOError) as e:
-                    errMsg = u"readArchiveFile(): [{0}]  {1}:{2} attempt#{3}".format(
-                        str(e), self.path, archive_file, tries)
-                    logger.info(errMsg)
-                    time.sleep(1)
-                except Exception as e:
-                    errMsg = u"Unexpected exception in readArchiveFile(): [{0}] for {1}:{2} attempt#{3}".format(
-                        str(e), self.path, archive_file, tries)
-                    logger.info(errMsg)
-                    break
+            else:
+                # Success. Entries is a list of of tuples:  ( rarinfo, filedata)
+                if tries > 1:
+                    logger.info("Attempted read_files() {%d} times", tries)
+                if len(entries) == 1:
+                    return entries[0][1]
 
-                else:
-                    # Success"
-                    # entries is a list of of tuples:  ( rarinfo, filedata)
-                    if tries > 1:
-                        errMsg = u"Attempted read_files() {0} times".format(tries)
-                        logger.info(errMsg)
-                    if len(entries) == 1:
-                        return entries[0][1]
-                    else:
-                        raise IOError
+                raise IOError
 
-            raise IOError
+        raise IOError
 
-        def writeArchiveFile(self, archive_file, data):
+    def write_file(self, archive_file, data):
 
-            if self.rar_exe_path is not None:
-                try:
-                    tmp_folder = tempfile.mkdtemp()
+        if self.rar_exe_path is not None:
+            try:
+                tmp_folder = tempfile.mkdtemp()
 
-                    tmp_file = os.path.join(tmp_folder, archive_file)
+                tmp_file = os.path.join(tmp_folder, archive_file)
 
-                    working_dir = os.path.dirname(os.path.abspath(self.path))
+                working_dir = os.path.dirname(os.path.abspath(self.path))
 
-                    # TODO: will this break if 'archive_file' is in a subfolder. i.e. "foo/bar.txt"
-                    # will need to create the subfolder above, I guess...
-                    f = open(tmp_file, 'w')
+                # TODO: will this break if 'archive_file' is in a subfolder. i.e. "foo/bar.txt"
+                # will need to create the subfolder above, I guess...
+                with open(tmp_file, "wb") as f:
                     f.write(data)
-                    f.close()
 
-                    # use external program to write file to Rar archive
-                    subprocess.call(
-                        [
-                            self.rar_exe_path, 'a', '-w' + working_dir, '-c-',
-                            '-ep', self.path, tmp_file
-                        ],
-                        startupinfo=self.startupinfo,
-                        stdout=RarArchiver.devnull)
-
-                    if platform.system() == "Darwin":
-                        time.sleep(1)
-                    os.remove(tmp_file)
-                    os.rmdir(tmp_folder)
-                except:
-                    return False
-                else:
-                    return True
-            else:
-                return False
+                # use external program to write file to Rar archive
+                subprocess.call(
+                    [self.rar_exe_path, "a", "-w" + working_dir, "-c-", "-ep", self.path, tmp_file],
+                    startupinfo=self.startupinfo,
+                    stdout=RarArchiver.devnull,
+                    stdin=RarArchiver.devnull,
+                    stderr=RarArchiver.devnull,
+                )
 
-        def removeArchiveFile(self, archive_file):
-            if self.rar_exe_path is not None:
-                try:
-                    # use external program to remove file from Rar archive
-                    subprocess.call(
-                        [self.rar_exe_path, 'd', '-c-', self.path, archive_file],
-                        startupinfo=self.startupinfo,
-                        stdout=RarArchiver.devnull)
-
-                    if platform.system() == "Darwin":
-                        time.sleep(1)
-                except:
-                    return False
-                else:
-                    return True
-            else:
+                if platform.system() == "Darwin":
+                    time.sleep(1)
+                os.remove(tmp_file)
+                os.rmdir(tmp_folder)
+            except Exception as e:
+                logger.info(str(e))
+                logger.exception("Failed write %s to rar archive", archive_file)
                 return False
+            else:
+                return True
+        else:
+            return False
 
-        def getArchiveFilenameList(self):
+    def remove_file(self, archive_file):
+        if self.rar_exe_path is not None:
+            try:
+                # use external program to remove file from Rar archive
+                subprocess.call(
+                    [self.rar_exe_path, "d", "-c-", self.path, archive_file],
+                    startupinfo=self.startupinfo,
+                    stdout=RarArchiver.devnull,
+                    stdin=RarArchiver.devnull,
+                    stderr=RarArchiver.devnull,
+                )
 
-            rarc = self.getRARObj()
-            # namelist = [ item.filename for item in rarc.infolist() ]
-            # return namelist
-
-            tries = 0
-            while tries < 7:
-                try:
-                    tries = tries + 1
-                    # namelist = [ item.filename for item in rarc.infolist() ]
-                    namelist = []
-                    for item in rarc.infolist():
-                        if item.file_size != 0:
-                            namelist.append(item.filename)
-
-                except (OSError, IOError) as e:
-                    errMsg = u"getArchiveFilenameList(): [{0}] {1} attempt#{2}".format(
-                        str(e), self.path, tries)
-                    logger.info(errMsg)
+                if platform.system() == "Darwin":
                     time.sleep(1)
+            except:
+                logger.exception("Failed to remove %s from rar archive", archive_file)
+                return False
+            else:
+                return True
+        else:
+            return False
 
-                else:
-                    # Success"
-                    return namelist
+    def get_filename_list(self):
+        rarc = self.get_rar_obj()
+        tries = 0
+        # while tries < 7:
+        try:
+            tries = tries + 1
+            namelist = []
+            for item in rarc.infolist():
+                if item.file_size != 0:
+                    namelist.append(item.filename)
+
+        except (OSError, IOError) as e:
+            logger.error(f"get_filename_list(): [{e}] {self.path} attempt #{tries}".format(str(e), self.path, tries))
+            time.sleep(1)
 
-            raise e
+        else:
+            # Success
+            return namelist
 
-        def getRARObj(self):
-            tries = 0
-            while tries < 7:
-                try:
-                    tries = tries + 1
-                    rarfile.UNRAR_TOOL = self.rar_exe_path
-                    rarc = rarfile.RarFile(self.path)
-
-                except (OSError, IOError) as e:
-                    errMsg = u"getRARObj(): [{0}] {1} attempt#{2}".format(
-                        str(e), self.path, tries)
-                    logger.info(errMsg)
-                    time.sleep(1)
+        return None
 
-                else:
-                    # Success"
-                    return rarc
+    def get_rar_obj(self):
+        tries = 0
+        try:
+            tries = tries + 1
+            rarfile.UNRAR_TOOL = self.rar_exe_path
+            rarc = rarfile.RarFile(self.path)
+
+        except (OSError, IOError) as e:
+            logger.error("getRARObj(): [%s] %s attempt #%s", e, self.path, tries)
+            time.sleep(1)
+
+        else:
+            return rarc
 
-            raise e
+        return None
 
 
-# ------------------------------------------
-# Folder implementation
 class FolderArchiver:
+
+    """Folder implementation"""
+
     def __init__(self, path):
         self.path = path
         self.comment_file_name = "ComicTaggerFolderComment.txt"
 
-    def getArchiveComment(self):
-        return self.readArchiveFile(self.comment_file_name)
+    def get_comment(self):
+        return self.read_file(self.comment_file_name)
 
-    def setArchiveComment(self, comment):
-        return self.writeArchiveFile(self.comment_file_name, comment)
+    def set_comment(self, comment):
+        return self.write_file(self.comment_file_name, comment)
 
-    def readArchiveFile(self, archive_file):
+    def read_file(self, archive_file):
 
         data = ""
         fname = os.path.join(self.path, archive_file)
         try:
-            with open(fname, 'rb') as f:
+            with open(fname, "rb") as f:
                 data = f.read()
-                f.close()
         except IOError:
-            pass
+            logger.exception("Failed to read: %s", fname)
 
         return data
 
-    def writeArchiveFile(self, archive_file, data):
+    def write_file(self, archive_file, data):
 
         fname = os.path.join(self.path, archive_file)
         try:
-            with open(fname, 'w+') as f:
+            with open(fname, "wb") as f:
                 f.write(data)
-                f.close()
         except:
+            logger.exception("Failed to write: %s", fname)
             return False
         else:
             return True
 
-    def removeArchiveFile(self, archive_file):
+    def remove_file(self, archive_file):
 
         fname = os.path.join(self.path, archive_file)
         try:
             os.remove(fname)
         except:
+            logger.exception("Failed to remove: %s", fname)
             return False
         else:
             return True
 
-    def getArchiveFilenameList(self):
-        return self.listFiles(self.path)
+    def get_filename_list(self):
+        return self.list_files(self.path)
 
-    def listFiles(self, folder):
+    def list_files(self, folder):
 
-        itemlist = list()
+        itemlist = []
 
         for item in os.listdir(folder):
             itemlist.append(item)
             if os.path.isdir(item):
-                itemlist.extend(self.listFiles(os.path.join(folder, item)))
+                itemlist.extend(self.list_files(os.path.join(folder, item)))
 
         return itemlist
 
 
-# ------------------------------------------
-# Unknown implementation
 class UnknownArchiver:
+
+    """Unknown implementation"""
+
     def __init__(self, path):
         self.path = path
 
-    def getArchiveComment(self):
+    def get_comment(self):
         return ""
 
-    def setArchiveComment(self, comment):
+    def set_comment(self, comment):
         return False
 
-    def readArchiveFile(self):
+    def read_file(self, archive_file):
         return ""
 
-    def writeArchiveFile(self, archive_file, data):
+    def write_file(self, archive_file, data):
         return False
 
-    def removeArchiveFile(self, archive_file):
+    def remove_file(self, archive_file):
         return False
 
-    def getArchiveFilenameList(self):
+    def get_filename_list(self):
         return []
 
 
-# ------------------------------------------------------------------
 class ComicArchive:
-
     logo_data = None
 
     class ArchiveType:
-        Zip, Rar, Tar, Folder, Pdf, Unknown = range(6)
+        SevenZip, Zip, Tar, Rar, Folder, Pdf, Unknown = list(range(7))
 
     def __init__(self, path, rar_exe_path=None, default_image_path=None):
+        self.cbi_md = None
+        self.cix_md = None
+        self.comet_filename = None
+        self.comet_md = None
+        self.has__cbi = None
+        self.has__cix = None
+        self.has__comet = None
         self.path = path
+        self.page_count = None
+        self.page_list = None
 
         self.rar_exe_path = rar_exe_path
-        self.ci_xml_filename = 'ComicInfo.xml'
-        self.comet_default_filename = 'CoMet.xml'
-        self.resetCache()
+        self.ci_xml_filename = "ComicInfo.xml"
+        self.comet_default_filename = "CoMet.xml"
+        self.reset_cache()
         self.default_image_path = default_image_path
 
         # Use file extension to decide which archive test we do first
         ext = os.path.splitext(path)[1].lower()
 
         self.archive_type = self.ArchiveType.Unknown
         self.archiver = UnknownArchiver(self.path)
 
-        if rarsupport and ext == ".cbr" or ext == ".rar":
-            if self.rarTest():
+        if ext in [".cbr", ".rar"]:
+            if self.rar_test():
                 self.archive_type = self.ArchiveType.Rar
-                self.archiver = RarArchiver(
-                    self.path, rar_exe_path=self.rar_exe_path)
+                self.archiver = RarArchiver(self.path, rar_exe_path=self.rar_exe_path)
 
-            elif self.zipTest():
+            elif self.zip_test():
                 self.archive_type = self.ArchiveType.Zip
                 self.archiver = ZipArchiver(self.path)
         else:
-            if self.zipTest():
+            if self.sevenzip_test():
+                self.archive_type = self.ArchiveType.SevenZip
+                self.archiver = SevenZipArchiver(self.path)
+
+            elif self.zip_test():
                 self.archive_type = self.ArchiveType.Zip
                 self.archiver = ZipArchiver(self.path)
 
-            if self.tarTest():
+            elif self.tar_test():
                 self.archive_type = self.ArchiveType.Tar
                 self.archiver = TarArchiver(self.path)
 
-            elif self.rarTest():
+            elif self.rar_test():
                 self.archive_type = self.ArchiveType.Rar
-                self.archiver = RarArchiver(
-                    self.path, rar_exe_path=self.rar_exe_path)
+                self.archiver = RarArchiver(self.path, rar_exe_path=self.rar_exe_path)
 
         if ComicArchive.logo_data is None and self.default_image_path:
             fname = self.default_image_path
-            with open(fname, 'rb') as fd:
+            with open(fname, "rb") as fd:
                 ComicArchive.logo_data = fd.read()
 
-    # Clears the cached data
-    def resetCache(self):
-        self.has_cix = None
-        self.has_cbi = None
-        self.has_comet = None
+    def reset_cache(self):
+        """Clears the cached data"""
+
+        self.has__cix = None
+        self.has__cbi = None
+        self.has__comet = None
         self.comet_filename = None
         self.page_count = None
         self.page_list = None
         self.cix_md = None
         self.cbi_md = None
         self.comet_md = None
 
-    def loadCache(self, style_list):
+    def load_cache(self, style_list):
         for style in style_list:
-            self.readMetadata(style)
+            self.read_metadata(style)
 
     def rename(self, path):
         self.path = path
         self.archiver.path = path
 
-    def zipTest(self):
+    def sevenzip_test(self):
+        return py7zr.is_7zfile(self.path)
+
+    def zip_test(self):
         return zipfile.is_zipfile(self.path)
 
-    def tarTest(self):
+    def tar_test(self):
         return tarfile.is_tarfile(self.path)
 
-    def rarTest(self):
+    def rar_test(self):
         try:
             rarc = rarfile.RarFile(self.path)
         except:  # InvalidRARArchive:
             return False
         else:
             return True
 
-    def isZip(self):
+    def is_sevenzip(self):
+        return self.archive_type == self.ArchiveType.SevenZip
+
+    def is_zip(self):
         return self.archive_type == self.ArchiveType.Zip
 
-    def isTar(self):
+    def is_tar(self):
         return self.archive_type == self.ArchiveType.Tar
 
-    def isRar(self):
+    def is_rar(self):
         return self.archive_type == self.ArchiveType.Rar
 
-    def isPdf(self):
+    def is_pdf(self):
         return self.archive_type == self.ArchiveType.Pdf
 
-    def isFolder(self):
+    def is_folder(self):
         return self.archive_type == self.ArchiveType.Folder
 
-    def isWritable(self, check_rar_status=True):
+    def is_writable(self, check_rar_status=True):
         if self.archive_type == self.ArchiveType.Unknown:
             return False
 
-        elif check_rar_status and self.isRar() and self.rar_exe_path is None:
+        if check_rar_status and self.is_rar() and not self.rar_exe_path:
             return False
 
-        elif not os.access(self.path, os.W_OK):
+        if not os.access(self.path, os.W_OK):
             return False
 
-        elif ((self.archive_type != self.ArchiveType.Folder)
-              and (not os.access(
-                  os.path.dirname(os.path.abspath(self.path)), os.W_OK))):
+        if (self.archive_type != self.ArchiveType.Folder) and (
+            not os.access(os.path.dirname(os.path.abspath(self.path)), os.W_OK)
+        ):
             return False
 
         return True
 
-    def isWritableForStyle(self, data_style):
+    def is_writable_for_style(self, data_style):
 
-        if self.isRar() and data_style == MetaDataStyle.CBI:
+        if (self.is_rar() or self.is_sevenzip()) and data_style == MetaDataStyle.CBI:
             return False
 
-        return self.isWritable()
+        return self.is_writable()
 
-    def seemsToBeAComicArchive(self):
-
-        if ((self.isZip() or self.isRar() or self.isPdf() or self.isTar()
-             )
-                and (self.getNumberOfPages() > 0)):
+    def seems_to_be_a_comic_archive(self):
+        if (self.is_zip() or self.is_rar() or self.is_sevenzip() or self.is_tar()) and (self.get_number_of_pages() > 0):
             return True
-        else:
-            return False
 
-    def readMetadata(self, style):
+        return False
+
+    def read_metadata(self, style):
 
         if style == MetaDataStyle.CIX:
-            return self.readCIX()
-        elif style == MetaDataStyle.CBI:
-            return self.readCBI()
-        elif style == MetaDataStyle.COMET:
-            return self.readCoMet()
-        else:
-            return GenericMetadata()
-
-    def writeMetadata(self, metadata, style):
+            return self.read_cix()
+        if style == MetaDataStyle.CBI:
+            return self.read_cbi()
+        if style == MetaDataStyle.COMET:
+            return self.read_comet()
+        return GenericMetadata()
 
+    def write_metadata(self, metadata, style):
         retcode = None
         if style == MetaDataStyle.CIX:
-            retcode = self.writeCIX(metadata)
-        elif style == MetaDataStyle.CBI:
-            retcode = self.writeCBI(metadata)
-        elif style == MetaDataStyle.COMET:
-            retcode = self.writeCoMet(metadata)
+            retcode = self.write_cix(metadata)
+        if style == MetaDataStyle.CBI:
+            retcode = self.write_cbi(metadata)
+        if style == MetaDataStyle.COMET:
+            retcode = self.write_comet(metadata)
         return retcode
 
-    def hasMetadata(self, style):
-
+    def has_metadata(self, style):
         if style == MetaDataStyle.CIX:
-            return self.hasCIX()
-        elif style == MetaDataStyle.CBI:
-            return self.hasCBI()
-        elif style == MetaDataStyle.COMET:
-            return self.hasCoMet()
-        else:
-            return False
+            return self.has_cix()
+        if style == MetaDataStyle.CBI:
+            return self.has_cbi()
+        if style == MetaDataStyle.COMET:
+            return self.has_comet()
+        return False
 
-    def removeMetadata(self, style):
+    def remove_metadata(self, style):
         retcode = True
         if style == MetaDataStyle.CIX:
-            retcode = self.removeCIX()
+            retcode = self.remove_cix()
         elif style == MetaDataStyle.CBI:
-            retcode = self.removeCBI()
+            retcode = self.remove_cbi()
         elif style == MetaDataStyle.COMET:
-            retcode = self.removeCoMet()
+            retcode = self.remove_co_met()
         return retcode
 
-    def getPage(self, index):
-
+    def get_page(self, index):
         image_data = None
 
-        filename = self.getPageName(index)
+        filename = self.get_page_name(index)
 
         if filename is not None:
             try:
-                image_data = self.archiver.readArchiveFile(filename)
+                image_data = self.archiver.read_file(filename)
             except IOError:
-                errMsg = u"Error reading in page. Substituting logo page."
-                logger.info(errMsg)
+                logger.exception("Error reading in page. Substituting logo page.")
                 image_data = ComicArchive.logo_data
 
         return image_data
 
-    def getPageName(self, index):
-
+    def get_page_name(self, index):
         if index is None:
             return None
 
-        page_list = self.getPageNameList()
+        page_list = self.get_page_name_list()
 
         num_pages = len(page_list)
         if num_pages == 0 or index >= num_pages:
             return None
 
         return page_list[index]
 
-    def getScannerPageIndex(self):
-
+    def get_scanner_page_index(self):
         scanner_page_index = None
 
         # make a guess at the scanner page
-        name_list = self.getPageNameList()
-        count = self.getNumberOfPages()
+        name_list = self.get_page_name_list()
+        count = self.get_number_of_pages()
 
         # too few pages to really know
         if count < 5:
             return None
 
-        # count the length of every filename, and count occurences
-        length_buckets = dict()
+        # count the length of every filename, and count occurrences
+        length_buckets = {}
         for name in name_list:
             fname = os.path.split(name)[1]
             length = len(fname)
             if length in length_buckets:
                 length_buckets[length] += 1
             else:
                 length_buckets[length] = 1
 
         # sort by most common
-        sorted_buckets = sorted(
-            length_buckets.items(), key=lambda k, v: (v, k), reverse=True)
+        sorted_buckets = sorted(iter(length_buckets.items()), key=lambda k_v: (k_v[1], k_v[0]), reverse=True)
 
-        # statistical mode occurence is first
+        # statistical mode occurrence is first
         mode_length = sorted_buckets[0][0]
 
         # we are only going to consider the final image file:
         final_name = os.path.split(name_list[count - 1])[1]
 
-        common_length_list = list()
+        common_length_list = []
         for name in name_list:
             if len(os.path.split(name)[1]) == mode_length:
                 common_length_list.append(os.path.split(name)[1])
 
         prefix = os.path.commonprefix(common_length_list)
 
         if mode_length <= 7 and prefix == "":
@@ -973,309 +1043,303 @@
 
         # see if the last page doesn't start with the same prefix as most others
         elif not final_name.startswith(prefix):
             scanner_page_index = count - 1
 
         return scanner_page_index
 
-    def getPageNameList(self, sort_list=True):
-
+    def get_page_name_list(self, sort_list=True):
         if self.page_list is None:
             # get the list file names in the archive, and sort
-            files = self.archiver.getArchiveFilenameList()
+            files = self.archiver.get_filename_list()
 
-            # seems like some archive creators are on  Windows, and don't know about case-sensitivity!
+            # seems like some archive creators are on Windows, and don't know about case-sensitivity!
             if sort_list:
 
-                def keyfunc(k):
-                    # hack to account for some weird scanner ID pages
-                    # basename=os.path.split(k)[1]
-                    # if basename < '0':
-                    #	k = os.path.join(os.path.split(k)[0], "z" + basename)
-                    return k.lower()
-
-                files = natsorted(files, key=keyfunc)  #, signed=False)
+                files = natsort.natsorted(files, alg=natsort.ns.IC | natsort.ns.I | natsort.ns.U)
 
             # make a sub-list of image files
             self.page_list = []
             for name in files:
-                if (name[-4:].lower() in [
-                        ".jpg", "jpeg", ".png", ".gif", "webp", ".bmp"
-                ] and os.path.basename(name)[0] != "."):
+                if (
+                    os.path.splitext(name)[1].lower() in [".jpg", ".jpeg", ".png", ".gif", ".webp", ".bmp"]
+                    and os.path.basename(name)[0] != "."
+                ):
                     self.page_list.append(name)
 
         return self.page_list
 
-    def getNumberOfPages(self):
-
+    def get_number_of_pages(self):
         if self.page_count is None:
-            self.page_count = len(self.getPageNameList())
+            self.page_count = len(self.get_page_name_list())
         return self.page_count
 
-    def readCBI(self):
+    def read_cbi(self):
         if self.cbi_md is None:
-            raw_cbi = self.readRawCBI()
+            raw_cbi = self.read_raw_cbi()
             if raw_cbi is None:
                 self.cbi_md = GenericMetadata()
             else:
-                self.cbi_md = ComicBookInfo().metadataFromString(raw_cbi)
+                self.cbi_md = ComicBookInfo().metadata_from_string(raw_cbi)
 
-            self.cbi_md.setDefaultPageList(self.getNumberOfPages())
+            self.cbi_md.set_default_page_list(self.get_number_of_pages())
 
         return self.cbi_md
 
-    def readRawCBI(self):
-        if not self.hasCBI():
+    def read_raw_cbi(self):
+        if not self.has_cbi():
             return None
-        else:
-            return self.archiver.getArchiveComment()
 
-    def hasCBI(self):
-        if self.has_cbi is None:
+        return self.archiver.get_comment()
 
-            # if ( not ( self.isZip() or self.isRar()) or not self.seemsToBeAComicArchive() ):
-            if not self.seemsToBeAComicArchive():
-                self.has_cbi = False
+    def has_cbi(self):
+        if self.has__cbi is None:
+            if not self.seems_to_be_a_comic_archive():
+                self.has__cbi = False
             else:
-                comment = self.archiver.getArchiveComment()
-                self.has_cbi = ComicBookInfo().validateString(comment)
+                comment = self.archiver.get_comment()
+                self.has__cbi = ComicBookInfo().validate_string(comment)
 
-        return self.has_cbi
+        return self.has__cbi
 
-    def writeCBI(self, metadata):
+    def write_cbi(self, metadata):
         if metadata is not None:
-            self.applyArchiveInfoToMetadata(metadata)
-            cbi_string = ComicBookInfo().stringFromMetadata(metadata)
-            write_success = self.archiver.setArchiveComment(cbi_string)
+            self.apply_archive_info_to_metadata(metadata)
+            cbi_string = ComicBookInfo().string_from_metadata(metadata)
+            write_success = self.archiver.set_comment(cbi_string)
             if write_success:
-                self.has_cbi = True
+                self.has__cbi = True
                 self.cbi_md = metadata
-            self.resetCache()
+            self.reset_cache()
             return write_success
-        else:
-            return False
 
-    def removeCBI(self):
-        if self.hasCBI():
-            write_success = self.archiver.setArchiveComment("")
+        return False
+
+    def remove_cbi(self):
+        if self.has_cbi():
+            write_success = self.archiver.set_comment("")
             if write_success:
-                self.has_cbi = False
+                self.has__cbi = False
                 self.cbi_md = None
-            self.resetCache()
+            self.reset_cache()
             return write_success
         return True
 
-    def readCIX(self):
+    def read_cix(self):
         if self.cix_md is None:
-            raw_cix = self.readRawCIX()
+            raw_cix = self.read_raw_cix()
             if raw_cix is None or raw_cix == "":
                 self.cix_md = GenericMetadata()
             else:
-                self.cix_md = ComicInfoXml().metadataFromString(raw_cix)
+                self.cix_md = ComicInfoXml().metadata_from_string(raw_cix)
 
             # validate the existing page list (make sure count is correct)
             if len(self.cix_md.pages) != 0:
-                if len(self.cix_md.pages) != self.getNumberOfPages():
+                if len(self.cix_md.pages) != self.get_number_of_pages():
                     # pages array doesn't match the actual number of images we're seeing
                     # in the archive, so discard the data
                     self.cix_md.pages = []
 
             if len(self.cix_md.pages) == 0:
-                self.cix_md.setDefaultPageList(self.getNumberOfPages())
+                self.cix_md.set_default_page_list(self.get_number_of_pages())
 
         return self.cix_md
 
-    def readRawCIX(self):
-        if not self.hasCIX():
+    def read_raw_cix(self):
+        if not self.has_cix():
             return None
         try:
-            raw_cix = self.archiver.readArchiveFile(self.ci_xml_filename)
-        except IOError:
-            print("Error reading in raw CIX!")
+            raw_cix = self.archiver.read_file(self.ci_xml_filename)
+        except IOError as e:
+            logger.error("Error reading in raw CIX!: %s", e)
             raw_cix = ""
         return raw_cix
 
-    def writeCIX(self, metadata):
-
+    def write_cix(self, metadata):
         if metadata is not None:
-            self.applyArchiveInfoToMetadata(metadata, calc_page_sizes=True)
-            cix_string = ComicInfoXml().stringFromMetadata(metadata)
-            write_success = self.archiver.writeArchiveFile(
-                self.ci_xml_filename, cix_string)
+            self.apply_archive_info_to_metadata(metadata, calc_page_sizes=True)
+            raw_cix = self.read_raw_cix()
+            if raw_cix == "":
+                raw_cix = None
+            cix_string = ComicInfoXml().string_from_metadata(metadata, xml=raw_cix)
+            write_success = self.archiver.write_file(self.ci_xml_filename, cix_string.encode("utf-8"))
             if write_success:
-                self.has_cix = True
+                self.has__cix = True
                 self.cix_md = metadata
-            self.resetCache()
+            self.reset_cache()
             return write_success
-        else:
-            return False
 
-    def removeCIX(self):
-        if self.hasCIX():
-            write_success = self.archiver.removeArchiveFile(
-                self.ci_xml_filename)
+        return False
+
+    def remove_cix(self):
+        if self.has_cix():
+            write_success = self.archiver.remove_file(self.ci_xml_filename)
             if write_success:
-                self.has_cix = False
+                self.has__cix = False
                 self.cix_md = None
-            self.resetCache()
+            self.reset_cache()
             return write_success
         return True
 
-    def hasCIX(self):
-        if self.has_cix is None:
+    def has_cix(self):
+        if self.has__cix is None:
 
-            if not self.seemsToBeAComicArchive():
-                self.has_cix = False
-            elif self.ci_xml_filename in self.archiver.getArchiveFilenameList(
-            ):
-                self.has_cix = True
+            if not self.seems_to_be_a_comic_archive():
+                self.has__cix = False
+            elif self.ci_xml_filename in self.archiver.get_filename_list():
+                self.has__cix = True
             else:
-                self.has_cix = False
-        return self.has_cix
+                self.has__cix = False
+        return self.has__cix
 
-    def readCoMet(self):
+    def read_comet(self):
         if self.comet_md is None:
-            raw_comet = self.readRawCoMet()
+            raw_comet = self.read_raw_comet()
             if raw_comet is None or raw_comet == "":
                 self.comet_md = GenericMetadata()
             else:
-                self.comet_md = CoMet().metadataFromString(raw_comet)
+                self.comet_md = CoMet().metadata_from_string(raw_comet)
 
-            self.comet_md.setDefaultPageList(self.getNumberOfPages())
+            self.comet_md.set_default_page_list(self.get_number_of_pages())
             # use the coverImage value from the comet_data to mark the cover in this struct
             # walk through list of images in file, and find the matching one for md.coverImage
             # need to remove the existing one in the default
-            if self.comet_md.coverImage is not None:
+            if self.comet_md.cover_image is not None:
                 cover_idx = 0
-                for idx, f in enumerate(self.getPageNameList()):
-                    if self.comet_md.coverImage == f:
+                for idx, f in enumerate(self.get_page_name_list()):
+                    if self.comet_md.cover_image == f:
                         cover_idx = idx
                         break
                 if cover_idx != 0:
-                    del (self.comet_md.pages[0]['Type'])
-                    self.comet_md.pages[cover_idx][
-                        'Type'] = PageType.FrontCover
+                    del self.comet_md.pages[0]["Type"]
+                    self.comet_md.pages[cover_idx]["Type"] = PageType.FrontCover
 
         return self.comet_md
 
-    def readRawCoMet(self):
-        if not self.hasCoMet():
-            errMsg = u"{} doesn't have CoMet data!".format(self.path)
-            logger.info(errMsg)
+    def read_raw_comet(self):
+        if not self.has_comet():
+            logger.info("%s doesn't have CoMet data!", self.path)
             return None
 
         try:
-            raw_comet = self.archiver.readArchiveFile(self.comet_filename)
-        except IOError:
-            errMsg = u"Error reading in raw CoMet!"
-            logger.info(errMsg)
+            raw_comet = self.archiver.read_file(self.comet_filename)
+        except:
+            logger.exception("Error reading in raw CoMet!")
             raw_comet = ""
         return raw_comet
 
-    def writeCoMet(self, metadata):
+    def write_comet(self, metadata):
 
         if metadata is not None:
-            if not self.hasCoMet():
+            if not self.has_comet():
                 self.comet_filename = self.comet_default_filename
 
-            self.applyArchiveInfoToMetadata(metadata)
+            self.apply_archive_info_to_metadata(metadata)
             # Set the coverImage value, if it's not the first page
-            cover_idx = int(metadata.getCoverPageIndexList()[0])
+            cover_idx = int(metadata.get_cover_page_index_list()[0])
             if cover_idx != 0:
-                metadata.coverImage = self.getPageName(cover_idx)
+                metadata.cover_image = self.get_page_name(cover_idx)
 
-            comet_string = CoMet().stringFromMetadata(metadata)
-            write_success = self.archiver.writeArchiveFile(
-                self.comet_filename, comet_string)
+            comet_string = CoMet().string_from_metadata(metadata)
+            write_success = self.archiver.write_file(self.comet_filename, comet_string)
             if write_success:
-                self.has_comet = True
+                self.has__comet = True
                 self.comet_md = metadata
-            self.resetCache()
+            self.reset_cache()
             return write_success
-        else:
-            return False
 
-    def removeCoMet(self):
-        if self.hasCoMet():
-            write_success = self.archiver.removeArchiveFile(
-                self.comet_filename)
+        return False
+
+    def remove_co_met(self):
+        if self.has_comet():
+            write_success = self.archiver.remove_file(self.comet_filename)
             if write_success:
-                self.has_comet = False
+                self.has__comet = False
                 self.comet_md = None
-            self.resetCache()
+            self.reset_cache()
             return write_success
         return True
 
-    def hasCoMet(self):
-        if self.has_comet is None:
-            self.has_comet = False
-            if not self.seemsToBeAComicArchive():
-                return self.has_comet
+    def has_comet(self):
+        if self.has__comet is None:
+            self.has__comet = False
+            if not self.seems_to_be_a_comic_archive():
+                return self.has__comet
 
             # look at all xml files in root, and search for CoMet data, get first
-            for n in self.archiver.getArchiveFilenameList():
-                if (os.path.dirname(n) == ""
-                        and os.path.splitext(n)[1].lower() == '.xml'):
+            for n in self.archiver.get_filename_list():
+                if os.path.dirname(n) == "" and os.path.splitext(n)[1].lower() == ".xml":
                     # read in XML file, and validate it
                     try:
-                        data = self.archiver.readArchiveFile(n)
-                    except:
+                        data = self.archiver.read_file(n)
+                    except Exception as e:
                         data = ""
-                        errMsg = u"Error reading in Comet XML for validation!"
-                        logger.info(errMsg)
-                    if CoMet().validateString(data):
+                        logger.warning("Error reading in Comet XML for validation!: %s", e)
+                    if CoMet().validate_string(data):
                         # since we found it, save it!
                         self.comet_filename = n
-                        self.has_comet = True
+                        self.has__comet = True
                         break
 
-            return self.has_comet
+        return self.has__comet
 
-    def applyArchiveInfoToMetadata(self, md, calc_page_sizes=False):
-        md.pageCount = self.getNumberOfPages()
+    def apply_archive_info_to_metadata(self, md, calc_page_sizes=False):
+        md.page_count = self.get_number_of_pages()
 
         if calc_page_sizes:
             for p in md.pages:
-                idx = int(p['Image'])
+                idx = int(p["Image"])
                 if pil_available:
-                    if 'ImageSize' not in p or 'ImageHeight' not in p or 'ImageWidth' not in p:
-                        data = self.getPage(idx)
+                    if "ImageSize" not in p or "ImageHeight" not in p or "ImageWidth" not in p:
+                        data = self.get_page(idx)
                         if data is not None:
                             try:
-                                im = Image.open(StringIO(data))
+                                if isinstance(data, bytes):
+                                    im = Image.open(io.BytesIO(data))
+                                else:
+                                    im = Image.open(io.StringIO(data))
                                 w, h = im.size
 
-                                p['ImageSize'] = str(len(data))
-                                p['ImageHeight'] = str(h)
-                                p['ImageWidth'] = str(w)
-                            except IOError:
-                                p['ImageSize'] = str(len(data))
+                                p["ImageSize"] = str(len(data))
+                                p["ImageHeight"] = str(h)
+                                p["ImageWidth"] = str(w)
+                            except Exception as e:
+                                logger.warning("decoding image failed: %s", e)
+                                p["ImageSize"] = str(len(data))
 
                 else:
-                    if 'ImageSize' not in p:
-                        data = self.getPage(idx)
-                        p['ImageSize'] = str(len(data))
+                    if "ImageSize" not in p:
+                        data = self.get_page(idx)
+                        p["ImageSize"] = str(len(data))
 
-    def metadataFromFilename(self, parse_scan_info=True):
+    def metadata_from_filename(self, parse_scan_info=True):
 
         metadata = GenericMetadata()
 
         fnp = FileNameParser()
-        fnp.parseFilename(self.path)
+        fnp.parse_filename(self.path)
 
         if fnp.issue != "":
             metadata.issue = fnp.issue
         if fnp.series != "":
             metadata.series = fnp.series
         if fnp.volume != "":
             metadata.volume = fnp.volume
         if fnp.year != "":
             metadata.year = fnp.year
         if fnp.issue_count != "":
-            metadata.issueCount = fnp.issue_count
+            metadata.issue_count = fnp.issue_count
         if parse_scan_info:
             if fnp.remainder != "":
-                metadata.scanInfo = fnp.remainder
+                metadata.scan_info = fnp.remainder
 
-        metadata.isEmpty = False
+        metadata.is_empty = False
 
         return metadata
+
+    def export_as_zip(self, zipfilename):
+        if self.archive_type == self.ArchiveType.Zip:
+            # nothing to do, we're already a zip
+            return True
+
+        zip_archiver = ZipArchiver(zipfilename)
+        return zip_archiver.copy_from_archive(self.archiver)
```

### Comparing `comicapi-2.2.1/comicapi/comicbookinfo.py` & `comicapi-3.0.0/comicapi/comicbookinfo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,147 +1,123 @@
-"""
-A python class to encapsulate the ComicBookInfo data
+"""A class to encapsulate the ComicBookInfo data"""
 
-Copyright 2012-2014  Anthony Beville
+# Copyright 2012-2014 Anthony Beville
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import json
+import logging
+from collections import defaultdict
 from datetime import datetime
 
+from comicapi import utils
 from comicapi.genericmetadata import GenericMetadata
-import comicapi.utils
+
+logger = logging.getLogger(__name__)
 
 
 class ComicBookInfo:
-    def metadataFromString(self, string):
+    def metadata_from_string(self, string):
 
-        cbi_container = json.loads(str(string, 'utf-8'))
+        cbi_container = json.loads(str(string, "utf-8"))
 
         metadata = GenericMetadata()
 
-        cbi = cbi_container['ComicBookInfo/1.0']
+        cbi = defaultdict(lambda: None, cbi_container["ComicBookInfo/1.0"])
 
-        # helper func
-        # If item is not in CBI, return None
-        def xlate(cbi_entry):
-            if cbi_entry in cbi:
-                return cbi[cbi_entry]
-            else:
-                return None
-
-        metadata.series = xlate('series')
-        metadata.title = xlate('title')
-        metadata.issue = xlate('issue')
-        metadata.publisher = xlate('publisher')
-        metadata.month = xlate('publicationMonth')
-        metadata.year = xlate('publicationYear')
-        metadata.issueCount = xlate('numberOfIssues')
-        metadata.comments = xlate('comments')
-        metadata.credits = xlate('credits')
-        metadata.genre = xlate('genre')
-        metadata.volume = xlate('volume')
-        metadata.volumeCount = xlate('numberOfVolumes')
-        metadata.language = xlate('language')
-        metadata.country = xlate('country')
-        metadata.criticalRating = xlate('rating')
-        metadata.tags = xlate('tags')
+        metadata.series = utils.xlate(cbi["series"])
+        metadata.title = utils.xlate(cbi["title"])
+        metadata.issue = utils.xlate(cbi["issue"])
+        metadata.publisher = utils.xlate(cbi["publisher"])
+        metadata.month = utils.xlate(cbi["publicationMonth"], True)
+        metadata.year = utils.xlate(cbi["publicationYear"], True)
+        metadata.issue_count = utils.xlate(cbi["numberOfIssues"], True)
+        metadata.comments = utils.xlate(cbi["comments"])
+        metadata.genre = utils.xlate(cbi["genre"])
+        metadata.volume = utils.xlate(cbi["volume"], True)
+        metadata.volume_count = utils.xlate(cbi["numberOfVolumes"], True)
+        metadata.language = utils.xlate(cbi["language"])
+        metadata.country = utils.xlate(cbi["country"])
+        metadata.critical_rating = utils.xlate(cbi["rating"])
+
+        metadata.credits = cbi["credits"]
+        metadata.tags = cbi["tags"]
 
         # make sure credits and tags are at least empty lists and not None
         if metadata.credits is None:
             metadata.credits = []
         if metadata.tags is None:
             metadata.tags = []
 
-        # need to massage the language string to be ISO
+        # need the language string to be ISO
         if metadata.language is not None:
-            # reverse look-up
-            pattern = metadata.language
-            metadata.language = None
-            for key in comicapi.utils.getLanguageDict():
-                if comicapi.utils.getLanguageDict()[key] == pattern.encode(
-                        'utf-8'):
-                    metadata.language = key
-                    break
+            metadata.language = utils.get_language(metadata.language)
 
-        metadata.isEmpty = False
+        metadata.is_empty = False
 
         return metadata
 
-    def stringFromMetadata(self, metadata):
+    def string_from_metadata(self, metadata):
 
-        cbi_container = self.createJSONDictionary(metadata)
+        cbi_container = self.create_json_dictionary(metadata)
         return json.dumps(cbi_container)
 
-    # verify that the string actually contains CBI data in JSON format
-    def validateString(self, string):
+    def validate_string(self, string):
+        """Verify that the string actually contains CBI data in JSON format"""
 
         try:
             cbi_container = json.loads(string)
         except:
             return False
 
-        return 'ComicBookInfo/1.0' in cbi_container
+        return "ComicBookInfo/1.0" in cbi_container
 
-    def createJSONDictionary(self, metadata):
+    def create_json_dictionary(self, metadata):
+        """Create the dictionary that we will convert to JSON text"""
 
-        # Create the dictionary that we will convert to JSON text
-        cbi = dict()
+        cbi = {}
         cbi_container = {
-            'appID': 'ComicTagger/' + '1.0.0',  # ctversion.version,
-            'lastModified': str(datetime.now()),
-            'ComicBookInfo/1.0': cbi
-        }
+            "appID": "ComicTagger/" + "1.0.0",
+            "lastModified": str(datetime.now()),
+            "ComicBookInfo/1.0": cbi,
+        }  # TODO: ctversion.version,
 
         # helper func
         def assign(cbi_entry, md_entry):
-            if md_entry is not None:
+            if md_entry is not None or isinstance(md_entry, str) and md_entry != "":
                 cbi[cbi_entry] = md_entry
 
-        # helper func
-        def toInt(s):
-            i = None
-            if type(s) in [str, int]:
-                try:
-                    i = int(s)
-                except ValueError:
-                    pass
-            return i
-
-        assign('series', metadata.series)
-        assign('title', metadata.title)
-        assign('issue', metadata.issue)
-        assign('publisher', metadata.publisher)
-        assign('publicationMonth', toInt(metadata.month))
-        assign('publicationYear', toInt(metadata.year))
-        assign('numberOfIssues', toInt(metadata.issueCount))
-        assign('comments', metadata.comments)
-        assign('genre', metadata.genre)
-        assign('volume', toInt(metadata.volume))
-        assign('numberOfVolumes', toInt(metadata.volumeCount))
-        assign('language', comicapi.utils.getLanguageFromISO(
-            metadata.language))
-        assign('country', metadata.country)
-        assign('rating', metadata.criticalRating)
-        assign('credits', metadata.credits)
-        assign('tags', metadata.tags)
+        assign("series", utils.xlate(metadata.series))
+        assign("title", utils.xlate(metadata.title))
+        assign("issue", utils.xlate(metadata.issue))
+        assign("publisher", utils.xlate(metadata.publisher))
+        assign("publicationMonth", utils.xlate(metadata.month, True))
+        assign("publicationYear", utils.xlate(metadata.year, True))
+        assign("numberOfIssues", utils.xlate(metadata.issue_count, True))
+        assign("comments", utils.xlate(metadata.comments))
+        assign("genre", utils.xlate(metadata.genre))
+        assign("volume", utils.xlate(metadata.volume, True))
+        assign("numberOfVolumes", utils.xlate(metadata.volume_count, True))
+        assign("language", utils.xlate(utils.get_language_from_iso(metadata.language)))
+        assign("country", utils.xlate(metadata.country))
+        assign("rating", utils.xlate(metadata.critical_rating))
+        assign("credits", metadata.credits)
+        assign("tags", metadata.tags)
 
         return cbi_container
 
-    def writeToExternalFile(self, filename, metadata):
+    def write_to_external_file(self, filename, metadata):
 
-        cbi_container = self.createJSONDictionary(metadata)
+        cbi_container = self.create_json_dictionary(metadata)
 
-        f = open(filename, 'w')
-        f.write(json.dumps(cbi_container, indent=4))
-        f.close()
+        with open(filename, "w", encoding="utf-8") as f:
+            f.write(json.dumps(cbi_container, indent=4))
```

### Comparing `comicapi-2.2.1/comicapi/comicinfoxml.py` & `comicapi-3.0.0/comicapi/comicinfoxml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,281 +1,273 @@
-"""
-A python class to encapsulate ComicRack's ComicInfo.xml data
+"""A class to encapsulate ComicRack's ComicInfo.xml data"""
 
-Copyright 2012-2014  Anthony Beville
+# Copyright 2012-2014 Anthony Beville
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import logging
 import xml.etree.ElementTree as ET
+
+from comicapi import utils
 from comicapi.genericmetadata import GenericMetadata
-import comicapi.utils
+from comicapi.issuestring import IssueString
+
+logger = logging.getLogger(__name__)
 
 
 class ComicInfoXml:
 
-    writer_synonyms = ['writer', 'plotter', 'scripter']
-    penciller_synonyms = ['artist', 'penciller', 'penciler', 'breakdowns']
-    inker_synonyms = ['inker', 'artist', 'finishes']
-    colorist_synonyms = ['colorist', 'colourist', 'colorer', 'colourer']
-    letterer_synonyms = ['letterer']
-    cover_synonyms = ['cover', 'covers', 'coverartist', 'cover artist']
-    editor_synonyms = ['editor']
+    writer_synonyms = ["writer", "plotter", "scripter"]
+    penciller_synonyms = ["artist", "penciller", "penciler", "breakdowns"]
+    inker_synonyms = ["inker", "artist", "finishes"]
+    colorist_synonyms = ["colorist", "colourist", "colorer", "colourer"]
+    letterer_synonyms = ["letterer"]
+    cover_synonyms = ["cover", "covers", "coverartist", "cover artist"]
+    editor_synonyms = ["editor"]
 
-    def getParseableCredits(self):
+    def get_parseable_credits(self):
         parsable_credits = []
         parsable_credits.extend(self.writer_synonyms)
         parsable_credits.extend(self.penciller_synonyms)
         parsable_credits.extend(self.inker_synonyms)
         parsable_credits.extend(self.colorist_synonyms)
         parsable_credits.extend(self.letterer_synonyms)
         parsable_credits.extend(self.cover_synonyms)
         parsable_credits.extend(self.editor_synonyms)
         return parsable_credits
 
-    def metadataFromString(self, string):
+    def metadata_from_string(self, string):
 
         tree = ET.ElementTree(ET.fromstring(string))
-        return self.convertXMLToMetadata(tree)
+        return self.convert_xml_to_metadata(tree)
 
-    def stringFromMetadata(self, metadata):
+    def string_from_metadata(self, metadata, xml=None):
+        tree = self.convert_metadata_to_xml(self, metadata, xml)
+        tree_str = ET.tostring(tree.getroot(), encoding="utf-8", xml_declaration=True).decode()
+        return tree_str
 
-        header = '<?xml version="1.0"?>\n'
-
-        tree = self.convertMetadataToXML(self, metadata)
-        return header + ET.tostring(tree.getroot())
-
-    def indent(self, elem, level=0):
-        # for making the XML output readable
-        i = "\n" + level * "  "
-        if len(elem):
-            if not elem.text or not elem.text.strip():
-                elem.text = i + "  "
-            if not elem.tail or not elem.tail.strip():
-                elem.tail = i
-            for elem in elem:
-                self.indent(elem, level + 1)
-            if not elem.tail or not elem.tail.strip():
-                elem.tail = i
-        else:
-            if level and (not elem.tail or not elem.tail.strip()):
-                elem.tail = i
-
-    def convertMetadataToXML(self, filename, metadata):
+    def convert_metadata_to_xml(self, filename, metadata, xml=None):
 
         # shorthand for the metadata
         md = metadata
 
-        # build a tree structure
-        root = ET.Element("ComicInfo")
-        root.attrib['xmlns:xsi'] = "http://www.w3.org/2001/XMLSchema-instance"
-        root.attrib['xmlns:xsd'] = "http://www.w3.org/2001/XMLSchema"
-
+        if xml:
+            root = ET.ElementTree(ET.fromstring(xml)).getroot()
+        else:
+            # build a tree structure
+            root = ET.Element("ComicInfo")
+            root.attrib["xmlns:xsi"] = "http://www.w3.org/2001/XMLSchema-instance"
+            root.attrib["xmlns:xsd"] = "http://www.w3.org/2001/XMLSchema"
         # helper func
-        def assign(cix_entry, md_entry):
-            if md_entry is not None:
-                ET.SubElement(root, cix_entry).text = u"{0}".format(md_entry)
 
-        assign('Title', md.title)
-        assign('Series', md.series)
-        assign('Number', md.issue)
-        assign('Count', md.issueCount)
-        assign('Volume', md.volume)
-        assign('AlternateSeries', md.alternateSeries)
-        assign('AlternateNumber', md.alternateNumber)
-        assign('StoryArc', md.storyArc)
-        assign('SeriesGroup', md.seriesGroup)
-        assign('AlternateCount', md.alternateCount)
-        assign('Summary', md.comments)
-        assign('Notes', md.notes)
-        assign('Year', md.year)
-        assign('Month', md.month)
-        assign('Day', md.day)
-
-        # need to specially process the credits, since they are structured differently than CIX
-        credit_writer_list = list()
-        credit_penciller_list = list()
-        credit_inker_list = list()
-        credit_colorist_list = list()
-        credit_letterer_list = list()
-        credit_cover_list = list()
-        credit_editor_list = list()
+        def assign(cix_entry, md_entry):
+            if md_entry is not None and md_entry:
+                et_entry = root.find(cix_entry)
+                if et_entry is not None:
+                    et_entry.text = str(md_entry)
+                else:
+                    ET.SubElement(root, cix_entry).text = str(md_entry)
+            else:
+                et_entry = root.find(cix_entry)
+                if et_entry is not None:
+                    et_entry.clear()
+
+        assign("Title", md.title)
+        assign("Series", md.series)
+        assign("Number", md.issue)
+        assign("Count", md.issue_count)
+        assign("Volume", md.volume)
+        assign("AlternateSeries", md.alternate_series)
+        assign("AlternateNumber", md.alternate_number)
+        assign("StoryArc", md.story_arc)
+        assign("SeriesGroup", md.series_group)
+        assign("AlternateCount", md.alternate_count)
+        assign("Summary", md.comments)
+        assign("Notes", md.notes)
+        assign("Year", md.year)
+        assign("Month", md.month)
+        assign("Day", md.day)
+
+        # need to specially process the credits, since they are structured
+        # differently than CIX
+        credit_writer_list = []
+        credit_penciller_list = []
+        credit_inker_list = []
+        credit_colorist_list = []
+        credit_letterer_list = []
+        credit_cover_list = []
+        credit_editor_list = []
 
-        # first, loop thru credits, and build a list for each role that CIX supports
+        # first, loop thru credits, and build a list for each role that CIX
+        # supports
         for credit in metadata.credits:
 
-            if credit['role'].lower() in set(self.writer_synonyms):
-                credit_writer_list.append(credit['person'].replace(",", ""))
+            if credit["role"].lower() in set(self.writer_synonyms):
+                credit_writer_list.append(credit["person"].replace(",", ""))
 
-            if credit['role'].lower() in set(self.penciller_synonyms):
-                credit_penciller_list.append(credit['person'].replace(",", ""))
+            if credit["role"].lower() in set(self.penciller_synonyms):
+                credit_penciller_list.append(credit["person"].replace(",", ""))
 
-            if credit['role'].lower() in set(self.inker_synonyms):
-                credit_inker_list.append(credit['person'].replace(",", ""))
+            if credit["role"].lower() in set(self.inker_synonyms):
+                credit_inker_list.append(credit["person"].replace(",", ""))
 
-            if credit['role'].lower() in set(self.colorist_synonyms):
-                credit_colorist_list.append(credit['person'].replace(",", ""))
+            if credit["role"].lower() in set(self.colorist_synonyms):
+                credit_colorist_list.append(credit["person"].replace(",", ""))
 
-            if credit['role'].lower() in set(self.letterer_synonyms):
-                credit_letterer_list.append(credit['person'].replace(",", ""))
+            if credit["role"].lower() in set(self.letterer_synonyms):
+                credit_letterer_list.append(credit["person"].replace(",", ""))
 
-            if credit['role'].lower() in set(self.cover_synonyms):
-                credit_cover_list.append(credit['person'].replace(",", ""))
+            if credit["role"].lower() in set(self.cover_synonyms):
+                credit_cover_list.append(credit["person"].replace(",", ""))
 
-            if credit['role'].lower() in set(self.editor_synonyms):
-                credit_editor_list.append(credit['person'].replace(",", ""))
+            if credit["role"].lower() in set(self.editor_synonyms):
+                credit_editor_list.append(credit["person"].replace(",", ""))
 
         # second, convert each list to string, and add to XML struct
-        if len(credit_writer_list) > 0:
-            node = ET.SubElement(root, 'Writer')
-            node.text = comicapi.utils.listToString(credit_writer_list)
-
-        if len(credit_penciller_list) > 0:
-            node = ET.SubElement(root, 'Penciller')
-            node.text = comicapi.utils.listToString(credit_penciller_list)
-
-        if len(credit_inker_list) > 0:
-            node = ET.SubElement(root, 'Inker')
-            node.text = comicapi.utils.listToString(credit_inker_list)
-
-        if len(credit_colorist_list) > 0:
-            node = ET.SubElement(root, 'Colorist')
-            node.text = comicapi.utils.listToString(credit_colorist_list)
-
-        if len(credit_letterer_list) > 0:
-            node = ET.SubElement(root, 'Letterer')
-            node.text = comicapi.utils.listToString(credit_letterer_list)
-
-        if len(credit_cover_list) > 0:
-            node = ET.SubElement(root, 'CoverArtist')
-            node.text = comicapi.utils.listToString(credit_cover_list)
-
-        if len(credit_editor_list) > 0:
-            node = ET.SubElement(root, 'Editor')
-            node.text = comicapi.utils.listToString(credit_editor_list)
-
-        assign('Publisher', md.publisher)
-        assign('Imprint', md.imprint)
-        assign('Genre', md.genre)
-        assign('Web', md.webLink)
-        assign('PageCount', md.pageCount)
-        assign('LanguageISO', md.language)
-        assign('Format', md.format)
-        assign('AgeRating', md.maturityRating)
-        if md.blackAndWhite is not None and md.blackAndWhite:
-            ET.SubElement(root, 'BlackAndWhite').text = "Yes"
-        assign('Manga', md.manga)
-        assign('Characters', md.characters)
-        assign('Teams', md.teams)
-        assign('Locations', md.locations)
-        assign('ScanInformation', md.scanInfo)
+        assign("Writer", utils.list_to_string(credit_writer_list))
+
+        assign("Penciller", utils.list_to_string(credit_penciller_list))
+
+        assign("Inker", utils.list_to_string(credit_inker_list))
+
+        assign("Colorist", utils.list_to_string(credit_colorist_list))
+
+        assign("Letterer", utils.list_to_string(credit_letterer_list))
+
+        assign("CoverArtist", utils.list_to_string(credit_cover_list))
+
+        assign("Editor", utils.list_to_string(credit_editor_list))
+
+        assign("Publisher", md.publisher)
+        assign("Imprint", md.imprint)
+        assign("Genre", md.genre)
+        assign("Web", md.web_link)
+        assign("PageCount", md.page_count)
+        assign("LanguageISO", md.language)
+        assign("Format", md.format)
+        assign("AgeRating", md.maturity_rating)
+        assign("BlackAndWhite", "Yes" if md.black_and_white else None)
+        assign("Manga", md.manga)
+        assign("Characters", md.characters)
+        assign("Teams", md.teams)
+        assign("Locations", md.locations)
+        assign("ScanInformation", md.scan_info)
 
         #  loop and add the page entries under pages node
-        if len(md.pages) > 0:
-            pages_node = ET.SubElement(root, 'Pages')
-            for page_dict in md.pages:
-                page_node = ET.SubElement(pages_node, 'Page')
-                page_node.attrib = page_dict
+        pages_node = root.find("Pages")
+        if pages_node is not None:
+            pages_node.clear()
+        else:
+            pages_node = ET.SubElement(root, "Pages")
+
+        for page_dict in md.pages:
+            page = page_dict
+            if "Image" in page:
+                page["Image"] = str(page["Image"])
+            page_node = ET.SubElement(pages_node, "Page")
+            page_node.attrib = dict(sorted(page_dict.items()))
 
-        # self pretty-print
-        self.indent(root)
+        utils.indent(root)
 
         # wrap it in an ElementTree instance, and save as XML
         tree = ET.ElementTree(root)
         return tree
 
-    def convertXMLToMetadata(self, tree):
+    def convert_xml_to_metadata(self, tree):
 
         root = tree.getroot()
 
-        if root.tag != 'ComicInfo':
-            raise KeyError("Not a ComicInfo XML!")
-            # return None
-
-        metadata = GenericMetadata()
-        md = metadata
+        if root.tag != "ComicInfo":
+            raise "1"
 
-        # Helper function
-        def xlate(tag):
-            node = root.find(tag)
-            if node is not None:
-                return node.text
-            else:
+        def get(name):
+            tag = root.find(name)
+            if tag is None:
                 return None
+            return tag.text
+
+        md = GenericMetadata()
 
-        md.series = xlate('Series')
-        md.title = xlate('Title')
-        md.issue = xlate('Number')
-        md.issueCount = xlate('Count')
-        md.volume = xlate('Volume')
-        md.alternateSeries = xlate('AlternateSeries')
-        md.alternateNumber = xlate('AlternateNumber')
-        md.alternateCount = xlate('AlternateCount')
-        md.comments = xlate('Summary')
-        md.notes = xlate('Notes')
-        md.year = xlate('Year')
-        md.month = xlate('Month')
-        md.day = xlate('Day')
-        md.publisher = xlate('Publisher')
-        md.imprint = xlate('Imprint')
-        md.genre = xlate('Genre')
-        md.webLink = xlate('Web')
-        md.language = xlate('LanguageISO')
-        md.format = xlate('Format')
-        md.manga = xlate('Manga')
-        md.characters = xlate('Characters')
-        md.teams = xlate('Teams')
-        md.locations = xlate('Locations')
-        md.pageCount = xlate('PageCount')
-        md.scanInfo = xlate('ScanInformation')
-        md.storyArc = xlate('StoryArc')
-        md.seriesGroup = xlate('SeriesGroup')
-        md.maturityRating = xlate('AgeRating')
+        md.series = utils.xlate(get("Series"))
+        md.title = utils.xlate(get("Title"))
+        md.issue = IssueString(utils.xlate(get("Number"))).as_string()
+        md.issue_count = utils.xlate(get("Count"), True)
+        md.volume = utils.xlate(get("Volume"), True)
+        md.alternate_series = utils.xlate(get("AlternateSeries"))
+        md.alternate_number = IssueString(utils.xlate(get("AlternateNumber"))).as_string()
+        md.alternate_count = utils.xlate(get("AlternateCount"), True)
+        md.comments = utils.xlate(get("Summary"))
+        md.notes = utils.xlate(get("Notes"))
+        md.year = utils.xlate(get("Year"), True)
+        md.month = utils.xlate(get("Month"), True)
+        md.day = utils.xlate(get("Day"), True)
+        md.publisher = utils.xlate(get("Publisher"))
+        md.imprint = utils.xlate(get("Imprint"))
+        md.genre = utils.xlate(get("Genre"))
+        md.web_link = utils.xlate(get("Web"))
+        md.language = utils.xlate(get("LanguageISO"))
+        md.format = utils.xlate(get("Format"))
+        md.manga = utils.xlate(get("Manga"))
+        md.characters = utils.xlate(get("Characters"))
+        md.teams = utils.xlate(get("Teams"))
+        md.locations = utils.xlate(get("Locations"))
+        md.page_count = utils.xlate(get("PageCount"), True)
+        md.scan_info = utils.xlate(get("ScanInformation"))
+        md.story_arc = utils.xlate(get("StoryArc"))
+        md.series_group = utils.xlate(get("SeriesGroup"))
+        md.maturity_rating = utils.xlate(get("AgeRating"))
 
-        tmp = xlate('BlackAndWhite')
-        md.blackAndWhite = False
+        tmp = utils.xlate(get("BlackAndWhite"))
         if tmp is not None and tmp.lower() in ["yes", "true", "1"]:
-            md.blackAndWhite = True
+            md.black_and_white = True
         # Now extract the credit info
         for n in root:
-            if (n.tag == 'Writer' or n.tag == 'Penciller' or n.tag == 'Inker'
-                    or n.tag == 'Colorist' or n.tag == 'Letterer'
-                    or n.tag == 'Editor'):
+            if any(
+                [
+                    n.tag == "Writer",
+                    n.tag == "Penciller",
+                    n.tag == "Inker",
+                    n.tag == "Colorist",
+                    n.tag == "Letterer",
+                    n.tag == "Editor",
+                ]
+            ):
                 if n.text is not None:
-                    for name in n.text.split(','):
-                        metadata.addCredit(name.strip(), n.tag)
+                    for name in n.text.split(","):
+                        md.add_credit(name.strip(), n.tag)
 
-            if n.tag == 'CoverArtist':
+            if n.tag == "CoverArtist":
                 if n.text is not None:
-                    for name in n.text.split(','):
-                        metadata.addCredit(name.strip(), "Cover")
+                    for name in n.text.split(","):
+                        md.add_credit(name.strip(), "Cover")
 
         # parse page data now
         pages_node = root.find("Pages")
         if pages_node is not None:
             for page in pages_node:
-                metadata.pages.append(page.attrib)
-                # print page.attrib
+                if "Image" in page.attrib:
+                    page.attrib["Image"] = int(page.attrib["Image"])
+                md.pages.append(page.attrib)
 
-        metadata.isEmpty = False
+        md.is_empty = False
 
-        return metadata
+        return md
 
-    def writeToExternalFile(self, filename, metadata):
+    def write_to_external_file(self, filename, metadata, xml=None):
 
-        tree = self.convertMetadataToXML(self, metadata)
-        tree.write(filename, encoding='utf-8')
+        tree = self.convert_metadata_to_xml(self, metadata, xml)
+        tree.write(filename, encoding="utf-8", xml_declaration=True)
 
-    def readFromExternalFile(self, filename):
+    def read_from_external_file(self, filename):
 
         tree = ET.parse(filename)
-        return self.convertXMLToMetadata(tree)
+        return self.convert_xml_to_metadata(tree)
```

### Comparing `comicapi-2.2.1/comicapi/filenameparser.py` & `comicapi-3.0.0/comicapi/filenameparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,268 +1,291 @@
-"""
-Functions for parsing comic info from filename
+"""Functions for parsing comic info from filename
 
 This should probably be re-written, but, well, it mostly works!
+"""
 
-Copyright 2012-2014  Anthony Beville
+# Copyright 2012-2014 Anthony Beville
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 # Some portions of this code were modified from pyComicMetaThis project
 # http://code.google.com/p/pycomicmetathis/
 
-import re
+import logging
 import os
+import re
 from urllib.parse import unquote
 
+logger = logging.getLogger(__name__)
+
 
 class FileNameParser:
+    def __init__(self):
+        self.series = ""
+        self.volume = ""
+        self.year = ""
+        self.issue_count = ""
+        self.remainder = ""
+        self.issue = ""
+
     def repl(self, m):
-        return ' ' * len(m.group())
+        return " " * len(m.group())
 
-    def fixSpaces(self, string, remove_dashes=True):
+    def fix_spaces(self, string, remove_dashes=True):
         if remove_dashes:
-            placeholders = ['[-_]', '  +']
+            placeholders = [r"[-_]", r"  +"]
         else:
-            placeholders = ['[_]', '  +']
+            placeholders = [r"[_]", r"  +"]
         for ph in placeholders:
             string = re.sub(ph, self.repl, string)
-        return string
+        return string  # .strip()
 
-    def getIssueCount(self, filename, issue_end):
+    def get_issue_count(self, filename, issue_end):
 
         count = ""
         filename = filename[issue_end:]
 
-        # replace any name seperators with spaces
-        tmpstr = self.fixSpaces(filename)
+        # replace any name separators with spaces
+        tmpstr = self.fix_spaces(filename)
         found = False
 
-        match = re.search('(?<=\sof\s)\d+(?=\s)', tmpstr, re.IGNORECASE)
+        match = re.search(r"(?<=\sof\s)\d+(?=\s)", tmpstr, re.IGNORECASE)
         if match:
             count = match.group()
             found = True
 
         if not found:
-            match = re.search('(?<=\(of\s)\d+(?=\))', tmpstr, re.IGNORECASE)
+            match = re.search(r"(?<=\(of\s)\d+(?=\))", tmpstr, re.IGNORECASE)
             if match:
                 count = match.group()
 
         count = count.lstrip("0")
 
         return count
 
-    def getIssueNumber(self, filename):
-
-        # Returns a tuple of issue number string, and start and end indexs in the filename
-        # (The indexes will be used to split the string up for further parsing)
+    def get_issue_number(self, filename):
+        """Returns a tuple of issue number string, and start and end indexes in the filename
+        (The indexes will be used to split the string up for further parsing)
+        """
 
         found = False
-        issue = ''
+        issue = ""
         start = 0
         end = 0
 
-        # first, look for multiple "--", this means it's formatted differently from most:
+        # first, look for multiple "--", this means it's formatted differently
+        # from most:
         if "--" in filename:
-            # the pattern seems to be that anything to left of the first "--" is the series name followed by issue
-            filename = re.sub("--.*", self.repl, filename)
-
-        elif "__" in filename:
-            # the pattern seems to be that anything to left of the first "__" is the series name followed by issue
-            filename = re.sub("__.*", self.repl, filename)
+            # the pattern seems to be that anything to left of the first "--"
+            # is the series name followed by issue
+            filename = re.sub(r"--.*", self.repl, filename)
+
+        elif "__" in filename and not re.search(r"\[__\d+__]", filename):
+            # the pattern seems to be that anything to left of the first "__"
+            # is the series name followed by issue
+            filename = re.sub(r"__.*", self.repl, filename)
 
         filename = filename.replace("+", " ")
 
         # replace parenthetical phrases with spaces
-        filename = re.sub("\(.*?\)", self.repl, filename)
-        filename = re.sub("\[.*?\]", self.repl, filename)
+        filename = re.sub(r"\(.*?\)", self.repl, filename)
+        filename = re.sub(r"\[.*?]", self.repl, filename)
 
-        # replace any name seperators with spaces
-        filename = self.fixSpaces(filename)
+        # replace any name separators with spaces
+        filename = self.fix_spaces(filename)
 
-        # remove any "of NN" phrase with spaces (problem: this could break on some titles)
-        filename = re.sub("of [\d]+", self.repl, filename)
+        # remove any "of NN" phrase with spaces (problem: this could break on
+        # some titles)
+        filename = re.sub(r"of [\d]+", self.repl, filename)
 
         # we should now have a cleaned up filename version with all the words in
         # the same positions as original filename
 
         # make a list of each word and its position
-        word_list = list()
-        for m in re.finditer("\S+", filename):
+        word_list = []
+        for m in re.finditer(r"\S+", filename):
             word_list.append((m.group(0), m.start(), m.end()))
 
         # remove the first word, since it can't be the issue number
         if len(word_list) > 1:
             word_list = word_list[1:]
         else:
             # only one word??  just bail.
             return issue, start, end
 
         # Now try to search for the likely issue number word in the list
 
-        # first look for a word with "#" followed by digits with optional sufix
+        # first look for a word with "#" followed by digits with optional suffix
         # this is almost certainly the issue number
         for w in reversed(word_list):
-            if re.match("#[-]?(([0-9]*\.[0-9]+|[0-9]+)(\w*))", w[0]):
+            if re.match(r"#[-]?(([0-9]*\.[0-9]+|[0-9]+)(\w*))", w[0]):
                 found = True
                 break
 
-        # same as above but w/o a '#', and only look at the last word in the list
+        # same as above but w/o a '#', and only look at the last word in the
+        # list
         if not found:
             w = word_list[-1]
-            if re.match("[-]?(([0-9]*\.[0-9]+|[0-9]+)(\w*))", w[0]):
+            if re.match(r"[-]?(([0-9]*\.[0-9]+|[0-9]+)(\w*))", w[0]):
                 found = True
 
         # now try to look for a # followed by any characters
         if not found:
             for w in reversed(word_list):
-                if re.match("#\S+", w[0]):
+                if re.match(r"#\S+", w[0]):
                     found = True
                     break
 
         if found:
             issue = w[0]
             start = w[1]
             end = w[2]
-            if issue[0] == '#':
+            if issue[0] == "#":
                 issue = issue[1:]
 
         return issue, start, end
 
-    def getSeriesName(self, filename, issue_start):
-
-        # use the issue number string index to split the filename string
+    def get_series_name(self, filename, issue_start):
+        """Use the issue number string index to split the filename string"""
 
         if issue_start != 0:
             filename = filename[:issue_start]
 
         # in case there is no issue number, remove some obvious stuff
         if "--" in filename:
-            # the pattern seems to be that anything to left of the first "--" is the series name followed by issue
-            filename = re.sub("--.*", self.repl, filename)
+            # the pattern seems to be that anything to left of the first "--"
+            # is the series name followed by issue
+            filename = re.sub(r"--.*", self.repl, filename)
 
         elif "__" in filename:
-            # the pattern seems to be that anything to left of the first "__" is the series name followed by issue
-            filename = re.sub("__.*", self.repl, filename)
+            # the pattern seems to be that anything to left of the first "__"
+            # is the series name followed by issue
+            filename = re.sub(r"__.*", self.repl, filename)
 
         filename = filename.replace("+", " ")
-        tmpstr = self.fixSpaces(filename, remove_dashes=False)
+        tmpstr = self.fix_spaces(filename, remove_dashes=False)
 
         series = tmpstr
         volume = ""
 
         # save the last word
         try:
             last_word = series.split()[-1]
         except:
             last_word = ""
 
         # remove any parenthetical phrases
-        series = re.sub("\(.*?\)", "", series)
+        series = re.sub(r"\(.*?\)", "", series)
 
         # search for volume number
-        match = re.search('(.+)([vV]|[Vv][oO][Ll]\.?\s?)(\d+)\s*$', series)
+        match = re.search(r"(.+)([vV]|[Vv][oO][Ll]\.?\s?)(\d+)\s*$", series)
         if match:
             series = match.group(1)
             volume = match.group(3)
 
         # if a volume wasn't found, see if the last word is a year in parentheses
         # since that's a common way to designate the volume
         if volume == "":
             # match either (YEAR), (YEAR-), or (YEAR-YEAR2)
-            match = re.search("(\()(\d{4})(-(\d{4}|)|)(\))", last_word)
+            match = re.search(r"(\()(\d{4})(-(\d{4}|)|)(\))", last_word)
             if match:
                 volume = match.group(2)
 
         series = series.strip()
 
         # if we don't have an issue number (issue_start==0), look
         # for hints i.e. "TPB", "one-shot", "OS", "OGN", etc that might
         # be removed to help search online
         if issue_start == 0:
             one_shot_words = ["tpb", "os", "one-shot", "ogn", "gn"]
             try:
                 last_word = series.split()[-1]
                 if last_word.lower() in one_shot_words:
-                    series = series.rsplit(' ', 1)[0]
+                    series = series.rsplit(" ", 1)[0]
             except:
                 pass
 
         return series, volume.strip()
 
-    def getYear(self, filename, issue_end):
+    def get_year(self, filename, issue_end):
 
         filename = filename[issue_end:]
 
         year = ""
         # look for four digit number with "(" ")" or "--" around it
-        match = re.search('(\(\d\d\d\d\))|(--\d\d\d\d--)', filename)
+        match = re.search(r"(\(\d\d\d\d\))|(--\d\d\d\d--)", filename)
         if match:
             year = match.group()
-            # remove non-numerics
-            year = re.sub("[^0-9]", "", year)
+            # remove non-digits
+            year = re.sub(r"[^0-9]", "", year)
         return year
 
-    def getRemainder(self, filename, year, count, issue_end):
+    def get_remainder(self, filename, year, count, volume, issue_end):
+        """Make a guess at where the the non-interesting stuff begins"""
 
-        # make a guess at where the the non-interesting stuff begins
         remainder = ""
 
         if "--" in filename:
             remainder = filename.split("--", 1)[1]
         elif "__" in filename:
             remainder = filename.split("__", 1)[1]
         elif issue_end != 0:
             remainder = filename[issue_end:]
 
-        remainder = self.fixSpaces(remainder, remove_dashes=False)
+        remainder = self.fix_spaces(remainder, remove_dashes=False)
+        if volume != "":
+            remainder = remainder.replace("Vol." + volume, "", 1)
         if year != "":
             remainder = remainder.replace(year, "", 1)
         if count != "":
             remainder = remainder.replace("of " + count, "", 1)
 
         remainder = remainder.replace("()", "")
+        remainder = remainder.replace("  ", " ")  # cleans some whitespace mess
 
         return remainder.strip()
 
-    def parseFilename(self, filename):
+    def parse_filename(self, filename):
 
         # remove the path
         filename = os.path.basename(filename)
 
         # remove the extension
         filename = os.path.splitext(filename)[0]
 
         # url decode, just in case
         filename = unquote(filename)
 
-        # sometimes archives get messed up names from too many decodings
+        # sometimes archives get messed up names from too many decodes
         # often url encodings will break and leave "_28" and "_29" in place
         # of "(" and ")"  see if there are a number of these, and replace them
         if filename.count("_28") > 1 and filename.count("_29") > 1:
             filename = filename.replace("_28", "(")
             filename = filename.replace("_29", ")")
 
-        self.issue, issue_start, issue_end = self.getIssueNumber(filename)
-        self.series, self.volume = self.getSeriesName(filename, issue_start)
-        self.year = self.getYear(filename, issue_end)
-        self.issue_count = self.getIssueCount(filename, issue_end)
-        self.remainder = self.getRemainder(filename, self.year,
-                                           self.issue_count, issue_end)
+        self.issue, issue_start, issue_end = self.get_issue_number(filename)
+        self.series, self.volume = self.get_series_name(filename, issue_start)
+
+        # provides proper value when the filename doesn't have a issue number
+        if issue_end == 0:
+            issue_end = len(self.series)
+
+        self.year = self.get_year(filename, issue_end)
+        self.issue_count = self.get_issue_count(filename, issue_end)
+        self.remainder = self.get_remainder(filename, self.year, self.issue_count, self.volume, issue_end)
 
         if self.issue != "":
             # strip off leading zeros
             self.issue = self.issue.lstrip("0")
             if self.issue == "":
                 self.issue = "0"
             if self.issue[0] == ".":
```

### Comparing `comicapi-2.2.1/comicapi/issuestring.py` & `comicapi-3.0.0/comicapi/issuestring.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-# coding=utf-8
+"""Support for mixed digit/string type Issue field
+
+Class for handling the odd permutations of an 'issue number' that the
+comics industry throws at us.
+  e.g.: "12", "12.1", "0", "-1", "5AU", "100-2"
 """
-Class for handling the odd permutations of an 'issue number' that the comics industry throws at us
 
-e.g.:
+# Copyright 2012-2014 Anthony Beville
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#     http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-"12"
-"12.1"
-"0"
-"-1"
-"5AU"
-"100-2"
-
-Copyright 2012-2014  Anthony Beville
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
+
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 class IssueString:
     def __init__(self, text):
 
-        #  break up the issue number string into 2 parts: the numeric and suffix string.
-        # ( assumes that the numeric portion is always first )
+        # break up the issue number string into 2 parts: the numeric and suffix string.
+        # (assumes that the numeric portion is always first)
 
         self.num = None
         self.suffix = ""
 
         if text is None:
             return
 
-        if type(text) == int:
-            text = str(text)
+        text = str(text)
 
         if len(text) == 0:
             return
 
         # skip the minus sign if it's first
-        if text[0] == '-':
+        if text[0] == "-":
             start = 1
         else:
             start = 0
 
         # if it's still not numeric at start skip it
         if text[start].isdigit() or text[start] == ".":
-            # walk through the string, look for split point (the first non-numeric)
+            # walk through the string, look for split point (the first
+            # non-numeric)
             decimal_count = 0
             for idx in range(start, len(text)):
                 if text[idx] not in "0123456789.":
                     break
                 # special case: also split on second "."
                 if text[idx] == ".":
                     decimal_count += 1
@@ -67,28 +65,29 @@
                 idx = len(text)
 
             # move trailing numeric decimal to suffix
             # (only if there is other junk after )
             if text[idx - 1] == "." and len(text) != idx:
                 idx = idx - 1
 
-            # if there is no numeric after the minus, make the minus part of the suffix
+            # if there is no numeric after the minus, make the minus part of
+            # the suffix
             if idx == 1 and start == 1:
                 idx = 0
 
             part1 = text[0:idx]
-            part2 = text[idx:len(text)]
+            part2 = text[idx : len(text)]
 
             if part1 != "":
                 self.num = float(part1)
             self.suffix = part2
         else:
             self.suffix = text
 
-    def asString(self, pad=0):
+    def as_string(self, pad=0):
         # return the float, left side zero-padded, with suffix attached
         if self.num is None:
             return self.suffix
 
         negative = self.num < 0
 
         num_f = abs(self.num)
@@ -98,31 +97,31 @@
         if float(num_int) != num_f:
             num_s = str(num_f)
 
         num_s += self.suffix
 
         # create padding
         padding = ""
-        l = len(str(num_int))
-        if l < pad:
-            padding = "0" * (pad - l)
+        length = len(str(num_int))
+        if length < pad:
+            padding = "0" * (pad - length)
 
         num_s = padding + num_s
         if negative:
             num_s = "-" + num_s
 
         return num_s
 
-    def asFloat(self):
+    def as_float(self):
         # return the float, with no suffix
-        if self.suffix == u"½":
+        if self.suffix == "½":
             if self.num is not None:
-                return self.num + .5
-            else:
-                return .5
+                return self.num + 0.5
+
+            return 0.5
         return self.num
 
-    def asInt(self):
+    def as_int(self):
         # return the int version of the float
         if self.num is None:
             return None
         return int(self.num)
```

