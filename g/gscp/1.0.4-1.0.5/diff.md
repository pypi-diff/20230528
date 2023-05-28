# Comparing `tmp/gscp-1.0.4.tar.gz` & `tmp/gscp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscp-1.0.4.tar", max compression
+gzip compressed data, was "gscp-1.0.5.tar", max compression
```

## Comparing `gscp-1.0.4.tar` & `gscp-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/__init__.py
--rw-r--r--   0        0        0     1892 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/__main__.py
--rw-r--r--   0        0        0     1174 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/commit.py
--rw-r--r--   0        0        0       66 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/entry.py
--rw-r--r--   0        0        0      284 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/git.py
--rw-r--r--   0        0        0     1784 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/push.py
--rw-r--r--   0        0        0      147 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/stage.py
--rw-r--r--   0        0        0     1363 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/version.py
--rw-r--r--   0        0        0      909 2023-03-23 14:15:19.884989 gscp-1.0.4/gscp/wrappers.py
--rw-r--r--   0        0        0     1089 2023-03-23 14:15:19.884989 gscp-1.0.4/LICENSE
--rw-r--r--   0        0        0      992 2023-03-23 14:15:19.884989 gscp-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1691 2023-03-23 14:15:19.884989 gscp-1.0.4/README.md
--rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 gscp-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/__init__.py
+-rw-r--r--   0        0        0     2163 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/__main__.py
+-rw-r--r--   0        0        0     1369 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/commit.py
+-rw-r--r--   0        0        0       66 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/entry.py
+-rw-r--r--   0        0        0      510 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/git.py
+-rw-r--r--   0        0        0     1784 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/push.py
+-rw-r--r--   0        0        0      200 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/stage.py
+-rw-r--r--   0        0        0     1363 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/version.py
+-rw-r--r--   0        0        0     2929 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/wrappers.py
+-rw-r--r--   0        0        0     1089 2023-05-28 20:30:10.843059 gscp-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1045 2023-05-28 20:30:10.858625 gscp-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1691 2023-05-28 20:30:10.843059 gscp-1.0.5/README.md
+-rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 gscp-1.0.5/PKG-INFO
```

### Comparing `gscp-1.0.4/gscp/__main__.py` & `gscp-1.0.5/gscp/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 gscp: `Git Stage Commit Push`
 Samuel Yvon <samuelyvon9@gmail.com>
 """
 
 import argparse
 from typing import cast
 
-from .commit import commit
-from .push import push
-from .stage import stage
-from .version import ApplicationVersion
+from rich.console import Console
+
+from gscp.commit import commit
+from gscp.git import git_is_in_repo
+from gscp.push import push
+from gscp.stage import stage
+from gscp.version import ApplicationVersion
 
 
 def _create_argparser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "-cp",
         "--commit-push",
         action="store_true",
-        help="Skip the push stage part; take what is already staged.",
+        help="Skip the stage part; take what is already staged.",
     )
 
     parser.add_argument(
         "--version", action="version", version=f"gscp {ApplicationVersion.parse()}"
     )
 
     parser.add_argument(
@@ -53,25 +56,32 @@
         "-f", "--force", action="store_true", help="If we use `git push --force`"
     )
 
     return parser
 
 
 def main() -> None:
+    console = Console()
+    in_repo = git_is_in_repo()
+
+    if not in_repo:
+        console.print("You are not in a git repository", style="bold red")
+        exit(1)
+
     parser = _create_argparser()
     args = parser.parse_args()
 
-    commit_under_push_only = cast(bool, args.commit_push)
+    commit_push_only = cast(bool, args.commit_push)
     message = args.message if args.message else ""
     no_verify = cast(bool, args.no_verify)
     amend = cast(bool, args.amend)
     force = cast(bool, args.force)
 
-    if not commit_under_push_only:
-        stage()
+    if not commit_push_only:
+        stage(console)
 
-    if commit(message, amend=amend, no_verify=no_verify):
+    if commit(message, amend=amend, no_verify=no_verify, console=console):
         push(force=force or amend)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gscp-1.0.4/gscp/commit.py` & `gscp-1.0.5/gscp/commit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from rich.console import Console
 from rich.prompt import Confirm
 
 from .wrappers import cmd_run_in_pty
 
 _COMMIT_BASE_COMMAND = ["git", "commit", "-v"]
 
 
 def _commit_with_message(
-    message: str, amend: bool = False, no_verify: bool = False
+    message: str, *, console: Console, amend: bool = False, no_verify: bool = False
 ) -> bool:
     cmd = [*_COMMIT_BASE_COMMAND, "-m", message]
 
     if amend:
         ok = Confirm.ask(
             "You are about to commit using git amend with a new message. "
             "Is this what you want?",
@@ -23,24 +24,32 @@
 
     if no_verify:
         cmd.append("-n")
 
     return 0 == cmd_run_in_pty(*cmd)[0]
 
 
-def _commit_without_message(amend: bool = False, no_verify: bool = False) -> bool:
+def _commit_without_message(
+    *, console: Console, amend: bool = False, no_verify: bool = False
+) -> bool:
     cmd = [*_COMMIT_BASE_COMMAND]
 
     if amend:
         cmd.append("--amend")
 
     if no_verify:
         cmd.append("-n")
 
     return 0 == cmd_run_in_pty(*cmd)[0]
 
 
-def commit(message: str, amend: bool = False, no_verify: bool = False) -> bool:
+def commit(
+    message: str, *, console: Console, amend: bool = False, no_verify: bool = False
+) -> bool:
     if message:
-        return _commit_with_message(message, amend=amend, no_verify=no_verify)
+        return _commit_with_message(
+            message, console=console, amend=amend, no_verify=no_verify
+        )
     else:
-        return _commit_without_message(amend=amend, no_verify=no_verify)
+        return _commit_without_message(
+            console=console, amend=amend, no_verify=no_verify
+        )
```

### Comparing `gscp-1.0.4/gscp/push.py` & `gscp-1.0.5/gscp/push.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.4/gscp/version.py` & `gscp-1.0.5/gscp/version.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.4/LICENSE` & `gscp-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gscp-1.0.4/pyproject.toml` & `gscp-1.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 [tool.poetry]
 name = "gscp"
-version = "1.0.4"
+version = "1.0.5"
 description = "A tool to quickly commit your work with git."
 authors = ["Samuel Yvon <samuelyvon9@gmail.com>"]
 readme = "README.md"
-packages = [{include = "gscp"}]
+packages = [{ include = "gscp" }]
 
 [tool.poetry.dependencies]
 rich = "^13.3.2"
 python = "^3.8"
+ptyprocess = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
-black="^23.1.0"
-mypy="^1.0.0"
-isort="^5.10.1"
-ruff="^0.0.254"
-pre-commit="^3.1.1"
-types-setuptools="^67.6.0.5"
+black = "^23.1.0"
+mypy = "^1.0.0"
+isort = "^5.10.1"
+ruff = "^0.0.254"
+pre-commit = "^3.1.1"
+types-setuptools = "^67.6.0.5"
 
 [tool.poetry.scripts]
 gscp = "gscp.entry:entry"
 
 [tool.black]
 target-version = ["py311", "py310", "py39", "py38", "py37"]
 
 [tool.mypy]
 python_version = "3.10"
 exclude = ['venv/.*/*\.py$']
-strict=true
+strict = true
 
 [tool.ruff]
 src = ["gscp"]
 target-version = "py37"
 select = [
-  "B", # flake8-bugbear
-  "C4", # flake8-comprehensions
-  "E", # pycodestyle
-  "F", # pyflakes
-  "W", # pycodestyle
-  "RUF", # ruff
-  "I", # isort
-  "PT",   # flake8-pytest-style
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
+    "E", # pycodestyle
+    "F", # pyflakes
+    "W", # pycodestyle
+    "RUF", # ruff
+    "I", # isort
+    "PT", # flake8-pytest-style
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gscp-1.0.4/README.md` & `gscp-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gscp-1.0.4/PKG-INFO` & `gscp-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: gscp
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool to quickly commit your work with git.
 Author: Samuel Yvon
 Author-email: samuelyvon9@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ptyprocess (>=0.7.0,<0.8.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Description-Content-Type: text/markdown
 
 # gscp: *G*it, *S*tage all, *C*ommit, *P*ush
 
 I often find myself writing a bunch of code and wanting to commit it all, in one singular command. It's not
 very hard:
```

