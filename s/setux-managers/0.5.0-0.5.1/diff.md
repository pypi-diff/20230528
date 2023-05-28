# Comparing `tmp/setux_managers-0.5.0.tar.gz` & `tmp/setux_managers-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setux_managers-0.5.0.tar", last modified: Mon Aug 31 09:22:24 2020, max compression
+gzip compressed data, was "dist/setux_managers-0.5.1.tar", last modified: Mon Aug 31 13:36:24 2020, max compression
```

## Comparing `setux_managers-0.5.0.tar` & `setux_managers-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/
--rw-r--r--   0 louis     (4444) louis     (4444)     1231 2020-08-31 09:22:24.519998 setux_managers-0.5.0/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      235 2020-08-09 08:17:01.000000 setux_managers-0.5.0/README.rst
--rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setup.cfg
--rw-r--r--   0 louis     (4444) louis     (4444)     1262 2020-08-31 09:00:45.000000 setux_managers-0.5.0/setup.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/common/
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/common/file/
--rw-r--r--   0 louis     (4444) louis     (4444)       50 2020-08-09 08:17:01.000000 setux_managers-0.5.0/setux/managers/common/file/__init__.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1486 2020-08-31 09:00:27.000000 setux_managers-0.5.0/setux/managers/common/file/directory.py
--rw-r--r--   0 louis     (4444) louis     (4444)     2069 2020-08-31 09:00:27.000000 setux_managers-0.5.0/setux/managers/common/file/file.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/common/host/
--rw-r--r--   0 louis     (4444) louis     (4444)       34 2020-08-09 08:17:01.000000 setux_managers-0.5.0/setux/managers/common/host/__init__.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1362 2020-08-31 09:00:21.000000 setux_managers-0.5.0/setux/managers/common/host/host.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/common/package/
--rw-r--r--   0 louis     (4444) louis     (4444)       63 2020-08-09 08:17:01.000000 setux_managers-0.5.0/setux/managers/common/package/__init__.py
--rw-r--r--   0 louis     (4444) louis     (4444)      747 2020-08-09 08:17:01.000000 setux_managers-0.5.0/setux/managers/common/package/gem.py
--rw-r--r--   0 louis     (4444) louis     (4444)      725 2020-08-09 08:17:01.000000 setux_managers-0.5.0/setux/managers/common/package/npm.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1298 2020-08-31 09:00:45.000000 setux_managers-0.5.0/setux/managers/common/package/pip.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/common/user/
--rw-r--r--   0 louis     (4444) louis     (4444)      162 2020-08-31 09:00:27.000000 setux_managers-0.5.0/setux/managers/common/user/__init__.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1063 2020-08-31 09:00:27.000000 setux_managers-0.5.0/setux/managers/common/user/group.py
--rw-r--r--   0 louis     (4444) louis     (4444)      836 2020-08-24 11:54:10.000000 setux_managers-0.5.0/setux/managers/common/user/groups.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1631 2020-08-31 09:00:27.000000 setux_managers-0.5.0/setux/managers/common/user/user.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/system/
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/system/package/
--rw-r--r--   0 louis     (4444) louis     (4444)     2194 2020-08-31 09:00:27.000000 setux_managers-0.5.0/setux/managers/system/package/apt.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux/managers/system/service/
--rw-r--r--   0 louis     (4444) louis     (4444)     1028 2020-08-09 08:17:01.000000 setux_managers-0.5.0/setux/managers/system/service/systemd.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:22:24.519998 setux_managers-0.5.0/setux_managers.egg-info/
--rw-r--r--   0 louis     (4444) louis     (4444)     1231 2020-08-31 09:22:24.000000 setux_managers-0.5.0/setux_managers.egg-info/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      784 2020-08-31 09:22:24.000000 setux_managers-0.5.0/setux_managers.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (4444) louis     (4444)        1 2020-08-31 09:22:24.000000 setux_managers-0.5.0/setux_managers.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (4444) louis     (4444)       33 2020-08-31 09:22:24.000000 setux_managers-0.5.0/setux_managers.egg-info/requires.txt
--rw-r--r--   0 louis     (4444) louis     (4444)        6 2020-08-31 09:22:24.000000 setux_managers-0.5.0/setux_managers.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/
+-rw-rw-r--   0 louis     (4444) louis     (4444)     1231 2020-08-31 13:36:24.000000 setux_managers-0.5.1/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      235 2020-08-09 08:17:01.000000 setux_managers-0.5.1/README.rst
+-rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setup.cfg
+-rw-r--r--   0 louis     (4444) louis     (4444)     1262 2020-08-31 13:28:29.000000 setux_managers-0.5.1/setup.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/common/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/common/file/
+-rw-r--r--   0 louis     (4444) louis     (4444)       50 2020-08-09 08:17:01.000000 setux_managers-0.5.1/setux/managers/common/file/__init__.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1486 2020-08-31 09:00:27.000000 setux_managers-0.5.1/setux/managers/common/file/directory.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     2069 2020-08-31 09:00:27.000000 setux_managers-0.5.1/setux/managers/common/file/file.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/common/host/
+-rw-r--r--   0 louis     (4444) louis     (4444)       34 2020-08-09 08:17:01.000000 setux_managers-0.5.1/setux/managers/common/host/__init__.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1362 2020-08-31 09:00:21.000000 setux_managers-0.5.1/setux/managers/common/host/host.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/common/package/
+-rw-r--r--   0 louis     (4444) louis     (4444)       63 2020-08-09 08:17:01.000000 setux_managers-0.5.1/setux/managers/common/package/__init__.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      747 2020-08-09 08:17:01.000000 setux_managers-0.5.1/setux/managers/common/package/gem.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      725 2020-08-09 08:17:01.000000 setux_managers-0.5.1/setux/managers/common/package/npm.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1239 2020-08-31 13:27:42.000000 setux_managers-0.5.1/setux/managers/common/package/pip.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/common/user/
+-rw-r--r--   0 louis     (4444) louis     (4444)      162 2020-08-31 09:00:27.000000 setux_managers-0.5.1/setux/managers/common/user/__init__.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1063 2020-08-31 09:00:27.000000 setux_managers-0.5.1/setux/managers/common/user/group.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      836 2020-08-24 11:54:10.000000 setux_managers-0.5.1/setux/managers/common/user/groups.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1631 2020-08-31 09:00:27.000000 setux_managers-0.5.1/setux/managers/common/user/user.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/system/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/system/package/
+-rw-r--r--   0 louis     (4444) louis     (4444)     2194 2020-08-31 09:00:27.000000 setux_managers-0.5.1/setux/managers/system/package/apt.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux/managers/system/service/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1028 2020-08-09 08:17:01.000000 setux_managers-0.5.1/setux/managers/system/service/systemd.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:36:24.000000 setux_managers-0.5.1/setux_managers.egg-info/
+-rw-rw-r--   0 louis     (4444) louis     (4444)     1231 2020-08-31 13:36:23.000000 setux_managers-0.5.1/setux_managers.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (4444) louis     (4444)      784 2020-08-31 13:36:23.000000 setux_managers-0.5.1/setux_managers.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)        1 2020-08-31 13:36:23.000000 setux_managers-0.5.1/setux_managers.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)       33 2020-08-31 13:36:23.000000 setux_managers-0.5.1/setux_managers.egg-info/requires.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)        6 2020-08-31 13:36:23.000000 setux_managers-0.5.1/setux_managers.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `setux_managers-0.5.0/PKG-INFO` & `setux_managers-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: setux_managers
-Version: 0.5.0
+Version: 0.5.1
 Summary: System deployment
 Home-page: https://bitbucket.org/dugres/setux_managers
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ########
          setux
```

### Comparing `setux_managers-0.5.0/setup.py` & `setux_managers-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_namespace_packages
 
 curdir = abspath(dirname(__file__))
 readme = open(join(curdir, 'README.rst')).read()
 
 setup(
     name             = 'setux_managers',
-    version          = '0.5.0',
+    version          = '0.5.1',
     description      = 'System deployment',
     long_description = readme,
     keywords         = ['utility', ],
     url              = 'https://bitbucket.org/dugres/setux_managers',
     author           = 'Louis RIVIERE',
     author_email     = 'louis@riviere.xyz',
     license          = 'MIT',
```

### Comparing `setux_managers-0.5.0/setux/managers/common/file/directory.py` & `setux_managers-0.5.1/setux/managers/common/file/directory.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/common/file/file.py` & `setux_managers-0.5.1/setux/managers/common/file/file.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/common/host/host.py` & `setux_managers-0.5.1/setux/managers/common/host/host.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/common/package/gem.py` & `setux_managers-0.5.1/setux/managers/common/package/gem.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/common/package/npm.py` & `setux_managers-0.5.1/setux/managers/common/package/npm.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/common/package/pip.py` & `setux_managers-0.5.1/setux/managers/common/package/pip.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,14 @@
                 yield n, v
             except:
                 error(line)
 
     def do_init(self):
         self.target.Package.install('pip')
         self.run(f'python3 -m pip install -qU pip')
-        self.run(f'python3 -m pip install -qU setuptools')
 
     def do_install(self, pkg, ver=None):
         ret, out, err = self.run(f'python3 -m pip install -qU {pkg}')
         for i in out:
             if ('already satisfied' in i
                 or 'Successfully installed' in i
             ):
```

### Comparing `setux_managers-0.5.0/setux/managers/common/user/group.py` & `setux_managers-0.5.1/setux/managers/common/user/group.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/common/user/groups.py` & `setux_managers-0.5.1/setux/managers/common/user/groups.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/common/user/user.py` & `setux_managers-0.5.1/setux/managers/common/user/user.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/system/package/apt.py` & `setux_managers-0.5.1/setux/managers/system/package/apt.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux/managers/system/service/systemd.py` & `setux_managers-0.5.1/setux/managers/system/service/systemd.py`

 * *Files identical despite different names*

### Comparing `setux_managers-0.5.0/setux_managers.egg-info/PKG-INFO` & `setux_managers-0.5.1/setux_managers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: setux-managers
-Version: 0.5.0
+Version: 0.5.1
 Summary: System deployment
 Home-page: https://bitbucket.org/dugres/setux_managers
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ########
          setux
```

### Comparing `setux_managers-0.5.0/setux_managers.egg-info/SOURCES.txt` & `setux_managers-0.5.1/setux_managers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

