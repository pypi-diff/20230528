# Comparing `tmp/soccminer-0.0.39a1.tar.gz` & `tmp/soccminer-0.0.40a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/projappl/project_2002565/soccminer_eval/soccminer/dist/tmpo1sca8tf/soccminer-0.0.39a1.tar", last modified: Mon Apr  3 11:12:15 2023, max compression
+gzip compressed data, was "/projappl/project_2002565/soccminer_eval/soccminer/dist/tmpzqlij1u0/soccminer-0.0.40a1.tar", last modified: Sun May 28 16:33:34 2023, max compression
```

## Comparing `soccminer-0.0.39a1.tar` & `soccminer-0.0.40a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-04-03 11:12:15.000000 soccminer-0.0.39a1/
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       38 2023-04-03 11:12:15.000000 soccminer-0.0.39a1/setup.cfg
--rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)     1136 2022-01-20 20:24:37.000000 soccminer-0.0.39a1/LICENSE
-drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-04-03 11:12:15.000000 soccminer-0.0.39a1/soccminer.egg-info/
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      835 2023-04-03 11:12:12.000000 soccminer-0.0.39a1/soccminer.egg-info/SOURCES.txt
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)        1 2023-04-03 11:12:12.000000 soccminer-0.0.39a1/soccminer.egg-info/not-zip-safe
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)        1 2023-04-03 11:12:12.000000 soccminer-0.0.39a1/soccminer.egg-info/dependency_links.txt
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      427 2023-04-03 11:12:12.000000 soccminer-0.0.39a1/soccminer.egg-info/PKG-INFO
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       91 2023-04-03 11:12:12.000000 soccminer-0.0.39a1/soccminer.egg-info/requires.txt
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       10 2023-04-03 11:12:12.000000 soccminer-0.0.39a1/soccminer.egg-info/top_level.txt
--rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)     5182 2022-01-20 20:24:37.000000 soccminer-0.0.39a1/README.md
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      427 2023-04-03 11:12:15.000000 soccminer-0.0.39a1/PKG-INFO
-drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-04-03 11:12:12.000000 soccminer-0.0.39a1/bin/
--rwxrwxr-x   0 sridhara (10009479) project_2002565 (2002565)    17839 2022-12-16 02:47:30.000000 soccminer-0.0.39a1/bin/main.py
--rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)      686 2023-04-03 11:10:24.000000 soccminer-0.0.39a1/setup.py
-drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-04-03 11:12:15.000000 soccminer-0.0.39a1/soccminer/
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)   100033 2023-01-02 21:30:26.000000 soccminer-0.0.39a1/soccminer/java_ast_parsing.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    27195 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/project_meta.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      969 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/java_proj_miner.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    17071 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/java_project_meta_attributes.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     4030 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/proj_comments_main_attr.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     2191 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/process_parameters.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      669 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/exception_monitoring.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     3167 2022-12-16 03:41:20.000000 soccminer-0.0.39a1/soccminer/srcml.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    23894 2023-01-12 15:01:49.000000 soccminer-0.0.39a1/soccminer/helper.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     1058 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/project_attributes.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    65563 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/comments_miner.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    29129 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/source_code_details.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     6298 2023-04-03 11:08:21.000000 soccminer-0.0.39a1/soccminer/parse_source_files.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      601 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/__init__.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     7812 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/comments.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    31360 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/json_serialization.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      400 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/environment.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      647 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/performance_time.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     1028 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/proj_comments_comprehensive_attr.py
--rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     2886 2022-12-16 02:30:58.000000 soccminer-0.0.39a1/soccminer/soccminer_logger.py
+drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       38 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/setup.cfg
+-rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)     1136 2022-01-20 20:24:37.000000 soccminer-0.0.40a1/LICENSE
+drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/soccminer.egg-info/
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      835 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/soccminer.egg-info/SOURCES.txt
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)        1 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/soccminer.egg-info/not-zip-safe
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)        1 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/soccminer.egg-info/dependency_links.txt
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      427 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/soccminer.egg-info/PKG-INFO
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       91 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/soccminer.egg-info/requires.txt
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)       10 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/soccminer.egg-info/top_level.txt
+-rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)     5182 2022-01-20 20:24:37.000000 soccminer-0.0.40a1/README.md
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      427 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/PKG-INFO
+drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/bin/
+-rwxrwxr-x   0 sridhara (10009479) project_2002565 (2002565)    18355 2023-05-28 16:22:19.000000 soccminer-0.0.40a1/bin/main.py
+-rw-rw-r--   0 sridhara (10009479) project_2002565 (2002565)      686 2023-05-28 16:31:24.000000 soccminer-0.0.40a1/setup.py
+drwxrws---   0 sridhara (10009479) project_2002565 (2002565)        0 2023-05-28 16:33:34.000000 soccminer-0.0.40a1/soccminer/
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)   102093 2023-05-28 16:20:14.000000 soccminer-0.0.40a1/soccminer/java_ast_parsing.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    27195 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/project_meta.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      969 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/java_proj_miner.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    17071 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/java_project_meta_attributes.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     4030 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/proj_comments_main_attr.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     2191 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/process_parameters.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      669 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/exception_monitoring.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     3167 2022-12-16 03:41:20.000000 soccminer-0.0.40a1/soccminer/srcml.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    23894 2023-01-12 15:01:49.000000 soccminer-0.0.40a1/soccminer/helper.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     1058 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/project_attributes.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    66096 2023-05-28 16:13:19.000000 soccminer-0.0.40a1/soccminer/comments_miner.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    29129 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/source_code_details.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     6298 2023-04-03 11:08:21.000000 soccminer-0.0.40a1/soccminer/parse_source_files.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      601 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/__init__.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     7812 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/comments.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)    31360 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/json_serialization.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      400 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/environment.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)      647 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/performance_time.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     1028 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/proj_comments_comprehensive_attr.py
+-rw-rw----   0 sridhara (10009479) project_2002565 (2002565)     2886 2022-12-16 02:30:58.000000 soccminer-0.0.40a1/soccminer/soccminer_logger.py
```

### Comparing `soccminer-0.0.39a1/LICENSE` & `soccminer-0.0.40a1/LICENSE`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer.egg-info/SOURCES.txt` & `soccminer-0.0.40a1/soccminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/README.md` & `soccminer-0.0.40a1/README.md`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/bin/main.py` & `soccminer-0.0.40a1/bin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,24 +40,25 @@
 
 def is_existing_file(file_loc):
     # validate if file exists
     return os.path.isfile(file_loc)
 
 
 def validate_cli(cl_args):
-    global local_inp_dir, inp_dir, level, load_proj_flag, log, programming_language, serialize_flag, output_dir, mode
+    global local_inp_dir, inp_dir, level, load_proj_flag, log, programming_language, serialize_flag, output_dir, mode, context_span
     local_inp_dir = cl_args.input
 
     # level comment - Basic Comment and Project Attributes, level comprehensive_comment - Comprehensive Comment Attributes
     # level project - Project Meta Attributes, level all - Project and Comprehensive Comment attributes
     level = cl_args.level
     log = cl_args.log  # 0 - No log, 1 - Debug, 2 - Info
     programming_language = cl_args.language.lower()
     load_proj_flag = cl_args.direct_load
     output_dir = cl_args.output
+    context_span = int(cl_args.context_span)
     if type(load_proj_flag) == str:
         if load_proj_flag.lower() == 'true':
             load_proj_flag = True
         elif load_proj_flag.lower() == 'false':
             load_proj_flag = False
 
     if load_proj_flag not in [0, 1]:
@@ -123,14 +124,19 @@
             log = 2
         elif log.strip().lower() == "info":
             log = 1
 
     if programming_language not in ['java']:
         print("Issue with programming language input {}".format(programming_language))
         return False
+
+    if context_span < 1:
+        print("Issue with context span input, context span cannot be less than 1")
+        return False
+
     return True
 
 def demo_project(cm):
     # Loads JavaMetaAttribute object for mining level 'project' that contains project
     # meta for all the entities.
     for proj in cm.fetch_mined_project_meta():
         ############################################################
@@ -221,15 +227,15 @@
         print("Total method level comments: ",len(proj.get_comprehensive_method_comment_attr()))
         print("Total interface level comments: ",len(proj.get_comprehensive_interface_comment_attr()))
         print("Total enum level comments: ",len(proj.get_comprehensive_enum_comment_attr()))
         print("Total StaticBlock level comments: ", len(proj.get_comprehensive_static_block_comment_attr()))
 
 
 def validate_cli_args():
-    global inp_dir, m_level, load_proj, log_level, prog_lang, output_dir, mode
+    global inp_dir, m_level, load_proj, log_level, prog_lang, output_dir, mode, context_span
     # parse input arguments
     parser = argparse.ArgumentParser(prog='main.py', description='Source Code Comments miner')
     parser.add_argument("-i", "--input",
                         help="Defines the input to the tool. Mandatory input argument. Can be 'local_dir' containing project source files or containing project repositories as sub-directories or 'Git Repo URL'")
     parser.add_argument("-l", "--language", default='java',
                         help="The programming language of the project, for now only java project are handled by SoCCMiner")
     parser.add_argument("-lvl", "--level", default='comment',
@@ -250,37 +256,40 @@
                         help="Defines the output directory where the mined entities will be stored by default it is current working directory. Accepts only valid existing directory.")
     parser.add_argument("-m", "--mode", default='single',
                         help="Defines SoCC-Miner execution mode, can be 'single' to mine single project directory (i.e., all files and directories within input directory will be treated as a single project), \n"
                              "'multiple' to mine multiple project directories in which all sub-directories within the input directory will be treated as separate project directories, or \n"
                              "NOTE: SoCC-Miner expects an input directory that contains only project directory/ies as sub-directory/ies in 'multiple' mode. \n")
                              #"'files' to mine individual source files that are not part of any project, all the individual files will be collectively treated as a single project. \n"
                              #"NOTE: SoCC-Miner expects an input directory that contains only project directory/ies as sub-directory/ies in 'multiple' mode. \n")
+    parser.add_argument("-cs", "--context_span", default=1,
+                        help="Length of the context span (in number of lines) to be fetched for both preceding and succeeding context for a source code context")
 
     if len(sys.argv) <= 1:
         parser.print_help()
         sys.exit(1)
 
     cl_args = parser.parse_args()
     inp_dir = cl_args.input
     m_level = cl_args.level
     load_proj = cl_args.direct_load
     log_level = cl_args.log
     prog_lang = cl_args.language
     output_dir = cl_args.output
     mode = cl_args.mode
+    context_span = int(cl_args.context_span)
 
     ret_stat = validate_cli(cl_args)
     if not ret_stat:
         parser.print_help()
         sys.exit(1)
 
 
 def main():
     global local_inp_dir, level, load_proj_flag, log, programming_language, output_dir
-    global inp_dir, m_level, load_proj, log_level, prog_lang, mode
+    global inp_dir, m_level, load_proj, log_level, prog_lang, mode, context_span
     project_name = None
 
     try:
         validate_cli_args()
         if log is not None or log != 0:
             SoCCMinerLogger(log, "")
         print("Instantiating from Main")
@@ -289,15 +298,15 @@
         # logging.debug("Found {} project repositories in the input dir argument {}".format(total_project_repositories, inp_dir))
 
         logging.info("Input Mining Level: {}".format(m_level))
         logging.info("Input Load_Project: {}, {}".format(load_proj, load_proj_flag))
         # Passing the args as rcvd from commandline without validation as there's a validation in the API call
         # However this validation here happens when invoked from commandline only
 
-        cm = CommentsMiner(inp_dir, prog_lang, m_level, load_proj, log_level, output_dir, mode)
+        cm = CommentsMiner(inp_dir, prog_lang, m_level, load_proj, log_level, output_dir, mode, context_span)
         if not load_proj_flag and cm.invalid_ing_arg_flag:
             print("Unable to mine the source code as SoccMiner did not execute due to invalid input argument.")
             sys.exit(1)
         elif load_proj_flag and cm.invalid_ing_arg_flag:
             print("Unable to load project as SoccMiner did not execute due to invalid input argument.")
             sys.exit(1)
 
@@ -328,13 +337,14 @@
 log = ""
 log_level = ""
 programming_language = ""
 prog_lang = ""
 load_proj_flag = ""
 load_proj = ""
 mode = ""
+context_span = 0
 
 # Main function
 if __name__ == '__main__':
     main()
```

### Comparing `soccminer-0.0.39a1/setup.py` & `soccminer-0.0.40a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='soccminer',
-    version='0.0.39a1',
+    version='0.0.40a1',
     packages=['soccminer'],
     scripts=['bin/main.py'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Topic :: Text Processing :: Linguistic',
```

### Comparing `soccminer-0.0.39a1/soccminer/java_ast_parsing.py` & `soccminer-0.0.40a1/soccminer/java_ast_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     no_specifier_label = "NO_SPECIFIER"
     srcml_ns = "{http://www.srcML.org/srcML/src}"
 
     def __init__(self, xml_file):
         self.top_level_elements = []
         self.project_dir = None
         self.src_file_name = None
+        self.abs_src_file_name = None
         self.comments_counter = 0
         self.nodes = []
         self.tree = etree.ElementTree()
         self.root = None
         self.comment_master_dict = {}
         self.file_header_comment = ''
         self.unit_ele = None
@@ -144,14 +145,15 @@
         self.xml_file_num = None
         self.existing_pckg_serialization_url = None
         self.logger = None
         self.file_obj = None
         self.all_cmnts_cntr = 0
         self.project_name = None
         self.xml_file = xml_file
+        self.context_span=1
 
         # fetch the program parameters set in the driver module CommentsMiner
         ProcessParameter.fetch_program_parameters()
 
     def set_unit_element(self):
         self.unit_ele = etree.Element(XmlProperties.unit_element)
 
@@ -522,18 +524,20 @@
         self.logger.debug("fetch_project_comments_count(): {}".format(self.project_comments_dir))
         src_files = SourceFiles(self.project_comments_dir)
         src_files.fetch_source_files(src_files.loc, 'json')
         comment_count = len(src_files.get_files())
         del src_files
         return comment_count
 
-    def proc_java_ast_elements(self, proj_dir, src_file_name, xml_file_name, xml_file_num):
+    def proc_java_ast_elements(self, proj_dir, src_file_name, xml_file_name, xml_file_num, cntxt_span):
         self.project_dir = proj_dir
         self.xml_file_num = xml_file_num
         self.src_file_name = src_file_name
+        self.abs_src_file_name = src_file_name
+        self.context_span = cntxt_span
 
         self.package_instance = None
 
         if Platform.is_unix_platform():
             proj_dir = proj_dir[:-1] if proj_dir.endswith('/') else proj_dir
             self.project_name = proj_dir.split('/')[-1].replace("/", "")
             if '/' in self.src_file_name:
@@ -1231,14 +1235,42 @@
                 parent_instance.append_method_info(construct_instance)
         elif type(construct_instance).__name__ == "StaticBlockInfo":
             if type(parent_instance).__name__ == "PackageInfo":
                 parent_instance.append_package_static_block_info(construct_instance)  # Encountered scenarios where it occurs outside class
             else:
                 parent_instance.append_static_block_info(construct_instance)  # for Most often found in Class
 
+    def proc_context_span(self, comment_instance, prec_ele, succ_ele):
+        cmnt_src_file = self.abs_src_file_name
+        
+        # source code line preceding comment
+        prec_comment_line_no = self.fetch_element_line_no(prec_ele)
+        # source code line after comment
+        succ_comment_line_no = self.fetch_element_line_no(succ_ele)
+        prec_beginning_span=0
+        succ_end_span=0
+
+        src_fh = open(cmnt_src_file, "r", encoding="utf-8")
+        file_lines=src_fh.readlines()
+        total_lines = len(file_lines)
+
+        if self.context_span > 1:
+            if prec_comment_line_no - self.context_span - 1 >= 0:
+                prec_beginning_span = prec_comment_line_no - self.context_span - 1
+            else:
+                prec_beginning_span = 0
+
+            if succ_comment_line_no + self.context_span <= total_lines:
+                succ_end_span = succ_comment_line_no + self.context_span
+            else:
+                succ_end_span = total_lines
+
+            comment_instance.set_preceding_code(file_lines[prec_beginning_span:self.context_span+prec_beginning_span])
+            comment_instance.set_succeeding_code(file_lines[succ_comment_line_no:succ_end_span])
+
     def fetch_succeeding_element(self, comment_instance, ele):
         try:
             if self.get_next_element(ele) is None:
                 comment_instance.set_comment_category("NON-HEADER")
                 self.logger.debug(
                     "fetch_succeding_element(): to identify parent of {} which is the last element".format(ele))
                 assoc_parent_ele_next = self.identify_parent(ele)
@@ -1247,26 +1279,26 @@
                     self.logger.debug("***Comment Next element- (Last element in): {}".format(assoc_parent_ele_next))
                     if self.get_next_element(assoc_parent_ele_next) is None:
                         # last element in block, hence fetching parent of the block and get the next element
                         ele_for_src_cd = self.get_next_element(self.get_parent(assoc_parent_ele_next))
                         if ele_for_src_cd is not None:
                             self.logger.debug("***e Comment Next element- (Next to assoc parent element's parent): {} at line {}".format(ele_for_src_cd,self.fetch_element_line_no(ele_for_src_cd)))
                             comment_instance.set_succeeding_element(ele_for_src_cd)  # contains the xml element; input for succeeding code
-                            comment_instance.set_succeeding_node(self.get_element_tag(ele_for_src_cd))  # contains the name (or tag)
+                            comment_instance.set_succeeding_node(self.get_element_tag(ele_for_src_cd).replace('{http://www.srcML.org/srcML/src}',''))  # contains the name (or tag)
                         else:
                             comment_instance.set_last_element_in("FILE")
                             comment_instance.set_succeeding_code("NA")
                             comment_instance.set_succeeding_element("EOF")
                             comment_instance.set_succeeding_node("EOF")  # contains the name (or tag)
                     else:
                         ele_for_src_cd = self.get_next_element(assoc_parent_ele_next)
                         self.logger.debug("***f Comment Next element- (Next to assoc parent element): {} at line {}".format(ele_for_src_cd,
                                       self.fetch_element_line_no(ele_for_src_cd)))
                         comment_instance.set_succeeding_element(ele_for_src_cd)
-                        comment_instance.set_succeeding_node(self.get_element_tag(ele_for_src_cd))
+                        comment_instance.set_succeeding_node(self.get_element_tag(ele_for_src_cd).replace('{http://www.srcML.org/srcML/src}',''))
 
                 else:
                     comment_instance.set_last_element_in("FILE")
                     comment_instance.set_succeeding_code("NA")
                     comment_instance.set_succeeding_element("EOF")
                     comment_instance.set_succeeding_node("EOF")
             else:
@@ -1277,42 +1309,42 @@
                 else:
                     comment_instance.set_comment_category("NON-HEADER")
                     self.logger.debug("****** Comment Next element 3: {}".format(ele_for_src_cd))
                     self.logger.debug("Set succeeding element: {},{} with the len(child) is {}".format(self.get_element_tag(ele_for_src_cd),
                                                                  self.fetch_element_line_no(ele_for_src_cd),
                                                                  len(list(ele_for_src_cd))))
                 comment_instance.set_succeeding_element(ele_for_src_cd)
-                comment_instance.set_succeeding_node(self.get_element_tag(ele_for_src_cd))
+                comment_instance.set_succeeding_node(self.get_element_tag(ele_for_src_cd).replace('{http://www.srcML.org/srcML/src}',''))
         except Exception as ex:
             self.logger.error("Unexpected error in fetching succeeding element {} {}".format(sys.exc_info()[0], ex))
             raise
 
     def fetch_preceding_element(self, comment_instance, ele):
         if self.get_previous_element(ele) is None:
             assoc_parent_ele_prev = self.identify_parent(ele)
             self.logger.debug("fetch_precceding_element(): Parent of the element {} at line {} is {} ".format(ele, self.fetch_element_line_no(assoc_parent_ele_prev), assoc_parent_ele_prev))
             if not(self.is_root_element(assoc_parent_ele_prev) and self.fetch_element_line_no(assoc_parent_ele_prev) == 1):
                 self.logger.debug("***********Comment Previous element parent (First element in): {}".format(assoc_parent_ele_prev))
                 comment_instance.set_first_element_in(self.get_element_tag(assoc_parent_ele_prev))
                 # since first element in construct/block, the construct/block is set as the preceding element, as
                 # it will be invalid to fetch the previous element to the construct/block and set it as preceding element
                 comment_instance.set_preceding_element(assoc_parent_ele_prev)
-                comment_instance.set_preceding_node(self.get_element_tag(assoc_parent_ele_prev))
+                comment_instance.set_preceding_node(self.get_element_tag(assoc_parent_ele_prev).replace('{http://www.srcML.org/srcML/src}',''))
             else:
                 comment_instance.set_first_element_in("FILE")
                 comment_instance.set_comment_category("HEADER")
                 comment_instance.set_preceding_code("NA")
                 comment_instance.set_preceding_element("NA")
                 comment_instance.set_preceding_node("NA")
         else:
             prev_ele = self.get_previous_element(ele)
             self.logger.debug("Comment Previous element 2: ".format(prev_ele))
             comment_instance.set_first_element_in("NA")
             comment_instance.set_preceding_element(prev_ele)
-            comment_instance.set_preceding_node(self.get_element_tag(prev_ele))
+            comment_instance.set_preceding_node(self.get_element_tag(prev_ele).replace('{http://www.srcML.org/srcML/src}',''))
 
     def identify_parent(self, element):
         try:
             self.logger.debug("identify_parent() begins for {} at line {}".format(element, self.fetch_element_line_no(element)))
             parent_node = self.get_parent(element)
             self.logger.debug(
                 "identify_parent(): parent for {} at line {} is {}".format(element, self.fetch_element_line_no(element), parent_node))
@@ -1605,28 +1637,39 @@
             comment_instance.set_comment_type(self.fetch_element_attribute(element, "type"))
             self.logger.debug("Setting comment category, sub-category, assoc_block_ele for comment at line {} {}".format(comment_line_no, len(list(self.root))))
             # category, sub-category, assoc_block_ele
             self.fetch_comment_assoc_block(comment_instance, element)
             self.logger.debug("Setting comment succeeding element, code for comment at line {} {}".format(comment_line_no, len(list(self.root))))
             # last element in, succeeding element, succeeding code
             # if consecutive comments, pass the first and last comment for fetching preceding and succeeding element
+            contxt_succ_ele=None
+            contxt_prec_ele=None
             if self.consecutive_comment_last is not None:
                 self.fetch_succeeding_element(comment_instance, self.consecutive_comment_last)
+                contxt_succ_ele=self.consecutive_comment_last
             else:
                 self.fetch_succeeding_element(comment_instance, element)
+                contxt_succ_ele=element
             self.logger.debug("Setting comment preceding element, code for comment at line {} {}".format(comment_line_no, len(list(self.root))))
             if self.consecutive_comment_first is not None:
                 self.fetch_preceding_element(comment_instance, self.consecutive_comment_first)
+                contxt_prec_ele=self.consecutive_comment_first
             else:
                 self.fetch_preceding_element(comment_instance, element)
-            # succeeding code - must be invoked after setting succeeding element
-            srcml_obj = SourceML()
-            comment_instance.set_succeeding_code(srcml_obj.fetch_code_from_srcml(copy(comment_instance.get_succeeding_element())))
-            # preceding code - must be invoked after setting preceding element
-            comment_instance.set_preceding_code(srcml_obj.fetch_code_from_srcml(copy(comment_instance.get_preceding_element())))
+                contxt_prec_ele=element
+
+            if self.context_span == 1:
+                # succeeding code - must be invoked after setting succeeding element
+                srcml_obj = SourceML()
+
+                comment_instance.set_succeeding_code(srcml_obj.fetch_code_from_srcml(copy(comment_instance.get_succeeding_element())))
+                # preceding code - must be invoked after setting preceding element
+                comment_instance.set_preceding_code(srcml_obj.fetch_code_from_srcml(copy(comment_instance.get_preceding_element())))
+            else:
+                self.proc_context_span(comment_instance, contxt_prec_ele, contxt_succ_ele)
 
         self.create_dir(self.project_comments_dir)
         self.logger.debug("Comments Directory: {}".format(self.project_comments_dir))
         proj_entity_type_comments_count = self.fetch_project_comments_count()
         logging.debug("proj_entity_type_comments_count: {}".format(proj_entity_type_comments_count))
         self.comments_counter = 1 if proj_entity_type_comments_count == 0 else proj_entity_type_comments_count + 1
         logging.debug("comments_counter: {}".format(self.comments_counter))
@@ -1656,15 +1699,15 @@
 
         # Clearing
         del xmlobj
         ASTHelper.clear_locals()
         gc.collect()
 
     @staticmethod
-    def ast_parsing_multiprocessing(src_file, xml_file, proj_dir, xml_file_number, exception_obj, log_level):
+    def ast_parsing_multiprocessing(src_file, xml_file, proj_dir, xml_file_number, cntxt_span, exception_obj, log_level):
         source_ast_parser_obj = XmlProperties(xml_file)
 
         # create exception dir
 
         # log for each AST parsing
         #ast_log = ""
         #if Platform.is_unix_platform():
```

### Comparing `soccminer-0.0.39a1/soccminer/project_meta.py` & `soccminer-0.0.40a1/soccminer/project_meta.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/java_proj_miner.py` & `soccminer-0.0.40a1/soccminer/java_proj_miner.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/java_project_meta_attributes.py` & `soccminer-0.0.40a1/soccminer/java_project_meta_attributes.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/proj_comments_main_attr.py` & `soccminer-0.0.40a1/soccminer/proj_comments_main_attr.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/process_parameters.py` & `soccminer-0.0.40a1/soccminer/process_parameters.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/exception_monitoring.py` & `soccminer-0.0.40a1/soccminer/exception_monitoring.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/srcml.py` & `soccminer-0.0.40a1/soccminer/srcml.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/helper.py` & `soccminer-0.0.40a1/soccminer/helper.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/project_attributes.py` & `soccminer-0.0.40a1/soccminer/project_attributes.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/comments_miner.py` & `soccminer-0.0.40a1/soccminer/comments_miner.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         CommentsMiner.load_project = load_project
 
     @staticmethod
     def set_mode(mode):
         CommentsMiner.mode = mode
 
     @staticmethod
+    def set_context_span(context_span):
+        CommentsMiner.mode = context_span
+
+    @staticmethod
     def validate_soccminer_dir_structure(proj_dir):
         soccminer_dir = [type(PackageInfo()).__name__, type(ClassInfo()).__name__, type(MethodInfo()).__name__,
                         type(InterfaceInfo()).__name__, type(StaticBlockInfo()).__name__]
         empty_folders = False
         empty_folder_count = 0
         soccminer_entity_dir_count = 0
         attr_dir = 'attributes'
@@ -147,28 +151,29 @@
             elif Platform.is_windows_platform():
                 if os.path.isfile(input_dir + '\\' + item):
                     print(
                         "Input directory cannot contain file but only project folders as sub-directories in multiple mode")
                     return False
         return True
 
-    def __init__(self, source_url, lang: str='java', m_level: str ='comment', direct_load=False, log: str = "nolog", output_dir: str =os.getcwd(), mode: str ='single'):
+    def __init__(self, source_url, lang: str='java', m_level: str ='comment', direct_load=False, log: str = "nolog", output_dir: str =os.getcwd(), mode: str ='single', context_span: int = 1):
         self.url = source_url
         if Platform.is_unix_platform():
             CommentsMiner.soccminer_cfg_file = os.getcwd() + '/' + 'soccminer.cfg'
         elif Platform.is_windows_platform():
             CommentsMiner.soccminer_cfg_file = os.getcwd() + '\\' + 'soccminer.cfg'
         self.lang = lang
         self.mining_level = m_level
         self.load_project = direct_load
         self.log = log
         self.output_dir = output_dir
         self.mode = mode
+        self.context_span = int(context_span)
         self.invalid_ing_arg_flag = False
-        if not self.validate_args(self.url, lang, m_level, direct_load, log, output_dir, mode):
+        if not self.validate_args(self.url, lang, m_level, direct_load, log, output_dir, mode, context_span):
             print("Exiting due to invalid arguments.")
             logging.info("Exiting due to invalid arguments.")
             self.invalid_ing_arg_flag = True
             return
 
         if not self.load_project and not Utility.validate_srcml():
             print("Exiting due to inadequate environment. srcML is either not installed or installed incorrectly. SoCCMiner unable to utilize srcML.")
@@ -199,14 +204,15 @@
         CommentsMiner.set_source_url(self.url)
         CommentsMiner.set_mining_level_inp(self.mining_level)
         CommentsMiner.set_lang_inp(self.lang)
         CommentsMiner.set_load_project(self.load_project)
         CommentsMiner.set_log_inp(self.log)
         CommentsMiner.set_output_inp(self.output_dir)
         CommentsMiner.set_mode(self.mode)
+        CommentsMiner.set_context_span(self.context_span)
         CommentsMiner.save_program_parameters()
         logging.debug("Config file created with program parameters")
 
         if self.log == 1 or self.log == 2:
             if SoCCMinerLogger.main_logger is None:
                 self.log_file_obj = SoCCMinerLogger(self.log, "")
 
@@ -501,15 +507,15 @@
             except Exception as project_exception:
                 if self.log != 0:
                     logging.error("Fetch_Mining_Status: - Unexpected error: {}".format(project_exception))
                 error_message = traceback.format_exc()
                 self.exception_obj.update_exception_message(project_name, error_message)
                 continue
 
-    def validate_args(self, input, programming_language, mining_level, load_proj_flag, log, output_dir, mode):
+    def validate_args(self, input, programming_language, mining_level, load_proj_flag, log, output_dir, mode, context_span):
         # level 'comment' - Basic Comment attributes
         # level 'comprehensive_comment' - Comprehensive Comment Attributes
         # level 'project' - Project Meta Attributes,
         # level 'all' - Project and Comprehensive Comment attributes
         # log can be none/nolog(0), info (1), debug(2)
         if type(load_proj_flag) == str:
             if load_proj_flag.lower() == 'true':
@@ -603,14 +609,21 @@
         if programming_language not in ['java']:
             print("Issue with programming language input {}".format(programming_language))
             self.invalid_ing_arg_flag = True
             return False
         else:
             self.lang = programming_language
 
+        if context_span < 1:
+            print("Issue with context span, cannot be less than 1 {}".format(context_span))
+            self.invalid_ing_arg_flag = True
+            return False
+        else:
+            self.context_span = context_span
+
         if Platform.is_unix_platform():
             self.output_dir = output_dir[:-1] if output_dir.endswith('/') else output_dir
         elif Platform.is_windows_platform():
             self.output_dir = output_dir[:-1] if output_dir.endswith('\\') else output_dir
         return True
 
     def initiate_mining(self):
@@ -719,22 +732,22 @@
 
                         for xml_file in src_files.cd_file_xml_mapping_dict:
                             try:
                                 file_cntr += 1
                                 # Source Code Parsing
                                 process = Process(target=XmlParsing.ast_parsing_multiprocessing,
                                                   args=(xml_file, src_files.cd_file_xml_mapping_dict[xml_file],
-                                                        self.project_directory, file_cntr, self.exception_obj, self.log))
+                                                        self.project_directory, file_cntr, self.context_span, self.exception_obj, self.log))
                                 process.start()
                                 process.join()
 
                             except Exception as proc_files_ex:
                                 if self.log != 0:
                                     logging.error(
-                                        "CM: Error while processing source code file {} {} {}".format(xml_file, sys.exc_info()[0],
+                                        "SoCCMiner: Error while processing source code file {} {} {}".format(xml_file, sys.exc_info()[0],
                                                                                                  proc_files_ex))
                                 error_message = traceback.format_exc()
                                 self.exception_obj.update_exception_message(project_name, error_message)
 
                                 error_file = ''
                                 if Platform.is_unix_platform():
                                     error_file = exception_dir + xml_file.split("/")[-1].replace(".java", ".error")
```

### Comparing `soccminer-0.0.39a1/soccminer/source_code_details.py` & `soccminer-0.0.40a1/soccminer/source_code_details.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/parse_source_files.py` & `soccminer-0.0.40a1/soccminer/parse_source_files.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/__init__.py` & `soccminer-0.0.40a1/soccminer/__init__.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/comments.py` & `soccminer-0.0.40a1/soccminer/comments.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/json_serialization.py` & `soccminer-0.0.40a1/soccminer/json_serialization.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/performance_time.py` & `soccminer-0.0.40a1/soccminer/performance_time.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/proj_comments_comprehensive_attr.py` & `soccminer-0.0.40a1/soccminer/proj_comments_comprehensive_attr.py`

 * *Files identical despite different names*

### Comparing `soccminer-0.0.39a1/soccminer/soccminer_logger.py` & `soccminer-0.0.40a1/soccminer/soccminer_logger.py`

 * *Files identical despite different names*

