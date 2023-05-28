# Comparing `tmp/keycloak_django-1.0.9.tar.gz` & `tmp/keycloak_django-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.0.9.tar", max compression
+gzip compressed data, was "keycloak_django-1.1.0.tar", max compression
```

## Comparing `keycloak_django-1.0.9.tar` & `keycloak_django-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.0.9/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.0.9/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.0.9/README.md
--rwxr-xr-x   0        0        0      971 2023-05-25 02:36:58.139497 keycloak_django-1.0.9/pyproject.toml
--rwxr-xr-x   0        0        0      114 2023-05-25 02:37:05.252146 keycloak_django-1.0.9/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.0.9/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.0.9/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.0.9/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.0.9/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.0.9/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.0.9/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.0.9/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.0.9/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    16413 2023-05-25 02:04:39.844129 keycloak_django-1.0.9/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7613 2023-05-05 04:43:24.995492 keycloak_django-1.0.9/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.0.9/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.0.9/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.0.9/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.0.9/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.0.9/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.0.9/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.0.9/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     3099 2023-05-25 02:36:23.865569 keycloak_django-1.0.9/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.0.9/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.0.9/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1576 2023-05-25 02:03:00.399252 keycloak_django-1.0.9/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.0.9/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.1.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.1.0/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.1.0/README.md
+-rwxr-xr-x   0        0        0      971 2023-05-28 07:00:13.372447 keycloak_django-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0      114 2023-05-28 07:00:03.625215 keycloak_django-1.1.0/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.1.0/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.1.0/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.1.0/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.1.0/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.1.0/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.1.0/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.1.0/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.1.0/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    17614 2023-05-28 06:27:35.153651 keycloak_django-1.1.0/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     7737 2023-05-28 06:57:38.923654 keycloak_django-1.1.0/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.1.0/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.1.0/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.1.0/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.1.0/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.1.0/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.1.0/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.1.0/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     3657 2023-05-28 06:54:58.462071 keycloak_django-1.1.0/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.1.0/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.1.0/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1576 2023-05-28 06:57:34.486798 keycloak_django-1.1.0/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.1.0/PKG-INFO
```

### Comparing `keycloak_django-1.0.9/LICENSE` & `keycloak_django-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/pyproject.toml` & `keycloak_django-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.0.9"
+version = "1.1.0"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.0.9/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.1.0/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/authentication.py` & `keycloak_django-1.1.0/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.1.0/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/keycloak.py` & `keycloak_django-1.1.0/src/keycloak_django/keycloak.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 from jose import jwt
 from .groups_permissions import GroupsPermissions
 
 
 class KeycloakAdminRepository(KeycloakAdmin):
 
+    URL_ADMIN_USER_ROLES = "admin/realms/{realm-name}/users/{id}/role-mappings"
+
     def __init__(
             self,
             server_url,
             username=None,
             password=None,
             token=None,
             totp=None,
@@ -236,14 +238,47 @@
         :param realm_name:  name of realm_name (not realm-id)
         :type realm_name: str
         :return: Client ID
         :rtype: str
         """
         self.realm_name = realm_name
 
+    def _get_roles_of_user(
+        self, role_mapping_url, user_id, **params
+    ):
+        """Get client roles of a single user helper.
+
+        :param client_level_role_mapping_url: Url for the client role mapping
+        :type client_level_role_mapping_url: str
+        :param user_id: User id
+        :type user_id: str
+        :param client_id: Client id
+        :type client_id: str
+        :param params: Additional parameters
+        :type params: dict
+        :returns: Client roles of a user
+        :rtype: list
+        """
+        params_path = {"realm-name": self.realm_name, "id": user_id}
+        data_raw = self.raw_get(
+            role_mapping_url.format(**params_path), **params)
+        return raise_error_from_response(data_raw, KeycloakGetError)
+
+    def get_roles_of_user(self, user_id):
+        """Get all roles for a user.
+
+        :param user_id: id of user
+        :type user_id: str
+        :return: Keycloak server response (array RoleMappingsRepresentation)
+        :rtype: list
+        """
+        return self._get_roles_of_user(
+            self.URL_ADMIN_USER_ROLES, user_id
+        )
+
 
 def get_default_keycloak_admin():
     config = settings.KEYCLOAK
     try:
         server_url = config['SERVER_URL']
         client_id = config['CLIENT_ID']
         realm = config['REALM_NAME']
```

### Comparing `keycloak_django-1.0.9/src/keycloak_django/middleware.py` & `keycloak_django-1.1.0/src/keycloak_django/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         self.create_user_if_not_exist = self.config.get(
             'CREATE_USER_IF_NOT_EXIST', False)
         self.attributes_fillable = self.config.get('ATTRIBUTES_FILLABLE', None)
         self.public_key_validate = self.config.get(
             'PUBLIC_KEY_VALIDATE', 'inter')
 
         # Create Keycloak instance
-        self.keycloak = KeycloakToken(client_id=self.client_id, realm_name=self.realm)
+        self.keycloak = KeycloakToken(
+            client_id=self.client_id, realm_name=self.realm)
 
         # # Read policies
         # if self.keycloak_authorization_config:
         #     self.keycloak.load_authorization_config(
         #         self.keycloak_authorization_config)
 
         # Django
@@ -89,28 +90,31 @@
             return JsonResponse({"detail": AuthenticationFailed.default_detail},
                                 status=AuthenticationFailed.status_code)
 
         UserModel = get_user_model()
 
         try:
             user = UserModel.objects.get(id=user_info['sub'])
-            user = set_profile(user=user, groups=user_groups, permissions=user_permissions, user_info=user_info)
+            user = set_profile(user=user, groups=user_groups,
+                               permissions=user_permissions, user_info=user_info)
 
             login(request, user)
         except UserModel.DoesNotExist:
             payload = {}
             for config in self.attributes_fillable:
                 if isinstance(config, tuple):
                     payload[config[0]] = user_info[config[1]]
                     continue
                 payload[config] = user_info[config]
+            payload['id'] = user_info['sub']
             user = None
             if self.create_user_if_not_exist:
                 user = UserModel(**payload)
-                user = set_profile(user=user, groups=user_groups, permissions=user_permissions, user_info=user_info)
+                user = set_profile(user=user, groups=user_groups,
+                                   permissions=user_permissions, user_info=user_info)
             if user:
                 login(request, user)
             else:
                 User = get_user_model_keycloak()
                 user = User(**payload)
                 user.groups = user_groups
                 user.permissions = user_permissions
```

### Comparing `keycloak_django-1.0.9/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.1.0/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/models.py` & `keycloak_django-1.1.0/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/security.py` & `keycloak_django-1.1.0/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.1.0/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.1.0/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.1.0/src/keycloak_django/services/realm_repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,13 +57,26 @@
     keycloak_admin = get_default_master_keycloak_admin()
     keycloak_admin.delete_realm(realm_name=realm_model.realm)
 
 
 def get_apps_login_by_owner(user):
     keycloak_admin = get_default_master_keycloak_admin()
     keycloak_admin.set_realm_name(realm_name=user.realm_name)
-    logins = set([group.name for group in user.groups if group.name.startswith(
-        f'login_{user.realm_name}')])
-    clients = keycloak_admin.get_clients()
-    clients = [
-        client for client in clients if f"login_{user.realm_name}_{client['clientId']}" in logins]
+    roles_mappings = keycloak_admin.get_roles_of_user(user_id=user.id)
+    roles = []
+    logins = []
+    clients = []
+    if roles_mappings in 'clientMappings':
+        clients_keys = [
+            client for client in roles_mappings['clientMappings'].keys()]
+        list_clients_roles = [roles_mappings['clientMappings']
+                              [client]['mappings'] for client in clients_keys]
+        for clients_roles in list_clients_roles:
+            for role in clients_roles:
+                roles.append(role)
+        logins = set([role['name'] for role in roles if role['name'].startswith(
+            f'login_{user.realm_name}')])
+    if logins:
+        clients = keycloak_admin.get_clients()
+        clients = [
+            client for client in clients if f"login_{user.realm_name}_{client['clientId']}" in logins]
     return clients
```

### Comparing `keycloak_django-1.0.9/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.1.0/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.1.0/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/src/keycloak_django/tools.py` & `keycloak_django-1.1.0/src/keycloak_django/tools.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.0.9/PKG-INFO` & `keycloak_django-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.0.9
+Version: 1.1.0
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

