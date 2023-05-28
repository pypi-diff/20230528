# Comparing `tmp/rising_plugin-0.0.6.tar.gz` & `tmp/rising_plugin-0.0.7.tar.gz`

## Comparing `rising_plugin-0.0.6.tar` & `rising_plugin-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/RisingPlugin.iml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/csv_embed.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/image_embedding.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/phone.csv
--rw-r--r--   0        0        0   283637 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/phone.json
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/pinecone_engine.py
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/risingplugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/common/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/src/rising_plugin/common/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/LICENSE
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 rising_plugin-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/.idea/RisingPlugin.iml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/csv_embed.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/image_embedding.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/phone.csv
+-rw-r--r--   0        0        0   283637 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/phone.json
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/pinecone_engine.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/risingplugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/common/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/src/rising_plugin/common/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/LICENSE
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 rising_plugin-0.0.7/PKG-INFO
```

### Comparing `rising_plugin-0.0.6/.idea/workspace.xml` & `rising_plugin-0.0.7/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `rising_plugin-0.0.6/.idea/workspace.xml` & `rising_plugin-0.0.7/.idea/workspace.xml`

```diff
@@ -96,15 +96,15 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="a286c75f-6878-46cb-a44d-a341ea83c212" name="Changes" comment=""/>
       <created>1685296306253</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685296306253</updated>
       <workItem from="1685296307822" duration="2522000"/>
-      <workItem from="1685299570603" duration="6760000"/>
+      <workItem from="1685299570603" duration="7826000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `rising_plugin-0.0.6/.idea/inspectionProfiles/Project_Default.xml` & `rising_plugin-0.0.7/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.6/src/rising_plugin/csv_embed.py` & `rising_plugin-0.0.7/src/rising_plugin/csv_embed.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.6/src/rising_plugin/image_embedding.py` & `rising_plugin-0.0.7/src/rising_plugin/image_embedding.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.6/src/rising_plugin/phone.csv` & `rising_plugin-0.0.7/src/rising_plugin/phone.csv`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.6/src/rising_plugin/phone.json` & `rising_plugin-0.0.7/src/rising_plugin/phone.json`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.6/src/rising_plugin/pinecone_engine.py` & `rising_plugin-0.0.7/src/rising_plugin/pinecone_engine.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.6/src/rising_plugin/risingplugin.py` & `rising_plugin-0.0.7/src/rising_plugin/risingplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     with open("src/langchain/phone.json", "r") as infile:
         data = json.load(infile)
     embeddings = OpenAIEmbeddings(openai_api_key=OPENAI_API_KEY)
 
     query_result = embeddings.embed_query(query)
     doclist = utils.maximal_marginal_relevance(query_result, data, k=1)
-    loader = CSVLoader(file_path="src/langchain/phone.csv", encoding="utf8")
+    loader = CSVLoader(file_path="phone.csv", encoding="utf8")
     csv_text = loader.load()
 
     docs = []
 
     for res in doclist:
         docs.append(
             Document(
```

### Comparing `rising_plugin-0.0.6/LICENSE` & `rising_plugin-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.0.6/pyproject.toml` & `rising_plugin-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rising_plugin"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Thomas Richardson", email="thomasr37oss@gmail.com" },
 ]
 description = "It is a plugin for Rising GPT"
 readme = "README.md"
 dependencies = [
     "langchain >= 0.0.148",
```

### Comparing `rising_plugin-0.0.6/PKG-INFO` & `rising_plugin-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rising_plugin
-Version: 0.0.6
+Version: 0.0.7
 Summary: It is a plugin for Rising GPT
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Thomas Richardson <thomasr37oss@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

