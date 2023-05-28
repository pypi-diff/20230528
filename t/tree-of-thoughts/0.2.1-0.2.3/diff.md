# Comparing `tmp/tree-of-thoughts-0.2.1.tar.gz` & `tmp/tree-of-thoughts-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.2.1.tar", last modified: Fri May 26 16:42:57 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.2.3.tar", last modified: Sat May 27 08:44:09 2023, max compression
```

## Comparing `tree-of-thoughts-0.2.1.tar` & `tree-of-thoughts-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41686 2023-05-26 16:42:44.000000 tree-of-thoughts-0.2.1/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:42:57.097295 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:42:57.000000 tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:44:09.793140 tree-of-thoughts-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 08:43:56.000000 tree-of-thoughts-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-27 08:44:09.793140 tree-of-thoughts-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-05-27 08:43:56.000000 tree-of-thoughts-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:44:09.793140 tree-of-thoughts-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-27 08:43:56.000000 tree-of-thoughts-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:44:09.793140 tree-of-thoughts-0.2.3/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-27 08:43:56.000000 tree-of-thoughts-0.2.3/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32933 2023-05-27 08:43:56.000000 tree-of-thoughts-0.2.3/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:44:09.793140 tree-of-thoughts-0.2.3/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-27 08:44:09.000000 tree-of-thoughts-0.2.3/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-27 08:44:09.000000 tree-of-thoughts-0.2.3/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:44:09.000000 tree-of-thoughts-0.2.3/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-27 08:44:09.000000 tree-of-thoughts-0.2.3/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 08:44:09.000000 tree-of-thoughts-0.2.3/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.2.1/LICENSE` & `tree-of-thoughts-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.1/PKG-INFO` & `tree-of-thoughts-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.1
+Version: 0.2.3
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.2.1/README.md` & `tree-of-thoughts-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,30 @@
 
 # Join Agora, Creators United
 This implementation of Tree of Thoughts is brought to you by Agora, Agora advances Humanity with open source SOTA Multi-Modality AI research! We plan on combating Humanity's grandest root problems like food insecurity, planetary insecurity, and disease, and hopefully death itself.
 
 [Join our Discord and contribute to this project](https://discord.gg/qUtxnK2NMf)
 
 ## Getting started
-Clone this repository with ```git clone https://github.com/kyegomez/tree-of-thoughts```
 
+## Method1
+Clone this repository with 
+
+```git clone https://github.com/kyegomez/tree-of-thoughts```
+
+``` 
+cd tree-of-thoughts
+cd tree_of_thoughts
+python3 treeofthoughts.py --problem "design an new transportation system for an all-new city" --search_algorithm="BFS"
+```
+Add ` OPENAI_API_KEY='API KEY'` in the .env!
+
+
+
+## Method2
 or:
 
 ```pip install tree-of-thoughts ```
 
 
 Navigate to the repository folder: ```cd tree-of-thoughts```
 
@@ -31,15 +45,17 @@
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
 from tree_of_thoughts.treeofthoughts import OpenAILanguageModel, CustomLanguageModel, TreeofThoughts, OptimizedOpenAILanguageModel, OptimizedTreeofThoughts, HuggingLanguageModel
 
 use_v2 = False
+
 api_key=""
+
 api_base= "" # leave it blank if you simply use default openai api url
 
 if not use_v2:
     #v1
     model = OpenAILanguageModel(api_key=api_key, api_base=api_base # api_model="gpt4" # for higher performance base model is not smart
     ) 
 else:
@@ -57,27 +73,31 @@
 
 #cot or propose
 strategy="cot"
 
 # value or vote
 evaluation_strategy = "value"
 
-if not use_v2:
-    #create an instance of the tree of thoughts class v1
-    tree_of_thoughts = TreeofThoughts(model, search_algorithm)
-else:
-    #or v2 -> dynamic beam width -< adjust the beam width [b] dynamically based on the search depth quality of the generated thoughts # does not work now use regular tree of thoughts
-    tree_of_thoughts= OptimizedTreeofThoughts(model, search_algorithm)
+# if not use_v2:
+#     #create an instance of the tree of thoughts class v1
+
+
+tree_of_thoughts = TreeofThoughts(model, search_algorithm)
+
+
+# else:
+#     #or v2 -> dynamic beam width -< adjust the beam width [b] dynamically based on the search depth quality of the generated thoughts # does not work now use regular tree of thoughts
+#     tree_of_thoughts= OptimizedTreeofThoughts(model, search_algorithm)
 
 input_problem = "use 4 numbers and basic arithmetic operations (+-*/) to obtain 24" #note for super intelligent responses you'll have to be more explicit in your prompt and select a better model
     
 
 
 input_problem = "What are the best reasoning methods to advance Large Language Models"
-k = 5 #number of thoughts to input
+k = 5 #number of thoughts to generate
 T = 3 # maximum depth of the search tree
 b = 5 # branching factor -< number of child nodes for each branch
 vth = 0.5 # pruning state -> any evaluated thought below this is eliminated
 timeout = 10 #10 seconds timeout before stop
 confidence = 0.8 #cmodel is confident on performance
 max_iterations = 40 #tree branh nodes 
 convergence_threshold = 0.01 #determining when the search process has converged
@@ -86,17 +106,17 @@
 
 #call the solve emthod with the input problem and other params
 solution = tree_of_thoughts.solve(input_problem, k, T, b, vth, timeout, confidence, max_iterations, convergence_threshold, convergence_count)
 
     
 
 
-# Save the tree and metrics to a JSON file
-file_name = "logs/tree_of_thoughts_output.json"
-tree_of_thoughts.save_tree_to_json(file_name)
+# # Save the tree and metrics to a JSON file
+# file_name = "logs/tree_of_thoughts_output.json"
+# tree_of_thoughts.save_tree_to_json(file_name)
 
 ```
 
 Or Integrate your own custom language model:
 
 ```python
 
@@ -315,35 +335,47 @@
 5. Optimize the algorithm for performance and resource usage, ensuring it scales well with large multi-modal datasets.
 6. Publish the results and gather feedback from the community to further improve the multi-modal Tree of Thoughts algorithm.
 
 Join us on this exciting journey to advance the Tree of Thoughts algorithm to multi-modality superintelligence! 🚀
 
 # Here's the documentation for the inputs of the optimized Tree of Thoughts model:
 
-x (str): The initial problem statement or prompt for which the Tree of Thoughts algorithm will generate a solution.
-
-k (int, default=5): The number of thoughts to generate at each state. A higher value of k will result in more thoughts being generated, potentially leading to a more diverse set of solutions. However, increasing k may also increase the computational complexity and time required to find a solution.
-
-T (int, default=3): The maximum depth of the search tree. A higher value of T allows the algorithm to explore deeper states, potentially leading to better solutions. However, increasing T may also increase the computational complexity and time required to find a solution.
+## x (str): 
+The initial problem statement or prompt for which the Tree of Thoughts algorithm will generate a solution.
 
-b (int, default=5): The branching factor of the search tree, which determines the maximum number of child nodes for each parent node. A higher value of b allows the algorithm to explore more states, potentially leading to better solutions. However, increasing b may also increase the computational complexity and time required to find a solution.
+## k (int, default=5): 
+The number of thoughts to generate at each state. 
+A higher value of k will result in more thoughts being generated, potentially leading to a more diverse set of solutions. However, increasing k may also increase the computational complexity and time required to find a solution.
 
-vth (float, default=0.5): The value threshold for pruning states. States with a value below this threshold will be discarded, reducing the search space. A higher value of vth will result in a more aggressive pruning strategy, potentially speeding up the search process. However, setting vth too high may cause the algorithm to discard promising states, leading to suboptimal solutions.
+## T (int, default=3): 
+The maximum depth of the search tree. 
+A higher value of T allows the algorithm to explore deeper states, potentially leading to better solutions. However, increasing T may also increase the computational complexity and time required to find a solution.
 
-timeout (int, default=10): The maximum time (in seconds) allowed for the search process. If the search process exceeds this time limit, the algorithm will return the best solution found so far.
+## b (int, default=5): 
+The branching factor of the search tree, which determines the maximum number of child nodes for each parent node.
+A higher value of b allows the algorithm to explore more states, potentially leading to better solutions. However, increasing b may also increase the computational complexity and time required to find a solution.
 
-confidence_threshold (float, default=0.8): The confidence threshold for determining when a solution is satisfactory. If the algorithm finds a solution with a confidence value above this threshold, it will return the solution immediately.
+## vth (float, default=0.5): 
+The value threshold for pruning states. 
+States with a value below this threshold will be discarded, reducing the search space. A higher value of vth will result in a more aggressive pruning strategy, potentially speeding up the search process. However, setting vth too high may cause the algorithm to discard promising states, leading to suboptimal solutions.
 
-max_iterations (int, default=40): The maximum number of iterations allowed for the search process. If the search process exceeds this number of iterations, the algorithm will return the best solution found so far.
+## timeout (int, default=10): 
+The maximum time (in seconds) allowed for the search process. If the search process exceeds this time limit, the algorithm will return the best solution found so far.
 
-convergence_threshold (float, default=0.01): The convergence threshold for determining when the search process has converged. If the difference in confidence values between consecutive iterations is below this threshold for a specified number of iterations (convergence_count), the algorithm will return the best solution found so far.
+## confidence_threshold (float, default=0.8): 
+The confidence threshold for determining when a solution is satisfactory. If the algorithm finds a solution with a confidence value above this threshold, it will return the solution immediately.
 
-convergence_count (int, default=5): The number of consecutive iterations required for the search process to be considered converged. If the difference in confidence values between consecutive iterations is below the convergence_threshold for this number of iterations, the algorithm will return the best solution found so far.
+## max_iterations (int, default=40): 
+The maximum number of iterations allowed for the search process. If the search process exceeds this number of iterations, the algorithm will return the best solution found so far.
 
+## convergence_threshold (float, default=0.01): 
+The convergence threshold for determining when the search process has converged. If the difference in confidence values between consecutive iterations is below this threshold for a specified number of iterations (convergence_count), the algorithm will return the best solution found so far.
 
+## convergence_count (int, default=5): 
+The number of consecutive iterations required for the search process to be considered converged. If the difference in confidence values between consecutive iterations is below the convergence_threshold for this number of iterations, the algorithm will return the best solution found so far.
 
 
 # Acknowledgements
 
 Thanks to: Shunyu Yao Princeton University, Dian Yu Google DeepMind, Jeffrey Zhao, Google DeepMind, Izhak Shafran Google DeepMind, Thomas L. Griffiths, Princeton University, Yuan Cao Google DeepMind, Karthik Narasimha, Princeton University for sharing this amazing work with the world!
 
 And, thanks to Phil Wang or Lucidrains for inspiring me to devote myself to open source AI Research
```

### Comparing `tree-of-thoughts-0.2.1/setup.py` & `tree-of-thoughts-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.2.1',
+  version = '0.2.3',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
@@ -15,14 +15,15 @@
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
   install_requires=[
     'guidance',
     'openai',
+    'transformers'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `tree-of-thoughts-0.2.1/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.2.3/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.1
+Version: 0.2.3
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

