# Comparing `tmp/mosek_license_server-0.2.0.tar.gz` & `tmp/mosek_license_server-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosek_license_server-0.2.0.tar", max compression
+gzip compressed data, was "mosek_license_server-0.5.1.tar", max compression
```

## Comparing `mosek_license_server-0.2.0.tar` & `mosek_license_server-0.5.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-28 04:30:34.134549 mosek_license_server-0.2.0/mosek_license/__init__.py
--rw-r--r--   0        0        0      499 2023-05-28 04:30:34.134549 mosek_license_server-0.2.0/mosek_license/license.py
--rw-r--r--   0        0        0      519 2023-05-28 04:30:51.938882 mosek_license_server-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2362 2023-05-28 04:30:34.134549 mosek_license_server-0.2.0/readme.md
--rw-r--r--   0        0        0     3043 1970-01-01 00:00:00.000000 mosek_license_server-0.2.0/setup.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 mosek_license_server-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-28 05:36:24.382351 mosek_license_server-0.5.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-28 05:36:24.382351 mosek_license_server-0.5.1/mosek_license/__init__.py
+-rw-r--r--   0        0        0      499 2023-05-28 05:36:24.382351 mosek_license_server-0.5.1/mosek_license/license.py
+-rw-r--r--   0        0        0      520 2023-05-28 05:36:42.690482 mosek_license_server-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2389 2023-05-28 05:36:24.386351 mosek_license_server-0.5.1/readme.md
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 mosek_license_server-0.5.1/setup.py
+-rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 mosek_license_server-0.5.1/PKG-INFO
```

### Comparing `mosek_license_server-0.2.0/pyproject.toml` & `mosek_license_server-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosek-license-server"
-version = "0.2.0"
+version = "v0.5.1"
 description = "Expose a mosek license via a nginx server"
 authors = ["Thomas Schmelzer <thomas.schmelzer@gmail.com>"]
 license = "Apache 2.0"
 readme = "readme.md"
 repository = "https://github.com/tschm/mosek-license-server"
 packages = [{include = "mosek_license"}]
```

### Comparing `mosek_license_server-0.2.0/readme.md` & `mosek_license_server-0.5.1/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 license file in the underlying repositories.
 
 This repository serves two purposes. It exposes the server but it is also the home
 for a little Python package to inject the license into your programs.
 
 We solve a common problem here. Assume $20$ researchers work on $50$ different strategies.
 Using local copies of the same license file is a tedious exercise as
-he file needs to get updated once a year.
+the file needs to get updated once a year.
 Rather, each strategy would connect to the server to fetch a license using the mosek_license
 Python package. Once the strategy expires we only need to update the server.
 No change for the strategies is required.
 
 ## License server
 
 ### Copy your license file into folder
 
-Copy the license file you have received (from Mosek) into the license folder.
-Name it `mosek'.
+Copy the license file you have received (from Mosek) into the `web` folder.
+Name it `mosek`.
 
 The file should look like
 
 ```bash
 START_LICENSE
 VENDOR MOSEKLM
 # PSN-4183
@@ -36,19 +36,19 @@
 # PSN-4182
 FEATURE PTON MOSEKLM 10 31-jan-2024 uncounted ...
 END_LICENSE
 ```
 
 ### Start the nginx server
 
-Share the license folder (after you have copied your personal Mosek license into)
+Share the web folder (after you have copied your personal Mosek license into)
 via
 
 ```bash
-docker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx
+docker run --name mosek -v $PWD/web:/usr/share/nginx/html:ro -p 8080:80 -d nginx
 ```
 
 The license will now be exposed via `http://localhost:8080/mosek`
 
 As an alternative you can run the script
 
 ```bash
@@ -65,12 +65,12 @@
 
 and then
 
 ```python
 from mosek_license import license
 
 # It's important to upsert the license before you import mosek
-license.upsert()
+license.upsert(server="http://localhost:8080/mosek")
 
 # only now import mosek
 import mosek
 ```
```

### Comparing `mosek_license_server-0.2.0/setup.py` & `mosek_license_server-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['mosek_license']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mosek-license-server',
-    'version': '0.2.0',
+    'version': '0.5.1',
     'description': 'Expose a mosek license via a nginx server',
-    'long_description': "# Mosek License Server\n\n[![Linting](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml/badge.svg)](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml)\n[![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)\n[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)\n[![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)\n\nUsing a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license\non a server to be accessible from various research machines without sharing the actual\nlicense file in the underlying repositories.\n\nThis repository serves two purposes. It exposes the server but it is also the home\nfor a little Python package to inject the license into your programs.\n\nWe solve a common problem here. Assume $20$ researchers work on $50$ different strategies.\nUsing local copies of the same license file is a tedious exercise as\nhe file needs to get updated once a year.\nRather, each strategy would connect to the server to fetch a license using the mosek_license\nPython package. Once the strategy expires we only need to update the server.\nNo change for the strategies is required.\n\n## License server\n\n### Copy your license file into folder\n\nCopy the license file you have received (from Mosek) into the license folder.\nName it `mosek'.\n\nThe file should look like\n\n```bash\nSTART_LICENSE\nVENDOR MOSEKLM\n# PSN-4183\nFEATURE PTS MOSEKLM 10 31-jan-2024 uncounted ...\n# PSN-4182\nFEATURE PTON MOSEKLM 10 31-jan-2024 uncounted ...\nEND_LICENSE\n```\n\n### Start the nginx server\n\nShare the license folder (after you have copied your personal Mosek license into)\nvia\n\n```bash\ndocker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx\n```\n\nThe license will now be exposed via `http://localhost:8080/mosek`\n\nAs an alternative you can run the script\n\n```bash\n./start_server.sh\n```\n\n## The mosek_license module\n\nInstall via\n\n```bash\npip install mosek-license-server\n```\n\nand then\n\n```python\nfrom mosek_license import license\n\n# It's important to upsert the license before you import mosek\nlicense.upsert()\n\n# only now import mosek\nimport mosek\n```\n",
+    'long_description': '# Mosek License Server\n\n[![Linting](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml/badge.svg)](https://github.com/tschm/mosek-license-server/actions/workflows/linting.yml)\n[![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)\n[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)\n[![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)\n\nUsing a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license\non a server to be accessible from various research machines without sharing the actual\nlicense file in the underlying repositories.\n\nThis repository serves two purposes. It exposes the server but it is also the home\nfor a little Python package to inject the license into your programs.\n\nWe solve a common problem here. Assume $20$ researchers work on $50$ different strategies.\nUsing local copies of the same license file is a tedious exercise as\nthe file needs to get updated once a year.\nRather, each strategy would connect to the server to fetch a license using the mosek_license\nPython package. Once the strategy expires we only need to update the server.\nNo change for the strategies is required.\n\n## License server\n\n### Copy your license file into folder\n\nCopy the license file you have received (from Mosek) into the `web` folder.\nName it `mosek`.\n\nThe file should look like\n\n```bash\nSTART_LICENSE\nVENDOR MOSEKLM\n# PSN-4183\nFEATURE PTS MOSEKLM 10 31-jan-2024 uncounted ...\n# PSN-4182\nFEATURE PTON MOSEKLM 10 31-jan-2024 uncounted ...\nEND_LICENSE\n```\n\n### Start the nginx server\n\nShare the web folder (after you have copied your personal Mosek license into)\nvia\n\n```bash\ndocker run --name mosek -v $PWD/web:/usr/share/nginx/html:ro -p 8080:80 -d nginx\n```\n\nThe license will now be exposed via `http://localhost:8080/mosek`\n\nAs an alternative you can run the script\n\n```bash\n./start_server.sh\n```\n\n## The mosek_license module\n\nInstall via\n\n```bash\npip install mosek-license-server\n```\n\nand then\n\n```python\nfrom mosek_license import license\n\n# It\'s important to upsert the license before you import mosek\nlicense.upsert(server="http://localhost:8080/mosek")\n\n# only now import mosek\nimport mosek\n```\n',
     'author': 'Thomas Schmelzer',
     'author_email': 'thomas.schmelzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tschm/mosek-license-server',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mosek_license_server-0.2.0/PKG-INFO` & `mosek_license_server-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosek-license-server
-Version: 0.2.0
+Version: 0.5.1
 Summary: Expose a mosek license via a nginx server
 Home-page: https://github.com/tschm/mosek-license-server
 License: Apache 2.0
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
@@ -27,25 +27,25 @@
 license file in the underlying repositories.
 
 This repository serves two purposes. It exposes the server but it is also the home
 for a little Python package to inject the license into your programs.
 
 We solve a common problem here. Assume $20$ researchers work on $50$ different strategies.
 Using local copies of the same license file is a tedious exercise as
-he file needs to get updated once a year.
+the file needs to get updated once a year.
 Rather, each strategy would connect to the server to fetch a license using the mosek_license
 Python package. Once the strategy expires we only need to update the server.
 No change for the strategies is required.
 
 ## License server
 
 ### Copy your license file into folder
 
-Copy the license file you have received (from Mosek) into the license folder.
-Name it `mosek'.
+Copy the license file you have received (from Mosek) into the `web` folder.
+Name it `mosek`.
 
 The file should look like
 
 ```bash
 START_LICENSE
 VENDOR MOSEKLM
 # PSN-4183
@@ -53,19 +53,19 @@
 # PSN-4182
 FEATURE PTON MOSEKLM 10 31-jan-2024 uncounted ...
 END_LICENSE
 ```
 
 ### Start the nginx server
 
-Share the license folder (after you have copied your personal Mosek license into)
+Share the web folder (after you have copied your personal Mosek license into)
 via
 
 ```bash
-docker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx
+docker run --name mosek -v $PWD/web:/usr/share/nginx/html:ro -p 8080:80 -d nginx
 ```
 
 The license will now be exposed via `http://localhost:8080/mosek`
 
 As an alternative you can run the script
 
 ```bash
@@ -82,13 +82,13 @@
 
 and then
 
 ```python
 from mosek_license import license
 
 # It's important to upsert the license before you import mosek
-license.upsert()
+license.upsert(server="http://localhost:8080/mosek")
 
 # only now import mosek
 import mosek
 ```
```

