# Comparing `tmp/q2terminal-0.1.8.tar.gz` & `tmp/q2terminal-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2terminal-0.1.8.tar", max compression
+gzip compressed data, was "q2terminal-0.1.9.tar", max compression
```

## Comparing `q2terminal-0.1.8.tar` & `q2terminal-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      385 2023-05-09 12:18:07.985586 q2terminal-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2421 2023-05-08 11:48:24.661192 q2terminal-0.1.8/q2terminal/q2terminal.py
--rw-r--r--   0        0        0       21 2023-05-09 12:18:10.878255 q2terminal-0.1.8/q2terminal/version.py
--rw-r--r--   0        0        0      523 2023-05-06 22:10:01.827611 q2terminal-0.1.8/README.md
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 q2terminal-0.1.8/setup.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 q2terminal-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-05-09 12:19:05.617815 q2terminal-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2421 2023-05-08 11:48:24.661192 q2terminal-0.1.9/q2terminal/q2terminal.py
+-rw-r--r--   0        0        0       21 2023-05-09 12:19:07.600790 q2terminal-0.1.9/q2terminal/version.py
+-rw-r--r--   0        0        0      523 2023-05-06 22:10:01.827611 q2terminal-0.1.9/README.md
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 q2terminal-0.1.9/setup.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 q2terminal-0.1.9/PKG-INFO
```

### Comparing `q2terminal-0.1.8/q2terminal/q2terminal.py` & `q2terminal-0.1.9/q2terminal/q2terminal.py`

 * *Files identical despite different names*

### Comparing `q2terminal-0.1.8/README.md` & `q2terminal-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `q2terminal-0.1.8/setup.py` & `q2terminal-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['q2terminal']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'q2terminal',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '[![Python application](https://github.com/AndreiPuchko/q2terminal/actions/workflows/main.yml/badge.svg)](https://github.com/AndreiPuchko/q2terminal/actions/workflows/main.yml)\n# Interaction with a terminal session\n\n```python\nfrom q2terminal.q2terminal import Q2Terminal\nimport sys\n\nt = Q2Terminal()\nt.run("programm", echo=True)\nassert t.exit_code != 0\n\nassert t.run("$q2 = 123") == []\nassert t.run("echo $q2") == ["123"]\n\n\nif "win32" in sys.platform:\n    t.run("notepad")\n    assert t.exit_code == 0\n```\n',
     'author': 'Andrei Puchko',
     'author_email': 'andrei.puchko@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8.1',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `q2terminal-0.1.8/PKG-INFO` & `q2terminal-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: q2terminal
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
-Requires-Python: >=3.8.1
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 [![Python application](https://github.com/AndreiPuchko/q2terminal/actions/workflows/main.yml/badge.svg)](https://github.com/AndreiPuchko/q2terminal/actions/workflows/main.yml)
```

