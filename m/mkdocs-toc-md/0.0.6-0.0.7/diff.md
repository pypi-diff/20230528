# Comparing `tmp/mkdocs-toc-md-0.0.6.tar.gz` & `tmp/mkdocs-toc-md-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-toc-md-0.0.6.tar", last modified: Sat May 20 11:55:37 2023, max compression
+gzip compressed data, was "mkdocs-toc-md-0.0.7.tar", last modified: Sun May 28 09:49:19 2023, max compression
```

## Comparing `mkdocs-toc-md-0.0.6.tar` & `mkdocs-toc-md-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-20 11:55:37.583474 mkdocs-toc-md-0.0.6/
--rwxrwxrwx   0 root         (0) root         (0)     1081 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       36 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.6/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     4353 2023-05-20 11:55:37.579475 mkdocs-toc-md-0.0.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3772 2023-05-20 11:30:58.000000 mkdocs-toc-md-0.0.6/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-20 11:55:37.365503 mkdocs-toc-md-0.0.6/mkdocs_toc_md/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11355 2023-05-20 10:34:12.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md/plugin.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-20 11:55:37.552470 mkdocs-toc-md-0.0.6/mkdocs_toc_md/template/
--rwxrwxrwx   0 root         (0) root         (0)      382 2023-04-09 12:50:24.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md/template/toc.md.j2
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-20 11:55:37.524472 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     4353 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      345 2023-05-20 11:55:37.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-05-20 11:55:36.000000 mkdocs-toc-md-0.0.6/mkdocs_toc_md.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-20 11:55:37.585476 mkdocs-toc-md-0.0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1300 2023-05-20 10:34:12.000000 mkdocs-toc-md-0.0.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 09:49:19.316244 mkdocs-toc-md-0.0.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1081 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       36 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.7/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     6610 2023-05-28 09:49:19.311237 mkdocs-toc-md-0.0.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6140 2023-05-28 08:31:10.000000 mkdocs-toc-md-0.0.7/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 09:49:19.101448 mkdocs-toc-md-0.0.7/mkdocs_toc_md/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-09 13:34:46.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2527 2023-05-28 06:03:42.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/hook.py
+-rwxrwxrwx   0 root         (0) root         (0)     2350 2023-05-28 07:35:59.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/objects.py
+-rwxrwxrwx   0 root         (0) root         (0)    12621 2023-05-28 09:34:39.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/plugin.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 09:49:19.284231 mkdocs-toc-md-0.0.7/mkdocs_toc_md/template/
+-rwxrwxrwx   0 root         (0) root         (0)      382 2023-04-09 12:50:24.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md/template/toc.md.j2
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 09:49:19.250235 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     6610 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      392 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-05-28 09:49:18.000000 mkdocs-toc-md-0.0.7/mkdocs_toc_md.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-28 09:49:19.317236 mkdocs-toc-md-0.0.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1300 2023-05-28 09:41:53.000000 mkdocs-toc-md-0.0.7/setup.py
```

### Comparing `mkdocs-toc-md-0.0.6/LICENSE` & `mkdocs-toc-md-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-toc-md-0.0.6/mkdocs_toc_md/plugin.py` & `mkdocs-toc-md-0.0.7/mkdocs_toc_md/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,81 +1,28 @@
+from pathlib import Path
 import sys
 import logging
 import os
 import re
 from mkdocs import plugins
 from mkdocs.plugins import BasePlugin
 from mkdocs.config import config_options
+from mkdocs.structure.pages import Page
+from mkdocs.structure.nav import Navigation
+from mkdocs_toc_md.objects import TocConfig, TocItem, TocPageData
+from mkdocs_toc_md.hook import TocExtendModule
 from bs4 import BeautifulSoup
 from jinja2 import Environment, FileSystemLoader
 try:
     from mkdocs.plugins import event_priority
 except ImportError:
-    event_priority = lambda priority: lambda f: f  # No-op fallback
+    def event_priority(priority): return lambda f: f  # No-op fallback
 
-logging.getLogger(__name__)
-
-
-class TocPageData:
-    """ Page params """
-    toc_output_comment = None
-    page_title = None
-    page_description = None
-    toc_headers = []
-
-class TocItem:
-    """ headers """
-    src_level = 1
-    text  = None
-    description = None
-    url = None
-    parent = None
-    children = []
-
-
-    def get_md_header_prefix(self) -> str:
-        """ Gets level as markdown header. """
-
-        prefix = '#'
-        for num in range(self.src_level):
-            prefix += '#'
-        return prefix
-
-
-    def get_text_as_md_header(self) -> str:
-        """ Gets text as markdown header. """
-
-        prefix = self.get_md_header_prefix()
-
-        if self.url:
-            return prefix + ' [' + self.text + '](' + self.url + ')'
-
-        return prefix + ' ' + self.text
-        
-
-    def get_text_as_md_ul_item(self) -> str:
-        """ Gets text as markdown list item. """
-
-        if self.url:
-            return '* [' + self.text + '](' + self.url + ')'
-        
-        return '* ' + self.text
-
-
-    def get_text_as_md_ol_item(self) -> str:
-        """ Gets text as markdown ordered list item. """
-
-        if self.url:
-            return '1. [' + self.text + '](' + self.url + ')'
-        
-        return '1. ' + self.text
-
-    def has_description(self) -> bool:
-        return self.description is not None 
 
+logging.getLogger(__name__)
 
 
 class TocMdPlugin(BasePlugin):
 
     config_scheme = (
         ('pickup_description_meta', config_options.Type(bool, default=False)),
         ('pickup_description_class', config_options.Type(bool, default=False)),
@@ -86,79 +33,79 @@
         ('toc_page_title', config_options.Type(str, default='Contents')),
         ('toc_page_description', config_options.Type(str, default=None)),
         ('header_level', config_options.Type(int, default=3)),
         ('template_dir_path', config_options.Type(str, default=None)),
         ('beautiful_soup_parser', config_options.Type(str, default='html.parser')),
         ('languages', config_options.Type(dict, default=dict())),
         ('integrate_mkdocs_static_i18n', config_options.Type(bool, default=False)),
+        ('extend_module', config_options.Type(bool, default=False)),
+        ('shift_header', config_options.Type(str, default='none')),
+        ('output_comment', config_options.Type(str, default='html')),
     )
 
-
     def __init__(self):
         self.logger = logging.getLogger('mkdocs.toc-md')
         self.logger.setLevel(logging.INFO)
-        
-        self.toc_description_class = 'toc-md-description'
-
-        self.toc_output_comment = ''
-        self.toc_output_comment += '<!-- ====================== TOC ====================== -->\n'
-        self.toc_output_comment += '<!-- Generated by mkdocs-toc-md plugin -->\n'
-        self.toc_output_comment += '<!-- ================================================= -->\n'
-        self.toc_output_comment += '\n'
 
+        self.toc_description_class = 'toc-md-description'
         self.is_build_command = 'build' in sys.argv
 
-
     def on_pre_build(self, config):
         self.logger.info("Enabled toc-md plugin")
 
+        self.toc_config = TocConfig(config, self.config)
+
+        self.toc_output_comment = self.toc_config.get_output_comment()
 
-    def on_nav(self, nav, config, files):
-        # keep navigations
-        self.nav = nav
-      
         # mkdocs-static-i18n
         self.i18n_plugin = None
         if self.config['integrate_mkdocs_static_i18n'] and 'i18n' in config['plugins']:
             self.i18n_plugin = config['plugins']['i18n']
 
+        self.hook = TocExtendModule(self.toc_config)
+
+    def on_serve(self, server, config, builder):
+        TocExtendModule.watch_file(server, builder)
+
+    def on_nav(self, nav, config, files):
+        # keep navigations
+        self.nav = nav
 
     def on_post_page(self, output_content, page, config):
         # remove navigation items
         pattern = self.config['remove_navigation_page_pattern']
         if pattern:
             remove_navigation_page_re = re.compile(pattern)
             if remove_navigation_page_re.match(page.file.src_path):
                 self.logger.info("toc-md: Remove toc")
 
-                soup = BeautifulSoup(output_content, self.config['beautiful_soup_parser'])
+                soup = BeautifulSoup(
+                    output_content, self.config['beautiful_soup_parser'])
                 for nav_elm in soup.find_all("nav", {"class": "md-nav md-nav--secondary"}):
                     nav_elm.decompose()
-        
+
                 souped_html = soup.prettify(soup.original_encoding)
-                return souped_html 
+                return souped_html
 
         return output_content
-    
 
-    @plugins.event_priority(-100) 
+    @plugins.event_priority(-100)
     def on_post_build(self, config):
 
         ignore_file_pattern = self.config['ignore_page_pattern']
         self.ignore_re = None
         if ignore_file_pattern:
             self.ignore_re = re.compile(ignore_file_pattern)
 
         self.header_names = []
         for level in range(self.config['header_level']):
             self.header_names.append('h' + str(level + 1))
 
         self.logger.info('toc-md: Lookup ' + ', '.join(self.header_names))
 
-
         if self.i18n_plugin:
             # mkdocs-static-i18n
             # https://github.com/ultrabug/mkdocs-static-i18n
 
             for lang in self.i18n_plugin.i18n_navs:
                 use_folder = 'folder' == self.i18n_plugin.config['docs_structure']
                 nav = self.i18n_plugin.i18n_navs[lang]
@@ -168,75 +115,102 @@
                     self.output(config, nav, lang, "")
 
         else:
             # default
 
             self.output(config, self.nav, "", "")
 
-
     def output(self, config, nav, lang, folder):
 
         # Pickup headers
         toc_headers = []
         for page in nav.pages:
             if 'output_path' in self.config:
                 output_path = self.config['output_path']
                 if page.file.src_path == output_path:
                     continue
 
-            ignore = self.ignore_re and self.ignore_re.match(page.file.src_path)
+            ignore = self.ignore_re and self.ignore_re.match(
+                page.file.src_path)
             if ignore:
                 continue
 
-            soup = BeautifulSoup(page.content, self.config['beautiful_soup_parser'])
+            soup = BeautifulSoup(
+                page.content, self.config['beautiful_soup_parser'])
 
             # extract page description
             toc_description = ''
             if 'pickup_description_meta' in self.config:
                 if self.config['pickup_description_meta']:
-                    description_elm = soup.find('meta', attrs={'name':'description'})
+                    description_elm = soup.find(
+                        'meta', attrs={'name': 'description'})
                     if description_elm is not None:
                         toc_description += description_elm['content']
 
             if 'pickup_description_class' in self.config:
                 if self.config['pickup_description_class']:
-                    description_elm = soup.find(True, class_=self.toc_description_class)
+                    description_elm = soup.find(
+                        True, class_=self.toc_description_class)
                     if description_elm is not None:
                         toc_description += description_elm.text
 
             if 'toc_md_description' in page.meta:
                 toc_description += page.meta['toc_md_description']
 
             # create TocItem
-            article_headers = soup.find_all(self.header_names)
-            for h in article_headers:
-
-                toc_header = TocItem()
-                if h.find('a', attrs={'class', 'headerlink'}):
-                     h.a.extract()
-
-                toc_header.text = h.text
-                toc_header.url = page.file.src_path + '#' + h.get('id')
-
-                if h.name == 'h1':
-                    toc_header.src_level = 1
-                    if toc_description:
-                        toc_header.description = toc_description
-                elif h.name == 'h2':
-                    toc_header.src_level = 2
-                elif h.name == 'h3' :
-                    toc_header.src_level = 3
-                elif h.name == 'h4' :
-                    toc_header.src_level = 4
-                elif h.name == 'h5' :
-                    toc_header.src_level = 5
-                elif h.name == 'h6' :
-                    toc_header.src_level = 6
-
-                toc_headers.append(toc_header)
+            src_elements = []
+            if self.use_extend_module('find_src_elements'):
+                # user impl
+                src_elements = self.hook.find_src_elements(soup, page)
+            else:
+                # default
+                src_elements = soup.find_all(self.header_names)
+
+            if self.use_extend_module('create_toc_items'):
+                # user impl
+                items = self.hook.create_toc_items(
+                    page, toc_description, src_elements)
+                toc_headers.extend(items)
+            else:
+                # default
+                for elm in src_elements:
+
+                    toc_header = TocItem()
+                    if elm.find('a', attrs={'class', 'headerlink'}):
+                        elm.a.extract()
+
+                    toc_header.text = elm.text
+                    toc_header.url = page.file.src_path + '#' + elm.get('id')
+
+                    if elm.name == 'h1':
+                        toc_header.src_level = 1
+                        if toc_description:
+                            toc_header.description = toc_description
+                    elif elm.name == 'h2':
+                        toc_header.src_level = 2
+                    elif elm.name == 'h3':
+                        toc_header.src_level = 3
+                    elif elm.name == 'h4':
+                        toc_header.src_level = 4
+                    elif elm.name == 'h5':
+                        toc_header.src_level = 5
+                    elif elm.name == 'h6':
+                        toc_header.src_level = 6
+
+                    if self.config['shift_header'] and not self.config['shift_header'] == 'none':
+                        self.shift_header(toc_header, page, lang)
+
+                    if self.use_extend_module('on_create_toc_item'):
+                        # user hook
+                        self.hook.on_create_toc_item(toc_header, elm, page)
+                    toc_headers.append(toc_header)
+
+        if self.use_extend_module('on_before_output'):
+            # user hook
+            self.hook.on_before_output(nav, toc_headers)
 
         # create template arg
         template_param = TocPageData()
         template_param.page_title = self.config['toc_page_title']
         if lang in self.config['languages']:
             if 'toc_page_title' in self.config['languages'][lang]:
                 template_param.page_title = self.config['languages'][lang]['toc_page_title']
@@ -247,63 +221,91 @@
                 template_param.page_description = self.config['languages'][lang]['toc_page_description']
 
         template_param.toc_headers = toc_headers
         template_param.toc_output_comment = self.toc_output_comment
 
         self.output_md_file(config, template_param, lang, folder)
 
-
     def output_md_file(self, config, template_param, file_suffix, append_folder):
         """ Outputs markdown file. """
-        
+
         base_path = os.path.abspath(os.path.dirname(__file__))
         template_path = [os.path.join(base_path, 'template')]
 
         # using custom template
         if 'template_dir_path' in self.config:
             if self.config['template_dir_path'] and os.path.exists(self.config['template_dir_path']):
                 template_path = self.config['template_dir_path']
                 self.logger.info("toc-md: Use custom template")
 
         # render contents
         jinja_env = Environment(
-            loader = FileSystemLoader(template_path),
-            trim_blocks = True
+            loader=FileSystemLoader(template_path),
+            trim_blocks=True
         )
         template = jinja_env.get_template('toc.md.j2')
-        toc_output = template.render(data = template_param)
+        toc_output = template.render(data=template_param)
 
         # print to console
         if 'output_log' in self.config:
             if self.config['output_log']:
                 print(toc_output)
 
         # save file
         if 'output_path' in self.config:
             output_path = self.config['output_path']
             if file_suffix:
                 output_path = re.sub('md$', file_suffix + '.md', output_path)
 
             if output_path:
-                abs_md_path = os.path.join(config['docs_dir'], append_folder, output_path)
+                abs_md_path = os.path.join(
+                    config['docs_dir'], append_folder, output_path)
                 os.makedirs(os.path.dirname(abs_md_path), exist_ok=True)
 
-                 # avoid infinite loop
+                # avoid infinite loop
                 if os.path.isfile(abs_md_path):
-                     with open(abs_md_path, 'r', encoding='utf-8') as file:
+                    with open(abs_md_path, 'r', encoding='utf-8') as file:
                         old_content = file.read()
                         if old_content == toc_output:
                             self.logger.info(f'toc-md: No changes')
                             return
 
                 mode = 'x'
                 if os.path.isfile(abs_md_path):
                     mode = 'w'
-                
+
                 with open(abs_md_path, mode, encoding='utf-8') as file:
                     file.write(toc_output)
-                
-                self.logger.info(f'toc-md: Output a toc markdown file to "{abs_md_path}".')
+
+                self.logger.info(
+                    f'toc-md: Output a toc markdown file to "{abs_md_path}".')
 
                 if self.is_build_command:
-                    self.logger.warning('toc-md: Command line contains [build]. You may need to build again to render toc md as html.')
+                    self.logger.warning(
+                        'toc-md: Command line contains [build]. You may need to build again to render toc md as html.')
+
+    def use_extend_module(self, name) -> bool:
+        return 'extend_module' in self.config and self.config['extend_module'] and self.hook.can_call(name)
+
+    def shift_header(self, item: TocItem, page: Page, lang):
 
+        if page.file.src_path.count(os.sep) <= 0:
+            # skip root
+            return
+
+        index_re = re.compile('.*(index.' + lang + '.md$|index.md$)')
+        hasindex = False
+        for path in os.listdir(Path(page.file.abs_src_path).parent):
+            if index_re.match(path):
+                hasindex = True
+                break
+
+        if self.config['shift_header'] == 'after_index':
+            if hasindex and not index_re.match(page.file.src_path):
+                item.src_level += 1
+
+        if self.config['shift_header'] == 'after_h1_of_index':
+            if hasindex and (not index_re.match(page.file.src_path)):
+                item.src_level += 1
+            elif index_re.match(page.file.src_path) and item.src_level > 1:
+                item.src_level += 1
+
```

### Comparing `mkdocs-toc-md-0.0.6/setup.py` & `mkdocs-toc-md-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # python setup.py develop
 # python setup.py sdist bdist_wheel
 # twine check dist/mkdocs-toc-md-x.x.x.tar.gz
 # twine upload --repository pypi dist/*
 setup(
     name='mkdocs-toc-md',
-    version='0.0.6',
+    version='0.0.7',
     description='Generate a table of contents markdown file',
     long_description=io.open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs plugin toc generator',
     author='Ryo Tsunoda',
     author_email='try0.development@gmail.com',
     url='https://github.com/try0/mkdocs-toc-md',
```

