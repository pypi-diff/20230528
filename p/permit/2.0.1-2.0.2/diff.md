# Comparing `tmp/permit-2.0.1.tar.gz` & `tmp/permit-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.0.1.tar", last modified: Mon May 22 12:10:30 2023, max compression
+gzip compressed data, was "permit-2.0.2.tar", last modified: Sun May 28 07:14:16 2023, max compression
```

## Comparing `permit-2.0.1.tar` & `permit-2.0.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.047623 permit-2.0.1/
--rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.1/LICENSE
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.1/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      467 2023-05-22 12:10:30.047501 permit-2.0.1/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.1/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.043583 permit-2.0.1/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.1/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.046121 permit-2.0.1/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     9730 2023-05-22 12:10:06.000000 permit-2.0.1/permit/api/base.py
--rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/condition_set_rules.py
--rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/condition_sets.py
--rw-r--r--   0 asafc      (501) staff       (20)     3534 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/context.py
--rw-r--r--   0 asafc      (501) staff       (20)     6805 2023-05-22 12:10:06.000000 permit-2.0.1/permit/api/deprecated.py
--rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.1/permit/api/elements.py
--rw-r--r--   0 asafc      (501) staff       (20)     8821 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/environments.py
--rw-r--r--   0 asafc      (501) staff       (20)   137541 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/models.py
--rw-r--r--   0 asafc      (501) staff       (20)     5098 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/resource_action_groups.py
--rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/sync_api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.1/permit/api/tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)     8875 2023-05-22 12:10:06.000000 permit-2.0.1/permit/api/users.py
--rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.1/permit/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.046393 permit-2.0.1/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.1/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.1/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.1/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     2865 2023-05-22 12:10:06.000000 permit-2.0.1/permit/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.1/permit/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.1/permit/permit.py
--rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.1/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.046779 permit-2.0.1/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.1/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.1/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.1/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.1/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.044085 permit-2.0.1/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      467 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2023-05-22 12:10:30.000000 permit-2.0.1/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.1/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-22 12:10:30.047661 permit-2.0.1/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      793 2023-05-22 12:10:06.000000 permit-2.0.1/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 12:10:30.047340 permit-2.0.1/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.1/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.1/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     9232 2023-05-22 06:43:35.000000 permit-2.0.1/tests/test_abac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8745 2023-05-22 11:43:03.000000 permit-2.0.1/tests/test_rbac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8666 2023-05-22 06:43:35.000000 permit-2.0.1/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.1/tests/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.343609 permit-2.0.2/
+-rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.2/LICENSE
+-rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.2/MANIFEST.in
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-05-28 07:14:16.343488 permit-2.0.2/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.2/README.md
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.339239 permit-2.0.2/permit/
+-rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.2/permit/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.342006 permit-2.0.2/permit/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9730 2023-05-28 06:52:45.000000 permit-2.0.2/permit/api/base.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/condition_set_rules.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/condition_sets.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3534 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6805 2023-05-22 12:10:06.000000 permit-2.0.2/permit/api/deprecated.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.2/permit/api/elements.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8821 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/environments.py
+-rw-r--r--   0 asafc      (501) staff       (20)   137660 2023-05-28 07:14:10.000000 permit-2.0.2/permit/api/models.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5098 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/projects.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/resource_action_groups.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/resource_actions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/resource_attributes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/resources.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/role_assignments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/sync_api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.2/permit/api/tenants.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8875 2023-05-22 12:10:06.000000 permit-2.0.2/permit/api/users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.2/permit/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.342310 permit-2.0.2/permit/enforcement/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.2/permit/enforcement/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.2/permit/enforcement/enforcer.py
+-rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.2/permit/enforcement/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2865 2023-05-22 12:10:06.000000 permit-2.0.2/permit/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.2/permit/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.2/permit/permit.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.2/permit/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.342662 permit-2.0.2/permit/utils/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.2/permit/utils/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.2/permit/utils/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.2/permit/utils/dicts.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.2/permit/utils/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.339751 permit-2.0.2/permit.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       13 2023-05-28 07:14:16.000000 permit-2.0.2/permit.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.2/requirements.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-28 07:14:16.343645 permit-2.0.2/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)      793 2023-05-28 07:14:10.000000 permit-2.0.2/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-28 07:14:16.343343 permit-2.0.2/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.2/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.2/tests/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9232 2023-05-22 06:43:35.000000 permit-2.0.2/tests/test_abac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8745 2023-05-28 06:54:39.000000 permit-2.0.2/tests/test_rbac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8666 2023-05-22 06:43:35.000000 permit-2.0.2/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.2/tests/utils.py
```

### Comparing `permit-2.0.1/LICENSE` & `permit-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/api_client.py` & `permit-2.0.2/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/base.py` & `permit-2.0.2/permit/api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/condition_set_rules.py` & `permit-2.0.2/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/condition_sets.py` & `permit-2.0.2/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/context.py` & `permit-2.0.2/permit/api/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/deprecated.py` & `permit-2.0.2/permit/api/deprecated.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/elements.py` & `permit-2.0.2/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/environments.py` & `permit-2.0.2/permit/api/environments.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/models.py` & `permit-2.0.2/permit/api/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3741,35 +3741,39 @@
     )
     status: UserStatus = Field(..., description="Whether the user has signed in or not")
 
 
 class UserRead(BaseModel):
     class Config:
         extra = Extra.allow
+        allow_population_by_field_name = True
 
     key: str = Field(
         ...,
         description="A unique id by which Permit will identify the user for permission checks.",
         title="Key",
     )
     id: UUID = Field(..., description="Unique id of the user", title="Id")
     organization_id: UUID = Field(
         ...,
         description="Unique id of the organization that the user belongs to.",
         title="Organization Id",
+        alias="org_id",
     )
     project_id: UUID = Field(
         ...,
         description="Unique id of the project that the user belongs to.",
         title="Project Id",
+        alias="proj_id",
     )
     environment_id: UUID = Field(
         ...,
         description="Unique id of the environment that the user belongs to.",
         title="Environment Id",
+        alias="env_id",
     )
     associated_tenants: Optional[List[UserInTenant]] = Field(
         [], title="Associated Tenants"
     )
     roles: Optional[List[UserRole]] = Field([], title="Roles")
     email: Optional[EmailStr] = Field(
         None,
```

### Comparing `permit-2.0.1/permit/api/projects.py` & `permit-2.0.2/permit/api/projects.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/resource_action_groups.py` & `permit-2.0.2/permit/api/resource_action_groups.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/resource_actions.py` & `permit-2.0.2/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/resource_attributes.py` & `permit-2.0.2/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/resources.py` & `permit-2.0.2/permit/api/resources.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/role_assignments.py` & `permit-2.0.2/permit/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/roles.py` & `permit-2.0.2/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/sync_api_client.py` & `permit-2.0.2/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/tenants.py` & `permit-2.0.2/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/api/users.py` & `permit-2.0.2/permit/api/users.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/config.py` & `permit-2.0.2/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/enforcement/enforcer.py` & `permit-2.0.2/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/enforcement/interfaces.py` & `permit-2.0.2/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/exceptions.py` & `permit-2.0.2/permit/exceptions.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/permit.py` & `permit-2.0.2/permit/permit.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/sync.py` & `permit-2.0.2/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/utils/context.py` & `permit-2.0.2/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit/utils/sync.py` & `permit-2.0.2/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/permit.egg-info/SOURCES.txt` & `permit-2.0.2/permit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/setup.py` & `permit-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
 setup(
     name="permit",
-    version="2.0.1",
+    version="2.0.2",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
```

### Comparing `permit-2.0.1/tests/conftest.py` & `permit-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/tests/test_abac_e2e.py` & `permit-2.0.2/tests/test_abac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/tests/test_rbac_e2e.py` & `permit-2.0.2/tests/test_rbac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.1/tests/test_rbac_e2e_sync.py` & `permit-2.0.2/tests/test_rbac_e2e_sync.py`

 * *Files identical despite different names*

