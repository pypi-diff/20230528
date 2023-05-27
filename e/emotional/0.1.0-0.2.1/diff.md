# Comparing `tmp/emotional-0.1.0.tar.gz` & `tmp/emotional-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotional-0.1.0.tar", last modified: Fri May 26 14:11:41 2023, max compression
+gzip compressed data, was "emotional-0.2.1.tar", last modified: Sat May 27 23:26:59 2023, max compression
```

## Comparing `emotional-0.1.0.tar` & `emotional-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     1064 2022-09-16 23:07:01.534539 emotional-0.1.0/LICENSE
--rw-r--r--   0        0        0     2826 2023-05-26 13:49:15.611433 emotional-0.1.0/README.md
--rw-r--r--   0        0        0      155 2022-10-15 11:23:09.077180 emotional-0.1.0/emotional/__init__.py
--rw-r--r--   0        0        0      240 2022-10-15 13:01:48.853918 emotional-0.1.0/emotional/_compat.py
--rw-r--r--   0        0        0       26 2022-09-16 23:25:13.176855 emotional-0.1.0/emotional/_version.py
--rw-r--r--   0        0        0     1016 2023-05-26 13:49:13.754792 emotional-0.1.0/emotional/changelog.md.jinja
--rw-r--r--   0        0        0      534 2022-12-14 23:26:05.855303 emotional-0.1.0/emotional/changelog.py
--rw-r--r--   0        0        0     4671 2023-05-26 13:57:34.107122 emotional-0.1.0/emotional/config.py
--rw-r--r--   0        0        0     7646 2022-10-15 12:56:13.873635 emotional-0.1.0/emotional/cz.py
--rw-r--r--   0        0        0     2846 2023-02-22 13:46:47.261154 emotional-0.1.0/emotional/defaults.py
--rw-r--r--   0        0        0      679 2022-09-30 23:32:44.967373 emotional-0.1.0/emotional/example.jinja
--rw-r--r--   0        0        0     1476 2022-10-15 12:56:13.266978 emotional-0.1.0/emotional/github.py
--rw-r--r--   0        0        0     1644 2022-10-15 12:56:13.253645 emotional-0.1.0/emotional/gitlab.py
--rw-r--r--   0        0        0     1285 2022-09-29 23:33:47.497768 emotional-0.1.0/emotional/info.md.jinja
--rw-r--r--   0        0        0     1154 2022-10-15 12:56:13.246978 emotional-0.1.0/emotional/jira.py
--rw-r--r--   0        0        0      483 2022-10-15 11:21:35.985698 emotional-0.1.0/emotional/utils.py
--rw-r--r--   0        0        0     3076 2023-05-26 14:06:58.198980 emotional-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-19 23:34:18.625328 emotional-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1760 2023-05-26 13:49:14.058121 emotional-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     2357 2023-05-26 13:49:13.754792 emotional-0.1.0/tests/fixtures/changelogs/default.md
--rw-r--r--   0        0        0     2365 2023-05-26 13:49:13.754792 emotional-0.1.0/tests/fixtures/changelogs/group-by-scope.md
--rw-r--r--   0        0        0    19723 2023-05-26 13:49:14.058121 emotional-0.1.0/tests/test_changelog.py
--rw-r--r--   0        0        0     5243 2023-05-26 13:49:14.058121 emotional-0.1.0/tests/test_commit.py
--rw-r--r--   0        0        0     1381 2022-12-18 16:24:15.888821 emotional-0.1.0/tests/test_config.py
--rw-r--r--   0        0        0      648 2022-10-15 12:56:46.836497 emotional-0.1.0/tests/test_cz.py
--rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.885488 emotional-0.1.0/tests/test_github.py
--rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.888821 emotional-0.1.0/tests/test_gitlab.py
--rw-r--r--   0        0        0     2588 2022-12-18 16:24:15.888821 emotional-0.1.0/tests/test_jira.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 emotional-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-09-16 23:07:01.534539 emotional-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2826 2023-05-26 13:49:15.611433 emotional-0.2.1/README.md
+-rw-r--r--   0        0        0       98 2023-05-27 03:08:22.776955 emotional-0.2.1/emotional/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-27 02:52:07.423635 emotional-0.2.1/emotional/_compat.py
+-rw-r--r--   0        0        0       26 2022-09-16 23:25:13.176855 emotional-0.2.1/emotional/_version.py
+-rw-r--r--   0        0        0      534 2022-12-14 23:26:05.855303 emotional-0.2.1/emotional/changelog.py
+-rw-r--r--   0        0        0     4867 2023-05-27 22:42:43.823053 emotional-0.2.1/emotional/config.py
+-rw-r--r--   0        0        0     2864 2023-05-27 22:47:44.207044 emotional-0.2.1/emotional/defaults.py
+-rw-r--r--   0        0        0     1476 2022-10-15 12:56:13.266978 emotional-0.2.1/emotional/github.py
+-rw-r--r--   0        0        0     1644 2022-10-15 12:56:13.253645 emotional-0.2.1/emotional/gitlab.py
+-rw-r--r--   0        0        0     1154 2022-10-15 12:56:13.246978 emotional-0.2.1/emotional/jira.py
+-rw-r--r--   0        0        0     8199 2023-05-27 23:13:14.873415 emotional-0.2.1/emotional/plugin.py
+-rw-r--r--   0        0        0     1038 2023-05-27 02:17:11.627205 emotional-0.2.1/emotional/templates/changelog.md.jinja
+-rw-r--r--   0        0        0      679 2022-09-30 23:32:44.967373 emotional-0.2.1/emotional/templates/example.jinja
+-rw-r--r--   0        0        0     1285 2022-09-29 23:33:47.497768 emotional-0.2.1/emotional/templates/info.md.jinja
+-rw-r--r--   0        0        0      492 2023-05-27 03:38:07.830591 emotional-0.2.1/emotional/utils.py
+-rw-r--r--   0        0        0     3155 2023-05-27 23:26:59.415051 emotional-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-19 23:34:18.625328 emotional-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1760 2023-05-26 13:49:14.058121 emotional-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     2326 2023-05-26 23:19:31.330807 emotional-0.2.1/tests/fixtures/changelogs/default.md
+-rw-r--r--   0        0        0     2322 2023-05-27 02:17:11.627205 emotional-0.2.1/tests/fixtures/changelogs/group_by_scope.md
+-rw-r--r--   0        0        0     2326 2023-05-27 02:17:11.627205 emotional-0.2.1/tests/fixtures/changelogs/release_emoji.md
+-rw-r--r--   0        0        0     2585 2023-05-27 23:13:14.806748 emotional-0.2.1/tests/test_bump.py
+-rw-r--r--   0        0        0    20365 2023-05-27 03:02:52.106089 emotional-0.2.1/tests/test_changelog.py
+-rw-r--r--   0        0        0     5595 2023-05-27 03:43:41.674835 emotional-0.2.1/tests/test_commit.py
+-rw-r--r--   0        0        0     1381 2022-12-18 16:24:15.888821 emotional-0.2.1/tests/test_config.py
+-rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.885488 emotional-0.2.1/tests/test_github.py
+-rw-r--r--   0        0        0     2655 2022-12-18 16:24:15.888821 emotional-0.2.1/tests/test_gitlab.py
+-rw-r--r--   0        0        0     2588 2022-12-18 16:24:15.888821 emotional-0.2.1/tests/test_jira.py
+-rw-r--r--   0        0        0      644 2023-05-27 03:02:52.109422 emotional-0.2.1/tests/test_plugin.py
+-rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 emotional-0.2.1/PKG-INFO
```

### Comparing `emotional-0.1.0/LICENSE` & `emotional-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/README.md` & `emotional-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/emotional/changelog.md.jinja` & `emotional-0.2.1/emotional/templates/changelog.md.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% for entry in tree %}
-## {% if entry.date %}🚀 {% endif %}{{ entry.version }}{% if entry.date %} ({{ entry.date }}){% endif %}
+## {% if entry.date %}{{ config.release_emoji }} {% endif %}{{ entry.version }}{% if entry.date %} ({{ entry.date }}){% endif %}
 
 {% for type, changes in entry.changes.items() %}
 
 {% if type -%}
 ### {{ type.emoji }} {{ type.heading }}
 {% endif -%}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `emotional-0.1.0/emotional/changelog.py` & `emotional-0.2.1/emotional/changelog.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/emotional/config.py` & `emotional-0.2.1/emotional/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,47 +4,54 @@
 import sys
 from dataclasses import dataclass, field, fields
 from functools import total_ordering
 
 from commitizen.config import read_cfg
 from commitizen.defaults import Settings
 
-from ._compat import Literal, cached_property  # type: ignore
-from .defaults import TYPES
+from . import defaults
+from ._compat import Literal, TypeAlias, cached_property  # type: ignore [attr-defined]
 
 RE_HTTP = re.compile(r"(?P<server>https?://.+)/(?P<repository>[^/]+/[^/]+/?)")
 
 
+Increment: TypeAlias = Literal["MAJOR", "MINOR", "PATCH"]  # noqa: F481
+
+
 @dataclass
 @total_ordering
 class CommitType:
     type: str
     """Key used as type in the commit header"""
 
     description: str
     """A human readable description of the type"""
 
     heading: str | None
     """The resulting heading in the changelog for this type"""
 
     emoji: str | None
-    """An optional emoji repsenting the type"""
+    """An optional emoji representing the type"""
 
     aliases: list[str] = field(default_factory=list)
     """Some known alternative keys (for legacy, typos...)"""
 
     changelog: bool = True
     """Wether this type should appear in the changelog or not"""
 
     question: bool = True
     """Wether this type should appear in the question choices"""
 
-    bump: Literal[MAJOR, MINOR, PATCH] = "PATCH"  # noqa: F821
+    bump: Increment | None = None
 
     key: str | None = None
+    """An optional shortcut key choices questions"""
+
+    regex: str | None = None
+    """An optional regular expression matching this type"""
 
     def __str__(self) -> str:
         return self.type
 
     def __hash__(self):
         return hash(self.type)
 
@@ -85,30 +92,26 @@
     github: str | None
 
     gitlab: str | None
 
     jira_url: str | None
     jira_prefixes: list[str] | None
 
-    group_by_scope: bool
+    group_by_scope: bool | None
 
-    release_type: str
-    """
-    If set to an existing type, this type will be ignored except for the release commit
-    and it body will serve as introduction (using markdown)
-    """
+    release_emoji: str | None
 
 
 @dataclass
 class EmotionalConfig:
     settings: EmotionalSettings = field(default_factory=lambda: read_cfg().settings)
 
     @property
     def types(self) -> list[CommitType]:
-        return CommitType.from_list(self.settings.get("types", TYPES))
+        return CommitType.from_list(self.settings.get("types", defaults.TYPES))
 
     @property
     def extra_types(self) -> list[CommitType]:
         return CommitType.from_list(self.settings.get("extra_types", []))
 
     @cached_property
     def known_types(self) -> list[CommitType]:
@@ -159,7 +162,11 @@
     @property
     def incremental(self) -> bool:
         return "--incremental" in sys.argv
 
     @property
     def group_by_scope(self) -> bool:
         return self.settings.get("group_by_scope", False)
+
+    @property
+    def release_emoji(self) -> str:
+        return self.settings.get("release_emoji", defaults.RELEASE_EMOJI)
```

### Comparing `emotional-0.1.0/emotional/cz.py` & `emotional-0.2.1/emotional/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import itertools
+from collections import OrderedDict
 from typing import Any
 
 from commitizen.cz.base import BaseCommitizen, BaseConfig
 from commitizen.cz.utils import multiple_line_breaker, required_validator
 from commitizen.git import GitCommit
 
 from . import github, gitlab, jira
-from .config import CommitType, EmotionalConfig
+from .config import CommitType, EmotionalConfig, Increment
 from .utils import render_template
 
 INTEGRATIONS = github, gitlab, jira
 
 RE_EMOJI = (
     "["
     "\U0001F1E0-\U0001F1FF"  # flags (iOS)
@@ -44,32 +45,69 @@
 def parse_subject(text):
     if isinstance(text, str):
         text = text.strip(".").strip()
 
     return required_validator(text, msg="Subject is required.")
 
 
-class CzEmotional(BaseCommitizen):
+class Emotional(BaseCommitizen):
     def __init__(self, config: BaseConfig):
         super().__init__(config)
         self.emotional_config = EmotionalConfig(config.settings)
 
+    @property
+    def known_types(self) -> dict[str, CommitType]:
+        return dict(
+            itertools.chain(
+                ((t.type, t) for t in self.emotional_config.known_types),
+                (
+                    (alias, t)
+                    for t in self.emotional_config.known_types
+                    for alias in t.aliases
+                    if t.aliases
+                ),
+            )
+        )
+
+    @property
+    def re_known_types(self) -> str:
+        return "|".join(t.regex or k for k, t in self.known_types.items())
+
+    @property
+    def bump_pattern(self) -> str:
+        """Regex to extract information from commit (subject and body)"""
+        re_types = "|".join(t.regex or k for k, t in self.known_types.items() if t.bump)
+        return rf"^((({re_types})(\(.+\))?(!)?)|\w+!):"
+
+    @property
+    def bump_map(self) -> dict[str, Increment]:
+        """
+        Mapping the extracted information to a SemVer increment type (MAJOR, MINOR, PATCH)
+        """
+        return OrderedDict(
+            (
+                (r"^.+!$", "MAJOR"),
+                *((rf"^{t.regex or k}", t.bump) for k, t in self.known_types.items() if t.bump),
+            )
+        )
+
     def questions(self) -> list:
         questions: list[dict[str, Any]] = [
             {
                 "type": "list",
                 "name": "prefix",
                 "message": "Select the type of change you are committing",
                 "choices": [
                     {
                         "value": t.type,
                         "name": f"{t.emoji} {t.type}: {t.description}",
                         "key": t.shortcut,
                     }
                     for t in self.emotional_config.known_types
+                    if t.question
                 ],
             },
             {
                 "type": "input",
                 "name": "scope",
                 "message": (
                     "Scope. Define Could be anything specifying place of the "
@@ -149,15 +187,14 @@
 
         message = f"{prefix}{scope}: {subject}{extra}{body}{footer}"
 
         return message
 
     def changelog_message_builder_hook(self, parsed_message: dict, commit: GitCommit) -> dict:
         """add github and jira links to the readme"""
-
         for integration in INTEGRATIONS:
             if hasattr(integration, "changelog_message_hook"):
                 parsed_message = integration.changelog_message_hook(
                     self.emotional_config, parsed_message, commit
                 )
         return parsed_message
 
@@ -165,53 +202,32 @@
     def change_type_order(self) -> list[str]:
         return [
             type for type in self.emotional_config.known_types if type.changelog and type.heading
         ]
 
     @property
     def changelog_pattern(self) -> str:
-        types = "|".join(
-            itertools.chain(
-                (t.type for t in self.emotional_config.known_types if t.changelog),
-                (
-                    alias
-                    for t in self.emotional_config.known_types
-                    for alias in t.aliases
-                    if t.changelog and t.aliases
-                ),
-            )
-        )
-        return rf"^({types})?(!)?"
+        re_known_types = "|".join(k for k, t in self.known_types.items() if t.changelog)
+        return rf"\A({re_known_types})(\(.+\))?(!)?"
 
     @property
     def commit_parser(self) -> str:
-        types = "|".join(
-            itertools.chain(
-                (t.type for t in self.emotional_config.known_types if t.changelog),
-                (
-                    alias
-                    for t in self.emotional_config.known_types
-                    for alias in t.aliases
-                    if t.changelog and t.aliases
-                ),
-            )
-        )
         return (
-            rf"^(?:(?P<emoji>{RE_EMOJI})\s*)?"
-            rf"(?P<change_type>{types})"
+            rf"\A(?:(?P<emoji>{RE_EMOJI})\s*)?"
+            rf"(?P<change_type>{self.re_known_types})"
             r"(?:\((?P<scope>[^()\r\n]*)\)|\()?"
             r"(?P<breaking>!)?:\s"
             r"(?P<message>.*)?"
             r"(?:\n{2,}(?P<body>.*))?"
             r"(?:\n{2,}(?P<footer>.*))?"
         )
 
     @property
     def change_type_map(self) -> dict[str, CommitType]:
-        return {t.type: t for t in self.emotional_config.known_types}
+        return self.known_types
 
     def info(self) -> str:
         return render_template("info.md.jinja", config=self.emotional_config)
 
     def example(self) -> str:
         return render_template("example.jinja", config=self.emotional_config)
 
@@ -224,13 +240,13 @@
             "(BREAKING CHANGE: <breaking changes>)*\n"
             "(<footers>)*"
         )
 
     def schema_pattern(self) -> str:
         PATTERN = (
             r"(?s)"  # To explictly make . match new line
-            r"(build|ci|docs|feat|fix|perf|refactor|style|test|chore|revert|bump)"  # type
+            rf"({self.re_known_types})"  # type
             r"(\(\S+\))?!?:"  # scope
             r"( [^\n\r]+)"  # subject
             r"((\n\n.*)|(\s*))?$"
         )
         return PATTERN
```

### Comparing `emotional-0.1.0/emotional/defaults.py` & `emotional-0.2.1/emotional/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from __future__ import annotations
 
-BREAKING_CHANGES_HEADING = "Breaking changes"
-BREAKING_CHANGES_EMOJI = "🚨"
-
+RELEASE_EMOJI = "🚀"
 
 TYPES: list[dict] = [
     dict(
+        type="BREAKING CHANGE",
+        description="Changes that are not backward-compatibles",
+        heading="Breaking changes",
+        emoji="🚨",
+        bump="MAJOR",
+        regex=r"BREAKING[\-\ ]CHANGE",
+        question=False,  # Breaking changes have a dedicated question
+    ),
+    dict(
         type="feat",
         description="A new feature",
         heading="New features",
         emoji="💫",
         bump="MINOR",
+        key="n",
     ),
-    # dict(
-    #     type="security",
-    #     description="A changeset fixing a security issue",
-    #     heading="Security",
-    #     emoji="🔒",
-    #     aliases=["sec"],
-    # ),
     dict(
         type="fix",
         description="A bug fix",
         heading="Bug fixes",
         emoji="🐛",
+        bump="PATCH",
     ),
     dict(
         type="perf",
         description="A changeset improving performance",
         heading="Performance",
         emoji="📈",
         aliases=["performance"],
+        bump="PATCH",
     ),
     dict(
         type="docs",
         description="Documentation only change",
         heading="Documentation",
         emoji="📖",
         aliases=["doc"],
@@ -70,42 +73,38 @@
     ),
     dict(
         type="refactor",
         description="A changeset neither fixing a bug nor adding a feature",
         heading="Refactorings",
         emoji="🔧",
         changelog=False,
+        bump="PATCH",
     ),
     dict(
         type="i18n",
         description="A changeset related to languages and translations",
         heading="Internationalization",
         emoji="🌍",
         aliases=["locales", "l10n"],
-    ),
-    dict(
-        type="release",
-        description="A new release",
-        heading="Release",
-        emoji="🚀",
-        aliases=["bump"],
-        changelog=False,
+        bump="PATCH",
     ),
     dict(
         type="chore",
         description="Changes not fitting in other categories",
         heading="Chores",
         emoji="🧹",
+        key="o",
     ),
     dict(
         type="revert",
         description="Revert one or more commits",
         heading="Reverted",
         emoji="🔙",
         changelog=False,
+        key="e",
     ),
     dict(
         type="wip",
         description="Work in progress",
         heading="Work in progress",
         emoji="🚧",
         changelog=False,
```

### Comparing `emotional-0.1.0/emotional/example.jinja` & `emotional-0.2.1/emotional/templates/example.jinja`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/emotional/github.py` & `emotional-0.2.1/emotional/github.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/emotional/gitlab.py` & `emotional-0.2.1/emotional/gitlab.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/emotional/info.md.jinja` & `emotional-0.2.1/emotional/templates/info.md.jinja`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/emotional/jira.py` & `emotional-0.2.1/emotional/jira.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/pyproject.toml` & `emotional-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [project]
 name = "emotional"
-version = "0.1.0"
-description = ""
+description = "A Commitizen plugin for conventional commit with emojis and integrations"
 authors = [
     { name = "Axel H.", email = "noirbizarre@gmail.com" },
 ]
 dependencies = [
     "commitizen>=3.0",
-    "typing-extensions>=4.4.0; python_version<'3.9'",
+    "typing-extensions>=4.4.0; python_version<'3.10'",
 ]
+dynamic = []
 requires-python = ">=3.7"
 readme = "README.md"
+version = "0.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."commitizen.plugin"]
-emotional = "emotional.cz:CzEmotional"
+emotional = "emotional.plugin:Emotional"
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.pdm.version]
 source = "scm"
 write_to = "emotional/_version.py"
 write_template = "__version__ = \"{}\""
 
 [tool.pdm.dev-dependencies]
```

### Comparing `emotional-0.1.0/tests/conftest.py` & `emotional-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/tests/fixtures/changelogs/default.md` & `emotional-0.2.1/tests/fixtures/changelogs/default.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,26 @@
 
 - removed all from commit
 - fix config file not working
 
 ### 📖 Documentation
 
 - **README**: some new information about bump
+- **README**: ensure type aliases works
 - added new changelog
 
 ## 🚀 v1.0.0 (2019-03-01)
 
 ### 📖 Documentation
 
 - **README**: new badges
 - updated test command
 
 ## 🚀 1.0.0b2 (2019-01-18)
 
-### 💫 New features
-
-- py3 only, tests and conventional commits 1.0
-
 ### 📖 Documentation
 
 - **README**: updated to reflect current state
 
 ## 🚀 v1.0.0b1 (2019-01-17)
 
 ### 💫 New features
```

### Comparing `emotional-0.1.0/tests/fixtures/changelogs/group-by-scope.md` & `emotional-0.2.1/tests/fixtures/changelogs/group_by_scope.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,31 +50,28 @@
 ### 📖 Documentation
 
 - added new changelog
 
 #### README
 
 - some new information about bump
+- ensure type aliases works
 
 ## 🚀 v1.0.0 (2019-03-01)
 
 ### 📖 Documentation
 
 - updated test command
 
 #### README
 
 - new badges
 
 ## 🚀 1.0.0b2 (2019-01-18)
 
-### 💫 New features
-
-- py3 only, tests and conventional commits 1.0
-
 ### 📖 Documentation
 
 #### README
 
 - updated to reflect current state
 
 ## 🚀 v1.0.0b1 (2019-01-17)
```

### Comparing `emotional-0.1.0/tests/test_changelog.py` & `emotional-0.2.1/tests/test_changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Callable
 
 import pytest
 from commitizen import changelog, git
 
 from emotional.changelog import render_changelog
-from emotional.cz import CzEmotional
+from emotional.plugin import Emotional
 
 FIXTURES = Path(__file__).parent / "fixtures/changelogs"
 
 COMMITS_DATA = [
     {
         "rev": "141ee441c9c9da0809c554103a558eb17c30ed17",
         "title": "bump: version 1.1.1 → 1.2.0",
@@ -128,14 +128,21 @@
         "rev": "0c7fb0ca0168864dfc55d83c210da57771a18319",
         "title": "docs(README): some new information about bump",
         "body": "",
         "author": "Commitizen",
         "author_email": "author@cz.dev",
     },
     {
+        "rev": "0c7fb0ca0168864dfc55d83c210da57771a18377",
+        "title": "doc(README): ensure type aliases works",
+        "body": "",
+        "author": "Commitizen",
+        "author_email": "author@cz.dev",
+    },
+    {
         "rev": "cb1dd2019d522644da5bdc2594dd6dee17122d7f",
         "title": "feat: new working bump command",
         "body": "",
         "author": "Commitizen",
         "author_email": "author@cz.dev",
     },
     {
@@ -163,14 +170,21 @@
         "rev": "d630d07d912e420f0880551f3ac94e933f9d3beb",
         "title": "fix: removed all from commit",
         "body": "",
         "author": "Commitizen",
         "author_email": "author@cz.dev",
     },
     {
+        "rev": "1792b8980c58787906dbe6836f93f31971b1ec77",
+        "title": "Merge pull request #85 from whatever",
+        "body": "feat(config): new set key, used to set version to cfg",
+        "author": "Commitizen",
+        "author_email": "author@cz.dev",
+    },
+    {
         "rev": "1792b8980c58787906dbe6836f93f31971b1ec2d",
         "title": "feat(config): new set key, used to set version to cfg",
         "body": "",
         "author": "Commitizen",
         "author_email": "author@cz.dev",
     },
     {
@@ -507,15 +521,15 @@
 
     return reader
 
 
 @pytest.fixture
 def assert_changelog(config, gitcommits, tags, read_changelog):
     def assertion(name: str):
-        cz = CzEmotional(config)
+        cz = Emotional(config)
 
         tree = changelog.generate_tree_from_commits(
             gitcommits,
             tags,
             cz.commit_parser,
             cz.changelog_pattern,
             change_type_map=cz.change_type_map,
@@ -532,15 +546,20 @@
 
 def test_render_changelog_with_default_settings(assert_changelog):
     assert_changelog("default")
 
 
 @pytest.mark.settings(group_by_scope=True)
 def test_render_changelog_group_by_scope(assert_changelog):
-    assert_changelog("group-by-scope")
+    assert_changelog("group_by_scope")
+
+
+@pytest.mark.settings(release_emoji="🎉")
+def test_render_changelog_release_emoji(assert_changelog):
+    assert_changelog("release_emoji")
 
 
 # def test_render_changelog_unreleased(config, gitcommits):
 #     shiny = CzShiny(config)
 #     some_commits = gitcommits[:7]
 #     tree = changelog.generate_tree_from_commits(
 #         some_commits, [], shiny.commit_parser, shiny.changelog_pattern
```

### Comparing `emotional-0.1.0/tests/test_commit.py` & `emotional-0.2.1/tests/test_commit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from commitizen.cz.exceptions import AnswerRequiredError
 
-from emotional.cz import CzEmotional, parse_scope, parse_subject
+from emotional.plugin import Emotional, parse_scope, parse_subject
 
 valid_scopes = ["", "simple", "dash-separated", "camelCase" "UPPERCASE"]
 
 scopes_transformations = [["with spaces", "with-spaces"], [None, ""]]
 
 valid_subjects = ["this is a normal text", "aword"]
 
@@ -39,59 +39,69 @@
 def test_subject_transformations():
     for subject_transformation in subjects_transformations:
         invalid_subject, transformed_subject = subject_transformation
         assert transformed_subject == parse_subject(invalid_subject)
 
 
 def test_questions(config):
-    emotional = CzEmotional(config)
+    emotional = Emotional(config)
     questions = emotional.questions()
     assert isinstance(questions, list)
     assert isinstance(questions[0], dict)
 
 
 def test_choices_all_have_keyboard_shortcuts(config):
-    emotional = CzEmotional(config)
+    emotional = Emotional(config)
     questions = emotional.questions()
 
     list_questions = (q for q in questions if q["type"] == "list")
     for select in list_questions:
         assert all("key" in choice for choice in select["choices"])
 
 
+def test_choices_dont_have_duplicate_keyboard_shortcuts(config):
+    emotional = Emotional(config)
+    questions = emotional.questions()
+
+    list_questions = (q for q in questions if q["type"] == "list")
+    for select in list_questions:
+        shortcuts = [choice.get("key") for choice in select["choices"]]
+        assert len(set(shortcuts)) == len(shortcuts)
+
+
 def test_small_answer(config):
-    emotional = CzEmotional(config)
+    emotional = Emotional(config)
     answers = {
         "prefix": "fix",
         "scope": "users",
         "subject": "email pattern corrected",
         "is_breaking_change": False,
         "body": "",
         "footer": "",
     }
     message = emotional.message(answers)
     assert message == "fix(users): email pattern corrected"
 
 
 def test_no_scope(config):
-    emotional = CzEmotional(config)
+    emotional = Emotional(config)
     answers = {
         "prefix": "fix",
         "scope": "",
         "subject": "email pattern corrected",
         "is_breaking_change": False,
         "body": "",
         "footer": "",
     }
     message = emotional.message(answers)
     assert message == "fix: email pattern corrected"
 
 
 def test_long_answer(config):
-    emotional = CzEmotional(config)
+    emotional = Emotional(config)
     answers = {
         "prefix": "fix",
         "scope": "users",
         "subject": "email pattern corrected",
         "is_breaking_change": False,
         "body": "complete content",
         "footer": "closes #24",
@@ -99,15 +109,15 @@
     message = emotional.message(answers)
     assert message == (
         "fix(users): email pattern corrected\n" "\n" "complete content\n" "\n" "closes #24"  # noqa
     )
 
 
 def test_breaking_change_in_footer(config):
-    emotional = CzEmotional(config)
+    emotional = Emotional(config)
     answers = {
         "prefix": "fix",
         "scope": "users",
         "subject": "email pattern corrected",
         "body": "complete content",
         "is_breaking_change": True,
         "breaking_change": "breaking change content",
@@ -121,15 +131,15 @@
         "\n"
         "BREAKING CHANGE: breaking change content\n"
         "Fixes #42"
     )
 
 
 def test_exclamation_mark_breaking_change(config):
-    emotional = CzEmotional(config)
+    emotional = Emotional(config)
     answers = {
         "prefix": "fix",
         "scope": "users",
         "subject": "email pattern corrected",
         "body": "complete content",
         "is_breaking_change": True,
         "breaking_change": "",
@@ -138,15 +148,15 @@
     message = emotional.message(answers)
     assert message == (
         "fix(users)!: email pattern corrected\n" "\n" "complete content\n" "\n" "Fixes #42"
     )
 
 
 def test_exclamation_mark_breaking_change_without_scope(config):
-    emotional = CzEmotional(config)
+    emotional = Emotional(config)
     answers = {
         "prefix": "fix",
         "scope": "",
         "subject": "email pattern corrected",
         "body": "complete content",
         "is_breaking_change": True,
         "breaking_change": "",
```

### Comparing `emotional-0.1.0/tests/test_config.py` & `emotional-0.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/tests/test_cz.py` & `emotional-0.2.1/tests/test_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from emotional.cz import CzEmotional
+from emotional.plugin import Emotional
 
 
 def test_example(config):
     """just testing a string is returned. not the content"""
-    emotional_config = CzEmotional(config)
+    emotional_config = Emotional(config)
     example = emotional_config.example()
     assert isinstance(example, str)
 
 
 def test_schema(config):
     """just testing a string is returned. not the content"""
-    emotional_config = CzEmotional(config)
+    emotional_config = Emotional(config)
     schema = emotional_config.schema()
     assert isinstance(schema, str)
 
 
 def test_info(config):
     """just testing a string is returned. not the content"""
-    emotional_config = CzEmotional(config)
+    emotional_config = Emotional(config)
     info = emotional_config.info()
     assert isinstance(info, str)
```

### Comparing `emotional-0.1.0/tests/test_github.py` & `emotional-0.2.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/tests/test_gitlab.py` & `emotional-0.2.1/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/tests/test_jira.py` & `emotional-0.2.1/tests/test_jira.py`

 * *Files identical despite different names*

### Comparing `emotional-0.1.0/PKG-INFO` & `emotional-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: emotional
-Version: 0.1.0
+Version: 0.2.1
+Summary: A Commitizen plugin for conventional commit with emojis and integrations
+Author-Email: Axel H. <noirbizarre@gmail.com>
 License: MIT
-Author-email: Axel H. <noirbizarre@gmail.com>
 Requires-Python: >=3.7
+Requires-Dist: commitizen>=3.0
+Requires-Dist: typing-extensions>=4.4.0; python_version < "3.10"
 Description-Content-Type: text/markdown
 
 # emotional
 
 [![CI](https://github.com/noirbizarre/emotional/actions/workflows/ci.yml/badge.svg)](https://github.com/noirbizarre/emotional/actions/workflows/ci.yml)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/2e6bed0a58cd88af159f/test_coverage)](https://codeclimate.com/github/noirbizarre/emotional/test_coverage)
 [![Maintainability](https://api.codeclimate.com/v1/badges/2e6bed0a58cd88af159f/maintainability)](https://codeclimate.com/github/noirbizarre/emotional/maintainability)
@@ -102,8 +105,7 @@
 keep in mind than `jira` is compatible with both `github` and `gitlab`
 while `github` and `gitlab` are conflicting because they use the same format.
 
 
 [commitizen]: https://commitizen-tools.github.io/commitizen/
 [commitizen-config]: https://commitizen-tools.github.io/commitizen/config/
 [conventional-commit]: https://www.conventionalcommits.org/
-
```

