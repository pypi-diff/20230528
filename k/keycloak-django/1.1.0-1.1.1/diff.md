# Comparing `tmp/keycloak_django-1.1.0.tar.gz` & `tmp/keycloak_django-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.1.0.tar", max compression
+gzip compressed data, was "keycloak_django-1.1.1.tar", max compression
```

## Comparing `keycloak_django-1.1.0.tar` & `keycloak_django-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.1.0/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.1.0/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.1.0/README.md
--rwxr-xr-x   0        0        0      971 2023-05-28 07:00:13.372447 keycloak_django-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      114 2023-05-28 07:00:03.625215 keycloak_django-1.1.0/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.1.0/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.1.0/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.1.0/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.1.0/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.1.0/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.1.0/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.1.0/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.1.0/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    17614 2023-05-28 06:27:35.153651 keycloak_django-1.1.0/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7737 2023-05-28 06:57:38.923654 keycloak_django-1.1.0/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.1.0/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.1.0/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.1.0/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.1.0/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.1.0/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.1.0/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.1.0/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     3657 2023-05-28 06:54:58.462071 keycloak_django-1.1.0/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.1.0/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.1.0/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1576 2023-05-28 06:57:34.486798 keycloak_django-1.1.0/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.1.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.1.1/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.1.1/README.md
+-rwxr-xr-x   0        0        0      971 2023-05-28 07:12:37.133036 keycloak_django-1.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0      114 2023-05-28 07:12:29.552892 keycloak_django-1.1.1/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.1.1/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.1.1/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.1.1/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.1.1/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.1.1/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.1.1/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.1.1/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.1.1/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    17614 2023-05-28 06:27:35.153651 keycloak_django-1.1.1/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7737 2023-05-28 06:57:38.923654 keycloak_django-1.1.1/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.1.1/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.1.1/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.1.1/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.1.1/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.1.1/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.1.1/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.1.1/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     3662 2023-05-28 07:12:21.675989 keycloak_django-1.1.1/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.1.1/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.1.1/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1576 2023-05-28 06:57:34.486798 keycloak_django-1.1.1/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.1.1/PKG-INFO
```

### Comparing `keycloak_django-1.1.0/LICENSE` & `keycloak_django-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/pyproject.toml` & `keycloak_django-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.1.0"
+version = "1.1.1"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.1.0/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.1.1/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/authentication.py` & `keycloak_django-1.1.1/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.1.1/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/keycloak.py` & `keycloak_django-1.1.1/src/keycloak_django/keycloak.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/middleware.py` & `keycloak_django-1.1.1/src/keycloak_django/middleware.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.1.1/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/models.py` & `keycloak_django-1.1.1/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/security.py` & `keycloak_django-1.1.1/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.1.1/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.1.1/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.1.1/src/keycloak_django/services/realm_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,22 @@
 def get_apps_login_by_owner(user):
     keycloak_admin = get_default_master_keycloak_admin()
     keycloak_admin.set_realm_name(realm_name=user.realm_name)
     roles_mappings = keycloak_admin.get_roles_of_user(user_id=user.id)
     roles = []
     logins = []
     clients = []
-    if roles_mappings in 'clientMappings':
+    if 'clientMappings' in roles_mappings:
         clients_keys = [
             client for client in roles_mappings['clientMappings'].keys()]
         list_clients_roles = [roles_mappings['clientMappings']
                               [client]['mappings'] for client in clients_keys]
         for clients_roles in list_clients_roles:
             for role in clients_roles:
                 roles.append(role)
         logins = set([role['name'] for role in roles if role['name'].startswith(
             f'login_{user.realm_name}')])
     if logins:
         clients = keycloak_admin.get_clients()
         clients = [
-            client for client in clients if f"login_{user.realm_name}_{client['clientId']}" in logins]
+            client for client in clients if f"login_{user.realm_name}_{client['clientId']}_role" in logins]
     return clients
```

### Comparing `keycloak_django-1.1.0/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.1.1/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.1.1/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/src/keycloak_django/tools.py` & `keycloak_django-1.1.1/src/keycloak_django/tools.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.0/PKG-INFO` & `keycloak_django-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.1.0
+Version: 1.1.1
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

