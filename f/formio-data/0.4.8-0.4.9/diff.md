# Comparing `tmp/formio-data-0.4.8.tar.gz` & `tmp/formio-data-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formio-data-0.4.8.tar", max compression
+gzip compressed data, was "formio-data-0.4.9.tar", max compression
```

## Comparing `formio-data-0.4.8.tar` & `formio-data-0.4.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2022-06-23 06:15:09.395447 formio-data-0.4.8/LICENSE
--rw-r--r--   0        0        0     5572 2022-07-12 10:29:21.994562 formio-data-0.4.8/README.md
--rw-r--r--   0        0        0      171 2022-06-23 06:15:09.396448 formio-data-0.4.8/formiodata/__init__.py
--rw-r--r--   0        0        0     3483 2022-06-23 06:15:09.396448 formio-data-0.4.8/formiodata/builder.py
--rw-r--r--   0        0        0    34792 2022-11-08 16:36:13.035709 formio-data-0.4.8/formiodata/components.py
--rw-r--r--   0        0        0     4215 2023-01-10 08:15:04.867856 formio-data-0.4.8/formiodata/form.py
--rw-r--r--   0        0        0      979 2022-06-23 06:15:09.396448 formio-data-0.4.8/formiodata/utils.py
--rw-r--r--   0        0        0      541 2023-01-10 08:12:19.361031 formio-data-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     6637 2023-01-10 08:16:07.911458 formio-data-0.4.8/setup.py
--rw-r--r--   0        0        0     6348 2023-01-10 08:16:07.912032 formio-data-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-06-23 06:15:09.395447 formio-data-0.4.9/LICENSE
+-rw-r--r--   0        0        0     5572 2022-07-12 10:29:21.994562 formio-data-0.4.9/README.md
+-rw-r--r--   0        0        0      171 2022-06-23 06:15:09.396448 formio-data-0.4.9/formiodata/__init__.py
+-rw-r--r--   0        0        0     3483 2022-06-23 06:15:09.396448 formio-data-0.4.9/formiodata/builder.py
+-rw-r--r--   0        0        0    35077 2023-01-12 15:57:13.521403 formio-data-0.4.9/formiodata/components.py
+-rw-r--r--   0        0        0     4198 2023-01-12 16:10:10.025916 formio-data-0.4.9/formiodata/form.py
+-rw-r--r--   0        0        0      979 2022-06-23 06:15:09.396448 formio-data-0.4.9/formiodata/utils.py
+-rw-r--r--   0        0        0      541 2023-01-12 15:57:34.426432 formio-data-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     6637 2023-01-12 16:14:46.875304 formio-data-0.4.9/setup.py
+-rw-r--r--   0        0        0     6348 2023-01-12 16:14:46.876249 formio-data-0.4.9/PKG-INFO
```

### Comparing `formio-data-0.4.8/LICENSE` & `formio-data-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `formio-data-0.4.8/README.md` & `formio-data-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `formio-data-0.4.8/formiodata/builder.py` & `formio-data-0.4.9/formiodata/builder.py`

 * *Files identical despite different names*

### Comparing `formio-data-0.4.8/formiodata/components.py` & `formio-data-0.4.9/formiodata/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,24 +163,35 @@
             default = self.defaultValue
         else:
             default = self._none_value
         return self.form.get('value', default)
 
     @value.setter
     def value(self, value):
+        self.set_value(value)
+
+    def _set_value(self, value):
         self.form['value'] = self._encode_value(value)
 
     @property
     def raw_value(self):
         return self.form['raw_value']
 
     @raw_value.setter
     def raw_value(self, value):
+        self._set_raw_value(value)
+
+    def _set_raw_value(self, value):
         self.form['raw_value'] = value
 
+    def set_value(self, value):
+        """ Set raw_value and value at once! """
+        self._set_raw_value(value)
+        self._set_value(value)
+
     @property
     def hidden(self):
         return self.raw.get('hidden')
 
     def _encode_value(self, value):
         return value
```

### Comparing `formio-data-0.4.8/formiodata/form.py` & `formio-data-0.4.9/formiodata/form.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,45 +69,45 @@
         return self._input
 
     @property
     def data(self):
         logging.warning('DEPRECATION WARNING: data attr/property shall be deleted in a future version.')
         return self._data
 
-    def get_component_owner_from_path(self, component, parent_component, path):
+    def get_component_from_path(self, component_path):
         """
-        Get component owner from path (provided by the Formio.js JS/API).
-        Especially handy for data Components eg datagridComponent, where
-        a row is a component owner.
+        Get component object from path (provided by the Formio.js JS/API)
+        Especially handy for data Components eg datagridComponent.
 
         Example path:
         dataGrid[0].lastname => lastname in the first row [0] of a datagrid
 
-        @param component: the component to start the traversal
-        @param parent_component: possible parent component of the component
-        @param path: the Formio.js JS/API path
-        return component_owner: JSON data ie the component owner
+        # Example path_nodes:
+        # dataGrid[0].lastname => ['dataGrid[0]', 'lastname']
+
+        @param component_path: the Formio.js JS/API path
+        @return component: a Component object
         """
-        path_nodes = path.split('.')
+        path_nodes = component_path.split('.')
         # Example path_nodes:
         # dataGrid[0].lastname => ['dataGrid[0]', 'lastname']
-        component_owner = self.form
-        if component and not path_nodes and component.key == path:
-            return component_owner
-        elif parent_component:
-            node = self.form[parent_component.key]
-            for path_node in path_nodes:
-                # get the component_owner eg row in datagrid
-                m = re.search(r"\[([A-Za-z0-9_]+)\]", path_node)
-                if m:
-                    idx = int(m.group(1))
-                    node = node[idx]
-            return node
-        else:
-            return self.form
+        components = self.input_components
+        for path_node in path_nodes:
+            # get the component_owner eg row in datagrid
+            m = re.search(r"\[([A-Za-z0-9_]+)\]", path_node)
+            if m:
+                idx_notation = m.group(0)  # eg: '[0]', '[1]', etc
+                idx = int(m.group(1))  # eg: 0, 1, etc
+                key = path_node.replace(idx_notation, '')
+                component = components[key]
+                if hasattr(component, 'rows'):
+                    components = component.rows[idx].input_components
+            else:
+                component = components[path_node]
+        return component
 
     def render_components(self, force=False):
         for key, component in self.input_components.items():
             if force or component.html_component == "":
                 if component.is_visible:
                     component.render()
                 else:
```

### Comparing `formio-data-0.4.8/formiodata/utils.py` & `formio-data-0.4.9/formiodata/utils.py`

 * *Files identical despite different names*

### Comparing `formio-data-0.4.8/pyproject.toml` & `formio-data-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formio-data"
-version = "0.4.8"
+version = "0.4.9"
 homepage = "https://github.com/novacode-nl/python-formio-data"
 description = "formio.js JSON-data API"
 readme = "README.md"
 authors = ["Bob Leers <bob@novacode.nl>"]
 license = "MIT"
 packages = [ { include = "formiodata/**/*.py" } ]
 exclude = ["tests/*"]
```

### Comparing `formio-data-0.4.8/setup.py` & `formio-data-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 extras_require = \
 {':python_version <= "3.6"': ['python-dateutil>=2.8.2,<3.0.0'],
  'json_logic': ['json_logic_qubit>=0.9.1,<0.10.0']}
 
 setup_kwargs = {
     'name': 'formio-data',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'formio.js JSON-data API',
     'long_description': '# formio-data (Python)\n\nformio.js (JSON Form Builder) data API for Python.\n\nFor information about the formio.js project, see https://github.com/formio/formio.js\n\n## Introduction\n\n**python-formio-data** is a Python package, which loads and transforms\nformio.js **Builder JSON** and **Form JSON** into **usable Python objects**.  It\'s main\naim is to provide easy access to a Form its components/fields, also\ncaptured as **Python objects**, which makes this API very versatile and usable.\n\n**Notes about terms:**\n  - **Builder:** The Form Builder which is the design/blueprint of a Form.\n  - **Form:** A filled-in Form, aka Form submission.\n  - **Component:** Input (field) or layout component in the Form Builder and Form.\n\n## Features\n\n  - Compatible with Python 3.6 and later\n  - Constructor of the **Builder** and **Form** class, only requires\n    the JSON and an optional language code for translations.\n  - Get a Form object its Components as a usable object e.g. datetime, boolean, dict (for select component) etc.\n  - Open source (MIT License)\n\n## Installation\n\nThe source code is currently hosted on GitHub at:\nhttps://github.com/novacode-nl/python-formio-data\n\n### PyPI - Python Package Index\n\nBinary installers for the latest released version are available at the [Python\nPackage Index](https://pypi.python.org/pypi/formio-data)\n\n```sh\npip(3) install formio-data\n```\n\n#### Optional dependencies\n\nTo support conditional visibility using JSON logic, you can install\nthe `json-logic-qubit` package (the `json-logic` package it is forked\noff of is currently unmaintained).  It\'s also possible to install it\nvia the pip feature `json_logic` like so:\n\n```sh\npip(3) install -U formio-data[json_logic]\n```\n\n### Source Install with Poetry (recommended)\n\nConvenient for developers. Also useful for running the (unit)tests.\n\n```sh\ngit clone git@github.com:novacode-nl/python-formio-data.git\npoetry install\n```\n\n#### Optional dependencies\n\nWhen working in the project itself, use\n\n```sh\npoetry install -E json_logic\n```\n\n### Source Install with pip\n\nOptional dependencies need to be installed separately.\n\n```sh\npip(3) install -U -e python-formio-data\n```\n\n## Using direnv\n\nYou can use [nixpkgs](https://nixos.org/) to run a self-contained\nPython environment without any additional setup.  Once you\'ve\ninstalled nixpkgs, switch into the directory and type "nix-shell" to\nget a shell from which the correct Python with packages is available.\n\nIf you\'re using [direnv](https://direnv.net/), use `direnv allow`\nafter changing into the project directory and you\'re good to go.  Also\nconsider [nix-direnv](https://github.com/nix-community/nix-direnv) to\nspeed up the experience (it can re-use a cached local installation).\n\n## License\n[MIT](LICENSE)\n\n## Contributing\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.\n\n## Usage examples\n\nFor more examples of usage, see the unit-tests.\n\n``` python\n>> from formiodata import Builder, Form\n>>\n# builder_json is a formio.js Builder JSON document (text/string)\n# form_json is a formio.js Form JSON document (text/string)\n>>\n>> builder = Builder(builder_json)\n>> form = Form(builder, form_json)\n\n##################\n# input components\n##################\n\n# textfield label\n>> print(form.input_components[\'firstname\'].label)\n\'First Name\'\n\n# textfield value\n>> print(form.input_components[\'firstname\'].value)\n\'Bob\'\n\n# datetime label\n>> print(form.input_components[\'birthday\'].label)\n\'Birthday\'\n\n# datetime value\n>> print(form.input_components[\'birthday\'].value)\ndatetime.date(2009 10 16)\n\n# datagrid (rows property)\n>> print(form.input_components[\'datagridMeasurements\'].rows)\n[\n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}, \n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}\n]\n\n>> for row in form.input_components[\'datagridMeasurements\'].rows:\n>>    dtime = row[\'measurementDatetime\']\n>>    fahrenheit = row[\'measurementFahrenheit\']\n>>    print(%s: %s, %s: %s\' % (dt.label, dt.value, fahrenheit.label, fahrenheit.value))\n\nDatetime: datetime.datetime(2021, 5, 8, 11, 39, 0, 296487), Fahrenheit: 122\nDatetime: datetime.datetime(2021, 5, 8, 11, 41, 5, 919943), Fahrenheit: 131\n\n# alternative example, by getattr\n>> print(form.data.firstname.label)\n\'First Name\'\n\n>> print(form.data.firstname.value)\n\'Bob\'\n\n#################################\n# components (layout, input etc.)\n#################################\n\n# columns\n>> print(form.components[\'addressColumns\'])\n<columnsComponent>\n\n>> print(form.components[\'addressColumns\'].rows)\n[ \n  {\'firstName\': <textfieldComponent>, \'lastName: <textfieldComponent>}, \n  {\'email\': <emailComponent>, \'companyName: <textfieldComponent>}\n]\n```\n\n## Unit tests\n\n**Note:**\n\nInternet access is recommended for running the `filecStorageUrlComponentTestCase`, because this also tests the URL Storage (type).\\\nIf no internet access, this test won\'t fail and a WARNING shall be logged regarding a ConnectionError.\n\n### Run all unittests\n\nFrom toplevel directory:\n\n```\npoetry install -E json_logic  # if you haven\'t already\npoetry run python -m unittest\n```\n\n### Run component unittests\n\nAll Components, from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_component_*.py\n```\n\nNested components (complexity), from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_nested_components.py\n```\n\n### Run specific component unittest\n\n```\npoetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear\n```\n',
     'author': 'Bob Leers',
     'author_email': 'bob@novacode.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/novacode-nl/python-formio-data',
```

### Comparing `formio-data-0.4.8/PKG-INFO` & `formio-data-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formio-data
-Version: 0.4.8
+Version: 0.4.9
 Summary: formio.js JSON-data API
 Home-page: https://github.com/novacode-nl/python-formio-data
 License: MIT
 Author: Bob Leers
 Author-email: bob@novacode.nl
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

