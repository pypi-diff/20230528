# Comparing `tmp/vector_vault-1.2.0.tar.gz` & `tmp/vector_vault-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.2.0.tar", last modified: Sat May 27 01:28:34 2023, max compression
+gzip compressed data, was "vector_vault-1.3.0.tar", last modified: Sun May 28 08:45:04 2023, max compression
```

## Comparing `vector_vault-1.2.0.tar` & `vector_vault-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-27 01:28:34.288622 vector_vault-1.2.0/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.2.0/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    17414 2023-05-27 01:28:34.288468 vector_vault-1.2.0/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    16689 2023-05-27 01:26:36.000000 vector_vault-1.2.0/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-27 01:28:34.288659 vector_vault-1.2.0/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-27 01:28:12.000000 vector_vault-1.2.0/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-27 01:28:34.285780 vector_vault-1.2.0/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    17414 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-27 01:28:34.288277 vector_vault-1.2.0/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.2.0/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6135 2023-05-24 22:54:17.000000 vector_vault-1.2.0/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-27 01:27:47.000000 vector_vault-1.2.0/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.2.0/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.2.0/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.2.0/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      890 2023-05-26 00:54:12.000000 vector_vault-1.2.0/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17812 2023-05-25 07:36:53.000000 vector_vault-1.2.0/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.2.0/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-28 08:45:04.479519 vector_vault-1.3.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.3.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20047 2023-05-28 08:45:04.479325 vector_vault-1.3.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19322 2023-05-27 22:01:20.000000 vector_vault-1.3.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-28 08:45:04.479568 vector_vault-1.3.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-28 08:43:08.000000 vector_vault-1.3.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-28 08:45:04.475514 vector_vault-1.3.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20047 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-28 08:45:04.478783 vector_vault-1.3.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.3.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.3.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3222 2023-05-28 08:43:39.000000 vector_vault-1.3.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.3.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.3.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1742 2023-05-28 08:43:47.000000 vector_vault-1.3.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.3.0/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17379 2023-05-28 08:43:26.000000 vector_vault-1.3.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2381 2023-05-28 08:31:16.000000 vector_vault-1.3.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.3.0/vectorvault/wrap.py
```

### Comparing `vector_vault-1.2.0/LICENSE` & `vector_vault-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.2.0/PKG-INFO` & `vector_vault-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: vector_vault
-Version: 1.2.0
-Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
-Home-page: https://github.com/John-Rood/VectorVault
-Author: VectorVault.io
-Author-email: john@johnrood.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
 
 By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
 Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
@@ -467,21 +448,39 @@
 <br>
 <br>
 
 ---
 <br>
 <br>
 
-If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
 
 
+### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
+Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
+
+<br>
 <br>
+<br>
+
+
+## FAQ
+
+### What is the latency on large datasets?
+To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is under one second response time with the similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking longer than 1 second, its recommended that you segment you data into multiple vaults to keep latency below 1 second on api calls. 
 
-Open the "examples" folder and try out the Google Colab tutorials we have.
+
+### How should I segment my data?
+Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
+
+
+### What if I'm a large company with very large data
+If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Custom cloud plan. In our Custom plan, we create a persistent storage pod that is always active. With a Custom plan, a billion vectors search will respond in under one second. For reference, the full text of 3.7 million books would be around 1.1 - 1.5 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
+
+<br>
 
 Happy coding!
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
-
-
+<br>
```

### Comparing `vector_vault-1.2.0/README.md` & `vector_vault-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: vector_vault
+Version: 1.3.0
+Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
+Home-page: https://github.com/John-Rood/VectorVault
+Author: VectorVault.io
+Author-email: john@johnrood.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
 
 By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
 Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
@@ -448,19 +467,41 @@
 <br>
 <br>
 
 ---
 <br>
 <br>
 
-If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
 
 
+### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
+Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
+
+<br>
 <br>
+<br>
+
+
+## FAQ
+
+### What is the latency on large datasets?
+To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is under one second response time with the similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking longer than 1 second, its recommended that you segment you data into multiple vaults to keep latency below 1 second on api calls. 
 
-Open the "examples" folder and try out the Google Colab tutorials we have.
+
+### How should I segment my data?
+Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
+
+
+### What if I'm a large company with very large data
+If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Custom cloud plan. In our Custom plan, we create a persistent storage pod that is always active. With a Custom plan, a billion vectors search will respond in under one second. For reference, the full text of 3.7 million books would be around 1.1 - 1.5 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
+
+<br>
 
 Happy coding!
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
+<br>
+
+
```

### Comparing `vector_vault-1.2.0/setup.py` & `vector_vault-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.2.0",
+    version="1.3.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.2.0/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.3.0/vector_vault.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.2.0
+Version: 1.3.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -467,21 +467,41 @@
 <br>
 <br>
 
 ---
 <br>
 <br>
 
-If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
 
 
+### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
+Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
+
+<br>
+<br>
 <br>
 
-Open the "examples" folder and try out the Google Colab tutorials we have.
+
+## FAQ
+
+### What is the latency on large datasets?
+To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is under one second response time with the similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking longer than 1 second, its recommended that you segment you data into multiple vaults to keep latency below 1 second on api calls. 
+
+
+### How should I segment my data?
+Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
+
+
+### What if I'm a large company with very large data
+If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Custom cloud plan. In our Custom plan, we create a persistent storage pod that is always active. With a Custom plan, a billion vectors search will respond in under one second. For reference, the full text of 3.7 million books would be around 1.1 - 1.5 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
+
+<br>
 
 Happy coding!
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
+<br>
```

### Comparing `vector_vault-1.2.0/vectorvault/__init__.py` & `vector_vault-1.3.0/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.2.0/vectorvault/ai.py` & `vector_vault-1.3.0/vectorvault/ai.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,16 @@
         encoding = tiktoken.get_encoding(encoding_name)
         num_tokens = len(encoding.encode(string))
         return num_tokens
 
 
 # Notes: OpenAI's CEO, Sam Altman, recently testified in congress to compel the government to regulate the creation of cutting edge ai 
 # by forcing anyone seeking to do so to acquire a license first, or pay heavy pentalties. This anti-competitive attack on the 
-# open-source community, and development community at large, is extremely not cool. While they claim that they take this action
+# open-source community, and development community at large is not cool. While they claim that they take this action
 # in the name of protecting the community, the community clearly sees the actual intent - which is to block competition.
 # If the claimed ai threats made public Altman hold true, then having the most capable models in the hands of only a few small companies 
-# is the real actual threat we need to watch out for. Diversity is our only true security, and that comes from an open community.
-# While "Open" AI has completely gone against it's original mission (to stay open and support the community) they are however, the
-# most used ai right now. Our goals are to support the community at large, therefore we integrate with them exclusively for now.
-# In the future, we will add open models, and competitors to OpenAI, as they become well-adopted, and with the exception that they
+# could be the real actual threat we really need to watch out for. Diversity is our only true security, and that comes from an open community.
+# While "Open" AI has gone against it's original mission (to stay open and transparent with data and models) they are however, the
+# most used ai right now. They have a great platform that can support massive load at high quality. No one else in the world has that.
+# Our goals are to support the community at large, therefore we integrate with them exclusively for now.
+# In the future, we will add open models, and competitors, as they become well-adopted, and with the exception that they
 # support the development community at large.
```

### Comparing `vector_vault-1.2.0/vectorvault/cloudmanager.py` & `vector_vault-1.3.0/vectorvault/cloudmanager.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 import tempfile
 import os
 import json
 from .creds import CustomCredentials
-from .itemize import name
+from .vecreq import call_proj
+from .itemize import cloud_name
 from google.cloud import storage
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
-
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
         self.user = self.get_user_id(user)
         self.api = api_key
         self.vault = vault
         # Creates the credentials
         credentials = CustomCredentials(user, self.api)
         # Instantiates the client 
-        self.storage_client = storage.Client(project='vectorvault-361ab', credentials=credentials)
+        self.storage_client = storage.Client(project=call_proj(), credentials=credentials)
         self.cloud = self.storage_client.bucket(self.user)
         print(f'Connected to Vault: {self.vault}')
 
     def vault_exists(self, vault_name):
         return storage.Blob(bucket=self.cloud, name=vault_name).exists(self.storage_client)
 
     def upload_to_cloud(self, vault_name, content):
@@ -54,16 +54,16 @@
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             blob = self.cloud.blob(vault_name)
             blob.download_to_filename(temp_file.name) 
             return temp_file.name
 
     def upload(self, item, text, meta):
         with ThreadPoolExecutor() as executor:
-            executor.submit(self.upload_to_cloud, name(self.vault, item, item=True), text)
-            executor.submit(self.upload_to_cloud, name(self.vault, item, meta=True), json.dumps(meta))
+            executor.submit(self.upload_to_cloud, cloud_name(self.vault, item, self.user, text, self.api, item=True), text)
+            executor.submit(self.upload_to_cloud, cloud_name(self.vault, item, self.user, meta, self.api, meta=True), json.dumps(meta))
     
     def delete_blob(self, blob):
         blob.delete()
      
     def get_user_id(self, input_string):
         return input_string.replace("@", "_at_").replace(".", "_dot_") + '_vvclient'
 
@@ -76,19 +76,8 @@
             futures = {executor.submit(self.delete_blob, blob): blob for blob in blobs}
 
             for future in as_completed(futures):
                 try:
                     future.result()
                 except Exception as e:
                     print(f"Failed to delete blob: {e}")
-        
-    def get_vaults(self, vault: str = None):
-        vault = self.vault if vault is None else vault
-        blobs = self.cloud.list_blobs(prefix=f'{vault}')
-    
-        directories = set()
-        for blob in blobs:
-            parts = blob.name.split('/')
-            if len(parts) > 2 and not parts[1][0].isdigit():
-                directories.add(parts[1])
-
-        return list(directories)
+
```

### Comparing `vector_vault-1.2.0/vectorvault/creds.py` & `vector_vault-1.3.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.2.0/vectorvault/download.py` & `vector_vault-1.3.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.2.0/vectorvault/signup.py` & `vector_vault-1.3.0/vectorvault/signup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,10 +22,10 @@
         'last': last_name,
         'email': email,
         'password': password
     }
     response = requests.post(url, headers=headers, data=data)
 
     if response.status_code != 200:
-        return {}
+        return {'error': response.text}
 
     return response.json()
```

### Comparing `vector_vault-1.2.0/vectorvault/vault.py` & `vector_vault-1.3.0/vectorvault/vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,116 +13,118 @@
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 import numpy as np
 import tempfile
 import os
 import time
-import json
 import re
 import openai
 from concurrent.futures import ThreadPoolExecutor
 from .cloudmanager import CloudManager
 from .ai import AI
-from .itemize import itemize, name, name_vecs, get_item, build_return, get_vectors
+from .itemize import itemize, name_vecs, get_item, get_vectors
+from .vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults
 
 
 class Vault:
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
+        self.api = api_key
         self.dims = dims
         try:
             self.cloud_manager = CloudManager(user, api_key, self.vault)
         except:
             print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work')
             # user can still use the get_chat() function without an api key
             pass
+        self.user = self.cloud_manager.user
         self.x = 0
         self.x_checked = False
+        self.vecs_loaded = False
         self.verbose = verbose
         self.items = []
         self.last_time = None
         self.last_chat_time = None
         self.first_run = True
         self.needed_sleep_time = None
         self.ai = AI()
 
-
-    def check_index(self):
-        start_time = time.time()
-        if self.cloud_manager.vault_exists(name_vecs(self.vault)):
-            self.load_vectors()
-            num_existing_items = self.vectors.get_n_items()
-            new_index = get_vectors(self.dims)
-            for i in range(num_existing_items):
-                vector = self.vectors.get_item_vector(i)
-                new_index.add_item(i, vector)
-            self.x = i + 1
-            self.vectors = new_index
-        else:
-            pass
-        
-        self.x_checked = True
-        if self.verbose == True:
-            print("initialize index --- %s seconds ---" % (time.time() - start_time))
-        
-
-    def load_vectors(self):
-        start_time = time.time()
-        # Download the .ann file from google cloud storage to a temporary file
-        temp_file_path = self.cloud_manager.download_to_temp_file(name_vecs(self.vault))
-
-        # Load the AnnoyIndex object from the temporary file, then delete the temp file
-        self.vectors.load(temp_file_path)
-        os.remove(temp_file_path)
-        if self.verbose:
-            print("get load vectors --- %s seconds ---" % (time.time() - start_time))
-
-    
     def get_vaults(self, vault: str = None):
         vault = self.vault if vault is None else vault
-        return self.cloud_manager.get_vaults(vault)
-
+        return call_get_vaults(self.user, self.api, vault)
 
     def get_total_vectors(self):
-        return self.vectors.get_n_items()
+        return call_get_total_vectors(self.user, self.vault, self.api)
     
-
     def save(self, trees=16):
         start_time = time.time()
         self.vectors.build(trees)
 
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             self.vectors.save(temp_file.name)
-            self.cloud_manager.upload_temp_file(temp_file.name, name_vecs(self.vault))
+            bytesize = os.path.getsize(temp_file.name)
+            self.cloud_manager.upload_temp_file(temp_file.name, name_vecs(self.vault, self.user, self.api, bytesize))
 
         total_saved_items = 0
         for item in self.items:
             item_text, item_id, item_meta = get_item(item)
             self.cloud_manager.upload(item_id, item_text, item_meta)
             total_saved_items += 1
 
         self.items.clear()
         self.x_checked = False
+        self.vecs_loaded = False
 
         if self.verbose:
             print("save vectors time --- %s seconds ---" % (time.time() - start_time))
 
+    def clear_cache(self):
+        self.items.clear()
+        self.x_checked = False
+        self.vecs_loaded = False
 
     def delete(self):
         if self.verbose == True:
             print('Deleting started. Note: this can take a while for large datasets')
         # Clear the local vector data
         self.vectors = get_vectors(self.dims)
         self.items.clear()
         self.x = 0
         self.cloud_manager.delete()
         print('Vault deleted')
-    
+
+    def check_index(self):
+        start_time = time.time()
+        if self.cloud_manager.vault_exists(name_vecs(self.vault, self.user, self.api)):
+            if self.vecs_loaded == False:
+                self.load_vectors()
+            num_existing_items = self.vectors.get_n_items()
+            new_index = get_vectors(self.dims)
+            for i in range(num_existing_items):
+                vector = self.vectors.get_item_vector(i)
+                new_index.add_item(i, vector)
+            self.x = i + 1
+            self.vectors = new_index
+        else:
+            pass
+        
+        self.x_checked = True
+        if self.verbose == True:
+            print("initialize index --- %s seconds ---" % (time.time() - start_time))
+        
+    def load_vectors(self):
+        start_time = time.time()
+        temp_file_path = self.cloud_manager.download_to_temp_file(name_vecs(self.vault, self.user, self.api))
+        self.vectors.load(temp_file_path)
+        os.remove(temp_file_path)
+        self.vecs_loaded = True
+        if self.verbose:
+            print("get load vectors --- %s seconds ---" % (time.time() - start_time))
 
     def split_text(self, text, min_threshold=1000, max_threshold=16000):
         segments = []
         sentence_spans = list(re.finditer(r"(?<=[.!?])\s+", text))
 
         current_segment = []
         current_length = 0
@@ -150,55 +152,32 @@
         if last_sentence:
             current_segment.append(last_sentence)
 
         if current_segment:
             segments.append(" ".join(current_segment))
 
         return segments
-
-
-    def get_items_by_vector(self, vector, n: int = 4):
-        self.load_vectors()
-        start_time = time.time()
-
-        results = []
-        vecs = self.vectors.get_nns_by_vector(vector, n)
-        for vec in vecs:
-            # Retrieve the item
-            item_data = self.cloud_manager.download_text_from_cloud(name(self.vault, vec, item=True))
-            # Retrieve the metadata
-            meta_data = self.cloud_manager.download_text_from_cloud(name(self.vault, vec, meta=True))
-            meta = json.loads(meta_data)
-            build_return(results, item_data, meta)
-
-        if self.verbose == True:
-            print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))
-
-        return results
     
-
     def get_similar(self, text, n: int = 4):
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
-        return self.get_items_by_vector(vector, n)
-
+        return call_items_by_vector(self.user, self.vault, vector, self.api, n)
 
     def add_item(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         if self.x_checked == False:
             self.check_index()
         else: 
             pass
 
         self.items.append(itemize(self.vault, self.x, meta, text, name))
         self.x += 1
 
-
     def add(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 4000 tokens, Vault.split_text(your_text)  
             will automatically be added
         """
 
         if self.ai.get_tokens(text) > 4000:
@@ -207,15 +186,14 @@
             texts = self.split_text(text) # returns list of text segments
         else:
             texts = [text]
 
         for text in texts:
             self.add_item(text, meta, name)
 
-    
     def add_item_with_vector(self, text: str, vector: list, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         if self.x_checked == False:
             self.check_index()
@@ -231,15 +209,14 @@
         self.items.append(itemize(self.vault, self.x, meta, text, name))
 
         self.x += 1
 
         if self.verbose == True:
             print("add item time --- %s seconds ---" % (time.time() - start_time))
 
-
     def process_batch(self, batch_text_chunks, never_stop, loop_timeout):
         loop_start_time = time.time()
         while True:
             try:
                 res = openai.Embedding.create(input=batch_text_chunks, engine="text-embedding-ada-002")
                 break
             except Exception as e:
@@ -249,15 +226,14 @@
                     try:
                         res = openai.Embedding.create(input=batch_text_chunks, engine="text-embedding-ada-002")
                         break
                     except Exception as e:
                         raise TimeoutError("Loop timed out")
         return [record['embedding'] for record in res['data']]
 
-
     def get_vectors(self, batch_size: int = 32, never_stop: bool = False, loop_timeout: int = 180):
         start_time = time.time()
         if not self.last_time:
             self.last_time = start_time - 1
         
         if not self.needed_sleep_time:
             self.needed_sleep_time = 0
@@ -297,16 +273,14 @@
                 time.sleep(1)
 
         # Process the batches in parallel using ThreadPoolExecutor
         with ThreadPoolExecutor() as executor:
             process_batch_with_params = lambda batch_text_chunks: self.process_batch(batch_text_chunks, never_stop, loop_timeout)
             batch_embeddings_list = list(executor.map(process_batch_with_params, batches_text_chunks))
 
-
-        # Add the embeddings to the AnnoyIndex using the index from the metadata
         current_item_index = 0
         for batch_embeddings in batch_embeddings_list:
             for embedding in batch_embeddings:
                 item_index = self.items[current_item_index]["meta"]["item_id"]
                 self.vectors.add_item(item_index, embedding)
                 current_item_index += 1
 
@@ -423,16 +397,16 @@
                             for text in context:
                                 input += text['data']
                         response = self.ai.llm_w_context(segment, input, history, model=model)
                     else:
                         response = self.ai.llm(segment, history, model=model)
                     break
                 except Exception as e:
-                    print(f"API Error: {e}. Sleeping 15 seconds")
-                    time.sleep(15)
+                    print(f"API Error: {e}. Sleeping 5 seconds")
+                    time.sleep(5)
                     
             self.last_chat_time = start_time
 
         if self.verbose == True:
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
         if return_context == False:
```

### Comparing `vector_vault-1.2.0/vectorvault/wrap.py` & `vector_vault-1.3.0/vectorvault/wrap.py`

 * *Files identical despite different names*

