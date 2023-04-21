# Comparing `tmp/StORF-Reporter-0.7.4.tar.gz` & `tmp/StORF-Reporter-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StORF-Reporter-0.7.4.tar", last modified: Fri Mar 10 12:14:47 2023, max compression
+gzip compressed data, was "StORF-Reporter-0.7.5.tar", last modified: Fri Apr 21 15:09:58 2023, max compression
```

## Comparing `StORF-Reporter-0.7.4.tar` & `StORF-Reporter-0.7.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-10 12:14:47.006589 StORF-Reporter-0.7.4/
--rw-r--r--   0 nick      (1000) nick      (1000)    35149 2021-12-28 14:08:10.000000 StORF-Reporter-0.7.4/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)    18560 2023-03-10 12:14:47.006589 StORF-Reporter-0.7.4/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    17916 2023-03-10 12:12:41.000000 StORF-Reporter-0.7.4/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-16 17:48:19.000000 StORF-Reporter-0.7.4/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1078 2023-03-10 12:14:47.006589 StORF-Reporter-0.7.4/setup.cfg
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-10 12:14:47.002589 StORF-Reporter-0.7.4/src/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-10 12:14:47.006589 StORF-Reporter-0.7.4/src/StORF_Reporter/
--rw-r--r--   0 nick      (1000) nick      (1000)       33 2023-03-10 12:13:16.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/Constants.py
--rw-r--r--   0 nick      (1000) nick      (1000)    16604 2023-02-04 14:01:43.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/StORF_Extractor.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    47414 2023-03-06 17:57:58.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/StORF_Finder.py
--rw-r--r--   0 nick      (1000) nick      (1000)    52062 2023-02-21 14:38:36.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/StORF_Reporter.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-10 12:14:47.006589 StORF-Reporter-0.7.4/src/StORF_Reporter/Tools/
--rw-r--r--   0 nick      (1000) nick      (1000)     2076 2022-09-29 20:25:03.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/Tools/StORF_Adder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-09-29 20:25:03.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/Tools/UR_Lenghts.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-09-29 20:25:03.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/Tools/Un_StORFed.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-09-29 20:25:03.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/Tools/__init__.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    15171 2023-02-04 14:01:43.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/UR_Extractor.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-06 11:38:05.000000 StORF-Reporter-0.7.4/src/StORF_Reporter/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-03-10 12:14:47.006589 StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)    18560 2023-03-10 12:14:46.000000 StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      659 2023-03-10 12:14:46.000000 StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-03-10 12:14:46.000000 StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      220 2023-03-10 12:14:46.000000 StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-03-10 12:14:46.000000 StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-03-10 12:14:46.000000 StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/top_level.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/
+-rw-r--r--   0 nick      (1000) nick      (1000)    35149 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/LICENSE
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18560 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    17916 2023-04-21 15:09:20.000000 StORF-Reporter-0.7.5/README.md
+-rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-19 15:34:48.000000 StORF-Reporter-0.7.5/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1078 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/src/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/src/StORF_Reporter/
+-rw-r--r--   0 nick      (1000) nick      (1000)       33 2023-04-21 15:09:20.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Constants.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16604 2023-03-28 18:56:17.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Extractor.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    47414 2023-03-28 18:56:17.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Finder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    52170 2023-04-21 15:07:12.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Reporter.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2076 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/StORF_Adder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/UR_Lenghts.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/Un_StORFed.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:53.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/__init__.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    15171 2023-03-28 18:56:17.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/UR_Extractor.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-06 19:37:38.000000 StORF-Reporter-0.7.5/src/StORF_Reporter/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-21 15:09:58.084600 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18560 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      659 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      220 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-04-21 15:09:58.000000 StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/top_level.txt
```

### Comparing `StORF-Reporter-0.7.4/LICENSE` & `StORF-Reporter-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.4/PKG-INFO` & `StORF-Reporter-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 0.7.4
+Version: 0.7.5
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
 
-# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.4.
+# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.5.
 ### This will also install the python-standard library numpy (>=1.22.0,<1.24.0), Pyrodigal - (https://github.com/althonos/pyrodigal) and ORForise (https://github.com/NickJD/ORForise). 
 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of StORF-Reporter.
 
 ## Please Note: To report Con-StORFs (Pseudogenes and genes that have alternative use of stop codons), use "-con_storfs True". To disable the reporting of StORFs use "-con_only". 
 
 ### The directory "Test_Datasets" is provided to confirm functionality of StORF-Reporter.
@@ -70,15 +70,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Reporter Run Parameters.
+StORF-Reporter v0.7.5: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -180,15 +180,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: UR-Extractor Run Parameters.
+StORF-Reporter v0.7.5: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -218,15 +218,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Finder Run Parameters.
+StORF-Reporter v0.7.5: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -282,15 +282,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Extractor Run Parameters.
+StORF-Reporter v0.7.5: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
```

### Comparing `StORF-Reporter-0.7.4/README.md` & `StORF-Reporter-0.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # StORF-Reporter - Preprint: https://www.biorxiv.org/content/10.1101/2022.03.31.486628v3
 
 ### StORF-Reporter, a toolkit that returns missed CDS genes from the Unannotated Regions (URs) of prokaryotic genomes.
 
-# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.4.
+# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.5.
 ### This will also install the python-standard library numpy (>=1.22.0,<1.24.0), Pyrodigal - (https://github.com/althonos/pyrodigal) and ORForise (https://github.com/NickJD/ORForise). 
 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of StORF-Reporter.
 
 ## Please Note: To report Con-StORFs (Pseudogenes and genes that have alternative use of stop codons), use "-con_storfs True". To disable the reporting of StORFs use "-con_only". 
 
 ### The directory "Test_Datasets" is provided to confirm functionality of StORF-Reporter.
@@ -55,15 +55,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Reporter Run Parameters.
+StORF-Reporter v0.7.5: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -165,15 +165,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: UR-Extractor Run Parameters.
+StORF-Reporter v0.7.5: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -203,15 +203,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Finder Run Parameters.
+StORF-Reporter v0.7.5: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -267,15 +267,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Extractor Run Parameters.
+StORF-Reporter v0.7.5: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
```

### Comparing `StORF-Reporter-0.7.4/setup.cfg` & `StORF-Reporter-0.7.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = StORF-Reporter
-version = v0.7.4
+version = v0.7.5
 author = Nicholas Dimonaco
 author_email = nicholas@dimonaco.co.uk
 description = StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NickJD/StORF-Reporter
 project_urls =
```

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter/StORF_Extractor.py` & `StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Extractor.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter/StORF_Finder.py` & `StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Finder.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter/StORF_Reporter.py` & `StORF-Reporter-0.7.5/src/StORF_Reporter/StORF_Reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,22 +477,25 @@
                         FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
                     StORF_Num += 1
             if line != written_line:
                 Reporter_options.gff_outfile.write(line.strip()+'\n')
                 written_line = line
             StORFs = None
         elif line.startswith('##sequence-region') and first_region != True:
-            StORFs = find_after_StORFs(Reporter_options, Contig_URS, track_prev_start, track_prev_stop,
+            try:
+                StORFs = find_after_StORFs(Reporter_options, Contig_URS, track_prev_start, track_prev_stop,
                                        track_prev_contig)  # Changed to prev stop because we are switching from previous contig
-            if StORFs:
-                for StORF in StORFs:
-                    GFF_StoRF_write(Reporter_options, track_prev_contig, Reporter_options.gff_outfile, StORF, StORF_Num)  # To keep consistency
-                    if Reporter_options.annotation_type[1] == 'Out_Dir':
-                        FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
-                    StORF_Num += 1
+                if StORFs:
+                    for StORF in StORFs:
+                        GFF_StoRF_write(Reporter_options, track_prev_contig, Reporter_options.gff_outfile, StORF, StORF_Num)  # To keep consistency
+                        if Reporter_options.annotation_type[1] == 'Out_Dir':
+                            FASTA_StORF_write(Reporter_options, track_contig, fasta_outfile, StORF)
+                        StORF_Num += 1
+            except UnboundLocalError:
+                continue
             Reporter_options.gff_outfile.write(line.strip() + '\n')
 
         elif line.startswith('##FASTA'):
             Reporter_options.gff_outfile.write(line.strip() + '\n')
             end = True
             # StORFs = find_after_StORFs(StORF_options, Contig_URS, track_prev_start, track_prev_stop, track_prev_contig)  # Changed to prev stop because we are switching from previous contig
             # if StORFs:
```

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter/Tools/StORF_Adder.py` & `StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/StORF_Adder.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter/Tools/UR_Lenghts.py` & `StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/UR_Lenghts.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter/Tools/Un_StORFed.py` & `StORF-Reporter-0.7.5/src/StORF_Reporter/Tools/Un_StORFed.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter/UR_Extractor.py` & `StORF-Reporter-0.7.5/src/StORF_Reporter/UR_Extractor.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/PKG-INFO` & `StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 0.7.4
+Version: 0.7.5
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
 
-# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.4.
+# Please use `pip3 install StORF-Reporter' to install StORF-Reporter v0.7.5.
 ### This will also install the python-standard library numpy (>=1.22.0,<1.24.0), Pyrodigal - (https://github.com/althonos/pyrodigal) and ORForise (https://github.com/NickJD/ORForise). 
 
 ### Consider using '--no-cache-dir' with pip to ensure the download of the newest version of StORF-Reporter.
 
 ## Please Note: To report Con-StORFs (Pseudogenes and genes that have alternative use of stop codons), use "-con_storfs True". To disable the reporting of StORFs use "-con_only". 
 
 ### The directory "Test_Datasets" is provided to confirm functionality of StORF-Reporter.
@@ -70,15 +70,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Reporter Run Parameters.
+StORF-Reporter v0.7.5: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -180,15 +180,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: UR-Extractor Run Parameters.
+StORF-Reporter v0.7.5: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -218,15 +218,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Finder Run Parameters.
+StORF-Reporter v0.7.5: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -282,15 +282,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v0.7.4: StORF-Extractor Run Parameters.
+StORF-Reporter v0.7.5: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
```

### Comparing `StORF-Reporter-0.7.4/src/StORF_Reporter.egg-info/SOURCES.txt` & `StORF-Reporter-0.7.5/src/StORF_Reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

