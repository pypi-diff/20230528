# Comparing `tmp/dnswrapper-0.0.3.tar.gz` & `tmp/dnswrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnswrapper-0.0.3.tar", last modified: Mon Oct 17 01:06:27 2022, max compression
+gzip compressed data, was "dnswrapper-0.0.4.tar", last modified: Sun May 28 15:57:23 2023, max compression
```

## Comparing `dnswrapper-0.0.3.tar` & `dnswrapper-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      346 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/PKG-INFO
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.404728 dnswrapper-0.0.3/dnswrapper/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      124 2022-10-16 20:10:08.000000 dnswrapper-0.0.3/dnswrapper/__init__.py
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/dnswrapper/provider/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      181 2022-10-16 17:39:09.000000 dnswrapper-0.0.3/dnswrapper/provider/__init__.py
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/dnswrapper/provider/aws/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)     1065 2022-10-16 17:30:49.000000 dnswrapper-0.0.3/dnswrapper/provider/aws/client.py
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/dnswrapper/provider/aws/response/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      281 2022-10-15 20:29:37.000000 dnswrapper-0.0.3/dnswrapper/provider/aws/response/list_hosted_zones.py
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      629 2022-10-15 20:29:37.000000 dnswrapper-0.0.3/dnswrapper/provider/aws/response/list_resource_record_sets.py
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)     1669 2022-10-16 17:33:57.000000 dnswrapper-0.0.3/dnswrapper/provider/aws/zonemanager.py
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/dnswrapper/provider/error/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       44 2022-10-15 20:29:37.000000 dnswrapper-0.0.3/dnswrapper/provider/error/awsresponse.py
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       44 2022-10-15 20:29:37.000000 dnswrapper-0.0.3/dnswrapper/provider/error/zonecontrol.py
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/dnswrapper/record/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      368 2022-10-15 20:29:37.000000 dnswrapper-0.0.3/dnswrapper/record/arecord.py
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      357 2022-10-15 20:29:37.000000 dnswrapper-0.0.3/dnswrapper/record/record.py
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      372 2022-10-16 20:29:42.000000 dnswrapper-0.0.3/dnswrapper/record/txt_record.py
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/dnswrapper/resolvers/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       79 2022-10-16 18:18:26.000000 dnswrapper-0.0.3/dnswrapper/resolvers/__init__.py
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      597 2022-10-16 18:40:37.000000 dnswrapper-0.0.3/dnswrapper/resolvers/local_client.py
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      605 2022-10-16 18:38:53.000000 dnswrapper-0.0.3/dnswrapper/resolvers/local_resolver.py
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       38 2022-10-16 18:16:41.000000 dnswrapper-0.0.3/dnswrapper/resolvers/lookup_error.py
-drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/dnswrapper.egg-info/
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      346 2022-10-17 01:06:27.000000 dnswrapper-0.0.3/dnswrapper.egg-info/PKG-INFO
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      744 2022-10-17 01:06:27.000000 dnswrapper-0.0.3/dnswrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)        1 2022-10-17 01:06:27.000000 dnswrapper-0.0.3/dnswrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       16 2022-10-17 01:06:27.000000 dnswrapper-0.0.3/dnswrapper.egg-info/requires.txt
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       11 2022-10-17 01:06:27.000000 dnswrapper-0.0.3/dnswrapper.egg-info/top_level.txt
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      392 2022-10-17 01:03:38.000000 dnswrapper-0.0.3/pyproject.toml
--rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       38 2022-10-17 01:06:27.408728 dnswrapper-0.0.3/setup.cfg
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.036816 dnswrapper-0.0.4/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      346 2023-05-28 15:57:23.036816 dnswrapper-0.0.4/PKG-INFO
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.032816 dnswrapper-0.0.4/dnswrapper/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      124 2022-10-16 20:10:08.000000 dnswrapper-0.0.4/dnswrapper/__init__.py
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.032816 dnswrapper-0.0.4/dnswrapper/provider/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      181 2022-10-16 17:39:09.000000 dnswrapper-0.0.4/dnswrapper/provider/__init__.py
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.032816 dnswrapper-0.0.4/dnswrapper/provider/aws/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)     1065 2022-10-16 17:30:49.000000 dnswrapper-0.0.4/dnswrapper/provider/aws/client.py
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.036816 dnswrapper-0.0.4/dnswrapper/provider/aws/response/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      281 2022-10-15 20:29:37.000000 dnswrapper-0.0.4/dnswrapper/provider/aws/response/list_hosted_zones.py
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      629 2022-10-15 20:29:37.000000 dnswrapper-0.0.4/dnswrapper/provider/aws/response/list_resource_record_sets.py
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)     1673 2023-05-28 15:46:38.000000 dnswrapper-0.0.4/dnswrapper/provider/aws/zonemanager.py
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.036816 dnswrapper-0.0.4/dnswrapper/provider/error/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       44 2022-10-15 20:29:37.000000 dnswrapper-0.0.4/dnswrapper/provider/error/awsresponse.py
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       44 2022-10-15 20:29:37.000000 dnswrapper-0.0.4/dnswrapper/provider/error/zonecontrol.py
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.036816 dnswrapper-0.0.4/dnswrapper/record/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      368 2022-10-15 20:29:37.000000 dnswrapper-0.0.4/dnswrapper/record/arecord.py
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      357 2022-10-15 20:29:37.000000 dnswrapper-0.0.4/dnswrapper/record/record.py
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      372 2022-10-16 20:29:42.000000 dnswrapper-0.0.4/dnswrapper/record/txt_record.py
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.036816 dnswrapper-0.0.4/dnswrapper/resolvers/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       79 2022-10-16 18:18:26.000000 dnswrapper-0.0.4/dnswrapper/resolvers/__init__.py
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      597 2022-10-16 18:40:37.000000 dnswrapper-0.0.4/dnswrapper/resolvers/local_client.py
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      605 2022-10-16 18:38:53.000000 dnswrapper-0.0.4/dnswrapper/resolvers/local_resolver.py
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       38 2022-10-16 18:16:41.000000 dnswrapper-0.0.4/dnswrapper/resolvers/lookup_error.py
+drwxrwxr-x   0 mmartinez  (1000) mmartinez  (1000)        0 2023-05-28 15:57:23.032816 dnswrapper-0.0.4/dnswrapper.egg-info/
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      346 2023-05-28 15:57:23.000000 dnswrapper-0.0.4/dnswrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      744 2023-05-28 15:57:23.000000 dnswrapper-0.0.4/dnswrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)        1 2023-05-28 15:57:23.000000 dnswrapper-0.0.4/dnswrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       16 2023-05-28 15:57:23.000000 dnswrapper-0.0.4/dnswrapper.egg-info/requires.txt
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       11 2023-05-28 15:57:23.000000 dnswrapper-0.0.4/dnswrapper.egg-info/top_level.txt
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)      393 2023-05-28 15:54:48.000000 dnswrapper-0.0.4/pyproject.toml
+-rw-rw-r--   0 mmartinez  (1000) mmartinez  (1000)       38 2023-05-28 15:57:23.036816 dnswrapper-0.0.4/setup.cfg
```

### Comparing `dnswrapper-0.0.3/dnswrapper/provider/aws/client.py` & `dnswrapper-0.0.4/dnswrapper/provider/aws/client.py`

 * *Files identical despite different names*

### Comparing `dnswrapper-0.0.3/dnswrapper/provider/aws/response/list_resource_record_sets.py` & `dnswrapper-0.0.4/dnswrapper/provider/aws/response/list_resource_record_sets.py`

 * *Files identical despite different names*

### Comparing `dnswrapper-0.0.3/dnswrapper/provider/aws/zonemanager.py` & `dnswrapper-0.0.4/dnswrapper/provider/aws/zonemanager.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def upsertRecord(self, record):
         batchedChanges = {
             'Action': 'UPSERT',
             'ResourceRecordSet': {
                 'Name': record.fqdn(),
                 'Type': record.type(),
-                'ResourceRecords': [{'Value': "{}".format(record.val())}],
+                'ResourceRecords': [{'Value': "\"{}\"".format(record.val())}],
                 'TTL': record.ttl()
             }
         }
         response = self.__client.change_resource_record_sets(
             HostedZoneId=self.getZoneId(),
             ChangeBatch={
                 'Changes': [ batchedChanges ]
```

### Comparing `dnswrapper-0.0.3/dnswrapper/resolvers/local_client.py` & `dnswrapper-0.0.4/dnswrapper/resolvers/local_client.py`

 * *Files identical despite different names*

### Comparing `dnswrapper-0.0.3/dnswrapper/resolvers/local_resolver.py` & `dnswrapper-0.0.4/dnswrapper/resolvers/local_resolver.py`

 * *Files identical despite different names*

### Comparing `dnswrapper-0.0.3/dnswrapper.egg-info/SOURCES.txt` & `dnswrapper-0.0.4/dnswrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

