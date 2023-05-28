# Comparing `tmp/mprov_ldap_manager-0.0.2.tar.gz` & `tmp/mprov_ldap_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mprov_ldap_manager-0.0.2.tar", last modified: Fri May 19 18:35:07 2023, max compression
+gzip compressed data, was "mprov_ldap_manager-0.0.3.tar", last modified: Sun May 28 18:47:16 2023, max compression
```

## Comparing `mprov_ldap_manager-0.0.2.tar` & `mprov_ldap_manager-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 18:34:59.000000 mprov_ldap_manager-0.0.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:35:07.219207 mprov_ldap_manager-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-19 18:34:18.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:35:07.223207 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 18:35:07.000000 mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:47:16.287368 mprov_ldap_manager-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-28 18:47:16.287368 mprov_ldap_manager-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 18:47:09.000000 mprov_ldap_manager-0.0.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-28 18:47:16.291368 mprov_ldap_manager-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:47:16.287368 mprov_ldap_manager-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:47:16.287368 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-28 18:46:41.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:47:16.287368 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-28 18:47:16.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-28 18:47:16.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:47:16.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 18:47:16.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 18:47:16.000000 mprov_ldap_manager-0.0.3/src/mprov_ldap_manager.egg-info/top_level.txt
```

### Comparing `mprov_ldap_manager-0.0.2/LICENSE` & `mprov_ldap_manager-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mprov_ldap_manager-0.0.2/PKG-INFO` & `mprov_ldap_manager-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mprov_ldap_manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: An add-on to the mPCC to enable it to manage an LDAP directory.
 Home-page: https://github.com/mprov-ng/mprov_ldap_manager
 Author: Jason Williams
 Author-email: jasonw@jhu.edu
 Project-URL: Bug Tracker, https://github.com/mprov-ng/mprov_ldap_manager/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mprov_ldap_manager-0.0.2/README.md` & `mprov_ldap_manager-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mprov_ldap_manager-0.0.2/setup.cfg` & `mprov_ldap_manager-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/admin.py` & `mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,31 @@
 # Copyright (c) The django-ldapdb project
 
 
 from django import forms
 from django.contrib import admin
 from django.contrib.admin.widgets import FilteredSelectMultiple
 
-from .models import LdapGroup, LdapUser, LdapServer
+from .models import LdapGroup, LdapUser
+from django.forms import ModelForm, PasswordInput
 
+class LdapUserForm(ModelForm):
+    password = forms.CharField(widget=PasswordInput())
+    class Meta:
+        model = LdapUser
+        exclude = ['dn', 'photo'] 
+    def clean(self):
+        password = self.cleaned_data['password']
+        if not password or password == "":
+            del self.cleaned_data['password']
+        return self.cleaned_data
 
 class LdapUserAdmin(admin.ModelAdmin):
-    exclude = ['dn', 'password', 'photo']
+    form = LdapUserForm
+    exclude = ['dn', 'photo']
     list_display = ['username', 'first_name', 'last_name', 'email', 'uid']
     search_fields = ['first_name', 'last_name', 'full_name', 'username']
 
 
 class LdapGroupForm(forms.ModelForm):
     usernames = forms.ModelMultipleChoiceField(
         queryset=LdapUser.objects.all(),
```

### Comparing `mprov_ldap_manager-0.0.2/src/mprov_ldap_manager/models.py` & `mprov_ldap_manager-0.0.3/src/mprov_ldap_manager/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Defines the DB Models that will be used by this Django App or section of mProv
 # -*- coding: utf-8 -*-
 # excerpts from https://github.com/django-ldapdb/django-ldapdb/tree/master/examples
 # This software is distributed under the two-clause BSD license.
 # Copyright (c) The django-ldapdb project
 
 from django.db.models import Manager
+from django import forms
+
 
 import ldapdb.models
 from ldapdb.models import fields
 
 from django.db import models
 from django.conf import settings
 from django.dispatch import receiver
@@ -22,15 +24,15 @@
 # - cn -> fisrt name
 # - sn -> last name
 # - mail -> email
 # - 
 
 class LdapUser(ldapdb.models.Model):
     """
-    Class for representing an LDAP user entry.
+    Area for managing LDAP users
     """
     # LDAP meta-data
     base_dn = settings.DATABASES['ldap']['BASEDN']
     object_classes = ['posixAccount', 'shadowAccount', 'inetOrgPerson']
     last_modified = fields.DateTimeField(db_column='modifyTimestamp', editable=False)
 
     # inetOrgPerson
@@ -45,15 +47,15 @@
     # posixAccount
     uid = fields.IntegerField(db_column='uidNumber', unique=True)
     group = models.ForeignKey('LdapGroup', to_field='gid', db_column='gidNumber', on_delete=models.SET_NULL, null=True)
     gecos = fields.CharField(db_column='gecos')
     home_directory = fields.CharField(db_column='homeDirectory')
     login_shell = fields.CharField(db_column='loginShell', default='/bin/bash')
     username = fields.CharField(db_column='uid', primary_key=True)
-    password = fields.CharField(db_column='userPassword')
+    password = fields.CharField(db_column='userPassword', blank=True, null=True, help_text="To remain unchanged, leave blank")
 
     # shadowAccount
     last_password_change = fields.TimestampField(db_column='shadowLastChange')
 
     def __str__(self):
         return self.username
 
@@ -63,15 +65,15 @@
 # groups
 # cn -> groupname
 # gidNumber -> gid
 # memberUid -> uid of member (multiple allowed)
 
 class LdapGroup(ldapdb.models.Model):
     """
-    Class for representing an LDAP group entry.
+    Area for managing LDAP groups
     """
     # LDAP meta-data
     base_dn =  settings.DATABASES['ldap']['BASEDN']
     object_classes = ['posixGroup']
 
     # posixGroup attributes
     gid = fields.IntegerField(db_column='gidNumber', unique=True)
```

### Comparing `mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/PKG-INFO` & `mprov_ldap_manager-0.0.3/src/mprov_ldap_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mprov-ldap-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: An add-on to the mPCC to enable it to manage an LDAP directory.
 Home-page: https://github.com/mprov-ng/mprov_ldap_manager
 Author: Jason Williams
 Author-email: jasonw@jhu.edu
 Project-URL: Bug Tracker, https://github.com/mprov-ng/mprov_ldap_manager/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mprov_ldap_manager-0.0.2/src/mprov_ldap_manager.egg-info/SOURCES.txt` & `mprov_ldap_manager-0.0.3/src/mprov_ldap_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

