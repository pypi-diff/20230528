# Comparing `tmp/onboardme-1.2.2.tar.gz` & `tmp/onboardme-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.2.2.tar", max compression
+gzip compressed data, was "onboardme-1.2.3.tar", max compression
```

## Comparing `onboardme-1.2.2.tar` & `onboardme-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.2.2/LICENSE.txt
--rw-r--r--   0        0        0    15653 2023-05-27 20:17:42.799017 onboardme-1.2.2/README.md
--rwxr-xr-x   0        0        0     6824 2023-05-27 20:17:42.807649 onboardme-1.2.2/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.2.2/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.2.2/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.2.2/onboardme/console_logging.py
--rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.2.2/onboardme/constants.py
--rw-r--r--   0        0        0     4940 2023-05-27 20:17:42.809853 onboardme-1.2.2/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5732 2023-05-27 20:17:42.810709 onboardme-1.2.2/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.2.2/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-21 15:49:30.802500 onboardme-1.2.2/onboardme/help_text.py
--rw-r--r--   0        0        0     3085 2023-05-27 20:17:37.897860 onboardme-1.2.2/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.2.2/onboardme/misc.py
--rwxr-xr-x   0        0        0     9362 2023-05-21 17:34:22.544320 onboardme-1.2.2/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.2.2/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.2.2/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.2.2/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.2.2/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1792 2023-05-27 20:17:42.812778 onboardme-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    17034 1970-01-01 00:00:00.000000 onboardme-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-27 22:09:37.401192 onboardme-1.2.3/LICENSE.txt
+-rw-r--r--   0        0        0    15653 2023-05-27 22:09:37.401192 onboardme-1.2.3/README.md
+-rwxr-xr-x   0        0        0     6824 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1793 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/constants.py
+-rw-r--r--   0        0        0     5141 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5732 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/help_text.py
+-rw-r--r--   0        0        0     3085 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/misc.py
+-rwxr-xr-x   0        0        0     9362 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2023-05-27 22:09:37.433193 onboardme-1.2.3/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1792 2023-05-27 22:09:37.433193 onboardme-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    16983 1970-01-01 00:00:00.000000 onboardme-1.2.3/PKG-INFO
```

### Comparing `onboardme-1.2.2/LICENSE.txt` & `onboardme-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/README.md` & `onboardme-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/__init__.py` & `onboardme-1.2.3/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/config/firewall/iptables.sh` & `onboardme-1.2.3/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/console_logging.py` & `onboardme-1.2.3/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/constants.py` & `onboardme-1.2.3/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/dot_files.py` & `onboardme-1.2.3/onboardme/dot_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from rich.table import Table
 # custom libs
 from .constants import HOME_DIR, PWD, XDG_CONFIG_DIR
 from .console_logging import print_panel, print_msg
 from .subproc import subproc
 
 
-XDG_CONFIG_GIT_PATH = path.join(XDG_CONFIG_DIR, 'git/config')
+XDG_GIT_CFG_DIR = path.join(XDG_CONFIG_DIR, 'git')
+Path(XDG_GIT_CFG_DIR).mkdir(exist_ok=True)
+XDG_GIT_PATH = path.join(XDG_GIT_CFG_DIR, 'config')
 
 
 def setup_dot_files(OS='Linux', overwrite=False,
                     git_url="https://github.com/jessebot/dot_files.git",
                     branch="main") -> None:
     """
     note on how we're doing things, seperate dot files repo:
@@ -25,18 +27,22 @@
     """
     git_dir = path.join(HOME_DIR, '.git_dot_files')
     # create ~/.git_dot_files if it does not exist
     Path(git_dir).mkdir(exist_ok=True)
     chdir(git_dir)
     opts = {'quiet': True, 'cwd': git_dir}
 
+    if git_url:
+        if "github.com" in git_url:
+            user_repo = "/".join(git_url.split("/")[-2:]).replace(".git", "")
+
     # global: use main as default branch, always push up new remote branch
-    git_raw = f"https://raw.githubusercontent.com/jessebot/dot_files/{branch}"
+    git_raw = f"https://raw.githubusercontent.com/{user_repo}/{branch}"
 
-    cmds = [f'curl {git_raw}/.config/git/config -o {XDG_CONFIG_GIT_PATH}',
+    cmds = [f'curl {git_raw}/.config/git/config -o {XDG_GIT_PATH}',
             f'git --git-dir={git_dir} --work-tree={HOME_DIR} init',
             'git config status.showUntrackedFiles no']
     subproc(cmds, spinner=False, **opts)
 
     # this one needs to be allowed to fail because it might already exist
     cmds = [f"git remote add origin {git_url}"]
     subproc(cmds, error_ok=True, spinner=False, **opts)
```

### Comparing `onboardme-1.2.2/onboardme/env_config.py` & `onboardme-1.2.3/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/firewall.py` & `onboardme-1.2.3/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/help_text.py` & `onboardme-1.2.3/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/ide_setup.py` & `onboardme-1.2.3/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/misc.py` & `onboardme-1.2.3/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/pkg_management.py` & `onboardme-1.2.3/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/subproc.py` & `onboardme-1.2.3/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/onboardme/sudo_setup.py` & `onboardme-1.2.3/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.2.2/pyproject.toml` & `onboardme-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.2.2"
+version       = "1.2.3"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.2.2/PKG-INFO` & `onboardme-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.2.2
+Version: 1.2.3
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Installation/Setup
 Requires-Dist: GitPython (>=3.1,<4.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: rich (>=13.3,<14.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.2.2 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.2.3 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: System ::
-Installation/Setup Requires-Dist: GitPython (>=3.1,<4.0) Requires-Dist: PyYAML
-(>=6.0,<7.0) Requires-Dist: click (>=8.1,<9.0) Requires-Dist: rich
-(>=13.3,<14.0) Requires-Dist: wget (>=3.2,<4.0) Requires-Dist: xdg-base-dirs
-(>=6.0,<7.0) Project-URL: Bug Tracker, http://github.com/jessebot/onboardme/
-issues Project-URL: Documentation, https://jessebot.github.io/onboardme/
-onboardme Project-URL: Repository, http://github.com/jessebot/onboardme
-Description-Content-Type: text/markdown
+Topic :: System :: Installation/Setup Requires-Dist: GitPython (>=3.1,<4.0)
+Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: click (>=8.1,<9.0) Requires-
+Dist: rich (>=13.3,<14.0) Requires-Dist: wget (>=3.2,<4.0) Requires-Dist: xdg-
+base-dirs (>=6.0,<7.0) Project-URL: Bug Tracker, http://github.com/jessebot/
+onboardme/issues Project-URL: Documentation, https://jessebot.github.io/
+onboardme/onboardme Project-URL: Repository, http://github.com/jessebot/
+onboardme Description-Content-Type: text/markdown
   ***** [https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/
    misc/transparent.png] ð» onboardme [https://raw.githubusercontent.com/
          catppuccin/catppuccin/main/assets/misc/transparent.png] *****
               [https://img.shields.io/github/v/release/jessebot/
 onboardme?style=plastic&labelColor=484848&color=3CA324&logo=GitHub&logoColor=white]
 GetÂ yourÂ dailyÂ driverÂ justÂ theÂ wayÂ youÂ likeÂ it,Â fromÂ dotÂ files
 management,Â toÂ packageÂ installation, to other little features you didn't
```

