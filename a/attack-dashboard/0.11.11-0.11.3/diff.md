# Comparing `tmp/attack_dashboard-0.11.11.tar.gz` & `tmp/attack_dashboard-0.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attack_dashboard-0.11.11.tar", max compression
+gzip compressed data, was "attack_dashboard-0.11.3.tar", max compression
```

## Comparing `attack_dashboard-0.11.11.tar` & `attack_dashboard-0.11.3.tar`

### file list

```diff
@@ -1,36 +1,33 @@
--rw-r--r--   0        0        0     3771 2023-05-26 21:54:18.044437 attack_dashboard-0.11.11/README.md
--rw-r--r--   0        0        0        0 2023-05-22 20:16:20.921545 attack_dashboard-0.11.11/attack_dashboard/__init__.py
--rw-r--r--   0        0        0      115 2023-05-22 20:16:20.921545 attack_dashboard-0.11.11/attack_dashboard/__main__.py
--rwxr-xr-x   0        0        0     3175 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/mitre_dashboards.sh
--rw-r--r--   0        0        0     3309 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/dashboard/ALL_MITRE_ATTACK__HELK.ndjson
--rw-r--r--   0        0        0     2837 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/dashboard/MITRE_ATTACK_GROUPS__HELK.ndjson
--rw-r--r--   0        0        0    16915 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/index-pattern/mitre_attack.ndjson
--rw-r--r--   0        0        0      701 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/search/Global_Discover.ndjson
--rw-r--r--   0        0        0      702 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/search/IOC_Discover.ndjson
--rw-r--r--   0        0        0      775 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/search/mitre_attack_discover.ndjson
--rw-r--r--   0        0        0     1403 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_data_sources_techniques.ndjson
--rw-r--r--   0        0        0     1397 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_relationship.ndjson
--rw-r--r--   0        0        0     1572 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_select.ndjson
--rw-r--r--   0        0        0     1505 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_matrices.ndjson
--rw-r--r--   0        0        0     1253 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_software_cloud.ndjson
--rw-r--r--   0        0        0     1365 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_tactics.ndjson
--rw-r--r--   0        0        0     1378 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques.ndjson
--rw-r--r--   0        0        0     2116 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques_bar.ndjson
--rw-r--r--   0        0        0     1335 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_mitigation_technique.ndjson
--rw-r--r--   0        0        0     1355 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_permissions_required.ndjson
--rw-r--r--   0        0        0     1210 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_select.ndjson
--rw-r--r--   0        0        0     2101 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_software_groups.ndjson
--rw-r--r--   0        0        0     1379 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_tactic_techniques.ndjson
--rw-r--r--   0        0        0     1397 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources.ndjson
--rw-r--r--   0        0        0     1282 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources_cloud.ndjson
--rw-r--r--   0        0        0     1378 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_groups.ndjson
--rw-r--r--   0        0        0     1522 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_matrices.ndjson
--rw-r--r--   0        0        0        0 2023-05-22 20:16:20.931545 attack_dashboard-0.11.11/attack_dashboard/join/__init__.py
--rw-r--r--   0        0        0     8199 2023-05-26 18:13:02.986763 attack_dashboard-0.11.11/attack_dashboard/join/join.py
--rw-r--r--   0        0        0     9663 2023-05-26 18:12:56.166587 attack_dashboard-0.11.11/attack_dashboard/join/join_helpers.py
--rw-r--r--   0        0        0      432 2023-05-28 08:14:40.157477 attack_dashboard-0.11.11/attack_dashboard/logstash/docker-compose.yml
--rw-r--r--   0        0        0     1651 2023-05-22 20:16:20.941545 attack_dashboard-0.11.11/attack_dashboard/logstash/logstash.conf
--rw-r--r--   0        0        0     1741 2023-05-22 20:27:27.102699 attack_dashboard-0.11.11/attack_dashboard/up_dash.py
--rw-r--r--   0        0        0     4928 2023-05-28 11:57:09.912908 attack_dashboard-0.11.11/attack_dashboard/up_data.py
--rw-r--r--   0        0        0      777 2023-05-26 18:21:20.542960 attack_dashboard-0.11.11/pyproject.toml
--rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 attack_dashboard-0.11.11/PKG-INFO
+-rw-r--r--   0        0        0     2766 2023-04-28 18:53:57.860694 attack_dashboard-0.11.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 16:34:44.467427 attack_dashboard-0.11.3/attack_dashboard/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-28 17:57:26.509249 attack_dashboard-0.11.3/attack_dashboard/__main__.py
+-rwxr-xr-x   0        0        0     3175 2023-05-01 19:48:01.009624 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/mitre_dashboards.sh
+-rw-r--r--   0        0        0     3309 2023-04-30 15:15:19.803918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/dashboard/ALL_MITRE_ATTACK__HELK.ndjson
+-rw-r--r--   0        0        0     2837 2023-04-30 15:15:19.803918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/dashboard/MITRE_ATTACK_GROUPS__HELK.ndjson
+-rw-r--r--   0        0        0    16915 2023-04-30 15:15:19.823918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/index-pattern/mitre_attack.ndjson
+-rw-r--r--   0        0        0      701 2023-04-30 15:15:19.823918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/Global_Discover.ndjson
+-rw-r--r--   0        0        0      702 2023-04-30 15:15:19.823918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/IOC_Discover.ndjson
+-rw-r--r--   0        0        0      775 2023-04-30 15:15:19.833918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/mitre_attack_discover.ndjson
+-rw-r--r--   0        0        0     1403 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_data_sources_techniques.ndjson
+-rw-r--r--   0        0        0     1397 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_relationship.ndjson
+-rw-r--r--   0        0        0     1572 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_select.ndjson
+-rw-r--r--   0        0        0     1505 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_matrices.ndjson
+-rw-r--r--   0        0        0     1253 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_software_cloud.ndjson
+-rw-r--r--   0        0        0     1365 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_tactics.ndjson
+-rw-r--r--   0        0        0     1378 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques.ndjson
+-rw-r--r--   0        0        0     2116 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques_bar.ndjson
+-rw-r--r--   0        0        0     1335 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_mitigation_technique.ndjson
+-rw-r--r--   0        0        0     1355 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_permissions_required.ndjson
+-rw-r--r--   0        0        0     1210 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_select.ndjson
+-rw-r--r--   0        0        0     2101 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_software_groups.ndjson
+-rw-r--r--   0        0        0     1379 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_tactic_techniques.ndjson
+-rw-r--r--   0        0        0     1397 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources.ndjson
+-rw-r--r--   0        0        0     1282 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources_cloud.ndjson
+-rw-r--r--   0        0        0     1378 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_groups.ndjson
+-rw-r--r--   0        0        0     1522 2023-04-30 15:15:19.873917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_matrices.ndjson
+-rw-r--r--   0        0        0        0 2023-04-28 16:35:03.959977 attack_dashboard-0.11.3/attack_dashboard/join/__init__.py
+-rw-r--r--   0        0        0     8199 2023-05-03 11:06:59.008344 attack_dashboard-0.11.3/attack_dashboard/join/join.py
+-rw-r--r--   0        0        0     9538 2023-05-03 10:28:50.424295 attack_dashboard-0.11.3/attack_dashboard/join/join_helpers.py
+-rw-r--r--   0        0        0     1567 2023-04-30 19:23:22.624204 attack_dashboard-0.11.3/attack_dashboard/up_dash.py
+-rw-r--r--   0        0        0      725 2023-05-03 11:08:40.841752 attack_dashboard-0.11.3/pyproject.toml
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 attack_dashboard-0.11.3/PKG-INFO
```

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/mitre_dashboards.sh` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/mitre_dashboards.sh`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/dashboard/ALL_MITRE_ATTACK__HELK.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/dashboard/ALL_MITRE_ATTACK__HELK.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/dashboard/MITRE_ATTACK_GROUPS__HELK.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/dashboard/MITRE_ATTACK_GROUPS__HELK.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/index-pattern/mitre_attack.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/index-pattern/mitre_attack.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/search/Global_Discover.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/Global_Discover.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/search/IOC_Discover.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/IOC_Discover.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/search/mitre_attack_discover.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/mitre_attack_discover.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_data_sources_techniques.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_data_sources_techniques.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_relationship.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_relationship.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_select.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_select.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_matrices.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_matrices.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_software_cloud.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_software_cloud.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_tactics.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_tactics.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques_bar.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques_bar.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_mitigation_technique.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_mitigation_technique.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_permissions_required.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_permissions_required.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_select.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_select.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_software_groups.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_software_groups.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_tactic_techniques.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_tactic_techniques.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources_cloud.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources_cloud.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_groups.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_groups.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_matrices.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_matrices.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/join/join.py` & `attack_dashboard-0.11.3/attack_dashboard/join/join.py`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.11/attack_dashboard/join/join_helpers.py` & `attack_dashboard-0.11.3/attack_dashboard/join/join_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         **kwargs: Arbitrary keyword arguments.
 
     Returns:
         pd.Series: The series with the function applied.
     """
     if is_cuda:
         # cuDF doesn't support apply yet -> copy the series to a pandas series
-        pd_series = pandas.Series(series.to_arrow().to_pylist())
+        pd_series = pandas.Series(series)
         pd_series = pd_series.apply(func, *args, **kwargs)
         return pd_series
     else:
         return series.apply(func, *args, **kwargs)
 
 
 def split_literals_cols(df: pd.DataFrame, cols: List, sep: str = ",") -> pd.DataFrame:
@@ -239,16 +239,14 @@
 
     Parameters:
         matrix_name (str): the att&ck matrix to fetch
 
     Returns:
         Dict: the MITRE data
     """
-    # Sanitize the matrix name against path traversal
-    matrix_name = matrix_name.replace("/", "_")
     path_pkl = "./mitre_data"
     name_pkl = f"{matrix_name}.pkl"
     name_pkl = os.path.join(path_pkl, name_pkl)
     if not os.path.exists(path_pkl):
         os.makedirs(path_pkl)
 
     if os.path.exists(name_pkl):
```

### Comparing `attack_dashboard-0.11.11/attack_dashboard/up_dash.py` & `attack_dashboard-0.11.3/attack_dashboard/up_dash.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # upload the Mitre ATT&CK dashboard to the Kibana instance
 import logging
 import os
 import sys
 from typing import Dict, List, Tuple
 from addict import Dict as ADict
-import shlex
-import getpass
 
 
 def promt_args() -> Dict:
     """Promt the user for the Kibana instance host-address and credentials.
 
     Returns:
         Dict: return args.
     """
     args = ADict()
     args.kibana_host = input("Kibana host-address: ")
-    username = shlex.quote(input("Username: "))
-    password = shlex.quote(
-        getpass.getpass(
-            "Password: ",
-        )
+    username = input("Username: ")
+    password = input(
+        "Password: ",
     )
     args.elasticsearch_creds = f"{username}:{password}"
     return args
 
 
 def run_upload_sh(args: Dict) -> None:
     """Run the upload.sh script with the given arguments.
@@ -34,15 +30,14 @@
         args (Dict): the arguments to pass to the script
     """
     # get the path to the upload.sh script
     upload_sh_path = os.path.join(
         os.path.dirname(os.path.abspath(__file__)), "dashboard_data/mitre_dashboards.sh"
     )
     # run the script and print the output
-    # file deepcode ignore CommandInjection: <please specify a reason of ignoring this>
     script_out = os.system(
         f"bash {upload_sh_path} {args.kibana_host} {args.elasticsearch_creds}"
     )
     logging.info(script_out)
 
 
 def main() -> None:
```

### Comparing `attack_dashboard-0.11.11/pyproject.toml` & `attack_dashboard-0.11.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "attack_dashboard"
-version = "0.11.11"
+version = "0.11.3"
 description = "Update ATT&CK data for the HELK kibana dashboard."
 authors = ["3lLobo <flocwolf@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/3lLobo/mitre-dash"
 
 [tool.poetry.dependencies]
@@ -23,10 +23,9 @@
 black = "^23.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-attack_fetch = "attack_dashboard.__main__:main"
-attack_dash_up = "attack_dashboard.up_dash:main"
-attack_data_up = "attack_dashboard.up_data:main"
+attack_join = "attack_dashboard.__main__:main"
+attack_uplaod = "attack_dashboard.up_dash:main"
```

