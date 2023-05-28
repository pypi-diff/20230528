# Comparing `tmp/auptitcafe-0.1.8.tar.gz` & `tmp/auptitcafe-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auptitcafe-0.1.8.tar", max compression
+gzip compressed data, was "auptitcafe-0.1.9.tar", max compression
```

## Comparing `auptitcafe-0.1.8.tar` & `auptitcafe-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1617 2023-05-21 22:23:53.020362 auptitcafe-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-21 22:24:30.480749 auptitcafe-0.1.8/auptitcafe/__init__.py
--rw-r--r--   0        0        0     2755 2023-05-21 22:23:53.020362 auptitcafe-0.1.8/auptitcafe/menus.py
--rw-r--r--   0        0        0      503 2023-05-21 22:23:53.020362 auptitcafe-0.1.8/auptitcafe/plat.py
--rw-r--r--   0        0        0      443 2023-05-21 22:23:53.020362 auptitcafe-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 auptitcafe-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1779 2023-05-28 02:24:25.422070 auptitcafe-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 02:25:06.106787 auptitcafe-0.1.9/auptitcafe/__init__.py
+-rw-r--r--   0        0        0     2832 2023-05-28 02:24:25.422070 auptitcafe-0.1.9/auptitcafe/menus.py
+-rw-r--r--   0        0        0      503 2023-05-28 02:24:25.422070 auptitcafe-0.1.9/auptitcafe/plat.py
+-rw-r--r--   0        0        0      443 2023-05-28 02:24:25.422070 auptitcafe-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 auptitcafe-0.1.9/PKG-INFO
```

### Comparing `auptitcafe-0.1.8/README.md` & `auptitcafe-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 ![PyPI - Format](https://img.shields.io/pypi/format/auptitcafe)
 ![PyPI](https://img.shields.io/pypi/v/auptitcafe)
 
 # ❔ About
 
 > Finally a Python package to make **getting Au p'it café's menus a piece of (cheese) cake.😅**
 
-# 🔖 Resources
+# 🔖 Social networks
 
 - [Official website](http://auptitcafe.nc/)
 - [TripAdvisor](https://www.tripadvisor.com/Restaurant_Review-g294130-d1952994-Reviews-Au_P_tit_Cafe-Noumea_Grand_Terre.html)
-- [`pypi`](https://pypi.org/project/auptitcafe/)
 - [Instagram](https://www.instagram.com/auptitcafe.nc/?hl=en) 
 - [Facebook](https://www.facebook.com/auptitcafe.nc/)
 - [Google Maps](https://goo.gl/maps/4UcxegSnxMsE8qKs8)
 
 [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/iRSInif_Zwc/0.jpg)](https://www.youtube.com/watch?v=iRSInif_Zwc)
 
+# 🤓 Nerd resources
+
+- [🐍 `pypi`](https://pypi.org/project/auptitcafe/)
+- [😋 Au p'tit café (pypi package intro on Kaggle) 🚀](https://www.kaggle.com/adriensales/au-p-tit-caf-pypi-package-intro)
 
 # 🚀 Quickstart
 
 For the impatients, here is a quick and ready to use code snippet:
 
 ```python
 # Install the package
```

### Comparing `auptitcafe-0.1.8/auptitcafe/menus.py` & `auptitcafe-0.1.9/auptitcafe/menus.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,16 @@
                 image = menu.find('img')['src']
             else:
                 image = ""
             # Get the details fo the receipe
             recette = menu.find('div', class_='contact_descriptions').text.strip()
             #print('name : <' + name + '>')
             titre_plat = name.split("-")[0].strip()
+            titre_plat = re.sub(r'\s+\d+\s*F$', '', titre_plat)
+            
             #print('Titre plat : <' + titre_plat + '>')
             #print('url image : <' + image + '>')
             #print('recette : <' + recette + '>')
             #image_url = menu.find('img')['src']
             #print(name + " : " + image_url)
             numbers = [int(s) for s in re.findall(r'\d+\.\d+|\d+', name)]
             #print('Prix : <' + str(numbers[0]) + '>')
```

### Comparing `auptitcafe-0.1.8/PKG-INFO` & `auptitcafe-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auptitcafe
-Version: 0.1.8
+Version: 0.1.9
 Summary: SDK pour interagir avec http://auptitcafe.nc/menu/
 Author: Adrien SALES
 Author-email: Adrien.Sales@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,25 +18,28 @@
 ![PyPI - Format](https://img.shields.io/pypi/format/auptitcafe)
 ![PyPI](https://img.shields.io/pypi/v/auptitcafe)
 
 # ❔ About
 
 > Finally a Python package to make **getting Au p'it café's menus a piece of (cheese) cake.😅**
 
-# 🔖 Resources
+# 🔖 Social networks
 
 - [Official website](http://auptitcafe.nc/)
 - [TripAdvisor](https://www.tripadvisor.com/Restaurant_Review-g294130-d1952994-Reviews-Au_P_tit_Cafe-Noumea_Grand_Terre.html)
-- [`pypi`](https://pypi.org/project/auptitcafe/)
 - [Instagram](https://www.instagram.com/auptitcafe.nc/?hl=en) 
 - [Facebook](https://www.facebook.com/auptitcafe.nc/)
 - [Google Maps](https://goo.gl/maps/4UcxegSnxMsE8qKs8)
 
 [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/iRSInif_Zwc/0.jpg)](https://www.youtube.com/watch?v=iRSInif_Zwc)
 
+# 🤓 Nerd resources
+
+- [🐍 `pypi`](https://pypi.org/project/auptitcafe/)
+- [😋 Au p'tit café (pypi package intro on Kaggle) 🚀](https://www.kaggle.com/adriensales/au-p-tit-caf-pypi-package-intro)
 
 # 🚀 Quickstart
 
 For the impatients, here is a quick and ready to use code snippet:
 
 ```python
 # Install the package
```

