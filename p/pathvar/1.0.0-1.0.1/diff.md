# Comparing `tmp/pathvar-1.0.0.tar.gz` & `tmp/pathvar-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathvar-1.0.0.tar", last modified: Sun May 28 10:00:42 2023, max compression
+gzip compressed data, was "pathvar-1.0.1.tar", last modified: Sun May 28 12:34:54 2023, max compression
```

## Comparing `pathvar-1.0.0.tar` & `pathvar-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,18 @@
-drwxrwxr-x   0 hussein   (1000) hussein   (1000)        0 2023-05-28 10:00:42.185550 pathvar-1.0.0/
--rw-rw-r--   0 hussein   (1000) hussein   (1000)       57 2023-05-28 09:40:55.000000 pathvar-1.0.0/.gitignore
--rw-rw-r--   0 hussein   (1000) hussein   (1000)     1079 2023-05-17 12:53:31.000000 pathvar-1.0.0/LICENSE.txt
--rw-rw-r--   0 hussein   (1000) hussein   (1000)     7592 2023-05-28 10:00:42.185550 pathvar-1.0.0/PKG-INFO
--rw-rw-r--   0 hussein   (1000) hussein   (1000)     7124 2023-05-27 19:37:37.000000 pathvar-1.0.0/README.md
--rw-rw-r--   0 hussein   (1000) hussein   (1000)      819 2023-05-27 19:37:37.000000 pathvar-1.0.0/pyproject.toml
--rw-rw-r--   0 hussein   (1000) hussein   (1000)        0 2023-05-26 19:48:24.000000 pathvar-1.0.0/requirements.txt
--rw-rw-r--   0 hussein   (1000) hussein   (1000)       38 2023-05-28 10:00:42.185550 pathvar-1.0.0/setup.cfg
-drwxrwxr-x   0 hussein   (1000) hussein   (1000)        0 2023-05-28 10:00:42.177550 pathvar-1.0.0/src/
-drwxrwxr-x   0 hussein   (1000) hussein   (1000)        0 2023-05-28 10:00:42.181550 pathvar-1.0.0/src/pathvar/
--rw-rw-r--   0 hussein   (1000) hussein   (1000)        0 2023-05-17 12:28:16.000000 pathvar-1.0.0/src/pathvar/__init__.py
-drwxrwxr-x   0 hussein   (1000) hussein   (1000)        0 2023-05-28 10:00:42.185550 pathvar-1.0.0/src/pathvar/old_pathvar/
-drwxrwxr-x   0 hussein   (1000) hussein   (1000)        0 2023-05-28 10:00:42.185550 pathvar-1.0.0/src/pathvar/old_pathvar/Sphinx-docs/
--rw-rw-r--   0 hussein   (1000) hussein   (1000)     1481 2023-05-26 18:37:51.000000 pathvar-1.0.0/src/pathvar/old_pathvar/Sphinx-docs/conf.py
--rw-rw-r--   0 hussein   (1000) hussein   (1000)     2033 2023-05-24 08:54:35.000000 pathvar-1.0.0/src/pathvar/old_pathvar/path_without_duplicates.py
--rw-rw-r--   0 hussein   (1000) hussein   (1000)    15326 2023-05-25 10:39:14.000000 pathvar-1.0.0/src/pathvar/old_pathvar/project.py
--rw-rw-r--   0 hussein   (1000) hussein   (1000)      245 2023-05-24 12:52:47.000000 pathvar-1.0.0/src/pathvar/old_pathvar/run_process.py
--rw-rw-r--   0 hussein   (1000) hussein   (1000)      731 2023-05-16 19:13:32.000000 pathvar-1.0.0/src/pathvar/old_pathvar/test_path_without_duplicates.py
--rw-rw-r--   0 hussein   (1000) hussein   (1000)    13381 2023-05-26 19:48:24.000000 pathvar-1.0.0/src/pathvar/project.py
-drwxrwxr-x   0 hussein   (1000) hussein   (1000)        0 2023-05-28 10:00:42.181550 pathvar-1.0.0/src/pathvar.egg-info/
--rw-rw-r--   0 hussein   (1000) hussein   (1000)     7592 2023-05-28 10:00:42.000000 pathvar-1.0.0/src/pathvar.egg-info/PKG-INFO
--rw-rw-r--   0 hussein   (1000) hussein   (1000)      554 2023-05-28 10:00:42.000000 pathvar-1.0.0/src/pathvar.egg-info/SOURCES.txt
--rw-rw-r--   0 hussein   (1000) hussein   (1000)        1 2023-05-28 10:00:42.000000 pathvar-1.0.0/src/pathvar.egg-info/dependency_links.txt
--rw-rw-r--   0 hussein   (1000) hussein   (1000)       49 2023-05-28 10:00:42.000000 pathvar-1.0.0/src/pathvar.egg-info/entry_points.txt
--rw-rw-r--   0 hussein   (1000) hussein   (1000)        8 2023-05-28 10:00:42.000000 pathvar-1.0.0/src/pathvar.egg-info/top_level.txt
-drwxrwxr-x   0 hussein   (1000) hussein   (1000)        0 2023-05-28 10:00:42.185550 pathvar-1.0.0/tests/
--rw-rw-r--   0 hussein   (1000) hussein   (1000)        0 2023-05-17 12:28:16.000000 pathvar-1.0.0/tests/__init__.py
--rw-rw-r--   0 hussein   (1000) hussein   (1000)     2280 2023-05-26 19:48:24.000000 pathvar-1.0.0/tests/test_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:34:54.753633 pathvar-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-28 12:34:44.000000 pathvar-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-28 12:34:54.753633 pathvar-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-28 12:34:44.000000 pathvar-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-28 12:34:44.000000 pathvar-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 12:34:54.753633 pathvar-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:34:54.753633 pathvar-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:34:54.753633 pathvar-1.0.1/src/pathvar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 12:34:44.000000 pathvar-1.0.1/src/pathvar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-05-28 12:34:44.000000 pathvar-1.0.1/src/pathvar/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:34:54.753633 pathvar-1.0.1/src/pathvar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-05-28 12:34:54.000000 pathvar-1.0.1/src/pathvar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-28 12:34:54.000000 pathvar-1.0.1/src/pathvar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:34:54.000000 pathvar-1.0.1/src/pathvar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-28 12:34:54.000000 pathvar-1.0.1/src/pathvar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 12:34:54.000000 pathvar-1.0.1/src/pathvar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:34:54.753633 pathvar-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-28 12:34:44.000000 pathvar-1.0.1/tests/test_project.py
```

### Comparing `pathvar-1.0.0/LICENSE.txt` & `pathvar-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathvar-1.0.0/PKG-INFO` & `pathvar-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathvar
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interacting with PATH variable from Linux BASH command line.
 Author-email: Hussine Mahmoud Kandil <hussein.mahmoud.s7s@gmail.com>
 Project-URL: Repository, https://github.com/hussein-m-kandil/pathvar/
 Keywords: path,command line,linux,terminal,environment variable,system,os
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pathvar-1.0.0/README.md` & `pathvar-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pathvar-1.0.0/pyproject.toml` & `pathvar-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pathvar"
-version = "1.0.0"
+version = "1.0.1"
 description = "Interacting with PATH variable from Linux BASH command line."
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 authors = [
     { name = "Hussine Mahmoud Kandil", email = "hussein.mahmoud.s7s@gmail.com" },
 ]
```

### Comparing `pathvar-1.0.0/src/pathvar/old_pathvar/project.py` & `pathvar-1.0.1/src/pathvar/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,43 +12,31 @@
 UNDERLINE_STYLE = "\033[4m"
 RED_STYLE = "\033[91m"
 GREEN_STYLE = "\033[92m"
 END_STYLE = "\033[0m"
 
 
 def main() -> None:
+    """pathvar main function
+
+    The Logic of the entire 'pathvar' program.
+
+    :return: Nothing, just execute the logic of the entire program.
+    :rtype: None
+    """
 
     # Get PATH
     old_path_value: str = get_path()
     if old_path_value == "__%NO_PATH%__":
         exit("Failure: Couldn't get PATH variable")
 
-    """ # Try to get the PATH in place holder for the current path
-    try:
-        old_path_value: str = os.environ["PATH"]
-    except KeyError:
-        print('\n' + BOLD_STYLE + RED_STYLE +
-              "PATH variable is not exist!" + END_STYLE)
-        while True:
-            ans = input("Do you want to set a new PATH variable [y|n]? ")
-            if ans.strip().lower() in ('y', "yes"):
-                os.environ.setdefault("PATH", '')
-                old_path_value: str = os.environ["PATH"]
-                print('\n' + BOLD_STYLE + GREEN_STYLE +
-                      "New PATH variable is available." + END_STYLE)
-                print('\n' + BOLD_STYLE +
-                      "Use -a or -p to insert new paths." + END_STYLE)
-                break
-            elif ans.strip().lower() in ('n', "no"):
-                exit() """
-
     # Create argument parser
     parser: ArgumentParser = ArgumentParser(
         description=f"This tool meant to facilitate the interaction \
-                with the system's PATH environment variable. \
+                with the system's PATH environment variable (Linux BASH shell only). \
                     To get the work done correctly do the following: \
                         Read the 'help' instruction well, \n\
                         Be careful about the paths you input (with some options), \n\
                         and Separate between multiple paths with a single '{PATH_SEP}'. \
                         Copyright (c) 2023 Hussein Mahmoud Kandil - MIT."
     )
     # Add arguments to the ArgumentParser object
@@ -64,27 +52,25 @@
     if new_path == FOUND_MSG:
         print('\n' + BOLD_STYLE + GREEN_STYLE + new_path + END_STYLE)
         new_path = old_path_value
     elif new_path == NOT_FOUND_MSG:
         print('\n' + BOLD_STYLE + RED_STYLE + new_path + END_STYLE)
         new_path = old_path_value
     elif new_path != old_path_value:
-        """ # Modify os.environ["PATH"] to hold the new clean value
-        os.environ["PATH"] = new_path """
+        # Update the old PATH
         new_path = path_duplicates_eliminator(new_path)
         update_path(new_path)
         is_path_modified = True
         print_msg("Old 'PATH'", old_path_value)
 
     # Print the current PATH value
-    """ print_msg("Current 'PATH'", os.environ["PATH"]) """
     print_msg("Current 'PATH'", new_path)
 
-    # Suggest source command
-    if is_path_modified:
+    # Suggest source command if the PATH IS modified and not on windows
+    if is_path_modified and PATH_SEP != ';':
         print_msg("Needed Command",
                   "Run 'source ~/.bash_profile' to apply the changes to the current session.")
 
 
 def get_path() -> str:
     """A simple function to get the current PATH
 
@@ -103,23 +89,14 @@
         process = run("echo $PATH", shell=True,
                       stdout=PIPE, stderr=PIPE, text=True)
         if process.stderr:
             print_msg(RED_STYLE + "STDERR", process.stderr)
             return path
         path = process.stdout.strip()
 
-    # WINDOWS
-    if PATH_SEP == ';':
-        process = run("echo %PATH%", shell=True,
-                      stdout=PIPE, stderr=PIPE, text=True)
-        if process.stderr:
-            print_msg(RED_STYLE + "STDERR", process.stderr)
-            return path
-        path = process.stdout.strip()
-
     return path
 
 
 def run_command_verbosely(cmd: str) -> None:
     """Run a given command in subprocess
 
     Run the given command in subprocess 
@@ -194,36 +171,14 @@
                 f.write(prog_sig_start)
                 f.write('export PATH="' + new_path_value + '"\n')
                 f.write(prog_sig_end)
 
         # Delete the temp state of the ~/.bash_profile
         run_command_verbosely("rm -f " + USER_BASH_PROFILE_PATH + "__~")
 
-        return None
-
-    # WINDOWS
-    elif PATH_SEP == ';':
-        if len(new_path_value) > 1024:
-            print('\n' + BOLD_STYLE + RED_STYLE +
-                  "WARNING: The new PATH value is more than 1024 characters, \
-                    so it will be truncated!" + END_STYLE)
-            print('\n' + BOLD_STYLE +
-                  "Hint: don't continue and \
-                    try first to delete some values using -d." + END_STYLE)
-            while True:
-                ans = input("Do you want to continue any way [y/n]? ")
-                if ans.strip().lower() in ('y', "yes"):
-                    break
-                elif ans.strip().lower() in ('n', "no"):
-                    return None
-            # Set the PATH for this session
-            run_command_verbosely("set PATH=" + new_path_value)
-            # Set the PATH globally
-            run_command_verbosely("setx PATH " + new_path_value)
-
     return None
 
 
 def add_args(parser_obj: ArgumentParser) -> None:
     """Adding CL arguments to and ArgumentParser object
 
     Manipulate the inputted ArgumentParser object 
@@ -436,14 +391,16 @@
     :type title: str
     :param msg: The body of the message
     :type msg: str
     :return: Nothing, just the print side effect
     :rtype: None
     """
     print()
+    print(BOLD_STYLE + GREEN_STYLE + "Welcome to PATHVAR" + END_STYLE)
+    print()
     print(BOLD_STYLE + title + ': ' + END_STYLE)
     print('_' * 28 + '\n')
     print(msg)
     print()
 
 
 if __name__ == "__main__":
```

### Comparing `pathvar-1.0.0/src/pathvar.egg-info/PKG-INFO` & `pathvar-1.0.1/src/pathvar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathvar
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interacting with PATH variable from Linux BASH command line.
 Author-email: Hussine Mahmoud Kandil <hussein.mahmoud.s7s@gmail.com>
 Project-URL: Repository, https://github.com/hussein-m-kandil/pathvar/
 Keywords: path,command line,linux,terminal,environment variable,system,os
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pathvar-1.0.0/tests/test_project.py` & `pathvar-1.0.1/tests/test_project.py`

 * *Files identical despite different names*

