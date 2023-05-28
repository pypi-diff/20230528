# Comparing `tmp/timona-0.0.1.tar.gz` & `tmp/timona-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timona-0.0.1.tar", max compression
+gzip compressed data, was "timona-0.0.2.tar", max compression
```

## Comparing `timona-0.0.1.tar` & `timona-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.1/LICENSE
--rw-r--r--   0        0        0       46 2023-05-26 12:19:29.287039 timona-0.0.1/README.md
--rw-r--r--   0        0        0      485 2023-05-26 13:28:59.772132 timona-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.1/timona/__init__.py
--rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.1/timona/__main__.py
--rw-r--r--   0        0        0       22 2023-05-26 13:28:59.772132 timona-0.0.1/timona/__version__.py
--rw-r--r--   0        0        0     1079 2023-05-26 12:19:29.311040 timona-0.0.1/timona/config.py
--rw-r--r--   0        0        0     2715 2023-05-26 12:19:29.311040 timona-0.0.1/timona/helm.py
--rw-r--r--   0        0        0     2766 2023-05-26 13:16:03.924441 timona-0.0.1/timona/main.py
--rw-r--r--   0        0        0     4876 2023-05-26 12:19:29.311040 timona-0.0.1/timona/releases.py
--rw-r--r--   0        0        0     1203 2023-05-26 12:19:29.311040 timona-0.0.1/timona/template.py
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 timona-0.0.1/setup.py
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 timona-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.2/LICENSE
+-rw-r--r--   0        0        0       46 2023-05-26 12:19:29.287039 timona-0.0.2/README.md
+-rw-r--r--   0        0        0      542 2023-05-28 07:29:37.581550 timona-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.2/timona/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.2/timona/__main__.py
+-rw-r--r--   0        0        0       38 2023-05-28 07:29:37.581550 timona-0.0.2/timona/__version__.py
+-rw-r--r--   0        0        0     1177 2023-05-28 07:24:27.978336 timona-0.0.2/timona/config.py
+-rw-r--r--   0        0        0     2715 2023-05-26 12:19:29.311040 timona-0.0.2/timona/helm.py
+-rw-r--r--   0        0        0     2766 2023-05-26 13:16:03.924441 timona-0.0.2/timona/main.py
+-rw-r--r--   0        0        0     5148 2023-05-28 06:06:31.058605 timona-0.0.2/timona/releases.py
+-rw-r--r--   0        0        0     1190 2023-05-26 17:41:50.796484 timona-0.0.2/timona/template.py
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 timona-0.0.2/setup.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 timona-0.0.2/PKG-INFO
```

### Comparing `timona-0.0.1/LICENSE` & `timona-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timona-0.0.1/timona/config.py` & `timona-0.0.2/timona/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import yaml
 import hashlib
+from deepmerge import always_merger
 
 CFG_FILE = 'timona.yaml'
 
 
 def load_config_file(c):
     _data = []
 
@@ -27,21 +28,21 @@
 
 
 def load_config(c=None):
     if c is None:
         c = CFG_FILE
     _data = {}
 
-    def _load_config(c):
+    def _load_config(c, _data):
         f = load_config_file(c)
         f = yaml.safe_load(f)
         if 'include' in f:
             for g in f['include']:
-                _load_config(g)
+                _load_config(g, _data)
             del(f['include'])
-        _data.update(f)
-    _load_config(c)
+        _data = always_merger.merge(_data, f)  # _data.update(f)
+    _load_config(c, _data)
     h = hashlib.sha256(
         yaml.safe_dump(_data).encode('utf-8')
     ).hexdigest()  # sha256(yaml(_data))
     _data['.hash'] = h
     return _data
```

### Comparing `timona-0.0.1/timona/helm.py` & `timona-0.0.2/timona/helm.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.1/timona/main.py` & `timona-0.0.2/timona/main.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.1/timona/releases.py` & `timona-0.0.2/timona/releases.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 import yaml
 from threading import Thread
 import subprocess
-from pprint import pprint
+from pprint import pformat
 import os
 import itertools
 
 
 def flatten_matrix(matrix):
     flat_matrix = []
     item_list = []
@@ -23,45 +23,55 @@
         for (var_name, var_value) in item:
             flat_item[var_name] = var_value
         flat_matrix.append(flat_item)
     return flat_matrix
 
 
 # Count the variables in a release
-def count_vars(data, var_re):
+def count_vars(data, tpl):
     c = 0
     for var_name, var_value in data.items():
         if var_name != '__count__':
-            if var_re:
-                c = c + len(var_re.findall(var_value))
+            if tpl.var_re:
+                c = c + len(tpl.var_re.findall(var_value))
             else:
                 for k in data.keys():
                     c = c + var_value.count(k)
+    if c == 0 and not tpl.var_re:
+        for var_name, var_value in data.items():
+            if var_name != '__count__':
+                try:
+                    tpl.render(var_value, {})
+                except Exception:
+                    c = 999
+                    break
     return c
 
 
 def solve_vars(in_data, out_data, tpl):
+    in_data['__count__'] = count_vars(in_data, tpl)
     while in_data['__count__'] > 0:
         tmp_data = {'__count__': 0}
         c = in_data['__count__']
         del(in_data['__count__'])
         err = None
         for var_name, var_value in in_data.items():
             try:
                 tmp_data[var_name] = tpl.render(var_value, in_data).strip()
             except Exception as e:
                 err = e
                 tmp_data[var_name] = var_value
-        tmp_data['__count__'] = count_vars(tmp_data, tpl.var_re)
+        tmp_data['__count__'] = count_vars(tmp_data, tpl)
         if c == tmp_data['__count__']:
             out_data['e']['last'] = in_data
             out_data['e']['err'] = err
+            out_data['e']['count'] = c
             return
         in_data = tmp_data
-    out_data['d'] = {**in_data}
+    out_data['d'] = dict(in_data)
 
 
 def get_releases(tpl, tmp, config):
     cache = '{}/releases.{}.yaml'.format(tmp, config['.hash'])
     if os.path.isfile(cache):
         with open(cache, 'r') as f:
             out = yaml.safe_load(f.read())
@@ -80,21 +90,14 @@
                 for matrix in data['matrix']:
                     flat_matrix = flatten_matrix(matrix)
                     for release_matrix in flat_matrix:
                         out.append({**release_template, **release_matrix})
             else:
                 out.append(release_template)
 
-        # Add __count__
-        _releases = []
-        for release in out:
-            c = {'__count__': count_vars(release, tpl.var_re)}
-            _releases.append({**release, **c})
-        out = _releases
-
         # Solve vars, each release in a thread
         _releases = []
         threads = []
         for release in out:
             x = {
                 't': None,    # thread
                 'r': {        # solved vars release
@@ -109,21 +112,23 @@
             threads.append(x)
             t.start()
         for x in threads:
             x['t'].join()
             if len(x['r']['e']) == 0:
                 _releases.append(x['r']['d'])
             else:
-                print('Loop or template error')
-                print('Latest data:')
-                pprint(x['r']['e']['last'])
-                print('Error: {}'.format(x['r']['e']['err']))
+                msg = ''
+                msg = msg + 'Loop or template error\n'
+                msg = msg + 'Latest data:\n'
+                msg = msg + pformat(x['r']['e']['last']) + '\n'
+                msg = msg + 'Error: {}\n'.format(x['r']['e']['err'])
                 if type(x['r']['e']['err']) is subprocess.CalledProcessError:
-                    print('  stderr: {}'.format(x['r']['e']['err'].stderr))
-                return None
+                    msg = msg + '  stderr: {}'.format(
+                        x['r']['e']['err'].stderr)
+                raise RuntimeError(msg)
         out = _releases
 
         # Cleanup variables staring with _
         # Check for duplicate names
         _releases = {}
         for release in out:
             n = release['__name__']
@@ -133,16 +138,16 @@
                     if k[0] == '_':
                         to_del.append(k)
                 for k in to_del:
                     del(release[k])
                 _releases[n] = release
             else:
                 raise RuntimeError(
-                    'Duplicate release name: {}\n{}\n{}'
-                    .format(n, _releases[n], release)
+                    'Duplicate release name: {}\n{}\n{}'.format(
+                        n, _releases[n], release)
                 )
         out = _releases
 
         with open(cache, 'w') as f:
             f.write(yaml.safe_dump(out))
 
     return out
```

### Comparing `timona-0.0.1/timona/template.py` & `timona-0.0.2/timona/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,19 @@
             self.cmd = config['command']['render']
             p = subprocess.run(
                 shlex.split(config['command']['version']),
                 capture_output=True, check=True, text=True
             )
             v = p.stdout.strip()
             v = 'command: {}'.format(v)
-            self.stderr = config['command'].get("stderr")
+            self.stderr = config['command'].get('stderr')
         self.version = v
-        if 'regex' in config:
-            self.var_re = re.compile(config['regex'])
-        else:
-            self.var_re = None
+        self.var_re = config.get('regex')
+        if self.var_re:
+            self.var_re = re.compile(self.var_re)
 
     def render(self, tpl, env):
         if self.cmd:
             p = subprocess.run(
                 shlex.split(self.cmd),
                 input=tpl, env={**env, **os.environ},
                 capture_output=True, check=True, text=True,
```

### Comparing `timona-0.0.1/setup.py` & `timona-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 
 packages = \
 ['timona']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['deepmerge', 'jinja2', 'pyyaml', 'requests']
+
 entry_points = \
 {'console_scripts': ['timona = timona.main:main']}
 
 setup_kwargs = {
     'name': 'timona',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Tool to automate Helm deployments',
     'long_description': '# timona\n\nA tool to automate Helm deployments\n',
     'author': 'mihaiush',
     'author_email': 'mihaiush@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mihaiush/timona',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `timona-0.0.1/PKG-INFO` & `timona-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: timona
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool to automate Helm deployments
 Home-page: https://github.com/mihaiush/timona
 Author: mihaiush
 Author-email: mihaiush@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: deepmerge
+Requires-Dist: jinja2
+Requires-Dist: pyyaml
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # timona
 
 A tool to automate Helm deployments
```

