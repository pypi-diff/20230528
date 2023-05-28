# Comparing `tmp/sway-0.1.2.tar.gz` & `tmp/sway-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sway-0.1.2.tar", max compression
+gzip compressed data, was "sway-0.1.3.tar", max compression
```

## Comparing `sway-0.1.2.tar` & `sway-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       71 2023-05-27 19:02:56.274387 sway-0.1.2/README.md
--rw-r--r--   0        0        0      440 2023-05-27 19:11:31.925235 sway-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-27 19:01:22.081625 sway-0.1.2/sway/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 19:01:22.081688 sway-0.1.2/sway/commands/__init__.py
--rw-r--r--   0        0        0      467 2023-05-27 19:01:22.082055 sway-0.1.2/sway/commands/branch.py
--rw-r--r--   0        0        0        0 2023-05-27 19:01:22.082089 sway-0.1.2/sway/commands/build.py
--rw-r--r--   0        0        0     3124 2023-05-27 19:01:22.082295 sway-0.1.2/sway/commands/config.py
--rw-r--r--   0        0        0     1878 2023-05-27 19:01:26.860545 sway-0.1.2/sway/main.py
--rw-r--r--   0        0        0        0 2023-05-27 19:01:22.082574 sway-0.1.2/sway/utils/__init__.py
--rw-r--r--   0        0        0      895 2023-05-27 19:01:22.082770 sway-0.1.2/sway/utils/yaml.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 sway-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      536 2023-05-28 18:21:43.172898 sway-0.1.3/README.md
+-rw-r--r--   0        0        0      472 2023-05-28 18:37:50.474302 sway-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 18:15:05.590094 sway-0.1.3/sway/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-28 18:15:05.590559 sway-0.1.3/sway/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:01:22.081688 sway-0.1.3/sway/commands/__init__.py
+-rw-r--r--   0        0        0     2295 2023-05-28 18:15:05.590839 sway-0.1.3/sway/commands/branch.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:01:22.082089 sway-0.1.3/sway/commands/build.py
+-rw-r--r--   0        0        0     3493 2023-05-28 18:15:05.591100 sway-0.1.3/sway/commands/config.py
+-rw-r--r--   0        0        0     1854 2023-05-28 18:15:05.591358 sway-0.1.3/sway/main.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:01:22.082574 sway-0.1.3/sway/utils/__init__.py
+-rw-r--r--   0        0        0      894 2023-05-28 18:15:05.591692 sway-0.1.3/sway/utils/yaml.py
+-rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 sway-0.1.3/PKG-INFO
```

### Comparing `sway-0.1.2/sway/commands/config.py` & `sway-0.1.3/sway/commands/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,134 @@
 from __future__ import annotations
 
 import argparse
+from typing import Any
 
 from sway.utils.yaml import get_config, set_config
 
+
 class RepoEnvConfig:
     def __init__(self, env: str, branch: str):
         self.env = env
         self.branch = branch
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.env} - {self.branch}"
 
 
 class RepoConfig:
-    def __init__(self, repo_id: str, repo: str, path: str | None = None, envs: RepoEnvConfig | None = None):
+    def __init__(
+        self,
+        repo_id: str,
+        repo: str,
+        path: str | None = None,
+        envs: list[RepoEnvConfig] | None = None,
+    ):
         self.id = repo_id
         self.repo = repo
         self.path = path
         self.envs = envs
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.id} | {self.repo} | {self.path} | {self.envs}"
 
 
 class SwayConfig:
     def __init__(self, repos: list[RepoConfig]):
         self.repos = repos
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.repos}"
 
 
 def get_config_object() -> SwayConfig:
     data = get_config()
 
     repos = []
     for repo in data["repos"]:
-
         repos.append(
             RepoConfig(
                 # make it optional, create id from repo when not given
                 repo_id=repo["id"],
                 repo=repo["repo"],
+                # default path would be parent dir
                 path=repo.get("path", "./../"),
                 envs=[
                     RepoEnvConfig(env=env["env"], branch=env["branch"])
                     for env in repo.get("envs", [])
-                ],
-            )
+                ]
+                or None,
+            ),
         )
 
     return SwayConfig(repos=repos)
 
 
 def config_init(args: argparse.Namespace) -> int:
     q = "Would you like to define your repos interactively? (yes/no) "
     a = input(q)
     if a not in ("yes", "y"):
-        print("Refer the README.md in the `sway` repository for config file instructions.")
+        print(
+            "Refer the README.md in the `sway` repository for config file instructions.",
+        )
         return 0
 
-    repos = []
+    repos: list[dict[str, Any]] = []
     while True:
         print("\nAdding Repository:")
         repo = input("repo: [Example: git@github.com:saurbhc/sway] ")
         repo_id = input("id: [Example: sway] ")
         repo_path = input("path: [Example: /home/ubuntu/dev/sway] ")
 
         q = f"\nWould you like to define --environment/-e for {repo_id}? (yes/no) "
         a = input(q)
         if a not in ("yes", "y"):
-            repos.append({
-                "id": repo_id,
-                "repo": repo,
-                "path": repo_path,
-            })
+            repos.append(
+                {
+                    "id": repo_id,
+                    "repo": repo,
+                    "path": repo_path,
+                },
+            )
             break
 
         envs = []
         while True:
             print(f"\n- Adding Environment for Repository {repo_id}:")
             env = input("- env: [Example: dev] ")
             branch = input("- branch: [Example: develop] ")
-            envs.append({
-                "env": env,
-                "branch": branch,
-            })
+            envs.append(
+                {
+                    "env": env,
+                    "branch": branch,
+                },
+            )
 
             q = f"\nWould you like to define more --environment/-e for {repo_id}? (yes/no) "
             a = input(q)
             if a not in ("yes", "y"):
                 break
 
-        repos.append({
-            "id": repo_id,
-            "repo": repo,
-            "path": repo_path,
-            "envs": envs,
-        })
+        repos.append(
+            {
+                "id": repo_id,
+                "repo": repo,
+                "path": repo_path,
+                "envs": envs,
+            },
+        )
 
         q = "Would you like to define more repos interactively? (yes/no) "
         a = input(q)
         if a not in ("yes", "y"):
             break
 
     set_config(data={"repos": repos})
 
     return 0
 
+
 def config_validate() -> int:
     config = get_config_object()
-    breakpoint()
+    # TODO: add validation, see #2
 
     return 0
-
```

### Comparing `sway-0.1.2/sway/main.py` & `sway-0.1.3/sway/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import argparse
 
 from sway.commands.branch import branch_cmd
-from sway.commands.config import get_config_object, config_init, config_validate
+from sway.commands.config import config_init, config_validate, get_config_object
 
 
 def main() -> int:
     parser = argparse.ArgumentParser(prog="sway")
 
     # subparsers
     subparsers = parser.add_subparsers(dest="command")
     config_parser = subparsers.add_parser(
         "config",
-        help=".pymonorepo-config.yaml options",
+        help=".sway-config.yaml options",
     )
     branch_parser = subparsers.add_parser(
         "branch",
         help="branch-management options",
     )
     build_parser = subparsers.add_parser(
         "build",
@@ -39,34 +39,34 @@
     branch_parser.add_argument(
         "--repo",
         "-r",
         type=str,
         nargs="*",
         action="append",
         metavar=("repo_id", "repo_branch"),
-        help="use repo-id with provided branch, use --repo/-r {repo-id} {repo-branch}",
+        help="use '--repo/-r {repo-id} {repo-branch}'",
     )
     branch_parser.add_argument(
         "--environment",
-        "-E",
-        help="Project env setup in .sway-config.yaml",
+        "-e",
+        required=True,
+        help="env setup provided in .sway-config.yaml",
     )
 
     args = parser.parse_args()
 
     if args.command == "config" and args.action == "init":
         return config_init(args=args)
 
     if args.command == "config" and args.action == "validate":
-        return config_validate(args=args)
+        return config_validate()
 
     config = get_config_object()
 
     if args.command == "branch":
         return branch_cmd(args=args, config=config)
 
     return 1
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
-
```

### Comparing `sway-0.1.2/sway/utils/yaml.py` & `sway-0.1.3/sway/utils/yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,7 @@
 def set_config(data: Any) -> None:
     with open(DEFAULT_CONFIG_FILE_PATH, "w") as f:
         f.write(yaml_dump(data))
 
 
 def touch_config() -> None:
     DEFAULT_CONFIG_FILE_PATH.touch(mode=0o600, exist_ok=True)
-
```

