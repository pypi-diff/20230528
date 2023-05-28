# Comparing `tmp/webpy-framework-1.1.1.tar.gz` & `tmp/webpy-framework-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-1.1.1.tar", last modified: Sat May 27 16:00:17 2023, max compression
+gzip compressed data, was "webpy-framework-1.1.2.tar", last modified: Sun May 28 02:31:48 2023, max compression
```

## Comparing `webpy-framework-1.1.1.tar` & `webpy-framework-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 16:00:17.140449 webpy-framework-1.1.1/
--rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6599 2023-05-27 16:00:17.139450 webpy-framework-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-05-27 01:42:52.000000 webpy-framework-1.1.1/README.md
--rw-rw-rw-   0        0        0     1075 2023-05-27 15:59:55.000000 webpy-framework-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 16:00:17.140449 webpy-framework-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 16:00:17.116834 webpy-framework-1.1.1/webpy/
--rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.1.1/webpy/__init__.py
--rw-rw-rw-   0        0        0    10520 2023-05-27 15:34:19.000000 webpy-framework-1.1.1/webpy/__main__.py
--rw-rw-rw-   0        0        0     1809 2023-05-27 15:07:10.000000 webpy-framework-1.1.1/webpy/fs_routes.py
--rw-rw-rw-   0        0        0     1492 2023-05-27 15:28:10.000000 webpy-framework-1.1.1/webpy/pysite_semantic_tags.py
-drwxrwxrwx   0        0        0        0 2023-05-27 16:00:17.137073 webpy-framework-1.1.1/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     6599 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 02:31:48.334001 webpy-framework-1.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6599 2023-05-28 02:31:48.330496 webpy-framework-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-05-27 01:42:52.000000 webpy-framework-1.1.2/README.md
+-rw-rw-rw-   0        0        0     1075 2023-05-28 02:31:11.000000 webpy-framework-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 02:31:48.334001 webpy-framework-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 02:31:48.301854 webpy-framework-1.1.2/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.1.2/webpy/__init__.py
+-rw-rw-rw-   0        0        0    10754 2023-05-28 01:50:22.000000 webpy-framework-1.1.2/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1809 2023-05-27 15:07:10.000000 webpy-framework-1.1.2/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0     1492 2023-05-27 15:28:10.000000 webpy-framework-1.1.2/webpy/pysite_semantic_tags.py
+drwxrwxrwx   0        0        0        0 2023-05-28 02:31:48.326473 webpy-framework-1.1.2/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     6599 2023-05-28 02:31:48.000000 webpy-framework-1.1.2/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-05-28 02:31:48.000000 webpy-framework-1.1.2/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 02:31:48.000000 webpy-framework-1.1.2/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-28 02:31:48.000000 webpy-framework-1.1.2/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      155 2023-05-28 02:31:48.000000 webpy-framework-1.1.2/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 02:31:48.000000 webpy-framework-1.1.2/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-1.1.1/LICENSE` & `webpy-framework-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.1/PKG-INFO` & `webpy-framework-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.1.1
+Version: 1.1.2
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `webpy-framework-1.1.1/README.md` & `webpy-framework-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.1/pyproject.toml` & `webpy-framework-1.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "1.1.1"
+version = "1.1.2"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
```

### Comparing `webpy-framework-1.1.1/webpy/__init__.py` & `webpy-framework-1.1.2/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.1/webpy/__main__.py` & `webpy-framework-1.1.2/webpy/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,17 +112,14 @@
 	
 	try:
 		app: Flask = appmod.app
 		setup: FunctionType = appmod.webpy_setup
 	except AttributeError:
 		print("app object and webpy_setup function are missing from app.py!")
 
-	if force_debug: app.debug = True
-	else: app.debug = False
-
 	prerules = list(app.url_map.iter_rules())
 
 	# TODO: use TypedDict for this
 	routes: dict[str, dict[str, Union[dict[str, str], bytes, str]]] = {}
 
 	if not parse_fs_routes(app, "root", routes):
 		exit(1)
@@ -147,14 +144,15 @@
 	{app.template_folder!r},
 	{app.instance_path!r},
 	{conf.get("instance_relative_config", False)!r},
 	{app.root_path!r}
 )
 
 loads({dill.dumps(setup)!r})(app)
+app.debug = {True if force_debug else False}
 """
 		)
 
 		for rule in prerules:
 			if rule.endpoint == "static": continue
 			
 			code+=(
@@ -381,19 +379,19 @@
 		"buildmd"
 		),
 		help="Possible commands --- webpy new {projectname} (create a new project) --- webpy route {routename} (create a new route directory) --- webpy run (start the application) --- webpy build (compile root/ and app.py into build.py) --- webpy compile (like build but create build.pyc) --- webpy buildpyx (compile all .pyx to .py) --- webpy buildmd (compile all .md to .html)"
 	)
 
 	parser.add_argument("name", help="name to be used for 'new' or 'route' commands", default=None, nargs='?')
 
-	parser.add_argument("--no-compile-md", action="store_true")
-	parser.add_argument("--no-compile-pyx", action="store_true")
-	parser.add_argument("--no-reload-md", action="store_true")
-	parser.add_argument("--no-reload-pyx", action="store_true")
-	parser.add_argument("--force-debug", action="store_true")
+	parser.add_argument("--no-compile-md", action="store_true", help="do not compile Markdown to HTML")
+	parser.add_argument("--no-compile-pyx", action="store_true", help="do not compile PyX to Python")
+	parser.add_argument("--no-reload-md", action="store_true", help="do not check for modifications in Markdown files while running")
+	parser.add_argument("--no-reload-pyx", action="store_true", help="do not check for modifications in PyX files while running")
+	parser.add_argument("--force-debug", action="store_true", help="make sure debug mode is used")
 
 
 	args = parser.parse_args()
 	cmd = args.command
 	name = args.name
 
 	compile_md = not args.no_compile_md
```

### Comparing `webpy-framework-1.1.1/webpy/fs_routes.py` & `webpy-framework-1.1.2/webpy/fs_routes.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.1/webpy/pysite_semantic_tags.py` & `webpy-framework-1.1.2/webpy/pysite_semantic_tags.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.1/webpy_framework.egg-info/PKG-INFO` & `webpy-framework-1.1.2/webpy_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.1.1
+Version: 1.1.2
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

