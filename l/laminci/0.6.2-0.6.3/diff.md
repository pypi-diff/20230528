# Comparing `tmp/laminci-0.6.2.tar.gz` & `tmp/laminci-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.6.2.tar", last modified: Sun May 28 21:39:19 2023, max compression
+gzip compressed data, was "laminci-0.6.3.tar", last modified: Sun May 28 21:51:16 2023, max compression
```

## Comparing `laminci-0.6.2.tar` & `laminci-0.6.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.2/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.2/README.md
--rw-r--r--   0        0        0     3052 2023-05-28 21:38:48.769732 laminci-0.6.2/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.2/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.2/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.2/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.2/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.2/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-05-28 21:38:43.116106 laminci-0.6.2/laminci/__init__.py
--rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.2/laminci/_artifacts.py
--rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.2/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.2/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.2/laminci/_env.py
--rw-r--r--   0        0        0     2423 2023-04-10 13:41:42.840205 laminci-0.6.2/laminci/_nox.py
--rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.2/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.2/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.2/noxfile.py
--rw-r--r--   0        0        0      706 2023-05-28 21:39:09.528997 laminci-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.2/tests/test_artifacts.py
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 laminci-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.6.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.6.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.6.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.6.3/README.md
+-rw-r--r--   0        0        0     3052 2023-05-28 21:50:42.304327 laminci-0.6.3/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.6.3/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-05-26 15:57:31.631988 laminci-0.6.3/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.6.3/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.6.3/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.6.3/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.6.3/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-05-28 21:50:39.640706 laminci-0.6.3/laminci/__init__.py
+-rw-r--r--   0        0        0     2122 2023-05-26 16:17:30.304228 laminci-0.6.3/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1358 2023-05-26 16:17:30.304517 laminci-0.6.3/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.6.3/laminci/_docs.py
+-rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.6.3/laminci/_env.py
+-rw-r--r--   0        0        0     2423 2023-04-10 13:41:42.840205 laminci-0.6.3/laminci/_nox.py
+-rw-r--r--   0        0        0      148 2023-05-26 16:33:21.362381 laminci-0.6.3/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.6.3/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.6.3/noxfile.py
+-rw-r--r--   0        0        0      708 2023-05-28 21:50:19.140197 laminci-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-05-26 16:17:30.304991 laminci-0.6.3/tests/test_artifacts.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 laminci-0.6.3/PKG-INFO
```

### Comparing `laminci-0.6.2/.github/workflows/build.yml` & `laminci-0.6.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/.github/workflows/latest-changes.yml` & `laminci-0.6.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/.gitignore` & `laminci-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/.pre-commit-config.yaml` & `laminci-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/docs/changelog.md` & `laminci-0.6.3/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-✨ Add aws cli based way of pushing a docs artifact | [20](https://github.com/laminlabs/laminci/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.6.2
+✨ Add aws cli based way of pushing a docs artifact | [20](https://github.com/laminlabs/laminci/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.6.3
 🚸 Allow passing version to `setup_local_test_postgres` | [19](https://github.com/laminlabs/laminci/pull/19) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 🚸 Close current instance before uploading docs artifacts | [17](https://github.com/laminlabs/laminci/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.3
 🚸 Add support for environments | [16](https://github.com/laminlabs/laminci/pull/16) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.1
 ⬆️ Upgrade to new replace API | [15](https://github.com/laminlabs/laminci/pull/15) | [falexwolf](https://github.com/falexwolf) | 2023-04-10 | 0.5.0
 ♻️ Replace `lndb` with `lamin` | [14](https://github.com/laminlabs/laminci/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-03-29 | 0.4.2
 🚸 Replace git checkout with git switch | [13](https://github.com/laminlabs/laminci/pull/13) | [falexwolf](https://github.com/falexwolf) | 2023-03-27 | 0.4.1
 ⬆️ Upgrade to LaminDB v0.35 | [12](https://github.com/laminlabs/laminci/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-03-26 | 0.4.0
```

### Comparing `laminci-0.6.2/docs/guide/quickstart.ipynb` & `laminci-0.6.3/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.6.3/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/laminci/_artifacts.py` & `laminci-0.6.3/laminci/_artifacts.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/laminci/_db.py` & `laminci-0.6.3/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/laminci/_env.py` & `laminci-0.6.3/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/laminci/_nox.py` & `laminci-0.6.3/laminci/_nox.py`

 * *Files identical despite different names*

### Comparing `laminci-0.6.2/pyproject.toml` & `laminci-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # this CANNOT depend on lamindb as long as we use it
     # as an upstream dependency within lndb!
     "nox",
     "lamin_logger",
-    "yaml",
+    "pyyaml",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/laminci"
 
 [project.optional-dependencies]
 dev = [
```

