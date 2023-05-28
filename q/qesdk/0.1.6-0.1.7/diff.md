# Comparing `tmp/qesdk-0.1.6.tar.gz` & `tmp/qesdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qesdk-0.1.6.tar", last modified: Fri May 26 12:56:42 2023, max compression
+gzip compressed data, was "qesdk-0.1.7.tar", last modified: Sun May 28 05:21:43 2023, max compression
```

## Comparing `qesdk-0.1.6.tar` & `qesdk-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:56:42.610748 qesdk-0.1.6/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       38 2023-05-26 12:51:28.000000 qesdk-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6225 2023-05-26 12:56:42.610748 qesdk-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.6/README.md
--rw-rw-rw-   0        0        0      751 2023-05-26 12:56:27.000000 qesdk-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 12:56:42.610748 qesdk-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 12:56:42.594750 qesdk-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 12:56:42.604747 qesdk-0.1.6/src/qesdk/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.6/src/qesdk/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.6/src/qesdk/aio_api.py
--rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.6/src/qesdk/api.py
--rw-rw-rw-   0        0        0     6805 2023-05-26 12:56:12.000000 qesdk-0.1.6/src/qesdk/client.py
--rw-rw-rw-   0        0        0      237 2023-05-26 12:40:26.000000 qesdk-0.1.6/src/qesdk/config.py
--rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.6/src/qesdk/qedata.thrift
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.6/src/qesdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:56:42.609749 qesdk-0.1.6/src/qesdk.egg-info/
--rw-rw-rw-   0        0        0     6225 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 05:21:43.977211 qesdk-0.1.7/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       38 2023-05-26 12:51:28.000000 qesdk-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6225 2023-05-28 05:21:43.977211 qesdk-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.7/README.md
+-rw-rw-rw-   0        0        0      751 2023-05-28 05:21:07.000000 qesdk-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 05:21:43.977211 qesdk-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 05:21:43.963352 qesdk-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 05:21:43.972551 qesdk-0.1.7/src/qesdk/
+-rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.7/src/qesdk/__init__.py
+-rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.7/src/qesdk/aio_api.py
+-rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.7/src/qesdk/api.py
+-rw-rw-rw-   0        0        0     7088 2023-05-28 05:20:54.000000 qesdk-0.1.7/src/qesdk/client.py
+-rw-rw-rw-   0        0        0      237 2023-05-26 12:40:26.000000 qesdk-0.1.7/src/qesdk/config.py
+-rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.7/src/qesdk/qedata.thrift
+-rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.7/src/qesdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 05:21:43.975879 qesdk-0.1.7/src/qesdk.egg-info/
+-rw-rw-rw-   0        0        0     6225 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 05:21:43.000000 qesdk-0.1.7/src/qesdk.egg-info/top_level.txt
```

### Comparing `qesdk-0.1.6/LICENSE` & `qesdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.6/PKG-INFO` & `qesdk-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qesdk-0.1.6/README.md` & `qesdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.6/pyproject.toml` & `qesdk-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qesdk"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Scott Zhang", email="scott2011@qq.com" },
 ]
 description = "Quantease SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `qesdk-0.1.6/src/qesdk/aio_api.py` & `qesdk-0.1.7/src/qesdk/aio_api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.6/src/qesdk/api.py` & `qesdk-0.1.7/src/qesdk/api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.6/src/qesdk/client.py` & `qesdk-0.1.7/src/qesdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,21 @@
     from .config import outside_server_config, second_server_config
     avail_servers = [outside_server_config, second_server_config]
     server_config = avail_servers[0]
     server_index = 0
 except ImportError:
     server_config = {'host' : '192.168.123.199',
                      'port' : 6001}  
+    avail_servers = [server_config]
+    server_index = 0                 
+
     
 
 
-__version__='0.1.6'
+__version__='0.1.7'
 
 thrift_path = path.join(sys.modules["ROOT_DIR"], "qedata.thrift")
 thrift_path = path.abspath(thrift_path)
 #print(thrift_path)
 qedata_thrift = thriftpy2.load(thrift_path, module_name="qedata_thrift")
 loop = asyncio.get_event_loop()
 def setTimeout(client, timeout):
@@ -78,22 +81,24 @@
     def check_login(cls):
         smtoken = cls._syssmtoken
         #print('auth',token)
         return smtoken != ''
     
     
     async def echo(self, name):
+        global server_config
         client = await make_aio_client(
             qedata_thrift.TestService, server_config['host'], server_config['port'])#,timeout=30*1000)
         #setTimeout(client, 30*1000)
         result = await client.echo(name)
         print(result,self._systoken)
         client.close()
     
     async def queryData(self, method, **kwargs):
+        global server_config, server_index, avail_servers
         try:
             client = await make_aio_client(
                 qedata_thrift.TestService, server_config['host'],  server_config['port'], timeout=self.request_timeout)
         except Exception as e:
             if len(avail_servers) > 1:
                 server_index = (server_index + 1) % len(avail_servers)
                 server_config = avail_servers[server_index]
@@ -121,14 +126,15 @@
             else:
                 return(result.msg)
         except Exception as e:
             return f'ERROR: {e}'
             
     @classmethod
     async def login(cls, username, password):
+        global server_config, server_index,avail_servers
         try:
             client = await make_aio_client(
                 qedata_thrift.TestService, server_config['host'],  server_config['port'],timeout=cls.request_timeout)
         except Exception as e:
             if len(avail_servers) > 1:
                 server_index = (server_index + 1) % len(avail_servers)
                 server_config = avail_servers[server_index]
@@ -149,14 +155,15 @@
                 print(f'LOGIN FAILED : {result.msg}')
                 return False
         except Exception as e:
             return f'ERROR: {e}'    
     
     @classmethod
     async def auth(cls, username, authcode):
+        global server_config, server_index,avail_servers
         try:
             client = await make_aio_client(
                 qedata_thrift.TestService, server_config['host'],  server_config['port'],timeout=cls.request_timeout)
         except Exception as e:
             if len(avail_servers) > 1:
                 server_index = (server_index + 1) % len(avail_servers)
                 server_config = avail_servers[server_index]
```

### Comparing `qesdk-0.1.6/src/qesdk/qedata.thrift` & `qesdk-0.1.7/src/qesdk/qedata.thrift`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.6/src/qesdk/utils.py` & `qesdk-0.1.7/src/qesdk/utils.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.6/src/qesdk.egg-info/PKG-INFO` & `qesdk-0.1.7/src/qesdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

