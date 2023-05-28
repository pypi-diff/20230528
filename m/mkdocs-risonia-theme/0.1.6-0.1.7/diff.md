# Comparing `tmp/mkdocs-risonia-theme-0.1.6.tar.gz` & `tmp/mkdocs-risonia-theme-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-risonia-theme-0.1.6.tar", last modified: Thu Apr 13 14:42:33 2023, max compression
+gzip compressed data, was "mkdocs-risonia-theme-0.1.7.tar", last modified: Sun May 28 20:47:07 2023, max compression
```

## Comparing `mkdocs-risonia-theme-0.1.6.tar` & `mkdocs-risonia-theme-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.648480 mkdocs-risonia-theme-0.1.6/
--rw-rw-rw-   0        0        0     2361 2022-09-13 18:26:48.000000 mkdocs-risonia-theme-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      167 2022-11-20 18:59:01.000000 mkdocs-risonia-theme-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6653 2023-04-13 14:42:33.648480 mkdocs-risonia-theme-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4832 2023-01-21 09:48:23.000000 mkdocs-risonia-theme-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.634475 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/
--rw-rw-rw-   0        0        0     6653 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      882 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      212 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-20 18:56:22.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.638480 mkdocs-risonia-theme-0.1.6/risonia_theme/
--rw-rw-rw-   0        0        0      118 2022-10-16 15:57:02.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/404.html
--rw-rw-rw-   0        0        0        0 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/__init__.py
--rw-rw-rw-   0        0        0    20666 2023-04-13 14:34:04.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/base.html
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.641481 mkdocs-risonia-theme-0.1.6/risonia_theme/css/
--rw-rw-rw-   0        0        0     1171 2023-04-13 14:07:49.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/theme.css
--rw-rw-rw-   0        0        0     1787 2022-11-24 18:22:21.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme-dark.css
--rw-rw-rw-   0        0        0     1787 2022-11-24 18:22:26.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme-light.css
--rw-rw-rw-   0        0        0     3872 2023-04-13 13:34:56.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme.css
--rw-rw-rw-   0        0        0    23427 2022-05-04 16:10:46.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3.css
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.642481 mkdocs-risonia-theme-0.1.6/risonia_theme/img/
--rw-rw-rw-   0        0        0     7406 2022-11-20 17:26:30.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/img/favicon.ico
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.643478 mkdocs-risonia-theme-0.1.6/risonia_theme/js/
--rw-rw-rw-   0        0        0     2246 2022-11-25 18:35:17.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/js/theme.js
--rw-rw-rw-   0        0        0       25 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/main.html
--rw-rw-rw-   0        0        0      133 2023-04-13 14:33:26.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/mkdocs_theme.yml
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.645480 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/
--rw-rw-rw-   0        0        0        0 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.646480 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/classes/
--rw-rw-rw-   0        0        0        0 2020-03-27 04:57:31.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/classes/__init__.py
--rw-rw-rw-   0        0        0     2759 2022-12-04 19:21:29.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/classes/plugin.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.647478 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/color/
--rw-rw-rw-   0        0        0        0 2020-03-27 04:57:31.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/color/__init__.py
--rw-rw-rw-   0        0        0    14004 2022-12-11 12:05:50.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/color/plugin.py
--rw-rw-rw-   0        0        0       42 2023-04-13 14:42:33.649483 mkdocs-risonia-theme-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1197 2023-01-21 09:48:12.000000 mkdocs-risonia-theme-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.051741 mkdocs-risonia-theme-0.1.7/
+-rw-rw-rw-   0        0        0     2361 2022-09-13 18:26:48.000000 mkdocs-risonia-theme-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      167 2022-11-20 18:59:01.000000 mkdocs-risonia-theme-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6749 2023-05-28 20:47:07.051741 mkdocs-risonia-theme-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4919 2023-04-13 15:09:02.000000 mkdocs-risonia-theme-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.034741 mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/
+-rw-rw-rw-   0        0        0     6749 2023-05-28 20:47:06.000000 mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      882 2023-05-28 20:47:06.000000 mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 20:47:06.000000 mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      212 2023-05-28 20:47:06.000000 mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-20 18:56:22.000000 mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2023-05-28 20:47:06.000000 mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-28 20:47:06.000000 mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.038741 mkdocs-risonia-theme-0.1.7/risonia_theme/
+-rw-rw-rw-   0        0        0      118 2022-10-16 15:57:02.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/404.html
+-rw-rw-rw-   0        0        0        0 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/__init__.py
+-rw-rw-rw-   0        0        0    20681 2023-04-13 15:09:52.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/base.html
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.043741 mkdocs-risonia-theme-0.1.7/risonia_theme/css/
+-rw-rw-rw-   0        0        0     1171 2023-04-13 14:07:49.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/css/theme.css
+-rw-rw-rw-   0        0        0     1787 2022-11-24 18:22:21.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/css/w3-theme-dark.css
+-rw-rw-rw-   0        0        0     1787 2022-11-24 18:22:26.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/css/w3-theme-light.css
+-rw-rw-rw-   0        0        0     3872 2023-04-13 13:34:56.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/css/w3-theme.css
+-rw-rw-rw-   0        0        0    23427 2022-05-04 16:10:46.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/css/w3.css
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.044741 mkdocs-risonia-theme-0.1.7/risonia_theme/img/
+-rw-rw-rw-   0        0        0     7406 2022-11-20 17:26:30.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/img/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.045741 mkdocs-risonia-theme-0.1.7/risonia_theme/js/
+-rw-rw-rw-   0        0        0     2246 2022-11-25 18:35:17.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/js/theme.js
+-rw-rw-rw-   0        0        0       25 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/main.html
+-rw-rw-rw-   0        0        0      133 2023-04-13 14:33:26.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/mkdocs_theme.yml
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.047740 mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/
+-rw-rw-rw-   0        0        0        0 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.048740 mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/classes/
+-rw-rw-rw-   0        0        0        0 2020-03-27 04:57:31.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/classes/__init__.py
+-rw-rw-rw-   0        0        0     2799 2023-05-28 20:41:40.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/classes/plugin.py
+drwxrwxrwx   0        0        0        0 2023-05-28 20:47:07.050742 mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/color/
+-rw-rw-rw-   0        0        0        0 2020-03-27 04:57:31.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/color/__init__.py
+-rw-rw-rw-   0        0        0    14004 2022-12-11 12:05:50.000000 mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/color/plugin.py
+-rw-rw-rw-   0        0        0       42 2023-05-28 20:47:07.051741 mkdocs-risonia-theme-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-04-13 15:09:03.000000 mkdocs-risonia-theme-0.1.7/setup.py
```

### Comparing `mkdocs-risonia-theme-0.1.6/LICENSE` & `mkdocs-risonia-theme-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/PKG-INFO` & `mkdocs-risonia-theme-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-risonia-theme
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple theme for MkDocs using using the w3.css framework and configurable color schemes
 Home-page: https://github.com/unverbuggt/mkdocs-risonia-theme
 Author: René Rüthlein
 License: MIT
 Description: # mkdocs-risonia-theme
         
         [![PyPI Version](https://img.shields.io/pypi/v/mkdocs-risonia-theme.svg)](https://pypi.org/project/mkdocs-risonia-theme/)
@@ -56,15 +56,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-risonia-theme/
         python setup.py sdist bdist_wheel
-        pip install dist/mkdocs_risonia_theme-0.1.6-py3-none-any.whl
+        pip install dist/mkdocs_risonia_theme-0.1.7-py3-none-any.whl
         ```
         
         ## Configuration
         
         Enable the theme and plugins in your `mkdocs.yml`:
         
         ```yaml
@@ -73,14 +73,15 @@
             #custom_dir: theme_override/ # add static files or overrides
             #logo: img/logo.svg # if undefined a burger symbol is displayed on mobile devices
             #favicon: img/logo.ico # if undefined img/favicon.ico is used
             #manifest: manifest.json # manifest for installable webapp
             #serviceworker: service-worker.js # for webapp an empty file is sufficient
             #extlink: true # mark external links with symbol
             #extblank: true # send external links to new browser tab
+            #toc_sidebar: true # If display is wide enough, then display TOC on the right side
             
         plugins:
             - search: {}
         
             #- i18n: {...} # mkdocs-static-i18n
         
             - color-theme: # optional
```

### Comparing `mkdocs-risonia-theme-0.1.6/README.md` & `mkdocs-risonia-theme-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ```
 
 Install the package from source with pip:
 
 ```bash
 cd mkdocs-risonia-theme/
 python setup.py sdist bdist_wheel
-pip install dist/mkdocs_risonia_theme-0.1.6-py3-none-any.whl
+pip install dist/mkdocs_risonia_theme-0.1.7-py3-none-any.whl
 ```
 
 ## Configuration
 
 Enable the theme and plugins in your `mkdocs.yml`:
 
 ```yaml
@@ -66,14 +66,15 @@
     #custom_dir: theme_override/ # add static files or overrides
     #logo: img/logo.svg # if undefined a burger symbol is displayed on mobile devices
     #favicon: img/logo.ico # if undefined img/favicon.ico is used
     #manifest: manifest.json # manifest for installable webapp
     #serviceworker: service-worker.js # for webapp an empty file is sufficient
     #extlink: true # mark external links with symbol
     #extblank: true # send external links to new browser tab
+    #toc_sidebar: true # If display is wide enough, then display TOC on the right side
     
 plugins:
     - search: {}
 
     #- i18n: {...} # mkdocs-static-i18n
 
     - color-theme: # optional
```

### Comparing `mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/PKG-INFO` & `mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-risonia-theme
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple theme for MkDocs using using the w3.css framework and configurable color schemes
 Home-page: https://github.com/unverbuggt/mkdocs-risonia-theme
 Author: René Rüthlein
 License: MIT
 Description: # mkdocs-risonia-theme
         
         [![PyPI Version](https://img.shields.io/pypi/v/mkdocs-risonia-theme.svg)](https://pypi.org/project/mkdocs-risonia-theme/)
@@ -56,15 +56,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-risonia-theme/
         python setup.py sdist bdist_wheel
-        pip install dist/mkdocs_risonia_theme-0.1.6-py3-none-any.whl
+        pip install dist/mkdocs_risonia_theme-0.1.7-py3-none-any.whl
         ```
         
         ## Configuration
         
         Enable the theme and plugins in your `mkdocs.yml`:
         
         ```yaml
@@ -73,14 +73,15 @@
             #custom_dir: theme_override/ # add static files or overrides
             #logo: img/logo.svg # if undefined a burger symbol is displayed on mobile devices
             #favicon: img/logo.ico # if undefined img/favicon.ico is used
             #manifest: manifest.json # manifest for installable webapp
             #serviceworker: service-worker.js # for webapp an empty file is sufficient
             #extlink: true # mark external links with symbol
             #extblank: true # send external links to new browser tab
+            #toc_sidebar: true # If display is wide enough, then display TOC on the right side
             
         plugins:
             - search: {}
         
             #- i18n: {...} # mkdocs-static-i18n
         
             - color-theme: # optional
```

### Comparing `mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/SOURCES.txt` & `mkdocs-risonia-theme-0.1.7/mkdocs_risonia_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/base.html` & `mkdocs-risonia-theme-0.1.7/risonia_theme/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     {%- endfor %}
   {%- endfor %}
   </div>
   <div class="w3-container w3-large" style="height: 8em;" >&nbsp;</div>
 </nav>
 {%- endif %}
 
-<div class="w3-main{% if config.theme.toc_sidebar %}-custom{% endif %}" style="margin-left:300px;{% if toc_check.anchors > 1 and config.theme.toc_sidebar %} margin-right:300px;{% endif %}">
+<div id="main-view" class="w3-main{% if config.theme.toc_sidebar %}-custom{% endif %}" style="margin-left:300px;{% if toc_check.anchors > 1 and config.theme.toc_sidebar %} margin-right:300px;{% endif %}">
 
 <div class="w3-container" style="padding: 32px;">
   <div class="w3-right w3-margin-bottom no-print">
   {%- if toc_check.anchors > 1 %}
     <div class="w3-dropdown-hover{% if config.theme.toc_sidebar %} w3-hide-large{% endif %}" id="myTocButton" style="z-index:1;">
       <button class="w3-button w3-hover-theme w3-theme-l3 w3-hover-theme"><svg class="svg-1em"><use xlink:href="#toc" /></svg></button>
       <div class="w3-dropdown-content w3-bar-block" style="right:0;">
```

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/css/theme.css` & `mkdocs-risonia-theme-0.1.7/risonia_theme/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme-dark.css` & `mkdocs-risonia-theme-0.1.7/risonia_theme/css/w3-theme-dark.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme-light.css` & `mkdocs-risonia-theme-0.1.7/risonia_theme/css/w3-theme-light.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme.css` & `mkdocs-risonia-theme-0.1.7/risonia_theme/css/w3-theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3.css` & `mkdocs-risonia-theme-0.1.7/risonia_theme/css/w3.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/img/favicon.ico` & `mkdocs-risonia-theme-0.1.7/risonia_theme/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/js/theme.js` & `mkdocs-risonia-theme-0.1.7/risonia_theme/js/theme.js`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/classes/plugin.py` & `mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/classes/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,12 +52,13 @@
                 svg_tag.append(svg_extlink)
                 if href.startswith('http://') or href.startswith('https://'):
                     link_tag.append(svg_tag)
         
         #send external links to new tab?
         if 'extblank' in config['theme']._vars and config['theme']._vars['extblank']:
             for link_tag in soup.find_all('a'):
+                href = link_tag['href']
                 if href.startswith('http://') or href.startswith('https://'):
                     if not 'target' in link_tag:
                         link_tag['target'] = '_blank'
         
         return str(soup)
```

### Comparing `mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/color/plugin.py` & `mkdocs-risonia-theme-0.1.7/risonia_theme/plugins/color/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.6/setup.py` & `mkdocs-risonia-theme-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     with open(file_path) as file:
         content = file.read()
     return content if content else 'no content read'
```

