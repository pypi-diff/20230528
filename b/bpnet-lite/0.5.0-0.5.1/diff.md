# Comparing `tmp/bpnet-lite-0.5.0.tar.gz` & `tmp/bpnet-lite-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpnet-lite-0.5.0.tar", last modified: Wed May 24 22:14:20 2023, max compression
+gzip compressed data, was "bpnet-lite-0.5.1.tar", last modified: Sun May 28 18:49:44 2023, max compression
```

## Comparing `bpnet-lite-0.5.0.tar` & `bpnet-lite-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-24 22:14:20.760610 bpnet-lite-0.5.0/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1072 2023-05-18 00:41:39.000000 bpnet-lite-0.5.0/LICENSE
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      341 2023-05-24 22:14:20.760610 bpnet-lite-0.5.0/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6478 2023-05-18 06:03:42.000000 bpnet-lite-0.5.0/README.md
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    16670 2023-05-24 20:59:49.000000 bpnet-lite-0.5.0/bpnet
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-24 22:14:20.728610 bpnet-lite-0.5.0/bpnet_lite.egg-info/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      341 2023-05-24 22:14:20.000000 bpnet-lite-0.5.0/bpnet_lite.egg-info/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      433 2023-05-24 22:14:20.000000 bpnet-lite-0.5.0/bpnet_lite.egg-info/SOURCES.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2023-05-24 22:14:20.000000 bpnet-lite-0.5.0/bpnet_lite.egg-info/dependency_links.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      167 2023-05-24 22:14:20.000000 bpnet-lite-0.5.0/bpnet_lite.egg-info/requires.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       10 2023-05-24 22:14:20.000000 bpnet-lite-0.5.0/bpnet_lite.egg-info/top_level.txt
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-24 22:14:20.756610 bpnet-lite-0.5.0/bpnetlite/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      175 2023-05-24 22:13:07.000000 bpnet-lite-0.5.0/bpnetlite/__init__.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    10843 2023-05-24 02:26:56.000000 bpnet-lite-0.5.0/bpnetlite/attributions.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    16333 2023-05-20 18:27:46.000000 bpnet-lite-0.5.0/bpnetlite/bpnet.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9078 2023-05-24 00:23:23.000000 bpnet-lite-0.5.0/bpnetlite/chrombpnet.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    17389 2023-05-23 04:09:48.000000 bpnet-lite-0.5.0/bpnetlite/io.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1643 2023-05-18 00:41:39.000000 bpnet-lite-0.5.0/bpnetlite/logging.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     2418 2023-05-18 00:41:39.000000 bpnet-lite-0.5.0/bpnetlite/losses.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     7645 2023-05-24 00:07:34.000000 bpnet-lite-0.5.0/bpnetlite/marginalize.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9144 2023-05-18 00:41:39.000000 bpnet-lite-0.5.0/bpnetlite/negatives.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13599 2023-05-18 00:41:39.000000 bpnet-lite-0.5.0/bpnetlite/performance.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12470 2023-05-24 05:38:57.000000 bpnet-lite-0.5.0/chrombpnet
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2023-05-24 22:14:20.760610 bpnet-lite-0.5.0/setup.cfg
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      791 2023-05-24 22:03:34.000000 bpnet-lite-0.5.0/setup.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-28 18:49:44.904793 bpnet-lite-0.5.1/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1072 2023-05-18 00:41:39.000000 bpnet-lite-0.5.1/LICENSE
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      341 2023-05-28 18:49:44.900793 bpnet-lite-0.5.1/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6478 2023-05-18 06:03:42.000000 bpnet-lite-0.5.1/README.md
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    17119 2023-05-28 18:37:31.000000 bpnet-lite-0.5.1/bpnet
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-28 18:49:44.812793 bpnet-lite-0.5.1/bpnet_lite.egg-info/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      341 2023-05-28 18:49:43.000000 bpnet-lite-0.5.1/bpnet_lite.egg-info/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      433 2023-05-28 18:49:44.000000 bpnet-lite-0.5.1/bpnet_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2023-05-28 18:49:43.000000 bpnet-lite-0.5.1/bpnet_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      187 2023-05-28 18:49:44.000000 bpnet-lite-0.5.1/bpnet_lite.egg-info/requires.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       10 2023-05-28 18:49:44.000000 bpnet-lite-0.5.1/bpnet_lite.egg-info/top_level.txt
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-28 18:49:44.892793 bpnet-lite-0.5.1/bpnetlite/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      175 2023-05-28 18:48:52.000000 bpnet-lite-0.5.1/bpnetlite/__init__.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    10849 2023-05-26 06:57:00.000000 bpnet-lite-0.5.1/bpnetlite/attributions.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    16333 2023-05-20 18:27:46.000000 bpnet-lite-0.5.1/bpnetlite/bpnet.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9078 2023-05-24 00:23:23.000000 bpnet-lite-0.5.1/bpnetlite/chrombpnet.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    17389 2023-05-23 04:09:48.000000 bpnet-lite-0.5.1/bpnetlite/io.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1643 2023-05-18 00:41:39.000000 bpnet-lite-0.5.1/bpnetlite/logging.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     2418 2023-05-18 00:41:39.000000 bpnet-lite-0.5.1/bpnetlite/losses.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    10643 2023-05-27 23:19:47.000000 bpnet-lite-0.5.1/bpnetlite/marginalize.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9144 2023-05-18 00:41:39.000000 bpnet-lite-0.5.1/bpnetlite/negatives.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13599 2023-05-18 00:41:39.000000 bpnet-lite-0.5.1/bpnetlite/performance.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12528 2023-05-27 20:51:47.000000 bpnet-lite-0.5.1/chrombpnet
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2023-05-28 18:49:44.904793 bpnet-lite-0.5.1/setup.cfg
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      824 2023-05-28 18:48:42.000000 bpnet-lite-0.5.1/setup.py
```

### Comparing `bpnet-lite-0.5.0/LICENSE` & `bpnet-lite-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/README.md` & `bpnet-lite-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/bpnet` & `bpnet-lite-0.5.1/bpnet`

 * *Files 2% similar despite different names*

```diff
@@ -1,74 +1,93 @@
 #!/usr/bin/env python
 # BPNet command-line tool
 # Author: Jacob Schreiber <jmschreiber91@gmail.com>
 
 import os
+os.environ['TORCH_CUDNN_V8_API_ENABLED'] = '1'
+
 import sys
 import numpy
 import torch
 import pyfaidx
 import argparse
 
 from bpnetlite import BPNet
 from bpnetlite.io import PeakGenerator
 from bpnetlite.io import extract_loci
 
 from bpnetlite.attributions import calculate_attributions
 from bpnetlite.marginalize import marginalization_report
 
 from bpnetlite.negatives import extract_matching_loci
+from bpnetlite.negatives import calculate_gc_genomewide
 
 import pandas
 import pyBigWig
 import json
 
+torch.backends.cudnn.benchmark = True
+
+
 desc = """BPNet is an neural network primarily composed of dilated residual
 	convolution layers for modeling the associations between biological
 	sequences and biochemical readouts. This tool will take in a fasta
 	file for the sequence, a bed file for signal peak locations, and bigWig
 	files for the signal to predict and the control signal, and train a
 	BPNet model for you."""
 
 _help = """Must be either 'negatives', 'fit', 'predict', 'interpret',
 	'marginalize', or 'pipeline'."""
 
+
 # Read in the arguments
 parser = argparse.ArgumentParser(description=desc)
 subparsers = parser.add_subparsers(help=_help, required=True, dest='cmd')
 
-negatives_parser = subparsers.add_parser("negatives", help="Sample GC-matched negatives.")
-negatives_parser.add_argument("-i", "--peaks", required=True, help="Peak bed file.")
+negatives_parser = subparsers.add_parser("negatives", 
+	help="Sample GC-matched negatives.")
+negatives_parser.add_argument("-i", "--peaks", required=True, 
+	help="Peak bed file.")
 negatives_parser.add_argument("-f", "--fasta", help="Genome FASTA file.")
-negatives_parser.add_argument("-b", "--bigwig", required=True, help="GC content bigwig.")
-negatives_parser.add_argument("-o", "--output", required=True, help="Output bed file.")
-negatives_parser.add_argument("-l", "--bin_width", type=float, default=0.02, help="GC bin width to match.")
-negatives_parser.add_argument("-w", "--width", type=int, default=2114, help="Width for calculating GC content.")
-negatives_parser.add_argument("-v", "--verbose", default=True, action='store_true')
+negatives_parser.add_argument("-b", "--bigwig", required=True, 
+	help="GC content bigwig.")
+negatives_parser.add_argument("-o", "--output", required=True, 
+	help="Output bed file.")
+negatives_parser.add_argument("-l", "--bin_width", type=float, default=0.02, 
+	help="GC bin width to match.")
+negatives_parser.add_argument("-w", "--width", type=int, default=2114, 
+	help="Width for calculating GC content.")
+negatives_parser.add_argument("-v", "--verbose", default=True, 
+	action='store_true')
 
 fit_parser = subparsers.add_parser("fit", help="Fit a BPNet model.")
 fit_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for fitting the model.")
 
-predict_parser = subparsers.add_parser("predict", help="Make predictions using a trained BPNet model.")
+predict_parser = subparsers.add_parser("predict", 
+	help="Make predictions using a trained BPNet model.")
 predict_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for making predictions.")
 
-interpret_parser = subparsers.add_parser("interpret", help="Make interpretations using a trained BPNet model.")
+interpret_parser = subparsers.add_parser("interpret", 
+	help="Make interpretations using a trained BPNet model.")
 interpret_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for calculating attributions.")
 
-marginalize_parser = subparsers.add_parser("marginalize", help="Run marginalizations given motifs.")
+marginalize_parser = subparsers.add_parser("marginalize", 
+	help="Run marginalizations given motifs.")
 marginalize_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for calculating attributions.")
 
-pipeline_parser = subparsers.add_parser("pipeline", help="Run each step on the given files.")
+pipeline_parser = subparsers.add_parser("pipeline", 
+	help="Run each step on the given files.")
 pipeline_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters used for each step.")
 
+
 ###
 # Default Parameters
 ###
 
 default_fit_parameters = {
 	'n_filters': 64,
 	'n_layers': 8,
@@ -195,19 +214,20 @@
 	'output': 'profile',
 	'ohe_filename': None,
 	'attr_filename': None,
 	'n_shuffles':20,
 
 	'n_seqlets': 100000,
 	'modisco_filename': None,
+	'modisco_motifs': None,
 
-	'motifs': None,
 	'n_loci': None,
 	'shuffle': False,
 	'marginalization_filename': None,
+	'marginalization_motifs': None,
 	'minimal': True
 }
 
 
 ###
 # Commands
 ###
@@ -319,14 +339,18 @@
 		alpha=parameters['alpha'],
 		trimming=trimming,
 		name=parameters['name'],
 		verbose=parameters['verbose']).cuda()
 
 	optimizer = torch.optim.AdamW(model.parameters(), lr=parameters['lr'])
 
+	if parameters['verbose']:
+		print("Training Set Size: ", training_data.dataset.sequences.shape[0])
+		print("Validation Set Size: ", valid_sequences.shape[0])
+
 	model.fit(training_data, optimizer, X_valid=valid_sequences, 
 		X_ctl_valid=valid_controls, y_valid=valid_signals, 
 		max_epochs=parameters['max_epochs'], 
 		validation_iter=parameters['validation_iter'], 
 		batch_size=parameters['batch_size'])
 
 
@@ -479,15 +503,15 @@
 
 	name = '{}.bpnet.predict.json'.format(parameters['name'])
 	with open(name, 'w') as outfile:
 		outfile.write(json.dumps(predict_parameters, sort_keys=True, indent=4))
 
 	os.system("bpnet predict -p {}".format(name))
 	
-	
+
 	# Step 3: Interpret the validation set
 	if parameters['verbose']:
 		print("\nStep 3: Calculating attributions")
 
 	interpret_parameters = {key: parameters[key] for key in 
 		default_interpret_parameters if key in parameters}
 	interpret_parameters['chroms'] = parameters['validation_chroms']
@@ -531,26 +555,27 @@
 		print("\nStep 5: TF-MoDISco reports")
 
 	if parameters['modisco_filename'] is None:
 		parameters['modisco_filename'] = '{}_modisco/'.format(
 			parameters['name'])
 
 	os.system('modisco report -i {0} -o {1} -s {1} -m {2}'.format(modisco_name, 
-		parameters['modisco_filename'], parameters['motifs']))
+		parameters['modisco_filename'], parameters['modisco_motifs']))
 	
 
 	# Step 6: Marginalization experiments
 	if parameters['verbose']:
 		print("\nStep 6: Run marginalizations")
 
 	marginalize_parameters = {key: parameters[key] for key in 
 		default_marginalize_parameters if key in parameters}
 	marginalize_parameters['chroms'] = parameters['validation_chroms']
 	marginalize_parameters['loci'] = parameters['negatives']
 	marginalize_parameters['output_filename'] = parameters['marginalization_filename']
+	marginalize_parameters['motifs'] = parameters['marginalization_motifs']
 
 	if marginalize_parameters['output_filename'] is None:
 		marginalize_parameters['output_filename'] = '{}_marginalize/'.format(
 			parameters['name'])
 
 	name = '{}.bpnet.marginalize.json'.format(parameters['name'])
```

### Comparing `bpnet-lite-0.5.0/bpnetlite/attributions.py` & `bpnet-lite-0.5.1/bpnetlite/attributions.py`

 * *Files 3% similar despite different names*

```diff
@@ -271,42 +271,41 @@
 	if model_output == "profile":
 		wrapper = ProfileWrapper(model)
 	elif model_output == "count":
 		wrapper = CountWrapper(model)
 	else:
 		raise ValueError("model_output must be one of 'profile' or 'count'.")
 
-	ig = DeepLiftShap(wrapper)
+	X = X.cuda()
 
 	attributions = []
 	references = []
 	with torch.no_grad():
 		for i in trange(len(X), disable=not verbose):
-			X_ = X[i:i+1]
-			reference = dinucleotide_shuffle(X_[0], n_shuffles=n_shuffles, 
-				random_state=random_state).cuda()
+			ig = DeepLiftShap(wrapper)
 
-			X_ = X_.cuda()
+			reference = dinucleotide_shuffle(X[i].cpu(), n_shuffles=n_shuffles, 
+				random_state=random_state).cuda()
 
 			if args is None:
 				args_ = None
 			else:
 				args_ = tuple([arg[i:i+1].cuda() for arg in args])
-						
-			attr = ig.attribute(X_, reference, target=0, 
+					
+			attr = ig.attribute(X[i:i+1], reference, target=0, 
 				additional_forward_args=args_, 
 				custom_attribution_func=hypothetical_attributions)
 
 			if not hypothetical:
-				attr = (attr * X_)
+				attr = (attr * X[i:i+1])
 			
 			if return_references:
 				references.append(reference.unsqueeze(0))
 
-			attributions.append(attr.cpu())
+			attributions.append(attr.cpu().detach())
 
 	attributions = torch.cat(attributions)
 
 	if return_references:
 		return attributions, torch.cat(references)
 	return attributions
```

### Comparing `bpnet-lite-0.5.0/bpnetlite/bpnet.py` & `bpnet-lite-0.5.1/bpnetlite/bpnet.py`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/bpnetlite/chrombpnet.py` & `bpnet-lite-0.5.1/bpnetlite/chrombpnet.py`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/bpnetlite/io.py` & `bpnet-lite-0.5.1/bpnetlite/io.py`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/bpnetlite/logging.py` & `bpnet-lite-0.5.1/bpnetlite/logging.py`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/bpnetlite/losses.py` & `bpnet-lite-0.5.1/bpnetlite/losses.py`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/bpnetlite/negatives.py` & `bpnet-lite-0.5.1/bpnetlite/negatives.py`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/bpnetlite/performance.py` & `bpnet-lite-0.5.1/bpnetlite/performance.py`

 * *Files identical despite different names*

### Comparing `bpnet-lite-0.5.0/chrombpnet` & `bpnet-lite-0.5.1/chrombpnet`

 * *Files 3% similar despite different names*

```diff
@@ -28,49 +28,53 @@
 	of the bias model and accessibility model and making predictions using it.
 	After training, the accessibility model can be used using the `bpnet`
 	tool."""
 
 _help = """Must be either 'fit', 'predict', 'interpret', 'marginalize', 
 	or 'pipeline'."""
 
+
 # Read in the arguments
 parser = argparse.ArgumentParser(description=desc)
 subparsers = parser.add_subparsers(help=_help, required=True, dest='cmd')
 
 train_parser = subparsers.add_parser("fit", help="Fit a BPNet model.")
 train_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for fitting the model.")
 
-predict_parser = subparsers.add_parser("predict", help="Make predictions using a trained BPNet model.")
+predict_parser = subparsers.add_parser("predict", 
+	help="Make predictions using a trained BPNet model.")
 predict_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for making predictions.")
 
-interpret_parser = subparsers.add_parser("interpret", help="Make interpretations using a trained BPNet model.")
+interpret_parser = subparsers.add_parser("interpret", 
+	help="Make interpretations using a trained BPNet model.")
 interpret_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for calculating attributions.")
 
-marginalize_parser = subparsers.add_parser("marginalize", help="Run marginalizations given motifs.")
+marginalize_parser = subparsers.add_parser("marginalize", 
+	help="Run marginalizations given motifs.")
 marginalize_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters for calculating attributions.")
 
-pipeline_parser = subparsers.add_parser("pipeline", help="Run each step on the given files.")
+pipeline_parser = subparsers.add_parser("pipeline", 
+	help="Run each step on the given files.")
 pipeline_parser.add_argument("-p", "--parameters", type=str, required=True,
 	help="A JSON file containing the parameters used for each step.")
 
-bias_parser = subparsers.add_parser("bias", help="Fit a bias model.")
-bias_parser.add_argument("-p", "--parameters", type=str, required=True,
-	help="A JSON file containing the parameters for fitting the model.")
 
 ###
 # Default Parameters
 ###
 
 default_fit_parameters = {
-	'n_filters': 64,
+	'n_filters': 256,
 	'n_layers': 8,
+	'bias_n_filters': 256,
+	'bias_n_layers': 4,
 	'profile_output_bias': True,
 	'count_output_bias': True,
 	'name': None,
 	'batch_size': 64,
 	'in_window': 2114,
 	'out_window': 1000,
 	'max_jitter': 128,
@@ -151,14 +155,16 @@
 	'minimal': True
 }
 
 default_pipeline_parameters = {
 	# Model architecture parameters
 	'n_filters': 64,
 	'n_layers': 8,
+	'bias_n_filters': 64,
+	'bias_n_layers': 4,
 	'profile_output_bias': True,
 	'count_output_bias': True,
 	'in_window': 2114,
 	'out_window': 1000,
 	'name': None,
 	'model': None,
 	'bias_model': None,
@@ -195,19 +201,20 @@
 	'output': 'profile',
 	'ohe_filename': None,
 	'attr_filename': None,
 	'n_shuffles':20,
 
 	'n_seqlets': 100000,
 	'modisco_filename': None,
+	'modisco_motifs': None,
 
-	'motifs': None,
 	'n_loci': None,
 	'shuffle': False,
 	'marginalization_filename': None,
+	'marginalization_motifs': None,
 	'minimal': True
 }
 
 
 ###
 # Commands
 ###
@@ -275,14 +282,16 @@
 
 	trimming = (parameters['in_window'] - parameters['out_window']) // 2
 
 	if parameters['bias_model'] is None:
 		bias_fit_parameters = {key: parameters[key] for key in 
 			default_fit_parameters}
 		bias_fit_parameters['loci'] = parameters['negatives']
+		bias_fit_parameters['n_layers'] = parameters['bias_n_layers']
+		bias_fit_parameters['n_filters'] = parameters['bias_n_filters']
 
 		min_counts = training_data.dataset.signals.sum(dim=(1, 2)).min().item()
 			
 		name = '{}.chrombpnet.bias.fit.json'.format(parameters['name'])
 		bias_fit_parameters['max_counts'] = min_counts * parameters['beta']
 		bias_fit_parameters['name'] = parameters['name'] + '.bias'
 		parameters['bias_model'] = bias_fit_parameters['name'] + '.torch'
```

### Comparing `bpnet-lite-0.5.0/setup.py` & `bpnet-lite-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='bpnet-lite',
-    version='0.5.0',
+    version='0.5.1',
     author='Jacob Schreiber',
     author_email='jmschreiber91@gmail.com',
     packages=['bpnetlite'],
     scripts=['bpnet', 'chrombpnet'],
     url='https://github.com/jmschrei/bpnet-lite',
     license='LICENSE.txt',
     description='bpnet-lite is a minimal implementation of BPNet, a neural network aimed at interpreting regulatory activity of the genome.',
@@ -18,10 +18,11 @@
         "torch >= 1.9.0",
         "h5py >= 3.7.0",
         "pyfaidx >= 0.7.2.1",
         "tqdm >= 4.64.1",
         "numba >= 0.55.1",
         "logomaker",
         "captum == 0.5.0",
-        "seaborn >= 0.11.2"
+        "seaborn >= 0.11.2",
+        "modisco-lite >= 2.0.0"
     ],
 )
```

