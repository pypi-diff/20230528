# Comparing `tmp/novella-0.2.5.tar.gz` & `tmp/novella-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novella-0.2.5.tar", max compression
+gzip compressed data, was "novella-0.2.6.tar", max compression
```

## Comparing `novella-0.2.5.tar` & `novella-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2029 2023-03-11 00:02:37.794004 novella-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      742 2022-11-12 22:52:13.628539 novella-0.2.5/readme.md
--rw-r--r--   0        0        0       23 2023-03-11 00:02:37.794004 novella-0.2.5/src/novella/__init__.py
--rw-r--r--   0        0        0     5983 2023-03-10 01:12:02.659779 novella-0.2.5/src/novella/__main__.py
--rw-r--r--   0        0        0     5390 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/action.py
--rw-r--r--   0        0        0     8991 2023-03-10 01:05:52.730239 novella-0.2.5/src/novella/build.py
--rw-r--r--   0        0        0      108 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/compat.py
--rw-r--r--   0        0        0     4409 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/graph.py
--rw-r--r--   0        0        0     1761 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/markdown/flavor.py
--rw-r--r--   0        0        0     6969 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/markdown/preprocessor.py
--rw-r--r--   0        0        0     7585 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/markdown/tagparser.py
--rw-r--r--   0        0        0     4321 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/markdown/tags/anchor.py
--rw-r--r--   0        0        0     6148 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/markdown/tags/cat.py
--rw-r--r--   0        0        0     2665 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/markdown/tags/shell.py
--rw-r--r--   0        0        0     7323 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/novella.py
--rw-r--r--   0        0        0        0 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/py.typed
--rw-r--r--   0        0        0     1047 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/repository.py
--rw-r--r--   0        0        0      772 2022-11-12 22:52:13.628539 novella-0.2.5/src/novella/template.py
--rw-r--r--   0        0        0     3520 2023-03-11 00:02:33.282132 novella-0.2.5/src/novella/templates/hugo/__init__.py
--rw-r--r--   0        0        0     4423 2023-03-10 01:29:33.350082 novella-0.2.5/src/novella/templates/hugo/installer.py
--rw-r--r--   0        0        0    11780 2023-03-11 00:02:33.282132 novella-0.2.5/src/novella/templates/mkdocs.py
--rw-r--r--   0        0        0     1732 1970-01-01 00:00:00.000000 novella-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2029 2023-05-28 02:43:33.211329 novella-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      742 2022-11-12 22:52:13.628539 novella-0.2.6/readme.md
+-rw-r--r--   0        0        0       23 2023-05-28 02:43:33.231329 novella-0.2.6/src/novella/__init__.py
+-rw-r--r--   0        0        0     5983 2023-05-28 02:38:59.747090 novella-0.2.6/src/novella/__main__.py
+-rw-r--r--   0        0        0     5390 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/action.py
+-rw-r--r--   0        0        0     8991 2023-05-28 02:38:59.747090 novella-0.2.6/src/novella/build.py
+-rw-r--r--   0        0        0      108 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/compat.py
+-rw-r--r--   0        0        0     4409 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/graph.py
+-rw-r--r--   0        0        0     1761 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/markdown/flavor.py
+-rw-r--r--   0        0        0     7278 2023-05-28 02:38:59.747090 novella-0.2.6/src/novella/markdown/preprocessor.py
+-rw-r--r--   0        0        0     7585 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/markdown/tagparser.py
+-rw-r--r--   0        0        0     4477 2023-05-28 02:40:54.187843 novella-0.2.6/src/novella/markdown/tags/anchor.py
+-rw-r--r--   0        0        0     6148 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/markdown/tags/cat.py
+-rw-r--r--   0        0        0     2665 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/markdown/tags/shell.py
+-rw-r--r--   0        0        0     7323 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/novella.py
+-rw-r--r--   0        0        0        0 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/py.typed
+-rw-r--r--   0        0        0     1047 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/repository.py
+-rw-r--r--   0        0        0      772 2022-11-12 22:52:13.628539 novella-0.2.6/src/novella/template.py
+-rw-r--r--   0        0        0     3520 2023-05-28 02:38:59.747090 novella-0.2.6/src/novella/templates/hugo/__init__.py
+-rw-r--r--   0        0        0     4496 2023-05-28 02:38:59.747090 novella-0.2.6/src/novella/templates/hugo/installer.py
+-rw-r--r--   0        0        0    11912 2023-05-28 02:38:59.747090 novella-0.2.6/src/novella/templates/mkdocs.py
+-rw-r--r--   0        0        0     1732 1970-01-01 00:00:00.000000 novella-0.2.6/PKG-INFO
```

### Comparing `novella-0.2.5/pyproject.toml` & `novella-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "novella"
-version = "0.2.5"
+version = "0.2.6"
 description = "Linear build system for Markdown preprocessing and static site generation."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include="novella", from="src" }]
 
   [tool.poetry.urls]
```

### Comparing `novella-0.2.5/readme.md` & `novella-0.2.6/readme.md`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/__main__.py` & `novella-0.2.6/src/novella/__main__.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/action.py` & `novella-0.2.6/src/novella/action.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/build.py` & `novella-0.2.6/src/novella/build.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/graph.py` & `novella-0.2.6/src/novella/graph.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/markdown/flavor.py` & `novella-0.2.6/src/novella/markdown/flavor.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/markdown/preprocessor.py` & `novella-0.2.6/src/novella/markdown/preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,19 +62,25 @@
   #: all Markdown files in the build directory will be preprocessed.
   path: str | None = None
 
   #: The encoding to read and write files as.
   encoding: str | None = None
 
   def __post_init__(self) -> None:
-    self._processors = Graph[MarkdownPreprocessor]()
+    self._updaters: list[t.Callable] = []
+    self._processors = Graph['MarkdownPreprocessor']()
     self.use('shell')
     self.use('cat')
     self.use('anchor')
 
+  def update_with(self, func: t.Callable[[MarkdownPreprocessor], None]) -> None:
+    """ Adds a callback that can modify the MarkdownPreprocessor before it executes. """
+
+    self._updaters.append(func)
+
   def use(
     self,
     processor: str | MarkdownPreprocessor,
     closure: _Closure | None = None,
     name: str | None = None,
   ) -> None:
     """ Register a processor for use in the plugin. """
@@ -93,14 +99,17 @@
       processor = processor_cls(self, name)
     else:
       if not isinstance(processor, MarkdownPreprocessor):
         raise TypeError(f'expected MarkdownProcessor, got {type(processor).__name__}')
       if name is not None and name != processor.name:
         raise RuntimeError('mismatching "name": {name!r} != {processor.name!r}')
 
+    for mutator in self._updaters:
+      mutator(processor)
+
     self._processors.add_node(processor, self._processors.last_node_added)
 
     if closure:
       closure(processor)
 
   def preprocessor(self, processor_name: str, closure: _Closure | None = None) -> MarkdownPreprocessor:
     """ Access or reconfigure a markdown processor that is already registered. """
```

### Comparing `novella-0.2.5/src/novella/markdown/tagparser.py` & `novella-0.2.6/src/novella/markdown/tagparser.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/markdown/tags/anchor.py` & `novella-0.2.6/src/novella/markdown/tags/anchor.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,21 @@
   def _replace_anchor(self, file: MarkdownFile, tag: Tag) -> str | None:
     # Find the next Markdown header that immediately follows the tag.
     pattern = re.compile(r'\s*(#+)(.*)(?:\n|$)', re.M)
     match = pattern.match(file.content, tag.offset_span[1])
     header_level = len(match.group(1)) if match else None
     header_text = match.group(2).strip() if match else None
 
-    anchor = Anchor(tag.args.strip(), tag.options.get('text', None), header_level, header_text, file.path)
+    args = [arg.strip() for arg in tag.args.strip().split(' ', 1)]
+    if len(args) == 2:
+      anchor_id, header_text = args
+    else:
+      anchor_id = args[0]
+
+    anchor = Anchor(anchor_id, tag.options.get('text', None), header_level, header_text, file.path)
 
     if anchor.id in self._anchor_index:
       logger.warning(
         '  <fg=cyan;attr=italic>@anchor %s</fg> in <fg=yellow>%s</fg> conflicts with same anchor in '
         '  <fg=yellow>%s</fg>',
         tag.args, file.path, self._anchor_index[anchor.id].file,
       )
```

### Comparing `novella-0.2.5/src/novella/markdown/tags/cat.py` & `novella-0.2.6/src/novella/markdown/tags/cat.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/markdown/tags/shell.py` & `novella-0.2.6/src/novella/markdown/tags/shell.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/novella.py` & `novella-0.2.6/src/novella/novella.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/repository.py` & `novella-0.2.6/src/novella/repository.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/template.py` & `novella-0.2.6/src/novella/template.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/templates/hugo/__init__.py` & `novella-0.2.6/src/novella/templates/hugo/__init__.py`

 * *Files identical despite different names*

### Comparing `novella-0.2.5/src/novella/templates/hugo/installer.py` & `novella-0.2.6/src/novella/templates/hugo/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
   os.makedirs(os.path.dirname(to), exist_ok=True)
   with tempfile.TemporaryDirectory() as tempdir:
     path = os.path.join(tempdir, filename)
     with open(path, 'wb') as fp:
       shutil.copyfileobj(requests.get(files[filename], stream=True).raw, fp)
     with tarfile.open(path) as archive:
       with open(to, 'wb') as fp:
-        shutil.copyfileobj(
+        shutil.copyfileobj(  # type: ignore[misc]  # See https://github.com/python/mypy/issues/15031
           t.cast(t.IO[bytes], archive.extractfile('hugo')),
           t.cast(t.IO[bytes], fp))
 
   chmod.update(to, '+x')
   logger.info('Hugo v%s installed to "%s"', version, to)
```

### Comparing `novella-0.2.5/src/novella/templates/mkdocs.py` & `novella-0.2.6/src/novella/templates/mkdocs.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,19 @@
     context.option("serve", description="Use mkdocs serve", flag=True)
     context.option("port", description="The port to serve under", default="8000")
     context.option("site-dir", description='Build directory for MkDocs (defaults to "_site")', default="_site", metavar='PATH')
     context.option("base-url", description='The base URL to prefix to autogenerated link inside the documentation.', metavar='URL')
 
     copy_files = t.cast('CopyFilesAction', context.do('copy-files', name='copy-files'))
     copy_files.paths = [ self.content_directory ]
-    if (context.project_directory / 'mkdocs.yml').exists():
-      copy_files.paths.append('mkdocs.yml')
+
+    for extension in ['yml', 'yaml']:
+      if (context.project_directory / f'mkdocs.{extension}').exists():
+        copy_files.paths.append(f'mkdocs.{extension}')
+        break
 
     update_config = t.cast('MkdocsUpdateConfigAction', context.do('mkdocs-update-config', name='mkdocs-update-config'))
     update_config.content_directory = self.content_directory
 
     preprocessor = t.cast('MarkdownPreprocessorAction', context.do('preprocess-markdown', name='preprocess-markdown'))
     preprocessor.path = self.content_directory
     def configure_anchor(anchor: AnchorTagProcessor) -> None:
@@ -268,20 +271,23 @@
   def __post_init__(self) -> None:
     self._updaters: list[t.Callable] = []
 
   def execute(self, build: BuildContext) -> None:
     import copy
     import yaml
 
-    mkdocs_yml = build.directory / 'mkdocs.yml'
+    mkdocs_config = {}
+
+    for extension in ['yml', 'yaml']:
+      mkdocs_yml = build.directory / f'mkdocs.{extension}'
+
+      if mkdocs_yml.exists():
+        mkdocs_config = yaml.safe_load(mkdocs_yml.read_text())
+        break
 
-    if mkdocs_yml.exists():
-      mkdocs_config = yaml.safe_load(mkdocs_yml.read_text())
-    else:
-      mkdocs_config = {}
     original_config = copy.deepcopy(mkdocs_config)
 
     if self.apply_defaults and self.profile:
       default_config = yaml.safe_load(self._get_profile(self.profile))
       for key in default_config:
         if key not in mkdocs_config:
           mkdocs_config[key] = default_config[key]
```

### Comparing `novella-0.2.5/PKG-INFO` & `novella-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novella
-Version: 0.2.5
+Version: 0.2.6
 Summary: Linear build system for Markdown preprocessing and static site generation.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

