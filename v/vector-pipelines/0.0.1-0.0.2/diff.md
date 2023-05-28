# Comparing `tmp/vector_pipelines-0.0.1.tar.gz` & `tmp/vector_pipelines-0.0.2.tar.gz`

## Comparing `vector_pipelines-0.0.1.tar` & `vector_pipelines-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,33 @@
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/docker-compose.yaml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/main.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/.ruff_cache/content/46a481b852ad66d0
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/.ruff_cache/content/a696c19d73c68540
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/vector_pipelines/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/vector_pipelines/py.typed
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/LICENSE
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/README.md
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 vector_pipelines-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/Makefile
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.github/workflows/smokeshow.yaml
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/test_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/components/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/components/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/components/embeddings/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/components/embeddings/test_sentence_transformers.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/cli/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/cli/app.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/cli/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/__init__.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/config.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/init.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/embeddings/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/embeddings/base.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/embeddings/sentence_transformers.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/embeddings/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/grpc/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2.pyi
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2_grpc.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/proto/embeddings.proto
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/LICENSE
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/README.md
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/PKG-INFO
```

### Comparing `vector_pipelines-0.0.1/.gitignore` & `vector_pipelines-0.0.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -123,7 +123,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# VSCode
+.vscode/
```

### Comparing `vector_pipelines-0.0.1/LICENSE` & `vector_pipelines-0.0.2/LICENSE`

 * *Files identical despite different names*

