# Comparing `tmp/debspawn-0.6.1.tar.gz` & `tmp/debspawn-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debspawn-0.6.1.tar", last modified: Thu Feb  2 21:42:08 2023, max compression
+gzip compressed data, was "debspawn-0.6.2.tar", last modified: Sun May 28 16:13:54 2023, max compression
```

## Comparing `debspawn-0.6.1.tar` & `debspawn-0.6.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-02-02 21:42:08.400337 debspawn-0.6.1/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       40 2022-02-11 23:20:53.000000 debspawn-0.6.1/AUTHORS
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7651 2022-02-11 23:20:53.000000 debspawn-0.6.1/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      115 2022-02-11 23:20:53.000000 debspawn-0.6.1/MANIFEST.in
--rw-r--r--   0 matthias  (1000) matthias  (1000)    10863 2023-02-02 21:42:08.400337 debspawn-0.6.1/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    10355 2022-02-11 23:20:53.000000 debspawn-0.6.1/README.md
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-02-02 21:42:08.388337 debspawn-0.6.1/data/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-02-02 21:42:08.392337 debspawn-0.6.1/data/services/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      499 2022-10-02 17:18:43.000000 debspawn-0.6.1/data/services/debspawn-clear-caches.service
--rw-r--r--   0 matthias  (1000) matthias  (1000)      461 2021-11-08 18:48:17.000000 debspawn-0.6.1/data/services/debspawn-clear-caches.timer
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-02-02 21:42:08.392337 debspawn-0.6.1/data/tmpfiles.d/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      407 2021-11-08 18:48:17.000000 debspawn-0.6.1/data/tmpfiles.d/debspawn.conf
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-02-02 21:42:08.392337 debspawn-0.6.1/debspawn/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      866 2022-10-02 17:15:54.000000 debspawn-0.6.1/debspawn/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3333 2022-02-21 12:43:23.000000 debspawn-0.6.1/debspawn/aptcache.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    21069 2023-01-26 22:58:50.000000 debspawn-0.6.1/debspawn/build.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    23304 2022-08-20 00:05:16.000000 debspawn-0.6.1/debspawn/cli.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5758 2022-10-01 01:17:56.000000 debspawn-0.6.1/debspawn/config.py
--rwxr-xr-x   0 matthias  (1000) matthias  (1000)    12781 2023-01-15 19:32:20.000000 debspawn-0.6.1/debspawn/dsrun
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4128 2022-02-21 12:41:37.000000 debspawn-0.6.1/debspawn/injectpkg.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8173 2022-09-30 23:32:01.000000 debspawn-0.6.1/debspawn/maintain.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    13607 2022-09-30 23:09:51.000000 debspawn-0.6.1/debspawn/nspawn.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    41892 2023-01-15 19:36:07.000000 debspawn-0.6.1/debspawn/osbase.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-02-02 21:42:08.396337 debspawn-0.6.1/debspawn/utils/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1408 2022-08-20 01:49:07.000000 debspawn-0.6.1/debspawn/utils/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3172 2022-02-21 12:41:37.000000 debspawn-0.6.1/debspawn/utils/command.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6130 2022-02-21 12:41:37.000000 debspawn-0.6.1/debspawn/utils/env.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5925 2022-10-01 00:16:21.000000 debspawn-0.6.1/debspawn/utils/log.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    10699 2022-08-20 03:33:44.000000 debspawn-0.6.1/debspawn/utils/misc.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1983 2022-02-21 12:43:22.000000 debspawn-0.6.1/debspawn/utils/zstd_tar.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-02-02 21:42:08.396337 debspawn-0.6.1/debspawn.egg-info/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    10863 2023-02-02 21:42:08.000000 debspawn-0.6.1/debspawn.egg-info/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1015 2023-02-02 21:42:08.000000 debspawn-0.6.1/debspawn.egg-info/SOURCES.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-02-02 21:42:08.000000 debspawn-0.6.1/debspawn.egg-info/dependency_links.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-02-02 21:42:08.000000 debspawn-0.6.1/debspawn.egg-info/not-zip-safe
--rw-r--r--   0 matthias  (1000) matthias  (1000)       13 2023-02-02 21:42:08.000000 debspawn-0.6.1/debspawn.egg-info/requires.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        9 2023-02-02 21:42:08.000000 debspawn-0.6.1/debspawn.egg-info/top_level.txt
--rwxr-xr-x   0 matthias  (1000) matthias  (1000)      236 2022-02-21 12:41:37.000000 debspawn-0.6.1/debspawn.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-02-02 21:42:08.400337 debspawn-0.6.1/docs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-11 23:20:53.000000 debspawn-0.6.1/docs/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4685 2022-02-21 12:43:23.000000 debspawn-0.6.1/docs/assemble_man.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5650 2022-10-13 23:41:39.000000 debspawn-0.6.1/docs/debspawn-build.1.xml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2720 2022-10-13 23:51:55.000000 debspawn-0.6.1/docs/debspawn-create.1.xml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1745 2022-10-13 23:50:08.000000 debspawn-0.6.1/docs/debspawn-delete.1.xml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1510 2022-10-13 23:41:22.000000 debspawn-0.6.1/docs/debspawn-list.1.xml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1817 2022-10-13 23:49:41.000000 debspawn-0.6.1/docs/debspawn-login.1.xml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2538 2022-10-13 23:49:36.000000 debspawn-0.6.1/docs/debspawn-maintain.1.xml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2108 2022-10-13 23:49:28.000000 debspawn-0.6.1/docs/debspawn-run.1.xml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2436 2022-10-13 23:48:56.000000 debspawn-0.6.1/docs/debspawn-update.1.xml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     9679 2022-10-13 23:41:01.000000 debspawn-0.6.1/docs/debspawn.1.xml
--rwxr-xr-x   0 matthias  (1000) matthias  (1000)     4358 2022-02-21 12:43:23.000000 debspawn-0.6.1/install-sysdata.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1116 2022-08-20 03:20:05.000000 debspawn-0.6.1/pyproject.toml
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      130 2023-02-02 21:42:08.400337 debspawn-0.6.1/setup.cfg
--rwxr-xr-x   0 matthias  (1000) matthias  (1000)     4376 2022-10-01 01:13:13.000000 debspawn-0.6.1/setup.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 16:13:54.722529 debspawn-0.6.2/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       40 2022-02-11 23:20:53.000000 debspawn-0.6.2/AUTHORS
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     7651 2022-02-11 23:20:53.000000 debspawn-0.6.2/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      115 2022-02-11 23:20:53.000000 debspawn-0.6.2/MANIFEST.in
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    10863 2023-05-28 16:13:54.722529 debspawn-0.6.2/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    10355 2022-02-11 23:20:53.000000 debspawn-0.6.2/README.md
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 16:13:54.718529 debspawn-0.6.2/data/
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 16:13:54.722529 debspawn-0.6.2/data/services/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      499 2022-10-02 17:18:43.000000 debspawn-0.6.2/data/services/debspawn-clear-caches.service
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      461 2021-11-08 18:48:17.000000 debspawn-0.6.2/data/services/debspawn-clear-caches.timer
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 16:13:54.722529 debspawn-0.6.2/data/tmpfiles.d/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      407 2021-11-08 18:48:17.000000 debspawn-0.6.2/data/tmpfiles.d/debspawn.conf
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 16:13:54.722529 debspawn-0.6.2/debspawn/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      866 2023-02-02 21:43:01.000000 debspawn-0.6.2/debspawn/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3333 2022-02-21 12:43:23.000000 debspawn-0.6.2/debspawn/aptcache.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    21155 2023-02-03 03:06:04.000000 debspawn-0.6.2/debspawn/build.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    23304 2022-08-20 00:05:16.000000 debspawn-0.6.2/debspawn/cli.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5758 2022-10-01 01:17:56.000000 debspawn-0.6.2/debspawn/config.py
+-rwxr-xr-x   0 matthias  (1000) matthias  (1000)    12551 2023-05-27 23:26:07.000000 debspawn-0.6.2/debspawn/dsrun
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4128 2022-02-21 12:41:37.000000 debspawn-0.6.2/debspawn/injectpkg.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8173 2022-09-30 23:32:01.000000 debspawn-0.6.2/debspawn/maintain.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    13636 2023-02-03 03:02:48.000000 debspawn-0.6.2/debspawn/nspawn.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    44310 2023-05-28 15:58:20.000000 debspawn-0.6.2/debspawn/osbase.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 16:13:54.722529 debspawn-0.6.2/debspawn/utils/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1408 2022-08-20 01:49:07.000000 debspawn-0.6.2/debspawn/utils/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3172 2022-02-21 12:41:37.000000 debspawn-0.6.2/debspawn/utils/command.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6130 2022-02-21 12:41:37.000000 debspawn-0.6.2/debspawn/utils/env.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5925 2022-10-01 00:16:21.000000 debspawn-0.6.2/debspawn/utils/log.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    10780 2023-02-03 03:08:53.000000 debspawn-0.6.2/debspawn/utils/misc.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2054 2023-02-03 03:08:53.000000 debspawn-0.6.2/debspawn/utils/zstd_tar.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 16:13:54.722529 debspawn-0.6.2/debspawn.egg-info/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    10863 2023-05-28 16:13:54.000000 debspawn-0.6.2/debspawn.egg-info/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1015 2023-05-28 16:13:54.000000 debspawn-0.6.2/debspawn.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-05-28 16:13:54.000000 debspawn-0.6.2/debspawn.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2023-05-28 16:13:54.000000 debspawn-0.6.2/debspawn.egg-info/not-zip-safe
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       13 2023-05-28 16:13:54.000000 debspawn-0.6.2/debspawn.egg-info/requires.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        9 2023-05-28 16:13:54.000000 debspawn-0.6.2/debspawn.egg-info/top_level.txt
+-rwxr-xr-x   0 matthias  (1000) matthias  (1000)      236 2022-02-21 12:41:37.000000 debspawn-0.6.2/debspawn.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-05-28 16:13:54.722529 debspawn-0.6.2/docs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-11 23:20:53.000000 debspawn-0.6.2/docs/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4682 2023-05-27 22:45:06.000000 debspawn-0.6.2/docs/assemble_man.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     5650 2022-10-13 23:41:39.000000 debspawn-0.6.2/docs/debspawn-build.1.xml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2720 2022-10-13 23:51:55.000000 debspawn-0.6.2/docs/debspawn-create.1.xml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1745 2022-10-13 23:50:08.000000 debspawn-0.6.2/docs/debspawn-delete.1.xml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1510 2022-10-13 23:41:22.000000 debspawn-0.6.2/docs/debspawn-list.1.xml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1817 2022-10-13 23:49:41.000000 debspawn-0.6.2/docs/debspawn-login.1.xml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2538 2022-10-13 23:49:36.000000 debspawn-0.6.2/docs/debspawn-maintain.1.xml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2108 2022-10-13 23:49:28.000000 debspawn-0.6.2/docs/debspawn-run.1.xml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2436 2022-10-13 23:48:56.000000 debspawn-0.6.2/docs/debspawn-update.1.xml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     9679 2022-10-13 23:41:01.000000 debspawn-0.6.2/docs/debspawn.1.xml
+-rwxr-xr-x   0 matthias  (1000) matthias  (1000)     4358 2022-02-21 12:43:23.000000 debspawn-0.6.2/install-sysdata.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1116 2022-08-20 03:20:05.000000 debspawn-0.6.2/pyproject.toml
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      130 2023-05-28 16:13:54.722529 debspawn-0.6.2/setup.cfg
+-rwxr-xr-x   0 matthias  (1000) matthias  (1000)     4376 2022-10-01 01:13:13.000000 debspawn-0.6.2/setup.py
```

### Comparing `debspawn-0.6.1/LICENSE` & `debspawn-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/PKG-INFO` & `debspawn-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debspawn
-Version: 0.6.1
+Version: 0.6.2
 Summary: Debian package builder and build helper using systemd-nspawn
 Home-page: https://github.com/lkhq/debspawn
 Author: Matthias Klumpp
 Author-email: Matthias Klumpp <matthias@tenstral.net>
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://github.com/lkhq/debspawn
 Project-URL: Source, https://github.com/lkhq/debspawn
```

### Comparing `debspawn-0.6.1/README.md` & `debspawn-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/__init__.py` & `debspawn-0.6.2/debspawn/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this software.  If not, see <http://www.gnu.org/licenses/>.
 
 __appname__ = 'debspawn'
-__version__ = '0.6.1'
+__version__ = '0.6.2'
```

### Comparing `debspawn-0.6.1/debspawn/aptcache.py` & `debspawn-0.6.2/debspawn/aptcache.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/build.py` & `debspawn-0.6.2/debspawn/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,18 @@
     safe_copy,
     format_filesize,
     version_noepoch,
 )
 from .utils.command import safe_run
 
 
+class BuildError(Exception):
+    """Package build failed with a generic error."""
+
+
 def interact_with_build_environment(
     osbase,
     instance_dir,
     machine_name,
     *,
     pkg_dir_root,
     source_pkg_dir,
@@ -191,15 +195,15 @@
     source_pkg_dir=None,
     buildflags: list[str] = None,
     build_env: dict[str, str] = None,
 ):
     '''Perform the actual build on an extracted package directory'''
     assert not build_only or isinstance(build_only, str)
     if not pkg_dir:
-        raise Exception('Package directory is missing!')
+        raise ValueError('Package directory is missing!')
     pkg_dir = os.path.normpath(pkg_dir)
     if not build_env:
         build_env = {}
 
     # get a fresh UID to give to our build user within the container
     builder_uid = get_random_free_uid_gid()[0]
 
@@ -328,15 +332,15 @@
     print_info('Architecture: {}'.format(osbase.arch))
     print_info()
 
 
 def _read_source_package_details():
     out, err, ret = safe_run(['dpkg-parsechangelog'])
     if ret != 0:
-        raise Exception('Running dpkg-parsechangelog failed: {}{}'.format(out, err))
+        raise BuildError('Running dpkg-parsechangelog failed: {}{}'.format(out, err))
 
     pkg_sourcename = None
     pkg_version = None
     for line in out.split('\n'):
         if line.startswith('Source: '):
             pkg_sourcename = line[8:].strip()
         elif line.startswith('Version: '):
```

### Comparing `debspawn-0.6.1/debspawn/cli.py` & `debspawn-0.6.2/debspawn/cli.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/config.py` & `debspawn-0.6.2/debspawn/config.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/dsrun` & `debspawn-0.6.2/debspawn/dsrun`

 * *Files 2% similar despite different names*

```diff
@@ -215,19 +215,14 @@
         if os.path.isdir(f):
             os.chdir(f)
             break
 
     print_section('Installing package build-dependencies')
     with eatmydata():
         cmd = ['build-dep']
-        # allow installations of packages from the suite we are building
-        # for, needed to use dependencies from a `NotAutomatic` suite
-        # like "experimental".
-        if suite:
-            cmd.extend(['-t', suite])
         if arch_only:
             cmd.append('--arch-only')
         cmd.append('./')
         run_apt_command(cmd)
 
     return True
```

### Comparing `debspawn-0.6.1/debspawn/injectpkg.py` & `debspawn-0.6.2/debspawn/injectpkg.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/maintain.py` & `debspawn-0.6.2/debspawn/maintain.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/nspawn.py` & `debspawn-0.6.2/debspawn/nspawn.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     osbase,
     base_dir,
     machine_name,
     helper_flags,
     chdir='/tmp',
     *,
     build_uid: int,
-    nspawn_flags=[],
+    nspawn_flags: T.Union[list[str], str] = None,
     tmp_apt_cache_dir=None,
     pkginjector=None,
     allowed: list[str] = None,
     syscall_filter: list[str] = None,
     env_vars: dict[str, str] = None,
     private_users: bool = False,
 ):
```

### Comparing `debspawn-0.6.1/debspawn/osbase.py` & `debspawn-0.6.2/debspawn/osbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 self._custom_name = None
         if self._custom_name == self._suite:
             self._custom_name = None
 
         if not self._arch:
             out, _, ret = safe_run(['dpkg', '--print-architecture'])
             if ret != 0:
-                raise Exception('Running dpkg --print-architecture failed: {}'.format(out))
+                raise RuntimeError('Running dpkg --print-architecture failed: {}'.format(out))
 
             self._arch = out.strip()
         if self._custom_name:
             return self._custom_name
         elif self._variant:
             return '{}-{}-{}'.format(self._suite, self._variant, self._arch)
         else:
@@ -306,15 +306,22 @@
         self, mirror, components, extra_suites, extra_source_lines, *, allow_recommends: bool, with_init: bool
     ):
         '''
         Create configuration file for this container base image
         '''
 
         print_info('Saving configuration settings.')
-        data: T.Dict[str, T.Union[str, bool]] = {'Suite': self.suite, 'Architecture': self.arch}
+        data: T.Dict[str, T.Union[str, bool]] = {
+            'Name': self.name,
+            'CustomName': self._custom_name,
+            'Suite': self.suite,
+            'BaseSuite': self.base_suite,
+            'Architecture': self.arch,
+        }
+
         if self.variant:
             data['Variant'] = self.variant
         if mirror:
             data['Mirror'] = mirror
         if components:
             data['Components'] = components
         if extra_suites:
@@ -383,14 +390,51 @@
         proxyconf_fname = os.path.join(instance_dir, 'etc', 'apt', 'apt.conf.d', '98debspawn_proxy')
         with open(proxyconf_fname, 'w') as f:
             if http_proxy:
                 f.write('Acquire::http::Proxy "{}";\n'.format(http_proxy))
             if https_proxy:
                 f.write('Acquire::https::Proxy "{}";\n'.format(https_proxy))
 
+    def _setup_apt_repo_preferences(self, instance_dir, preferred_suites):
+        '''Setup APT repository preferences.
+        APT somtimes wants to install packages from older repositories to satisfy
+        dependencies, even though we must build with versions from the newer repositories.
+        This especially is the case for `NotAutomatic` suites like "experimental", where packages
+        would not get auto-installed from.
+        Passing "-t <suite>" to the APT commands restricts the solver way too much, so
+        valid dependency chains are no chosen for partial suites if the suites don't
+        contain all dependencies as well.
+        This is a compromise to make APT do the right thing, by simply setting all suites
+        to the same priority.
+        NOTE: With suites like experimental, we may need to set the preferences later if we want
+        to avoid experimental packages being added to the base image. That comes with its own
+        difficulties though, so we avoid that for now.
+        '''
+
+        # enusre all suites are represented in the "preferred suites" list
+        if not preferred_suites:
+            preferred_suites = []
+        if self.has_base_suite:
+            if self.base_suite not in preferred_suites:
+                preferred_suites.insert(0, self.base_suite)
+        if self.suite not in preferred_suites:
+            preferred_suites.insert(0, self.suite)
+
+        aptpref_fname = os.path.join(instance_dir, 'etc', 'apt', 'preferences.d', '10debspawn')
+        with open(aptpref_fname, 'w') as f:
+            first = True
+            for suite in preferred_suites:
+                if not first:
+                    f.write('\n')
+                first = False
+                priority = 500
+                if suite == self.suite:
+                    priority = 600
+                f.write(('Package: *\n' 'Pin: release a={}\n' 'Pin-Priority: {}\n').format(suite, priority))
+
     def _create_internal(
         self,
         mirror=None,
         components=None,
         *,
         extra_suites: list[str] = None,
         extra_source_lines: str = None,
@@ -508,14 +552,17 @@
                             )
 
                     if extra_source_lines:
                         f.write('\n')
                         for line in extra_source_lines.split('\\n'):
                             f.write('{}\n'.format(line.strip()))
 
+            # set preference suites in dependency resolution
+            self._setup_apt_repo_preferences(tdir, extra_suites)
+
             # write our default APT settings for this container
             aptconf_fname = os.path.join(tdir, 'etc', 'apt', 'apt.conf.d', '99debspawn')
             with open(aptconf_fname, 'w') as f:
                 # fail immediately with a proper exit code when e.g. apt update fails,
                 # so we can retry and don't silently use old packages
                 # (only available with newer APT versions)
                 f.write('APT::Update::Error-Mode "any";\n')
@@ -741,15 +788,18 @@
             return False
 
         print_header('Recreating container image')
 
         # read configuration data
         with open(config_fname, 'rt') as f:
             cdata: T.Dict[str, T.Union[str, bool]] = json.loads(f.read())
+            self._name = cdata.get('Name', self.name)
+            self._custom_name = cdata.get('CustomName', self._custom_name)
             self._suite = cdata.get('Suite', self.suite)
+            self._base_suite = cdata.get('BaseSuite', self.base_suite)
             self._arch = cdata.get('Architecture', self.arch)
             self._variant = cdata.get('Variant', self.variant)
             mirror = cdata.get('Mirror')
             components = cdata.get('Components')
             extra_suites = cdata.get('ExtraSuites', [])
             extra_source_lines = cdata.get('ExtraSourceLines')
             allow_recommends = cdata.get('AllowRecommends', False)
```

### Comparing `debspawn-0.6.1/debspawn/utils/__init__.py` & `debspawn-0.6.2/debspawn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/utils/command.py` & `debspawn-0.6.2/debspawn/utils/command.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/utils/env.py` & `debspawn-0.6.2/debspawn/utils/env.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/utils/log.py` & `debspawn-0.6.2/debspawn/utils/log.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/debspawn/utils/misc.py` & `debspawn-0.6.2/debspawn/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 import subprocess
 from pathlib import Path
 from contextlib import contextmanager
 
 from ..config import GlobalConfig
 
 
+class MountError(Exception):
+    """Error while dealing with mountpoints."""
+
+
 def listify(item: T.Any):
     '''
     Return a list of :item, unless :item already is a lit.
     '''
     if not item:
         return []
     return item if type(item) == list else [item]
@@ -198,27 +202,27 @@
 
 def bindmount(from_path, to_path):
     '''Create a bindmount point.'''
 
     cmd = ['mount', '--bind', from_path, to_path]
     ret = subprocess.run(cmd, capture_output=True, check=False)
     if ret.returncode != 0:
-        raise Exception('Unable to create bindmount {} -> {}'.format(from_path, to_path))
+        raise MountError('Unable to create bindmount {} -> {}'.format(from_path, to_path))
 
 
 def umount(path, lazy: bool = True):
     '''Try to unmount a path.'''
 
     cmd = ['umount']
     if lazy:
         cmd.append('-l')
     cmd.append(path)
     ret = subprocess.run(cmd, capture_output=True, check=False)
     if ret.returncode != 0:
-        raise Exception('Unable to umount path {}'.format(path))
+        raise MountError('Unable to umount path {}'.format(path))
 
     # try again if the mountpoint is still there, as
     # overmounting may have happened
     if is_mountpoint(path):
         umount(path, lazy=lazy)
```

### Comparing `debspawn-0.6.1/debspawn/utils/zstd_tar.py` & `debspawn-0.6.2/debspawn/utils/zstd_tar.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,43 +18,47 @@
 # along with this software.  If not, see <http://www.gnu.org/licenses/>.
 
 import shutil
 
 from .command import run_command
 
 
+class TarError(Exception):
+    """Generic error while using tar/zstd."""
+
+
 def ensure_tar_zstd():
     '''Check if the required binaries for compression are available'''
 
     if not shutil.which('zstd'):
-        raise Exception(
+        raise TarError(
             (
                 'The "zsdt" binary was not found, we can not compress tarballs. '
                 'Please install zstd to continue!'
             )
         )
     if not shutil.which('tar'):
-        raise Exception(
+        raise TarError(
             'The "tar" binary was not found, we can not create tarballs. Please install tar to continue!'
         )
 
 
 def compress_directory(dirname, tarname):
     '''Compress a directory to a given tarball'''
 
     cmd = ['tar', '-C', dirname, '-I', 'zstd', '-cf', tarname, '.']
 
     out, err, ret = run_command(cmd)
 
     if ret != 0:
-        raise Exception('Unable to create tarball "{}":\n{}{}'.format(tarname, out, err))
+        raise TarError('Unable to create tarball "{}":\n{}{}'.format(tarname, out, err))
 
 
 def decompress_tarball(tarname, dirname):
     '''Compress a directory to a given tarball'''
 
     cmd = ['tar', '-C', dirname, '-I', 'zstd', '-xf', tarname]
 
     out, err, ret = run_command(cmd)
 
     if ret != 0:
-        raise Exception('Unable to decompress tarball "{}":\n{}{}'.format(tarname, out, err))
+        raise TarError('Unable to decompress tarball "{}":\n{}{}'.format(tarname, out, err))
```

### Comparing `debspawn-0.6.1/debspawn.egg-info/PKG-INFO` & `debspawn-0.6.2/debspawn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debspawn
-Version: 0.6.1
+Version: 0.6.2
 Summary: Debian package builder and build helper using systemd-nspawn
 Home-page: https://github.com/lkhq/debspawn
 Author: Matthias Klumpp
 Author-email: Matthias Klumpp <matthias@tenstral.net>
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://github.com/lkhq/debspawn
 Project-URL: Source, https://github.com/lkhq/debspawn
```

### Comparing `debspawn-0.6.1/debspawn.egg-info/SOURCES.txt` & `debspawn-0.6.2/debspawn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/assemble_man.py` & `debspawn-0.6.2/docs/assemble_man.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     def __init__(self):
         self._replacements = {}
 
     def add_substvar(self, name, replacement):
         self._replacements['@{}@'.format(name)] = replacement
 
     def register_command_flag_synopsis(self, actions, command_name):
-
         flags_text = ''
         flags_entries = ''
         for item in actions:
             options_text = xml_escape('|'.join(item.option_strings))
             flags_text += '<arg>{}</arg>\n'.format(options_text)
 
             oid = item.option_strings[0]
@@ -61,15 +60,14 @@
                 options_text, desc_text
             )
 
         self.add_substvar('{}_FLAGS_SYNOPSIS'.format(command_name.upper()), flags_text)
         self.add_substvar('{}_FLAGS_ENTRIES'.format(command_name.upper()), flags_entries)
 
     def process_file(self, input_fname, output_fname):
-
         with open(input_fname, 'r') as f:
             template_content = f.read()
 
         result = reduce(
             lambda x, y: x.replace(y, self._replacements[y]), self._replacements, template_content
         )
 
@@ -88,15 +86,14 @@
     editor = DocbookEditor()
     editor.register_command_flag_synopsis(parser._get_optional_actions(), 'BASE')
 
     xml_manpages = []
     xml_manpages.append(editor.process_file('docs/debspawn.1.xml', os.path.join(build_dir, 'debspawn.1.xml')))
 
     for command, sp in parser._get_positional_actions()[0]._name_parser_map.items():
-
         editor.register_command_flag_synopsis(sp._get_optional_actions(), command)
         template_fname = 'docs/debspawn-{}.1.xml'.format(command)
         if not os.path.isfile(template_fname):
             if command in ['ls', 'b']:
                 continue  # the ls and b shorthands need to manual page
             print('Manual page template {} is missing! Skipping it.'.format(template_fname))
             continue
```

### Comparing `debspawn-0.6.1/docs/debspawn-build.1.xml` & `debspawn-0.6.2/docs/debspawn-build.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/debspawn-create.1.xml` & `debspawn-0.6.2/docs/debspawn-create.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/debspawn-delete.1.xml` & `debspawn-0.6.2/docs/debspawn-delete.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/debspawn-list.1.xml` & `debspawn-0.6.2/docs/debspawn-list.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/debspawn-login.1.xml` & `debspawn-0.6.2/docs/debspawn-login.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/debspawn-maintain.1.xml` & `debspawn-0.6.2/docs/debspawn-maintain.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/debspawn-run.1.xml` & `debspawn-0.6.2/docs/debspawn-run.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/debspawn-update.1.xml` & `debspawn-0.6.2/docs/debspawn-update.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/docs/debspawn.1.xml` & `debspawn-0.6.2/docs/debspawn.1.xml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/install-sysdata.py` & `debspawn-0.6.2/install-sysdata.py`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/pyproject.toml` & `debspawn-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `debspawn-0.6.1/setup.py` & `debspawn-0.6.2/setup.py`

 * *Files identical despite different names*

