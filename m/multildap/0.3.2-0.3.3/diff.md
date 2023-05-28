# Comparing `tmp/multildap-0.3.2.tar.gz` & `tmp/multildap-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multildap-0.3.2.tar", last modified: Wed Jul 14 07:58:24 2021, max compression
+gzip compressed data, was "multildap-0.3.3.tar", last modified: Sun May 28 16:21:26 2023, max compression
```

## Comparing `multildap-0.3.2.tar` & `multildap-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2021-07-14 07:58:24.292387 multildap-0.3.2/
--rw-rw-r--   0 wert      (1000) wert      (1000)     9925 2021-07-14 07:58:24.292387 multildap-0.3.2/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)     7460 2020-03-04 17:48:48.000000 multildap-0.3.2/README.md
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2021-07-14 07:58:24.288387 multildap-0.3.2/multildap/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2019-07-31 12:00:28.000000 multildap-0.3.2/multildap/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2403 2021-07-14 07:55:57.000000 multildap-0.3.2/multildap/attr_rewrite.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     7801 2019-07-31 12:00:28.000000 multildap-0.3.2/multildap/client.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     6609 2019-07-31 12:00:28.000000 multildap-0.3.2/multildap/commands.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      621 2019-07-31 12:00:28.000000 multildap-0.3.2/multildap/decorators.py
--rwxrwxr-x   0 wert      (1000) wert      (1000)     9372 2021-07-14 07:54:24.000000 multildap-0.3.2/multildap/multildapd.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2021-07-14 07:58:24.292387 multildap-0.3.2/multildap/satosa/
--rw-rw-r--   0 wert      (1000) wert      (1000)     3617 2020-03-04 17:48:48.000000 multildap-0.3.2/multildap/satosa/multiple_ldap_attribute_store.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2021-07-14 07:58:24.292387 multildap-0.3.2/multildap.egg-info/
--rw-rw-r--   0 wert      (1000) wert      (1000)     9925 2021-07-14 07:58:24.000000 multildap-0.3.2/multildap.egg-info/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)      402 2021-07-14 07:58:24.000000 multildap-0.3.2/multildap.egg-info/SOURCES.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2021-07-14 07:58:24.000000 multildap-0.3.2/multildap.egg-info/dependency_links.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2021-07-14 07:58:24.000000 multildap-0.3.2/multildap.egg-info/not-zip-safe
--rw-rw-r--   0 wert      (1000) wert      (1000)       26 2021-07-14 07:58:24.000000 multildap-0.3.2/multildap.egg-info/requires.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)       27 2021-07-14 07:58:24.000000 multildap-0.3.2/multildap.egg-info/top_level.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)       38 2021-07-14 07:58:24.292387 multildap-0.3.2/setup.cfg
--rw-rw-r--   0 wert      (1000) wert      (1000)      930 2021-07-14 07:57:06.000000 multildap-0.3.2/setup.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-28 16:21:26.721586 multildap-0.3.3/
+-rw-rw-r--   0 wert      (1000) wert      (1000)       47 2023-05-28 16:20:30.000000 multildap-0.3.3/AUTHORS
+-rw-rw-r--   0 wert      (1000) wert      (1000)      834 2023-05-28 16:20:30.000000 multildap-0.3.3/LICENSE
+-rw-rw-r--   0 wert      (1000) wert      (1000)     7988 2023-05-28 16:21:26.721586 multildap-0.3.3/PKG-INFO
+-rw-rw-r--   0 wert      (1000) wert      (1000)     7460 2023-05-28 16:20:30.000000 multildap-0.3.3/README.md
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-28 16:21:26.721586 multildap-0.3.3/multildap/
+-rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-05-28 16:20:30.000000 multildap-0.3.3/multildap/__init__.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2403 2023-05-28 16:20:30.000000 multildap-0.3.3/multildap/attr_rewrite.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     7719 2023-05-28 16:20:30.000000 multildap-0.3.3/multildap/client.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6609 2023-05-28 16:20:30.000000 multildap-0.3.3/multildap/commands.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)      621 2023-05-28 16:20:30.000000 multildap-0.3.3/multildap/decorators.py
+-rwxrwxr-x   0 wert      (1000) wert      (1000)     9372 2023-05-28 16:20:30.000000 multildap-0.3.3/multildap/multildapd.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-28 16:21:26.721586 multildap-0.3.3/multildap/satosa/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3617 2023-05-28 16:20:30.000000 multildap-0.3.3/multildap/satosa/multiple_ldap_attribute_store.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-28 16:21:26.721586 multildap-0.3.3/multildap.egg-info/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     7988 2023-05-28 16:21:26.000000 multildap-0.3.3/multildap.egg-info/PKG-INFO
+-rw-rw-r--   0 wert      (1000) wert      (1000)      418 2023-05-28 16:21:26.000000 multildap-0.3.3/multildap.egg-info/SOURCES.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-28 16:21:26.000000 multildap-0.3.3/multildap.egg-info/dependency_links.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-28 16:21:26.000000 multildap-0.3.3/multildap.egg-info/not-zip-safe
+-rw-rw-r--   0 wert      (1000) wert      (1000)       13 2023-05-28 16:21:26.000000 multildap-0.3.3/multildap.egg-info/requires.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)       27 2023-05-28 16:21:26.000000 multildap-0.3.3/multildap.egg-info/top_level.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)       38 2023-05-28 16:21:26.721586 multildap-0.3.3/setup.cfg
+-rw-rw-r--   0 wert      (1000) wert      (1000)      888 2023-05-28 16:20:30.000000 multildap-0.3.3/setup.py
```

### Comparing `multildap-0.3.2/README.md` & `multildap-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `multildap-0.3.2/multildap/attr_rewrite.py` & `multildap-0.3.3/multildap/attr_rewrite.py`

 * *Files identical despite different names*

### Comparing `multildap-0.3.2/multildap/client.py` & `multildap-0.3.3/multildap/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         self.conf['connection']['client_strategy'] = strategy_type
         self.connect()
         self.strategy = strategy_type
 
     def ensure_connection(self):
         search_kwargs = copy.deepcopy(self.conf['search'])
         search_kwargs['size_limit'] = 1
-        search_kwargs['connect_timeout'] = self.conf['server']['connect_timeout']
         if self.conn and not self.conn.closed:
             try:
                 self.conn.search(**search_kwargs)
             except Exception as excp:
                 logger.debug('Connection error: {}...'.format(excp))
                 self.connect()
         else:
```

### Comparing `multildap-0.3.2/multildap/commands.py` & `multildap-0.3.3/multildap/commands.py`

 * *Files identical despite different names*

### Comparing `multildap-0.3.2/multildap/decorators.py` & `multildap-0.3.3/multildap/decorators.py`

 * *Files identical despite different names*

### Comparing `multildap-0.3.2/multildap/multildapd.py` & `multildap-0.3.3/multildap/multildapd.py`

 * *Files identical despite different names*

### Comparing `multildap-0.3.2/multildap/satosa/multiple_ldap_attribute_store.py` & `multildap-0.3.3/multildap/satosa/multiple_ldap_attribute_store.py`

 * *Files identical despite different names*

### Comparing `multildap-0.3.2/setup.py` & `multildap-0.3.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 _name = 'multildap'
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(name=_name,
-      version='0.3.2',
+      version='0.3.3',
       zip_safe = False,
       description="LDAP client or proxy to multiple LDAP server",
       long_description=readme(),
       long_description_content_type="text/markdown",
       classifiers=['Development Status :: 5 - Production/Stable',
                    'License :: OSI Approved :: BSD License',
                    'Programming Language :: Python :: 2',
                    'Programming Language :: Python :: 3'],
-      url='https://github.com/peppelinux/{}'.format(_name),
+      url='https://github.com/peppelinux/pyMultiLDAP',
       author='Giuseppe De Marco',
       author_email='giuseppe.demarco@unical.it',
       license='BSD',
       scripts=['{}/multildapd.py'.format(_name)],
       packages=[_name, 'multildap/satosa'],
-      install_requires=[
-        'ldap3>=2.9',
-        'gevent>=21.1.2'
-      ],
+      install_requires=['ldap3', 'gevent'],
      )
```

