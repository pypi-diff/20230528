# Comparing `tmp/StORF-Reporter-0.7.5.tar.gz` & `tmp/StORF-Reporter-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StORF-Reporter-0.7.5.tar", last modified: Fri Apr 21 15:09:58 2023, max compression
+gzip compressed data, was "StORF-Reporter-0.7.6.tar", last modified: Sun May 28 20:52:42 2023, max compression
```

## Comparing `StORF-Reporter-0.7.5.tar` & `StORF-Reporter-0.7.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/
--rw-r--r--   0 nick      (1000) nick      (1000)    35149 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)    18560 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    17916 2023-04-21 15:09:20.000000 StORF-Reporter-0.7.5/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-19 15:34:48.000000 StORF-Reporter-0.7.5/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1078 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/setup.cfg
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/src/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/src/StORF_Reporter/
--rw-r--r--   0 nick      (1000) nick      (1000)       33 2023-04-21 15:09:20.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Constants.py
--rw-r--r--   0 nick      (1000) nick      (1000)    16604 2023-03-28 18:56:17.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Extractor.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    47414 2023-03-28 18:56:17.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Finder.py
--rw-r--r--   0 nick      (1000) nick      (1000)    52170 2023-04-21 15:07:12.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Reporter.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/
--rw-r--r--   0 nick      (1000) nick      (1000)     2076 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/StORF_Adder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/UR_Lenghts.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/Un_StORFed.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/__init__.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    15171 2023-03-28 18:56:17.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/UR_Extractor.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-06 19:37:38.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)    18560 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      659 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      220 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/top_level.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:52:42.788776 StORF-Reporter-0.7.6/
+-rw-r--r--   0 nick      (1000) nick      (1000)    35149 2022-12-23 17:28:19.000000 StORF-Reporter-0.7.6/LICENSE
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-05-28 20:52:42.788776 StORF-Reporter-0.7.6/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    19279 2023-05-28 20:46:50.000000 StORF-Reporter-0.7.6/README.md
+-rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-23 17:28:19.000000 StORF-Reporter-0.7.6/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1128 2023-05-28 20:52:42.788776 StORF-Reporter-0.7.6/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:52:42.784776 StORF-Reporter-0.7.6/src/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:52:42.788776 StORF-Reporter-0.7.6/src/StORF_Reporter/
+-rw-r--r--   0 nick      (1000) nick      (1000)       33 2023-05-28 20:28:06.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/Constants.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16596 2023-05-28 20:30:57.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/StORF_Extractor.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    47406 2023-05-28 20:30:57.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/StORF_Finder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5306 2023-05-28 20:30:57.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/StORF_Remover.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    52243 2023-05-28 20:43:07.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/StORF_Reporter.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:52:42.788776 StORF-Reporter-0.7.6/src/StORF_Reporter/Tools/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2075 2023-05-28 20:30:57.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/Tools/StORF_Adder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-12-23 17:28:19.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/Tools/UR_Lenghts.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-12-23 17:28:19.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/Tools/Un_StORFed.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-23 17:28:19.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/Tools/__init__.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    15208 2023-05-28 20:36:27.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/UR_Extractor.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-07 16:36:44.000000 StORF-Reporter-0.7.6/src/StORF_Reporter/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-28 20:52:42.788776 StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-05-28 20:52:42.000000 StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      695 2023-05-28 20:52:42.000000 StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-28 20:52:42.000000 StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      269 2023-05-28 20:52:42.000000 StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-05-28 20:52:42.000000 StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-05-28 20:52:42.000000 StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/top_level.txt
```

### Comparing `StORF-Reporter-0.7.5/LICENSE` & `StORF-Reporter-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.5/PKG-INFO` & `StORF-Reporter-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 0.7.5
+Version: 0.7.6
 Summary: StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 Home-page: https://github.com/NickJD/StORF-Reporter
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/StORF-Reporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # StORF-Reporter - Preprint: https://www.biorxiv.org/content/10.1101/2022.03.31.486628v3
 
 ### StORF-Reporter, a toolkit that returns missed CDS genes from the Unannotated Regions (URs) of prokaryotic genomes.
 
-# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.5.
+# Please use `pip3 install StORF-Reporter' to install StORF-Reporter.
 ### This will also install the python-standard library numpy (>=1.22.0,<1.24.0), Pyrodigal - (https://github.com/althonos/pyrodigal) and ORForise (https://github.com/NickJD/ORForise). 
 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of StORF-Reporter.
 
 ## Please Note: To report Con-StORFs (Pseudogenes and genes that have alternative use of stop codons), use "-con_storfs True". To disable the reporting of StORFs use "-con_only". 
 
 ### The directory "Test_Datasets" is provided to confirm functionality of StORF-Reporter.
@@ -57,28 +57,31 @@
 
 #### To perform a fresh end-to-end annotation of a genome without an annotation, StORF-Reporter will use Pyrodigal to predict CDS genes and then supplement with StORFs. 
 ```console
 StORF-Reporter -anno Pyrodigal Single_FASTA -p .../Test_Datasets/Pyrodigal/E-coli.fa
 ```
 
 ### Menu - (StORF-Reporter -h):
+```console
+StORF-Reporter -anno Ensembl Single_Genome -p .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
+```
 ```python
 usage: StORF_Reporter.py [-h]
                          [-anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]]
                          [-p PATH] [-oname O_NAME] [-odir O_DIR] [-sout {True,False}] [-lw {True,False}] [-aa {True,False}]
                          [-gz {True,False}] [-py_train [{longest,individual,meta}]] [-py_fasta {True,False}]
                          [-py_unstorfed {True,False}] [-gene_ident GENE_IDENT] [-min_len MINLEN] [-max_len MAXLEN]
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.0: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -180,15 +183,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -218,15 +221,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.0: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -282,15 +285,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.0: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -303,9 +306,43 @@
 Misc:
   -verbose {True,False}
                         Default - False: Print out runtime messages
   -v                    Default - False: Print out version number and exit
 
 ```
 
+## StORF-Remover
+Subpackage to remove sequences reported by StORF-Reporter without a Blast/Diamond hit (any alignment in BLAST 6 format).
+
+### Menu - (StORF-Remover -h):   
+```console
+StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
+```
+
+```python
+usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
+                        [-verbose {True,False}] [-v]
+
+StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+
+Required Arguments:
+  -gff GFF              GFF annotation file for the FASTA
+  -blast BLAST          BLAST format 6 annotation file
+
+Optional Arguments:
+  -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
+
+Output:
+  -oname O_NAME         Default - Appends '_UR' to end of input GFF filename
+  -odir O_DIR           Default - Same directory as input GFF
+  -gz {True,False}      Default - False: Output as .gz
+
+Misc:
+  -verbose {True,False}
+                        Default - False: Print out runtime messages
+  -v                    Default - False: Print out version number and exit
+```
+
+
+
 ## Test Datasets: 
-### The directory 'Test_Datasets' contains GFF and FASTA files to test the installation and use of StORF-Reporter. 
+### The directory 'Test_Datasets' contains GFF and FASTA files to test the installation and use of StORF-Reporter - Example output files are also provided for comparison.
```

### Comparing `StORF-Reporter-0.7.5/README.md` & `StORF-Reporter-0.7.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # StORF-Reporter - Preprint: https://www.biorxiv.org/content/10.1101/2022.03.31.486628v3
 
 ### StORF-Reporter, a toolkit that returns missed CDS genes from the Unannotated Regions (URs) of prokaryotic genomes.
 
-# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.5.
+# Please use `pip3 install StORF-Reporter' to install StORF-Reporter.
 ### This will also install the python-standard library numpy (>=1.22.0,<1.24.0), Pyrodigal - (https://github.com/althonos/pyrodigal) and ORForise (https://github.com/NickJD/ORForise). 
 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of StORF-Reporter.
 
 ## Please Note: To report Con-StORFs (Pseudogenes and genes that have alternative use of stop codons), use "-con_storfs True". To disable the reporting of StORFs use "-con_only". 
 
 ### The directory "Test_Datasets" is provided to confirm functionality of StORF-Reporter.
@@ -42,28 +42,31 @@
 
 #### To perform a fresh end-to-end annotation of a genome without an annotation, StORF-Reporter will use Pyrodigal to predict CDS genes and then supplement with StORFs. 
 ```console
 StORF-Reporter -anno Pyrodigal Single_FASTA -p .../Test_Datasets/Pyrodigal/E-coli.fa
 ```
 
 ### Menu - (StORF-Reporter -h):
+```console
+StORF-Reporter -anno Ensembl Single_Genome -p .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
+```
 ```python
 usage: StORF_Reporter.py [-h]
                          [-anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]]
                          [-p PATH] [-oname O_NAME] [-odir O_DIR] [-sout {True,False}] [-lw {True,False}] [-aa {True,False}]
                          [-gz {True,False}] [-py_train [{longest,individual,meta}]] [-py_fasta {True,False}]
                          [-py_unstorfed {True,False}] [-gene_ident GENE_IDENT] [-min_len MINLEN] [-max_len MAXLEN]
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.0: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -165,15 +168,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -203,15 +206,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.0: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -267,15 +270,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.0: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -288,9 +291,43 @@
 Misc:
   -verbose {True,False}
                         Default - False: Print out runtime messages
   -v                    Default - False: Print out version number and exit
 
 ```
 
+## StORF-Remover
+Subpackage to remove sequences reported by StORF-Reporter without a Blast/Diamond hit (any alignment in BLAST 6 format).
+
+### Menu - (StORF-Remover -h):   
+```console
+StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
+```
+
+```python
+usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
+                        [-verbose {True,False}] [-v]
+
+StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+
+Required Arguments:
+  -gff GFF              GFF annotation file for the FASTA
+  -blast BLAST          BLAST format 6 annotation file
+
+Optional Arguments:
+  -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
+
+Output:
+  -oname O_NAME         Default - Appends '_UR' to end of input GFF filename
+  -odir O_DIR           Default - Same directory as input GFF
+  -gz {True,False}      Default - False: Output as .gz
+
+Misc:
+  -verbose {True,False}
+                        Default - False: Print out runtime messages
+  -v                    Default - False: Print out version number and exit
+```
+
+
+
 ## Test Datasets: 
-### The directory 'Test_Datasets' contains GFF and FASTA files to test the installation and use of StORF-Reporter. 
+### The directory 'Test_Datasets' contains GFF and FASTA files to test the installation and use of StORF-Reporter - Example output files are also provided for comparison.
```

### Comparing `StORF-Reporter-0.7.5/setup.cfg` & `StORF-Reporter-0.7.6/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = StORF-Reporter
-version = v0.7.5
+version = v0.7.6
 author = Nicholas Dimonaco
 author_email = nicholas@dimonaco.co.uk
 description = StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NickJD/StORF-Reporter
 project_urls = 
@@ -30,12 +30,13 @@
 
 [options.entry_points]
 console_scripts = 
 	StORF-Reporter = StORF_Reporter.StORF_Reporter:main
 	StORF-Finder = StORF_Reporter.StORF_Finder:main
 	UR-Extractor = StORF_Reporter.UR_Extractor:main
 	StORF-Extractor = StORF_Reporter.StORF_Extractor:main
+	StORF-Remover = StORF_Remover.StORF_Remover:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Extractor.py` & `StORF-Reporter-0.7.6/src/StORF_Reporter/StORF_Extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,24 +72,24 @@
             for storf, seq in dna_region_ur[3].items():
                 fasta_outfile.write('>Start=' + storf.split('_')[0] + ';Stop=' + storf.split('_')[1] + ';Frame=' +
                                 storf.split('_')[2] + storf.split(';')[1] + '\n' + seq + '\n')
     fasta_outfile.close()
 
 def write_gff(dna_regions,options,gff_outfile, gff):
     gff_outfile.write("##gff-version\t3\n#\tStORF-Extractor \n#\tRun Date:" + str(date.today()) + '\n')
-    gff_outfile.write('##StORF-Reporter ' + StORF_Reporter_Version + '\n')
+    gff_outfile.write('##Single_Genome ' + StORF_Reporter_Version + '\n')
     for seq_reg in dna_regions:
         gff_outfile.write('##sequence-region\t' + seq_reg + ' 1 ' + str(dna_regions[seq_reg][1]) + '\n')
     gff_outfile.write("##Original File: " + gff.split('/')[-1] + '\n\n')
     for dna_region, storf_data in dna_regions.items():
         #ur_ident = dna_region + options.ident
         if storf_data[3]:
             for storf, seq in storf_data[3].items():
 
-                entry = (dna_region + '\tStORF-Reporter\tCDS\t' + storf.split('_')[0] + '\t' + storf.split('_')[1]+ '\t.\t' +
+                entry = (dna_region + '\tSingle_Genome\tCDS\t' + storf.split('_')[0] + '\t' + storf.split('_')[1]+ '\t.\t' +
                          storf.split('_')[2].split(';')[0]  + '\t.\t' + storf.split(';',1)[1] + '\n')
                 gff_outfile.write(entry)
     gff_outfile.close()
 
 def fasta_load(fasta_in):
     dna_regions = collections.OrderedDict()
     first = True
@@ -238,30 +238,29 @@
 
     write_fasta(dna_regions, options.fasta_outfile)
     if options.gff_out != False:
         write_gff(dna_regions, options, options.gff_outfile, gff)
 
 def main():
 
-    parser = argparse.ArgumentParser(description='StORF-Reporter ' + StORF_Reporter_Version + ': StORF-Extractor Run Parameters.')
+    parser = argparse.ArgumentParser(description='Single_Genome ' + StORF_Reporter_Version + ': StORF-Extractor Run Parameters.')
     parser._action_groups.pop()
 
     required = parser.add_argument_group('Required Arguments')
     required.add_argument('-storf_input', action='store', dest='storf_input', required=False,
                         choices=['Combined', 'Separate'],
                         help='Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?\n')
     required.add_argument('-p', action='store', dest='path', default='', required=False,
-                        help='Provide input file or directory path')
+                        help='Provide input files or directory path')
 
     ### Not implemented yet
     # optional = parser.add_argument_group('Optional Arguments')
-    # optional.add_argument('-tool_ident', action='store', dest='tool_ident', default='StORF-Reporter',
-    #                         help='Default "StORF-Reporter": Tool-name Identifier used for extraction of StORFs or other genomic elements'
-    #                              ' "StORF-Reporter, Prodigal, Pyrodigal" (second GFF column)')
-
+    # optional.add_argument('-tool_ident', action='store', dest='tool_ident', default='Single_Genome',
+    #                         help='Default "Single_Genome": Tool-name Identifier used for extraction of StORFs or other genomic elements'
+    #                              ' "Single_Genome, Prodigal, Pyrodigal" (second GFF column)')
 
     output = parser.add_argument_group('Output')
     output.add_argument('-gff_out', action='store', dest='gff_out', default=False, type=eval, choices=[True, False],
                         help='Default - False: Output StORFs in GFF format')
     output.add_argument('-oname', action="store", dest='o_name', required=False,
                         help='Default - Appends \'_Extracted_StORFs\' to end of input GFF filename')
     output.add_argument('-odir', action="store", dest='o_dir', required=False,
@@ -275,24 +274,24 @@
                         help='Default - False: Print out runtime messages')
     misc.add_argument('-v', action='store_true', dest='version',
                         help='Default - False: Print out version number and exit')
 
 
 
     options = parser.parse_args()
-    options.tool_ident = ['StORF-Reporter']#options.tool_ident.split(',')
+    options.tool_ident = ['Single_Genome']#options.tool_ident.split(',')
 
 
     if options.storf_input == None or options.path == None:
         if options.version:
             sys.exit(StORF_Reporter_Version)
         else:
             exit('StORF-Extractor: error: the following arguments are required: -storf_input, -p')
 
-    print("Thank you for using StORF-Reporter -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
+    print("Thank you for using Single_Genome -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
           "Please report any issues to: https://github.com/NickJD/StORF-Reporter/issues\n#####")
 
 
     #### Output Directory and Filename handling
     if options.o_dir == None and options.o_name == None:
         tmp_extension = options.path.split('.')[-1]  # could be .fa/.fasta etc
         output_file = options.path.replace('.' + tmp_extension, '')
```

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Finder.py` & `StORF-Reporter-0.7.6/src/StORF_Reporter/StORF_Finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 gff_stop = str(stop - 3 + int(ur_name.split('_')[-2]))
                 if options.stop_inclusive == False:  # To remove the start and stop codon positions.
                     gff_stop = gff_stop - 3
                 frame = (int(gff_stop) % 3) + 4
 
             storf_name = native_seq + '_' + storf_Type + '_' + str(idx) + ':' + gff_start + '-' + gff_stop
 
-            gff_entries.append(native_seq.split('_UR')[0] + '\tStORF-Reporter\t' + options.feature_type + '\t' + gff_start + '\t' + gff_stop + '\t.\t' + data[2] +
+            gff_entries.append(native_seq.split('_UR')[0] + '\tSingle_Genome\t' + options.feature_type + '\t' + gff_start + '\t' + gff_stop + '\t.\t' + data[2] +
                 '\t.\tID=' + storf_name + ';UR=' + ur_name.replace('>','')  + ';UR_Stop_Locations=' + '-'.join(pos_) + ';Length=' + str(
                     length) + ';Strand=' + data[2] +
                 ';Frame=' + str(frame) + ';UR_Frame=' + str(ur_frame) +
                 ';Start_Stop=' + start_stop + ';Mid_Stop=' + mid_stop  + ';End_Stop=' + end_stop + ';StORF_Type=' + storf_Type + '\n')
 
             ### need to add - if con-storf then add middle stops
             fasta_entries.update({'>' + storf_name + ';UR=' + ur_name.replace('>','')  + ';UR_Stop_Locations=' + '-'.join(pos_) + ';Length=' +
@@ -613,15 +613,15 @@
             sequence_name = line.strip()
         elif line:
             seq += str(line)
             first = False
     sequences.update({sequence_name: [sequence_region_length,seq.strip()]})
     return sequence_regions, sequences
 
-## Function to control how StORF-Finder handles StORF-Reporter output
+## Function to control how StORF-Finder handles Single_Genome output
 def StORF_Reported(options, Contigs):
     Reporter_StORFs = collections.OrderedDict()
     for Contig_ID, Contig_URs in Contigs.items():
         Reporter_StORFs.update({Contig_ID:[]})
         URs = Contig_URs[3]
         try:
             for UR in URs:
@@ -641,15 +641,15 @@
         except TypeError:
             if options.verbose == True:
                 print("No URs in seq")
     return Reporter_StORFs
 
 
 def main():
-    parser = argparse.ArgumentParser(description='StORF-Reporter ' + StORF_Reporter_Version + ': StORF-Finder Run Parameters.')
+    parser = argparse.ArgumentParser(description='Single_Genome ' + StORF_Reporter_Version + ': StORF-Finder Run Parameters.')
     parser._action_groups.pop()
 
     required = parser.add_argument_group('Required Arguments')
     required.add_argument('-f', action="store", dest='fasta', required=False,
                         help='Input FASTA File - (UR_Extractor output)')
 
     optional = parser.add_argument_group('Optional Arguments')
@@ -732,15 +732,15 @@
 
     if options.fasta == None:
         if options.version:
             sys.exit(StORF_Reporter_Version)
         else:
             exit('StORF-Finder: error: the following arguments are required: -f')
 
-    print("Thank you for using StORF-Reporter -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
+    print("Thank you for using Single_Genome -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
           "Please report any issues to: https://github.com/NickJD/StORF-Reporter/issues\n#####")
 
 
     #ns_nt = defaultdict  # Used to Record non-standard nucleotides - not implemented yet
     ##### Load in fasta file
     sequences = OrderedDict()
     sequence_regions = []
@@ -769,31 +769,31 @@
         tmp_filename = options.fasta.split('/')[-1]  # could be .fa/.fasta etc
         output_file = options.fasta.replace(tmp_filename, '')
         output_file = output_file + options.o_name
 
     if not options.gz: # Clear fasta and gff files if not empty - Needs an elegant solution
         if not options.aa_only:
             gff_out = open(output_file + '.gff', 'w', newline='\n', encoding='utf-8')
-            gff_out.write("##gff-version\t3\n#\tStORF-Reporter - Stop ORF Predictions\n#\tRun Date:" + str(date.today()) + '\n')
-            gff_out.write('##StORF-Reporter ' + StORF_Reporter_Version + '\n')
+            gff_out.write("##gff-version\t3\n#\tSingle_Genome - Stop ORF Predictions\n#\tRun Date:" + str(date.today()) + '\n')
+            gff_out.write('##Single_Genome ' + StORF_Reporter_Version + '\n')
             for seq_reg in sequence_regions:
                 gff_out.write(seq_reg + '\n')
             gff_out.write("##Original File: " + options.fasta.split('/')[-1] + '\n\n')
             fasta_out = open(output_file + '.fasta', 'w', newline='\n', encoding='utf-8')
             if options.translate:
                 aa_fasta_out = open(output_file + '_aa.fasta', 'w', newline='\n', encoding='utf-8')
             else:
                 aa_fasta_out = None
         elif options.aa_only:
             aa_fasta_out = open(output_file + '_aa.fasta', 'w', newline='\n', encoding='utf-8')
     elif options.gz:
         if not options.aa_only:
             gff_out = gzip.open(output_file + '.gff.gz', 'wt', newline='\n', encoding='utf-8')
-            gff_out.write("##gff-version\t3\n#\tStORF-Reporter - Stop ORF Predictions\n#\tRun Date:" + str(date.today()) + '\n')
-            gff_out.write('##StORF-Reporter ' + StORF_Reporter_Version + '\n')
+            gff_out.write("##gff-version\t3\n#\tSingle_Genome - Stop ORF Predictions\n#\tRun Date:" + str(date.today()) + '\n')
+            gff_out.write('##Single_Genome ' + StORF_Reporter_Version + '\n')
             for seq_reg in sequence_regions:
                 gff_out.write(seq_reg + '\n')
             gff_out.write("##Original File: " + options.gff + '\n\n')
             fasta_out = gzip.open(output_file + '.fasta.gz', 'wt', newline='\n', encoding='utf-8')
             if options.translate:
                 aa_fasta_out = gzip.open(output_file + '_aa.fasta.gz', 'wt', newline='\n', encoding='utf-8')
             else:
```

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Reporter.py` & `StORF-Reporter-0.7.6/src/StORF_Reporter/StORF_Reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,18 +408,18 @@
                 fasta_outfile = open(Reporter_options.output_file + '.fasta', 'w', newline='\n', encoding='utf-8')
         elif Reporter_options.gz == True:
                 fasta_outfile = gzip.open(Reporter_options.output_file + '.fasta.gz', 'wt', newline='\n', encoding='utf-8')
         faa_infile = Reporter_options.gff.replace('.gff3', '.faa').replace('.gff','.faa')
         ffn_infile = Reporter_options.gff.replace('.gff3', '.ffn').replace('.gff','.ffn')
         Original_AA,Original_NT = FASTA_Load(faa_infile,ffn_infile)
     if Reporter_options.annotation_type[0] == 'Pyrodigal':
-        Reporter_options.gff_outfile.write('##Pyrodigal annotation and StORF-Reporter extended GFF annotation of ' + Reporter_options.fasta.split('/')[-1] + '\n')
+        Reporter_options.gff_outfile.write('##Pyrodigal annotation and Single_Genome extended GFF annotation of ' + Reporter_options.fasta.split('/')[-1] + '\n')
     else:
-        Reporter_options.gff_outfile.write('##StORF-Reporter extended annotation of ' + gff_name.split('/')[-1] + '\n')
-    Reporter_options.gff_outfile.write('##StORF-Reporter ' + StORF_Reporter_Version + '\n')
+        Reporter_options.gff_outfile.write('##Single_Genome extended annotation of ' + gff_name.split('/')[-1] + '\n')
+    Reporter_options.gff_outfile.write('##Single_Genome ' + StORF_Reporter_Version + '\n')
 
     first_region = True
     for line in gff_in.splitlines( ):
         if not line.startswith('#') and end == False:
             data = line.split('\t')
             track_current_start = int(data[3])
             track_current_stop = int(data[4])
@@ -477,25 +477,22 @@
                         FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
                     StORF_Num += 1
             if line != written_line:
                 Reporter_options.gff_outfile.write(line.strip()+'\n')
                 written_line = line
             StORFs = None
         elif line.startswith('##sequence-region') and first_region != True:
-            try:
-                StORFs = find_after_StORFs(Reporter_options, Contig_URS, track_prev_start, track_prev_stop,
+            StORFs = find_after_StORFs(Reporter_options, Contig_URS, track_prev_start, track_prev_stop,
                                        track_prev_contig)  # Changed to prev stop because we are switching from previous contig
-                if StORFs:
-                    for StORF in StORFs:
-                        GFF_StoRF_write(Reporter_options, track_prev_contig, Reporter_options.gff_outfile, StORF, StORF_Num)  # To keep consistency
-                        if Reporter_options.annotation_type[1] == 'Out_Dir':
-                            FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
-                        StORF_Num += 1
-            except UnboundLocalError:
-                continue
+            if StORFs:
+                for StORF in StORFs:
+                    GFF_StoRF_write(Reporter_options, track_prev_contig, Reporter_options.gff_outfile, StORF, StORF_Num)  # To keep consistency
+                    if Reporter_options.annotation_type[1] == 'Out_Dir':
+                        FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
+                    StORF_Num += 1
             Reporter_options.gff_outfile.write(line.strip() + '\n')
 
         elif line.startswith('##FASTA'):
             Reporter_options.gff_outfile.write(line.strip() + '\n')
             end = True
             # StORFs = find_after_StORFs(StORF_options, Contig_URS, track_prev_start, track_prev_stop, track_prev_contig)  # Changed to prev stop because we are switching from previous contig
             # if StORFs:
@@ -512,15 +509,15 @@
             Reporter_options.gff_outfile.write(line.strip()+'\n')
             written_line = line
 ##############################################################
 
 
 
 def main():
-    parser = argparse.ArgumentParser(description='StORF-Reporter ' + StORF_Reporter_Version + ': StORF-Reporter Run Parameters.', formatter_class=SmartFormatter)
+    parser = argparse.ArgumentParser(description='Single_Genome ' + StORF_Reporter_Version + ': Single_Genome Run Parameters.', formatter_class=SmartFormatter)
     parser._action_groups.pop()
 
     required = parser.add_argument_group('Required Options')
     required.add_argument('-anno', action='store', dest='annotation_type', required=False,
                         choices=['Prokka', 'Bakta', 'Out_Dir', 'Single_GFF', 'Multiple_GFFs', 'Ensembl', 'Feature_Types',
                                   'Single_Genome', 'Multiple_Genomes','Single_Combined_GFF', 'Multiple_Combined_GFFs',
                                  'Pyrodigal', 'Single_FASTA', 'Multiple_FASTA'], nargs='*',
@@ -547,15 +544,15 @@
                              '--- Complete Annotation Input Options: \n'
                              '\tSingle_FASTA = To provide a single FASTA file; \n'
                              '\tMultiple_FASTA = To provide a directory containing multiple FASTA files (will detect .fna,.fa,.fasta); \n\n')
 
     required.add_argument('-p', action='store', dest='path', default='', required=False,
                         help='Provide input file or directory path')
     ###
-    StORF_Reporter_args = parser.add_argument_group('StORF-Reporter Options')
+    StORF_Reporter_args = parser.add_argument_group('Single_Genome Options')
     ### Add options to redirect into new output directory and filename - and output StORFs on their own in their own GFF -
     StORF_Reporter_args.add_argument('-oname', action="store", dest='o_name', required=False,
                         help='Default - Appends \'_StORF-R\' to end of input FASTA filename - Multiple_* runs will be numbered')
     StORF_Reporter_args.add_argument('-odir', action="store", dest='o_dir', required=False,
                         help='Default -  Same directory as input FASTA')
     StORF_Reporter_args.add_argument('-sout', action="store", dest='storfs_out', default=False, type=eval, choices=[True, False],
                         help='Default - False: Print out StORF sequences separately from Prokka/Bakta annotations')
@@ -643,15 +640,15 @@
     #optional.add_argument('-comb', action='store', dest='combined_gffs', default='', required=False,
     #                    help='Provide directory containing GFFs with sequences combined into single file to be StORFed - Only produces modified GFFs')
 
     misc = parser.add_argument_group('Misc')
 
 
     misc.add_argument('-overwrite', action='store', dest='overwrite', default=False, type=eval, choices=[True, False],
-                        help='Default - False: Overwrite StORF-Reporter output if already present')
+                        help='Default - False: Overwrite Single_Genome output if already present')
     misc.add_argument('-verbose', action='store', dest='verbose', default=False, type=eval, choices=[True, False],
                         help='Default - False: Print out runtime messages')
     misc.add_argument('-v', action='store_true', dest='version',
                         help='Default - False: Print out version number and exit')
     misc.add_argument('-nout', action='store', dest='nout', default=True, type=eval, choices=[True, False],
                         help=argparse.SUPPRESS)
     misc.add_argument('-nout_pyrodigal', action='store', dest='nout_pyrodigal', default=True, type=eval, choices=[True, False],
@@ -661,28 +658,29 @@
     Reporter_options.gff_fasta = None # To be done
     Reporter_options.reporter = True
 
     if Reporter_options.annotation_type == None or Reporter_options.path == None:
         if Reporter_options.version:
             sys.exit(StORF_Reporter_Version)
         else:
-            exit('StORF-Reporter: error: the following arguments are required: -anno, -p')
-    print("Thank you for using StORF-Reporter -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
+            exit('Single_Genome: error: the following arguments are required: -anno, -p')
+    print("Thank you for using Single_Genome -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
           "Please report any issues to: https://github.com/NickJD/StORF-Reporter/issues\n#####")
 
     ##############
     ## Print out user chosen annotation options
 
     ##############
     ## Incompatible argument catching
     if len(Reporter_options.annotation_type) != 2:
         parser.error('Please select two compatible options for required argument -anno.')
     ##############
     #### Output Directory and Filename handling
     ### Add '/' to end of directory path
+    Reporter_options.path = os.path.abspath(Reporter_options.path) # If given relative path, convert to absolute path
     if Reporter_options.annotation_type[1] in ['Multiple_GFFs','Multiple_Genomes','Multiple_FASTA','Out_Dir','Comb_GFFs', 'Multiple_Combined_GFFs']:
         Reporter_options.path = Reporter_options.path + '/' if not Reporter_options.path.endswith('/') else Reporter_options.path
 
     if Reporter_options.o_dir == None and Reporter_options.o_name == None:
         if Reporter_options.annotation_type[1] == 'Out_Dir':
             output_file = Reporter_options.path#.split('.')[-1]
             output_file = output_file + output_file.split('/')[-2] + '_StORF-Reporter_Extended'
@@ -722,19 +720,19 @@
     ############## Setup for Prokka/Bakta output directory
     if Reporter_options.annotation_type[0] in ('Prokka','Bakta') and Reporter_options.annotation_type[1] == 'Out_Dir':
         Reporter_options.output_file = output_file
         #### Checking and cleaning
         for fname in os.listdir(Reporter_options.path):
             if '_StORF-Reporter_Extended' in fname and Reporter_options.overwrite == False:
                 parser.error(
-                    'Prokka/Bakta directory not clean and already contains a StORF-Reporter output. Please delete or use "-overwrite True" and try again.')
+                    'Prokka/Bakta directory not clean and already contains a Single_Genome output. Please delete or use "-overwrite True" and try again.')
             elif '_StORF-Reporter_Extended' in fname and Reporter_options.overwrite == True:
                 os.remove(Reporter_options.path + '/' + fname)
                 if Reporter_options.verbose == True:
-                    print('StORF-Reporter output ' + fname + ' will be overwritten.')
+                    print('Single_Genome output ' + fname + ' will be overwritten.')
         ####
         Reporter_options.gene_ident = "misc_RNA,gene,mRNA,CDS,rRNA,tRNA,tmRNA,CRISPR,ncRNA,regulatory_region,oriC,pseudo"
         Contigs, Reporter_options = run_UR_Extractor_Directory(Reporter_options)
         ################## Find StORFs in URs - Setup StORF_Reporter-Finder Run
         Reporter_StORFs = StORF_Reported(Reporter_options, Contigs)
         StORF_Filler(Reporter_options, Reporter_StORFs)
         if Reporter_options.verbose == True:
@@ -747,23 +745,23 @@
         elif Reporter_options.annotation_type[1]  == "Multiple_GFFs":
             gff_list = list(pathlib.Path(Reporter_options.path).glob('*.gff'))
             gff_list.extend(pathlib.Path(Reporter_options.path).glob('*.gff3'))
         #### Checking and cleaning
         gff_list = list(map(str, gff_list))
         gffs_to_filter = []
         for gff in gff_list:
-            if '_StORF-Reporter_Extended.gff' in gff and os.path.isfile(gff) and Reporter_options.overwrite == False:
+            if '_StORF-Reporter_Extended' in gff and os.path.isfile(gff) and Reporter_options.overwrite == False:
                 gffs_to_filter.append(gff)
                 gffs_to_filter.append(gff.replace('_StORF-Reporter_Extended.gff','.gff'))
-                print('Prokka/Bakta GFF has already been processed and a StORF-Reporter output exists for ' + gff.split('/')[-1] + '. Please delete or use "-overwrite True" and try again.')
-            elif '_StORF-Reporter_Extended.gff' in gff and os.path.isfile(gff) and Reporter_options.overwrite == True:
+                print('GFF has already been processed and a Single_Genome output exists for ' + gff.split('/')[-1] + '. Please delete or use "-overwrite True" and try again.')
+            elif '_StORF-Reporter_Extended' in gff and os.path.isfile(gff) and Reporter_options.overwrite == True:
                 os.remove(gff)
                 gffs_to_filter.append(gff)
                 if Reporter_options.verbose == True:
-                    print('StORF-Reporter output '  + gff.split('/')[-1] +  ' will be overwritten.')
+                    print('Single_Genome output '  + gff.split('/')[-1] +  ' will be overwritten.')
         gff_list = [x for x in gff_list if x not in gffs_to_filter]
         ####
         Reporter_options.gene_ident = "misc_RNA,gene,mRNA,CDS,rRNA,tRNA,tmRNA,CRISPR,ncRNA,regulatory_region,oriC,pseudo"
         file_counter = 0
         for gff in gff_list:
             # Finalising output_file name
             if Reporter_options.annotation_type[1]  == "Multiple_GFFs" and Reporter_options.o_name != None:
@@ -779,15 +777,15 @@
             Contigs, Reporter_options = run_UR_Extractor_Matched(Reporter_options,gff) # used to be extended
             ################## Find StORFs in URs - Setup StORF_Reporter-Finder Run
             Reporter_StORFs = StORF_Reported(Reporter_options, Contigs)
             StORF_Filler(Reporter_options, Reporter_StORFs)
             if Reporter_options.verbose == True:
                 print("Finished: " + gff.split('/')[-1]) # Will add number of additional StORFs here
 
-    ################ Run StORF-Reporter on standardGFFs
+    ################ Run Single_Genome on standardGFFs
     elif Reporter_options.annotation_type[0] in ('Ensembl', 'Feature_Types'):
         if Reporter_options.annotation_type[0] == 'Ensembl':
             Reporter_options.gene_ident = "ID=gene"
         elif Reporter_options.annotation_type[0] == 'Feature_Types':
             Reporter_options.gene_ident = Reporter_options.gene_ident.split(',')
         ####
         if Reporter_options.annotation_type[1] in ("Single_Genome", "Single_Combined_GFF"):
@@ -797,33 +795,33 @@
             gff_list.extend(pathlib.Path(Reporter_options.path).glob('*.gff3'))
         else:
             parser.error('Please select two compatible options for required argument -anno.')
         #### Checking and cleaning
         gff_list = list(map(str, gff_list))
         gffs_to_filter = []
         for gff in gff_list:
-            if '_StORF-Reporter_Extended.gff' in gff and os.path.isfile(gff) and Reporter_options.overwrite == False:
+            if '_StORF-Reporter_Extended' in gff and os.path.isfile(gff) and Reporter_options.overwrite == False:
                 gffs_to_filter.append(gff)
                 gffs_to_filter.append(gff.replace('_StORF-Reporter_Extended.gff', '.gff'))
-                print('Prokka/Bakta GFF has already been processed and a StORF-Reporter output exists for ' +
+                print('GFF has already been processed and a Single_Genome output exists for ' +
                       gff.split('/')[-1] + '. Please delete or use "-overwrite True" and try again.')
-            elif '_StORF-Reporter_Extended.gff' in gff and os.path.isfile(gff) and Reporter_options.overwrite == True:
+            elif '_StORF-Reporter_Extended' in gff and os.path.isfile(gff) and Reporter_options.overwrite == True:
                 os.remove(gff)
                 gffs_to_filter.append(gff)
                 if Reporter_options.verbose == True:
-                    print('StORF-Reporter output ' + gff.split('/')[-1] + ' will be overwritten.')
+                    print('Single_Genome output ' + gff.split('/')[-1] + ' will be overwritten.')
         gff_list = [x for x in gff_list if x not in gffs_to_filter]
         ####
         file_counter = 0
         for gff in gff_list:
             # Finalising output_file name
-            if Reporter_options.annotation_type[1]  == "Multiple_Combined_GFFs" and Reporter_options.o_name != None:
+            if (Reporter_options.annotation_type[1] == "Multiple_Combined_GFFs" or Reporter_options.annotation_type[1] == "Multiple_Genomes") and Reporter_options.o_name != None:
                 Reporter_options.output_file = output_file + '_' + str(file_counter)
                 file_counter += 1
-            elif Reporter_options.annotation_type[1]  == "Multiple_Combined_GFFs":
+            elif Reporter_options.annotation_type[1] == "Multiple_Combined_GFFs" or Reporter_options.annotation_type[1] == "Multiple_Genomes":
                 tmp_filename = gff.split('/')[-1].split('.gff')[0]  # could be .fa/.fasta etc
                 Reporter_options.output_file = output_file.replace('_StORF-Reporter',tmp_filename + '_StORF-Reporter')
             else:
                 Reporter_options.output_file = output_file
 
 
             if Reporter_options.verbose == True:
@@ -834,15 +832,15 @@
                 Contigs, Reporter_options = run_UR_Extractor_Matched(Reporter_options, gff)
             ################## Find StORFs in URs - Setup StORF_Reporter-Finder Run
             Reporter_StORFs = StORF_Reported(Reporter_options, Contigs)
             StORF_Filler(Reporter_options, Reporter_StORFs)
             if Reporter_options.verbose == True:
                 print("Finished: " + gff.split('/')[-1])  # Will add number of additional StORFs here`
 
-    ####### Run Pyrodigal and then StORF-Reporter on either a single or directory of FASTA files
+    ####### Run Pyrodigal and then Single_Genome on either a single or directory of FASTA files
     elif Reporter_options.annotation_type[0] == 'Pyrodigal' and Reporter_options.annotation_type[1] in ("Single_FASTA", "Multiple_FASTA"):  # needs cleaning
         Reporter_options.gene_ident = "gene"
         if os.path.isdir(Reporter_options.path) and Reporter_options.annotation_type[1]  == "Multiple_FASTA":
             fasta_list = list(pathlib.Path(Reporter_options.path).glob('*.fasta'))
             fasta_list.extend(list(pathlib.Path(Reporter_options.path).glob('*.fna')))
             fasta_list.extend(list(pathlib.Path(Reporter_options.path).glob('*.fa')))
             fasta_list = list(map(str, fasta_list))
```

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/StORF_Adder.py` & `StORF-Reporter-0.7.6/src/StORF_Reporter/Tools/StORF_Adder.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from ORForise.src.ORForise.GFF_Adder import gff_adder  # Calling from ORForise locally (StORF_Reporter and ORForise in same dir)
 
 
 
 
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description='StORF-Reporter v0.5.4: StORF-Adder Run Parameters.')
+    parser = argparse.ArgumentParser(description='Single_Genome v0.5.4: StORF-Adder Run Parameters.')
     parser.add_argument('-dna', '--genome_DNA', required=True, help='Genome DNA file (.fa) which both annotations '
                                                                     'are based on')
     parser.add_argument('-rt', '--reference_tool', required=False,
                         help='Which tool format to use as reference? - If not provided, will default to '
                              'standard Ensembl GFF format, can be Prodigal or any of the other tools available')
     parser.add_argument('-ref', '--reference_annotation', required=True,
                         help='Which reference annotation file to use as reference?')
```

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/UR_Lenghts.py` & `StORF-Reporter-0.7.6/src/StORF_Reporter/Tools/UR_Lenghts.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/Un_StORFed.py` & `StORF-Reporter-0.7.6/src/StORF_Reporter/Tools/Un_StORFed.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter/UR_Extractor.py` & `StORF-Reporter-0.7.6/src/StORF_Reporter/UR_Extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     from .Constants import *
 except (ModuleNotFoundError, ImportError, NameError, TypeError) as error:
     from Constants import *
 
 #Output FASTA and GFF separately using the same filename but with respective extensions - gz output optional
 def write_fasta(dna_regions, options, fasta_out):
     fasta_out.write("##\tUR-Extractor \n#\tRun Date:" + str(date.today()) + '\n')
-    fasta_out.write('##StORF-Reporter ' + StORF_Reporter_Version + '\n')
+    fasta_out.write('##Single_Genome ' + StORF_Reporter_Version + '\n')
     fasta_out.write("##Original Files: " + options.fasta.split('/')[-1] + ' | ' + options.gff.split('/')[-1] + '\n')
     for dna_region, dna_region_ur in dna_regions.items():
         fasta_out.write('\n##sequence-region\t' + dna_region + ' 1 ' + str(len(dna_region_ur[0])) + '\n')
         ur_ident = dna_region + options.ident # Add user ident onto name of dna regions
         if dna_region_ur[3]:
             for ex_ur, data in dna_region_ur[3].items():
                 original_ur = data[0]
                 ur_seq = data[1]
                 fasta_out.write('>' + ur_ident + '_' + ex_ur + '\n' + ur_seq + '\n')
     fasta_out.close()
 
 def write_gff(dna_regions,options,gff_out):
     gff_out.write("##gff-version\t3\n#\tUR-Extractor \n#\tRun Date:" + str(date.today()) + '\n')
-    gff_out.write('##StORF-Reporter ' + StORF_Reporter_Version + '\n')
+    gff_out.write('##Single_Genome ' + StORF_Reporter_Version + '\n')
     for seq_reg in dna_regions:
         gff_out.write('##sequence-region\t' + seq_reg + ' 1 ' + str(dna_regions[seq_reg][1]) + '\n')
     gff_out.write("##Original Files: " + options.fasta.split('/')[-1] + ' | ' + options.gff.split('/')[-1] + '\n\n')
     for dna_region, dna_region_ur in dna_regions.items():
         ur_ident = dna_region + options.ident
         if dna_region_ur[3]:
             for ex_ur, data in dna_region_ur[3].items():
@@ -105,15 +105,15 @@
                 except IndexError:
                     continue
     return dna_regions
 
 def gff_load(options,gff_in,dna_regions):
     for line in gff_in:  # Get gene loci from GFF - ID=Gene will also classify Pseudogenes as genes
         line_data = line.split()
-        if line.startswith('\n') or line.startswith('#'):  # Not to crash on empty lines in GFF
+        if line.startswith('\n') or line.startswith('#') or 'European Nucleotide Archive' in line:  # Not to crash on empty lines in GFF
             continue
         elif options.gene_ident[0] == 'ID=gene':
             if line_data[0] in dna_regions and options.gene_ident[0] in line_data[8]:
                 pos = line_data[3] + '_' + line_data[4]
                 dna_regions[line_data[0]][2].append(pos) # This will add to list
         else:
             try:
@@ -193,15 +193,15 @@
         write_gff(dna_regions, options, options.gff_out)
     else:
         return dna_regions
 
 
 def main():
 
-    parser = argparse.ArgumentParser(description='StORF-Reporter ' + StORF_Reporter_Version + ': UR-Extractor Run Parameters.')
+    parser = argparse.ArgumentParser(description='Single_Genome ' + StORF_Reporter_Version + ': UR-Extractor Run Parameters.')
     parser._action_groups.pop()
 
     required = parser.add_argument_group('Required Arguments')
     required.add_argument('-f', action='store', dest='fasta', required=False,
                         help='FASTA file for Unannotated Region seq extraction')
     required.add_argument('-gff', action='store', dest='gff', help='GFF annotation file for the FASTA',
                         required=False)
@@ -244,15 +244,15 @@
     options = parser.parse_args()
     if options.fasta == None or options.gff == None:
         if options.version:
             sys.exit(StORF_Reporter_Version)
         else:
             exit('UR-Extractor: error: the following arguments are required: -f, -gff')
 
-    print("Thank you for using StORF-Reporter -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
+    print("Thank you for using Single_Genome -- A detailed user manual can be found at https://github.com/NickJD/StORF-Reporter\n"
           "Please report any issues to: https://github.com/NickJD/StORF-Reporter/issues\n#####")
 
     options.annotation_type = [None,None]
 
     #### Output Directory and Filename handling
     if options.o_dir == None and options.o_name == None:
         tmp_extension = options.gff.split('.')[-1]
```

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/PKG-INFO` & `StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 0.7.5
+Version: 0.7.6
 Summary: StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 Home-page: https://github.com/NickJD/StORF-Reporter
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/StORF-Reporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # StORF-Reporter - Preprint: https://www.biorxiv.org/content/10.1101/2022.03.31.486628v3
 
 ### StORF-Reporter, a toolkit that returns missed CDS genes from the Unannotated Regions (URs) of prokaryotic genomes.
 
-# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.5.
+# Please use `pip3 install StORF-Reporter' to install StORF-Reporter.
 ### This will also install the python-standard library numpy (>=1.22.0,<1.24.0), Pyrodigal - (https://github.com/althonos/pyrodigal) and ORForise (https://github.com/NickJD/ORForise). 
 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of StORF-Reporter.
 
 ## Please Note: To report Con-StORFs (Pseudogenes and genes that have alternative use of stop codons), use "-con_storfs True". To disable the reporting of StORFs use "-con_only". 
 
 ### The directory "Test_Datasets" is provided to confirm functionality of StORF-Reporter.
@@ -57,28 +57,31 @@
 
 #### To perform a fresh end-to-end annotation of a genome without an annotation, StORF-Reporter will use Pyrodigal to predict CDS genes and then supplement with StORFs. 
 ```console
 StORF-Reporter -anno Pyrodigal Single_FASTA -p .../Test_Datasets/Pyrodigal/E-coli.fa
 ```
 
 ### Menu - (StORF-Reporter -h):
+```console
+StORF-Reporter -anno Ensembl Single_Genome -p .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
+```
 ```python
 usage: StORF_Reporter.py [-h]
                          [-anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]]
                          [-p PATH] [-oname O_NAME] [-odir O_DIR] [-sout {True,False}] [-lw {True,False}] [-aa {True,False}]
                          [-gz {True,False}] [-py_train [{longest,individual,meta}]] [-py_fasta {True,False}]
                          [-py_unstorfed {True,False}] [-gene_ident GENE_IDENT] [-min_len MINLEN] [-max_len MAXLEN]
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.0: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -180,15 +183,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -218,15 +221,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.0: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -282,15 +285,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.5: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.0: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -303,9 +306,43 @@
 Misc:
   -verbose {True,False}
                         Default - False: Print out runtime messages
   -v                    Default - False: Print out version number and exit
 
 ```
 
+## StORF-Remover
+Subpackage to remove sequences reported by StORF-Reporter without a Blast/Diamond hit (any alignment in BLAST 6 format).
+
+### Menu - (StORF-Remover -h):   
+```console
+StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
+```
+
+```python
+usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
+                        [-verbose {True,False}] [-v]
+
+StORF-Reporter v1.0.0: UR-Extractor Run Parameters.
+
+Required Arguments:
+  -gff GFF              GFF annotation file for the FASTA
+  -blast BLAST          BLAST format 6 annotation file
+
+Optional Arguments:
+  -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
+
+Output:
+  -oname O_NAME         Default - Appends '_UR' to end of input GFF filename
+  -odir O_DIR           Default - Same directory as input GFF
+  -gz {True,False}      Default - False: Output as .gz
+
+Misc:
+  -verbose {True,False}
+                        Default - False: Print out runtime messages
+  -v                    Default - False: Print out version number and exit
+```
+
+
+
 ## Test Datasets: 
-### The directory 'Test_Datasets' contains GFF and FASTA files to test the installation and use of StORF-Reporter. 
+### The directory 'Test_Datasets' contains GFF and FASTA files to test the installation and use of StORF-Reporter - Example output files are also provided for comparison.
```

### Comparing `StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/SOURCES.txt` & `StORF-Reporter-0.7.6/src/StORF_Reporter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/StORF_Reporter/Constants.py
 src/StORF_Reporter/StORF_Extractor.py
 src/StORF_Reporter/StORF_Finder.py
+src/StORF_Reporter/StORF_Remover.py
 src/StORF_Reporter/StORF_Reporter.py
 src/StORF_Reporter/UR_Extractor.py
 src/StORF_Reporter/__init__.py
 src/StORF_Reporter.egg-info/PKG-INFO
 src/StORF_Reporter.egg-info/SOURCES.txt
 src/StORF_Reporter.egg-info/dependency_links.txt
 src/StORF_Reporter.egg-info/entry_points.txt
```

