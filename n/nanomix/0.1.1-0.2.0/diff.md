# Comparing `tmp/nanomix-0.1.1.tar.gz` & `tmp/nanomix-0.2.0.tar.gz`

## Comparing `nanomix-0.1.1.tar` & `nanomix-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,35 @@
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 nanomix-0.1.1/Cargo.toml
--rw-rw----   0     3161     1159       30 2023-01-06 18:58:44.000000 nanomix-0.1.1/.gitignore
--rw-rw-r--   0     3161     1159     1067 2023-01-06 16:48:41.000000 nanomix-0.1.1/LICENSE
--rw-rw-r--   0     3161     1159     4300 2023-01-19 16:47:18.000000 nanomix-0.1.1/README.md
--rw-rw-r--   0     3161     1159 11674791 2023-01-17 21:20:50.000000 nanomix-0.1.1/atlases/25Array.tsv
--rw-rw----   0     3161     1159  1685159 2023-01-17 21:20:20.000000 nanomix-0.1.1/atlases/39Bisulfite.tsv
--rw-rw----   0     3161     1159     1031 2023-01-19 17:32:51.000000 nanomix-0.1.1/pyproject.toml
--rw-rw----   0     3161     1159      213 2023-01-18 21:18:48.000000 nanomix-0.1.1/python/nanomix/__init__.py
--rw-rw----   0     3161     1159     1757 2023-01-18 18:50:23.000000 nanomix-0.1.1/python/nanomix/atlas.py
--rw-rw----   0     3161     1159     7418 2023-01-19 15:05:27.000000 nanomix-0.1.1/python/nanomix/functions.py
--rw-rw----   0     3161     1159     9480 2023-01-19 15:01:26.000000 nanomix-0.1.1/python/nanomix/main.py
--rw-rw-r--   0     3161     1159     7570 2023-01-19 14:55:15.000000 nanomix-0.1.1/python/nanomix/models.py
--rw-rw----   0     3161     1159      140 2023-01-12 16:44:36.000000 nanomix-0.1.1/python/nanomix/run_tests.py
--rw-rw----   0     3161     1159     2255 2023-01-17 18:05:18.000000 nanomix-0.1.1/python/nanomix/tests/test_assign.py
--rw-rw----   0     3161     1159  1685159 2022-11-17 19:59:43.000000 nanomix-0.1.1/python/nanomix/tests/test_data/39Bisulfite.tsv
--rw-rw----   0     3161     1159       72 2023-01-19 15:02:28.000000 nanomix-0.1.1/python/nanomix/tests/test_data/sigma.tsv
--rw-rw----   0     3161     1159       69 2023-01-17 19:17:16.000000 nanomix-0.1.1/python/nanomix/tests/test_data/test_atlas.tsv
--rw-rw----   0     3161     1159     4351 2023-01-17 19:17:16.000000 nanomix-0.1.1/python/nanomix/tests/test_data/test_methylome.tsv
--rw-rw----   0     3161     1159       41 2023-01-17 19:17:16.000000 nanomix-0.1.1/python/nanomix/tests/test_data/test_sigma.tsv
--rw-rw----   0     3161     1159     2729 2023-01-19 16:20:41.000000 nanomix-0.1.1/python/nanomix/tests/test_deconvolute.py
--rw-rw----   0     3161     1159     2141 2023-01-13 15:48:19.000000 nanomix-0.1.1/python/nanomix/tests/test_evaluate.py
--rw-rw----   0     3161     1159     2446 2023-01-12 19:02:02.000000 nanomix-0.1.1/python/nanomix/tests/test_simulate.py
--rw-rw----   0     3161     1159      458 2023-01-18 18:50:00.000000 nanomix-0.1.1/python/nanomix/tools.py
--rw-rw----   0     3161     1159    16769 2023-01-18 22:06:19.000000 nanomix-0.1.1/src/lib.rs
--rw-rw----   0     3161     1159       41 2023-01-17 22:03:52.000000 nanomix-0.1.1/test_sigma.tsv
--rw-rw----   0     3161     1159    17022 2023-01-06 16:51:06.000000 nanomix-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     5052 1970-01-01 00:00:00.000000 nanomix-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 nanomix-0.2.0/Cargo.toml
+-rw-rw-r--   0     3161     1159     6148 2023-02-28 20:50:40.000000 nanomix-0.2.0/.DS_Store
+-rw-rw----   0     3161     1159     4096 2023-02-28 20:50:40.000000 nanomix-0.2.0/._.DS_Store
+-rw-rw----   0     3161     1159       30 2023-01-06 18:58:44.000000 nanomix-0.2.0/.gitignore
+-rw-rw-r--   0     3161     1159     1067 2023-01-06 16:48:41.000000 nanomix-0.2.0/LICENSE
+-rwxrwx--x   0     3161     1159     1275 2023-03-07 18:32:00.000000 nanomix-0.2.0/R/plot_bamstats.r
+-rwxrwxr-x   0     3161     1159     3730 2023-03-20 11:53:19.000000 nanomix-0.2.0/R/plot_scatter.r
+-rw-rw-r--   0     3161     1159     4977 2023-02-17 18:39:32.000000 nanomix-0.2.0/README.md
+-rw-rw-r--   0     3161     1159 11674791 2023-01-17 21:20:50.000000 nanomix-0.2.0/atlases/25Array.tsv
+-rw-rw----   0     3161     1159  1685159 2023-01-17 21:20:20.000000 nanomix-0.2.0/atlases/39Bisulfite.tsv
+-rw-rw----   0     3161     1159    43812 2023-02-20 15:22:06.000000 nanomix-0.2.0/err.txt
+-rw-rw----   0     3161     1159     1046 2023-04-21 17:06:28.000000 nanomix-0.2.0/pyproject.toml
+-rw-rw----   0     3161     1159      213 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/__init__.py
+-rw-rw----   0     3161     1159     4061 2023-04-12 19:46:40.000000 nanomix-0.2.0/python/nanomix/atlas.py
+-rw-rw----   0     3161     1159    12577 2023-04-12 16:32:47.000000 nanomix-0.2.0/python/nanomix/functions.py
+-rw-rw----   0     3161     1159    12024 2023-04-17 19:21:17.000000 nanomix-0.2.0/python/nanomix/main.py
+-rw-rw-r--   0     3161     1159     7945 2023-04-12 19:44:51.000000 nanomix-0.2.0/python/nanomix/models.py
+-rw-rw-r--   0     3161     1159    11632 2023-03-19 14:54:05.000000 nanomix-0.2.0/python/nanomix/plot.py
+-rw-rw----   0     3161     1159      140 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/run_tests.py
+-rw-rw----   0     3161     1159     2312 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_assign.py
+-rw-rw----   0     3161     1159  1807073 2023-02-15 16:55:03.000000 nanomix-0.2.0/python/nanomix/tests/test_data/39Bisulfite-endothelial.tsv
+-rw-rw-r--   0     3161     1159  1684170 2023-02-20 19:03:12.000000 nanomix-0.2.0/python/nanomix/tests/test_data/39Bisulfite.tsv
+-rw-rw----   0     3161     1159       69 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_data/test_atlas.tsv
+-rw-rw----   0     3161     1159     3166 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_data/test_methylome.tsv
+-rw-rw----   0     3161     1159       41 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_data/test_sigma.tsv
+-rw-rw----   0     3161     1159     2812 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_deconvolute.py
+-rw-rw----   0     3161     1159     2198 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_evaluate.py
+-rw-rw----   0     3161     1159     2032 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_load_atlas.py
+-rw-rw----   0     3161     1159     3216 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_mmse.py
+-rw-rw----   0     3161     1159     2500 2023-03-06 22:39:43.000000 nanomix-0.2.0/python/nanomix/tests/test_simulate.py
+-rw-rw----   0     3161     1159     2126 2023-04-12 16:23:29.000000 nanomix-0.2.0/python/nanomix/tools.py
+-rw-rw----   0     3161     1159    25223 2023-03-23 17:12:37.000000 nanomix-0.2.0/src/lib.rs
+-rw-rw----   0     3161     1159       41 2023-01-17 22:03:52.000000 nanomix-0.2.0/test_sigma.tsv
+-rw-rw----   0     3161     1159    21780 2023-04-21 16:53:22.000000 nanomix-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     5774 1970-01-01 00:00:00.000000 nanomix-0.2.0/PKG-INFO
```

### Comparing `nanomix-0.1.1/Cargo.toml` & `nanomix-0.2.0/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nanomix"
-version = "0.1.0"
+version = "0.2.0"
 edition = "2021"
 
 [package.metadata.maturin]
 name = "nanomix._nanomix"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
@@ -18,7 +18,9 @@
 clap = "2.33.0"
 probability = "0.15.5"
 rand = "0.5.6"
 csv = "1.1.6"
 ndarray = "0.15.4"
 rulinalg = "0.4.2"
 intervaltree = "0.2.7"
+logaddexp = "0.1.1"
+statrs = "0.16.0"
```

### Comparing `nanomix-0.1.1/LICENSE` & `nanomix-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomix-0.1.1/README.md` & `nanomix-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,76 +4,84 @@
 
 
 ## Installation
 This package is available on PyPI
 ```
 pip install nanomix
 ```
-or alternatively on Conda:
+Alternatively you can install from source. Installing from source requires [maturin](https://github.com/PyO3/maturin)
 ```
-conda install nanomix
-```
-Installing from source requires [maturin](https://github.com/PyO3/maturin)
-```
-conda install maturin
+pip install maturin
 git clone https://github.com/Jonbroad15/nanomix.git
 cd nanomix
 maturin develop
 ```
 
 ## Usage
+### Reference Atlas
+Deconvolution determines the mixture proportion based on methylation propensities of previously resolved sequencing runs of purified reference cells across the genome. This information is collated into an *atlas*. We suggest using the atlas from [Loyfer et. al](https://www.biorxiv.org/content/10.1101/2022.01.24.477547v1.full) which we have curated and labelled as `39Bisulfite.tsv` and is set for default. Their tool [wgbstools](https://github.com/nloyfer/wgbs_tools) also provides the means to create an atlas suited to the cell types you are interested in.
+
+### Deconvolution
 To deconvolute a sequencing run, one must simply provide `nanomix` with a methylome. We define a methylome as a `tsv` file with columns `{chr, start, end, total_calls, modified_calls}`. Such a file can be created from a `.bam` file using our associated program, [mbtools](https://github.com/jts/mbtools)
-Then the mixture proportion can be found by calling:
 ```
-nanomix deconvolute <METHYLOME>
+mbtools region-frequency -r ATLAS.tsv SAMPLE.bam > METHYLOME.tsv
 ```
-
-### Reference Atlas
-Deconvolution determines the mixture proportion based on methylation propensities of previously resolved sequencing runs of purified reference cells across the genome. This information is collated into an *atlas*. We suggest using the atlas from [Loyfer et. al](https://www.biorxiv.org/content/10.1101/2022.01.24.477547v1.full) which we have curated and labelled as `39Bisulfite.tsv` and is set for default. Their tool [wgbstools](https://github.com/nloyfer/wgbs_tools) also provides the means to create an atlas suited to the cell types you are interested in.
+Then the mixture proportion can be found by calling:
 ```
-nanomix deconvolute <METHYLOME> -a <ATLAS>
+nanomix deconvolute -a ATLAS.tsv METHYLOME.tsv
 ```
 
 ### Model
 We provide four deconvolution models
 
-- **llse (default):**   log-likelihood with sequencing errors. Maximize the likelihood of the methylome, atlas and sigma
+- **llse (default):**   log-likelihood with sequencing errors. Maximize the likelihood of sigma
                     by assuming modification calls follow a binomial distribution. Good for sequencing data with high error
-                    rate and non-uniform coverage distribution. (Oxford Nanopore)
+                    rate. (Oxford Nanopore)
 - **nnls:**             non-negative least squares. Minimize the squared error between the methylome and what we expect for
                     the methylome (given sigma and the atlas). Recommended for fast deconvolution of methylomes with high
                     coverage. (Methylation Arrays)
+- **llsp:**             log-likelihood with sequencing perfect. Same as llse, without error modelling. Useful for differentiating the
+                    effect of sequencing errors on deconvolution loss and accuracy.
 - **mmse:**             mixture model with sequencing errors. Also follows a binomial distribution, but softly assigns fragments
                     to cell-types. Optimization uses expectation maximization (slower than above). Recommended for high resolution
                     deconvolution (many cell types) and an atlas with large regions of grouped CpGs.
-- **llsp:**             log-likelihood with sequencing perfect. Same as llse, without error modelling. Useful for differentiating the
-                    effect of sequencing errors on deconvolution loss and accuracy.
 Select a model by:
 ```
-nanomix deconvolute <METHYLOME> -m <MODEL>
+nanomix deconvolute -m MODEL METHYLOME.tsv 
+```
+The **mmse model is distinct** in that it works by assigning reads to cell types. To this effect, one would need a methylome where every row represents a read and columns contain `{read_id, chr, start, end, total_calls, modified_calls}`, this also be constructed from a `.bam` file with [mbtools](https://github.com/jts/mbtools)
+```
+mbtools read-frequency SAMPLE.bam > METHYLOME.tsv
+nanomix deconvolute -m mmse METHYLOME.tsv
 ```
 For more info on other option hparams, run
 ```
 nanomix deconvolute -h
 ```
 
 ### Assign fragments
 Our tools also allows you to assign fragments in the methylome to cell types in the atlas based off of the deconvoluted sigma vector.
 ```
-nanomix assign <METHYLOME> -s <SIGMA> 
+nanomix assign -s SIGMA.tsv METHYLOME.tsv 
 ```
 ### Simulate 
 We provide functionality to simulate methylomes of complex cell mixtures given a `sigma.tsv` file that indicates the cell\_type in the first column and the corresponding proportion in the second column. All the proportions must add up to 1 and the cell-types must be the same as those in the supplied reference atlas. To simulate a methylome:
 ```
-nanomix simulate <SIGMA>
+nanomix simulate -a ATLAS.tsv SIGMA.tsv
 ```
 
 ### Evaluate
 Simulating data provides true cell-type assignments in the last column of the methylome. We can evaluate the performance of a models deconvolution on this methylome. This will output the deconvolution loss (euclidean distance between true and predicted sigma vector) and the read assignment accuracy at confidence levels from 0.5 to 0.9.
 ```
-nanomix evaluate <METHYLOME>
+nanomix evaluate -a ATLAS.tsv METHYLOME.tsv
 ```
 
+### Plot
+You can plot a list of deconvolution mixtures by providing them to the plot function. This will produce a stacked bar plot.
+```
+nanomix plot -o NAME.png *sigma.tsv
+```
+![exampledeconvplot](Images/example_deconvolution_plot.png)
```

### Comparing `nanomix-0.1.1/atlases/25Array.tsv` & `nanomix-0.2.0/atlases/25Array.tsv`

 * *Files identical despite different names*

### Comparing `nanomix-0.1.1/atlases/39Bisulfite.tsv` & `nanomix-0.2.0/atlases/39Bisulfite.tsv`

 * *Files identical despite different names*

### Comparing `nanomix-0.1.1/pyproject.toml` & `nanomix-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "nanomix"
-version = "0.1.1"
+version = "0.2.0"
 description = "Methods for cell type deconvolution from Oxford Nanopore methylation calling"
 readme = "README.md"
 keywords = ["nanopore", "methylation", "deconvolution"]
 authors = [ { name = "Jonathan Broadbent", email = "jonbroad15@gmail.com" },
             { name = "Jared Simpson", email = "jsimpson@oicr.on.ca" } ]
 maintainers = [ { name = "Jonathan Broadbent", email = "jonbroad15@gmail.com" } ]
-dependencies = ["pandas~=1.5.2", "pyranges==0.0.120", "numpy~=1.24.1", "scipy~=1.10.0"]
+dependencies = ["pandas~=1.5.2", "pyranges==0.0.120", "numpy~=1.24.1", "scipy~=1.10.0", "matplotlib", "ray"]
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [projects.urls]
 repository = "https://github.com/simpsonlab/nanomix"
 
 [project.scripts]
 nanomix = "nanomix:main"
 
 [tool.maturin]
-sdist-include = ["README.md", "LICENSE", "atlases/*"]
+include = ["README.md", "LICENSE", "atlases/*"]
 python-source = "python"
```

### Comparing `nanomix-0.1.1/python/nanomix/main.py` & `nanomix-0.2.0/python/nanomix/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import sys
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(script_dir)
 
 from functions import *
+from plot import plot_mixture_proportions
 BISULFITE_ATLAS = os.path.join(script_dir, '..', '..', 'atlases', '39Bisulfite.tsv')
 
 def main():
     parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter,
     description="""
 Nanomix: a tool for cell-type deconvolution of mixed methylation calls from Oxford Nanopore sequencing data.
 ------------------------------------------------------------------------------------------------------------
@@ -27,14 +28,15 @@
 Deconvolute:    Find the proportion of cell types present in a methylome
 Evaluate:       Evaluate the accuracy of a deconvolution model on a given methylome with labelled cell types
 Simulate:       Generate a methylome from a given cell-type mixture
 Assign:         Assign reads in the methylome to cell-types
 
 All outputs are directed to stdout. Select a sub-command with the [-h] flag for info on hparams
                                      """)
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.1.1')
     subparsers = parser.add_subparsers(dest='command', required=True,
                                        help="nanomix functions")
     parser_deconvolute = subparsers.add_parser('deconvolute',formatter_class=argparse.RawDescriptionHelpFormatter,
 description="""
 Deconvolute a methylome. Return the mixture proportions (sigma) in a tsv format to stdout.
 
 Methylome: A tsv file containing the methylome to be deconvoluted. The file must contain the following columns:
@@ -55,22 +57,26 @@
     mmse:               mixture model with sequencing errors. Also follows a binomial distribution, but softly assigns fragments
                         to cell-types. Optimization uses expectation maximization (slower than above). Recommended for high resolution
                         deconvolution (many cell types) and an atlas with large regions of grouped CpGs.
     llsp:               log-likelihood with sequencing perfect. Same as llse, without error modelling. Useful for differentiating the
                         effect of sequencing errors on deconvolution loss and accuracy.
 """)
     parser_deconvolute.add_argument('methylome', help='Path to methylome tsv file with columns: {chr, start, end, total_calls, modified_calls}')
-    parser_deconvolute.add_argument('-a', '--atlas', type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
-    parser_deconvolute.add_argument('-p01', default=0.05, type=float, help='Sequencing miscall rate')
-    parser_deconvolute.add_argument('-p11', default=0.95, type=float, help='Sequencing correct call rate')
+    parser_deconvolute.add_argument('-a', '--atlas', required=True, type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
+    parser_deconvolute.add_argument('-p01', default=0.05, help='Sequencing miscall rate')
+    parser_deconvolute.add_argument('-p11', default=0.95, help='Sequencing correct call rate')
     parser_deconvolute.add_argument('-m', '--model', default='llse', type=str, help='Deconvolution model options: [nnls, llse, llsp, mmse]')
-    parser_deconvolute.add_argument('-i', '--sigma_init', default='null', type=str, help='Initalize sigma with one of the other models (mmse only)')
-    parser_deconvolute.add_argument('-n', '--max_iter', default=100, type=int, help='Maximum number of iterations for the EM optimization (mmse only)')
+    parser_deconvolute.add_argument('-@', '--threads', default=1, type=int, help='Number of threads to use')
+    parser_deconvolute.add_argument('-nt', '--n_trials', default=3, type=int, help='Number of trials to run')
+    parser_deconvolute.add_argument('--nnls_init' , action='store_true', help='Initialize nnls with llse')
+    parser_deconvolute.add_argument('--concentration', type=float, help='Concentration parameter for Dirichlet prior')
+    parser_deconvolute.add_argument('-i', '--sigma_init', default='null', type=str, help='Initalize sigma with a tsv file')
+    parser_deconvolute.add_argument('-n', '--max_iter', default=200, type=int, help='Maximum number of iterations for the EM optimization (mmse only)')
     parser_deconvolute.add_argument('-p', '--min_proportion', default=0.01, type=float, help='Minimum proportion of a cell type to be considered (mmse only)')
-    parser_deconvolute.add_argument('-t', '--stop_thresh', default=1e-3, type=float, help='Stop EM iterations when percent change in log-likelihood falls below this value (mmse only)')
+    parser_deconvolute.add_argument('-t', '--stop_thresh', default=1e-5, type=float, help='Stop EM iterations when percent change in log-likelihood falls below this value (mmse only)')
     parser_deconvolute.set_defaults(func=deconvolute)
 
     parser_evaluate = subparsers.add_parser('evaluate', formatter_class=argparse.RawDescriptionHelpFormatter, description="""
 Evaluate the loss and accuracy of cell-type deconvolution on a given methylome with known cell types.
 
 Metrics outputed to stdout:
     Deconvolution loss:         Euclidean distance between the computed and true mixture proportion.
@@ -82,30 +88,30 @@
     start:              The start position of the read
     end:                The end position of the read
     total_calls:        The total number of reads mapped to the region
     modified_calls:     The number of modified reads mapped to the region
     cell_type:          String identifier of cell_type that matches that in the atlas header
 The simulate function can be used to create this file.
 """)
-    parser_evaluate.add_argument('methylome', help='Path to methylome tsv file with columns: {chr, start, end, total_calls, modified_calls, cell_type}')
-    parser_evaluate.add_argument('-a', '--atlas', type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
+    parser_evaluate.add_argument('methylome', help='Path to methylome tsv file with columns: {read_name, chr, start_position, end_position, total_calls, modified_calls, cell_type}')
+    parser_evaluate.add_argument('-a', '--atlas', required=True, type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
+    parser_evaluate.add_argument('-s', '--sigma', type=str, help='Path to sigma tsv file')
     parser_evaluate.add_argument('-p01', default=0.05, type=float, help='Sequencing miscall rate')
     parser_evaluate.add_argument('-p11', default=0.95, type=float, help='Sequencing correct call rate')
-    parser_evaluate.add_argument('-m', '--model', default='llse', type=str, help='Deconvolution model options: [nnls, llse, llsp, mmse]')
     parser_evaluate.set_defaults(func=evaluate)
 
     parser_simulate = subparsers.add_parser('simulate', formatter_class=argparse.RawDescriptionHelpFormatter, description="""
 Simulate a methylome from a given cell-type mixture (sigma).
 
 Sigma: A tsv file containing the cell-type mixture proportions. The file must contain the following columns:
     cell_type:          String identifier of cell_type that matches that in the atlas header
     proportion:         float between 0 and 1
 """)
     parser_simulate.add_argument('sigma', type=str, help='Path to sigma tsv file')
-    parser_simulate.add_argument('-a', '--atlas', type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
+    parser_simulate.add_argument('-a', '--atlas', required=True, type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
     parser_simulate.add_argument('-p01', default=0.05, type=float, help='Sequencing miscall rate')
     parser_simulate.add_argument('-p11', default=0.95, type=float, help='Sequencing correct call rate')
     parser_simulate.add_argument('-c', '--coverage', default=1, type=float, help='Sequencing coverage')
     parser_simulate.add_argument('-r', '--region_size', default=5, type=int, help='Number of CpGs in each region')
     parser_simulate.set_defaults(func=simulate)
 
     parser_assign = subparsers.add_parser('assign', formatter_class=argparse.RawDescriptionHelpFormatter, description="""
@@ -118,19 +124,47 @@
     end:                The end position of the read
     total_calls:        The total number of reads mapped to the region
     modified_calls:     The number of modified reads mapped to the region
     cell_type:          String identifier of cell_type that matches that in the atlas header
 The simulate function can be used to create this file.
 """)
     parser_assign.add_argument('methylome', help='Path to methylome tsv file with columns: {chr, start, end, total_calls, modified_calls}')
-    parser_assign.add_argument('-a', '--atlas', type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
+    parser_assign.add_argument('-a', '--atlas', required=True, type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
     parser_assign.add_argument('-p01', default=0.05, type=float, help='Sequencing miscall rate')
     parser_assign.add_argument('-p11', default=0.95, type=float, help='Sequencing correct call rate')
     parser_assign.add_argument('-s', '--sigma', required=True, type=str, help='Path to sigma tsv file')
     parser_assign.set_defaults(func=assign_fragments)
 
+    parser_plot = subparsers.add_parser('plot', formatter_class=argparse.RawDescriptionHelpFormatter, description="""
+Plot the results of a deconvolution into a stacked bar chart.
+
+Provide a list of sigma files to combine plots into one chart
+Sigma: A tsv file containing the cell-type mixture proportions. The file must contain the following columns:
+    cell_type:          String identifier of cell_type that matches that in the atlas header
+    proportion:         float between 0 and 1
+""")
+    parser_plot.add_argument('sigma', nargs='+', type=str, help='Path to sigma tsv files')
+    parser_plot.add_argument('-o', '--outpath', type=str, help='Name of the plot')
+    parser_plot.add_argument('-l', '--group_lung', action='store_true', help='Group lung cell types into one category')
+    parser_plot.add_argument('-c', '--chart', type=str, default='bar', help='Chart type: [bar, scatter]')
+    parser_plot.add_argument('-ct', '--cell_types', nargs='+', type=str, help='List of cell types to plot')
+    parser_plot.set_defaults(func=plot)
+
+    parser_ll = subparsers.add_parser('ll', formatter_class=argparse.RawDescriptionHelpFormatter, description="""
+Compute the log-likelihood of a given methylome given a cell-type mixture (sigma).
+""")
+    parser_ll.add_argument('methylome', help='Path to methylome tsv file with columns: {chr, start, end, total_calls, modified_calls}')
+    parser_ll.add_argument('-a', '--atlas', required=True, type=str, default=BISULFITE_ATLAS, help='Path to reference atlas')
+    parser_ll.add_argument('-m', '--model', default='llse', type=str, help='Deconvolution model options: [llse, llsp, mmse]')
+    parser_ll.add_argument('-p01', default=0.05, type=float, help='Sequencing miscall rate')
+    parser_ll.add_argument('-p11', default=0.95, type=float, help='Sequencing correct call rate')
+    parser_ll.add_argument('-s', '--sigma', required=True, type=str, help='Path to sigma tsv file')
+    parser_ll.set_defaults(func=log_likelihood)
+
+
+
     args = parser.parse_args()
     arg_dict = {k : v for k, v in vars(args).items() if k not in ['func','command']}
     args.func(**arg_dict)
 
 if __name__ == "__main__":
     main()
```

### Comparing `nanomix-0.1.1/python/nanomix/models.py` & `nanomix-0.2.0/python/nanomix/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,220 +4,235 @@
 import pandas as pd
 import pyranges as pr
 import math
 from scipy.stats import binom, dirichlet
 from scipy.optimize import minimize, nnls, Bounds
 import os
 import sys
+from multiprocessing import Queue
+import threading
+from functools import partial
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(script_dir)
 
 from _nanomix import *
-from atlas import ReferenceAtlas, Sample
+from atlas import AtlasMethylome
 from tools import *
 
-
-def fit_model(methylome, atlas_path, model, p01, p11):
+def fit_model(methylome, atlas, model, p01, p11,
+              threads=1, n_trials=5,
+              nnls_init=False, concentration=1.0):
     """
     Wrapper function to select model for deconvolution
     mmse model is initalized seperately with Rust bindings
-    methylome and atlas are joined on covered regions before deconvolution
+    methylome and data are joined on covered regions before deconvolution
 
     :param methylome: path to simulated methylome
-    :param atlas_path: path to reference atlas
+    :param data_path: path to reference data
     :param model: model to fit
     :param p01: nanopore miscall rate
     :param p11: nanopore correct call rate
-    :return: None
+    :return: cell-type proportions
     """
-    # load atlas
-    columns={'chromosome':'Chromosome', 'chr':'Chromosome',
-                            'start':'Start',
-                            'end':'End'}
-    df_atlas = pd.read_csv(atlas_path, sep='\t').rename(columns=columns)
-    df_atlas.drop_duplicates(inplace=True)
-    if 'label' in df_atlas.columns: df_atlas.drop('label', axis=1, inplace=True)
-    df_atlas.dropna(inplace=True)
-    gr_atlas = pr.PyRanges(df_atlas).sort()
-
-    # Read methylomes data from mbtools
-    try:
-        df = pd.read_csv(methylome, sep='\t').rename(columns=columns)
-    except pd.errors.EmptyDataError:
-        Exception("Empty methylome file")
-    df.dropna(inplace=True)
-    gr_sample = pr.PyRanges(df).sort()
-
-    # Join atlas and sample
-    gr = gr_atlas.join(gr_sample)
-    # Check for empty upon join
-    if len(gr) == 0:
-        Exception("Empty join between atlas and sample. The sample does not overlap with any regions in the atlas.")
-    atlas = ReferenceAtlas(gr.df.loc[:, gr_atlas.columns])
-    t = np.array(gr.total_calls, dtype=np.float32)
-    m = np.array(gr.modified_calls, dtype=np.float32)
-
-    xhat = m/t
-    s = Sample('methylome', xhat, m, t)
+    data = AtlasMethylome(methylome, atlas, threads=threads)
     if model == 'nnls':
-        sigma = fit_nnls(atlas, s)
+        sigma = fit_nnls(data)
     elif model == 'llse':
-        sigma = fit_llse(atlas, s, p01, p11)
+        sigma = fit_llse_parallel(data, p01, p11, n_trials, threads, concentration, nnls_init)
     elif model == 'llsp':
-        sigma = fit_llsp(atlas, s)
+        sigma = fit_llsp(data)
     elif model == 'null':
-        sigma = fit_uniform(atlas, s)
+        sigma = fit_uniform(data)
     else:
         raise ValueError(f"no such model: {model}. Choose from [nnls, llse, llsp, mmse]")
     return sigma
 
-def log_likelihood_sequencing_perfect(atlas, sigma, sample):
+def log_likelihood_sequencing_perfect(data, sigma):
     """
     Compute the log-likelihood of the llsp model
 
-    :param atlas: reference atlas
+    :param data: reference data
     :param sigma: cell-type proportions
-    :param sample: sample methylome
+    :param data: data methylome
     :return: log-likelihood
     :rtype: float
     """
-    sigma_t = sigma.reshape( (atlas.K, 1) )
-    x = np.clip(np.ravel(atlas.get_x(sigma_t)), 0, 1.0)
-    b =  binom.logpmf(sample.m, sample.t, x)
+    sigma_t = sigma.reshape( (data.K, 1) )
+    x = np.clip(np.ravel(data.get_x(sigma_t)), 0, 1.0)
+    b =  binom.logpmf(data.m, data.t, x)
     return np.sum(b)
 
-def fit_llsp(atlas, sample,
-             n_trials=10):
+def fit_llsp(data, n_trials=10):
     """
     fit the log-likelihood sequencing perfect model
 
-    :param atlas: reference atlas
-    :param sample: sample methylome
+    :param data: reference data
+    :param data: data methylome
     :param n_trials: number of trials to run with random initalizations of sigma
     :return: cell-type proportions
     :rtype: np.array
     """
-    f = lambda x: -1 * log_likelihood_sequencing_perfect(atlas, x, sample)
-    bnds = [ (0.0, 1.0) ] * atlas.K
+    f = lambda x: -1 * log_likelihood_sequencing_perfect(data, x)
+    bnds = [ (0.0, 1.0) ] * data.K
     cons = ({'type': 'eq', 'fun': eq_constraint})
-    alpha = np.array([ 1.0 / atlas.K ] * atlas.K)
+    alpha = np.array([ 1.0 / data.K ] * data.K)
     n_trials = 10
     best_ll = np.inf
     best_sol = None
     initializations = dirichlet.rvs(alpha, size=n_trials).tolist()
 
     for (i, init) in enumerate(initializations):
         res = minimize(f, init, method='SLSQP', options={'maxiter': 100, 'disp':False}, bounds=bnds, constraints=cons)
         ll = res.get("fun")
         if ll < best_ll:
             best_ll = ll
             best_sol = res
     return best_sol.x/np.sum(best_sol.x)
 
-def log_likelihood_sequencing_with_errors(atlas, sigma, sample, p01,p11):
+def log_likelihood_sequencing_with_errors(data, sigma, p01, p11):
     """
     Compute the log-likelihood of the llse model
 
-    :param atlas: reference atlas
+    :param data: reference data
     :param sigma: cell-type proportions
-    :param sample: sample methylome
+    :param data: data methylome
     :param p01: nanopore miscall rate
     :param p11: nanopore correct call rate
     :return: log-likelihood
     :rtype: float
     """
-    sigma_t = sigma.reshape( (atlas.K, 1) )
 
-    # the solver we use can try values that are outside
-    # the constraints we impose, we need to clip here to prevent
-    # things from blowing up
-    x = np.clip(np.ravel(atlas.get_x(sigma_t)), 0, 1.0)
-    if p11:
-        p = x * p11 + (1-x) * p01
+    sigma_t = sigma.reshape( (data.K, 1) )
+
+    # if p01 is a vector then reshape if not then make it a vector
+    if isinstance(p01, np.ndarray):
+        p01 = p01.reshape( (data.K, 1) )
     else:
-        p = x * (1 - p01) + (1 - x) * p01
-    b =  binom.logpmf(sample.m, sample.t, p)
-    binomial_coef = sum([math.log(math.comb(int(t), int(m))) for m,t in zip(sample.m, sample.t)])
+        p01 = np.array([p01] * data.K).reshape( (data.K, 1) )
+    if isinstance(p11, np.ndarray):
+        p11 = p11.reshape( (data.K, 1) )
+    else:
+        p11 = np.array([p11] * data.K).reshape( (data.K, 1) )
+    p = np.clip(np.ravel(data.get_x(sigma_t, p01, p11)), 0, 1.0)
+    # breakpoint()
+    # x = np.clip(np.ravel(np.dot(data.A, sigma_t)), 0, 1.0)
+    # p = x * p11 + (1-x) * p01
+    b =  binom.logpmf(data.m, data.t, p)
+    binomial_coef = sum([math.log(math.comb(int(t), int(m))) for m,t in zip(data.m, data.t)])
 
-    return np.sum(b) - binomial_coef
+    return np.sum(b) #- binomial_coef
 
-def fit_uniform(atlas, sample):
+def fit_uniform(K):
     """
     fit the uniform model (null model)
 
-    :param atlas: reference atlas
-    :param sample: sample methylome
+    :param K: number of cell-types
     :return: cell-type proportions
     :rtype: np.array
     """
-    return np.array([1.0 / atlas.K ] * atlas.K)
+    return np.array([1.0 / K ] * K)
 
-def fit_llse(atlas, sample, p01, p11,
-             n_trials=10):
+class my_thread(threading.Thread):
+    """
+    thread class for parallel processing of fit_llse
+    """
+    def __init__(self, data, p01, p11, queue):
+        super(my_thread, self).__init__()
+        self.data = data
+        self.p01 = p01
+        self.p11 = p11
+        self.queue = queue
+        self.res = []
+    def run(self):
+        alpha = self.queue.get()
+        f = lambda x: -1 * log_likelihood_sequencing_with_errors(self.data, x, self.p01, self.p11)
+        bnds = [ (0.0, 1.0) ] * self.data.K
+        cons = ({'type': 'eq', 'fun': eq_constraint})
+        self.res.append(minimize(f, alpha, method='SLSQP', options={'maxiter': 200, 'disp':False}, bounds=bnds, constraints=cons))
+
+
+def fit_llse_parallel(data, p01, p11, n_trials, threads, concentration, init_nnls):
+    alpha = np.array([concentration] * data.K)
+    initializations = dirichlet.rvs(alpha, size=n_trials).tolist()
+    if init_nnls:
+        initializations.append(fit_nnls(data))
+
+    queues = [Queue() for i in range(threads)]
+    res = []
+    for i in range(n_trials):
+        queues[i % threads].put(initializations[i])
+    threads = [my_thread(data, p01, p11, queues[i]) for i in range(threads)]
+    for t in threads:
+        t.start()
+    for t in threads:
+        t.join()
+        res += t.res
+
+    best_ll = np.inf
+    best_sol = None
+    for r in res:
+        ll = r.get("fun")
+        if ll < best_ll:
+            best_ll = ll
+            best_sol = r
+    return best_sol.x/np.sum(best_sol.x)
+
+def fit_llse(data, p01, p11):
     """
     fit the log-likelihood sequencing with errors model
 
-    :param atlas: reference atlas
-    :param sample: sample methylome
+    :param data: reference data
+    :param data: data methylome
     :param p01: nanopore miscall rate
     :param p11: nanopore correct call rate
     :param n_trials: number of trials to run with random initalizations of sigma
     :return: cell-type proportions
     :rtype: np.array
     """
-    f = lambda x: -1 * log_likelihood_sequencing_with_errors(atlas, x, sample, p01, p11)
-    bnds = [ (0.0, 1.0) ] * atlas.K
+    f = lambda x: -1 * log_likelihood_sequencing_with_errors(data, x, p01, p11)
+    bnds = [ (0.0, 1.0) ] * data.K
     cons = ({'type': 'eq', 'fun': eq_constraint})
-    alpha = np.array([ 1.0 / atlas.K ] * atlas.K)
-    best_ll = np.inf
-    best_sol = None
-    initializations = dirichlet.rvs(alpha, size=n_trials).tolist()
-
-    for (i, init) in enumerate(initializations):
-        res = minimize(f, init, method='SLSQP', options={'maxiter': 100, 'disp':False}, bounds=bnds, constraints=cons)
-        ll = res.get("fun")
-        if ll < best_ll:
-            best_ll = ll
-            best_sol = res
-    return best_sol.x/np.sum(best_sol.x)
+    alpha = np.array([ 1.0 / data.K ] * data.K)
+    res = minimize(f, alpha, method='SLSQP', options={'maxiter': 100, 'disp':False}, bounds=bnds, constraints=cons)
+    return res.x/np.sum(res.x)
 
-def fit_nnls(atlas, sample):
+def fit_nnls(data):
     """
     fit the non-negative least squares model
 
-    :param atlas: reference atlas
-    :param sample: sample methylome
+    :param data: reference data
+    :param data: data methylome
     :return: cell-type proportions
     :rtype: np.array
     """
 
     # add sum=1 constraint
-    t = np.array([1.0] * atlas.K).reshape( (1, atlas.K) )
-    A = np.append(atlas.A, t, axis=0)
-    b = np.append(sample.x_hat, [1.0], axis=0)
+    t = np.array([1.0] * data.K).reshape( (1, data.K) )
+    A = np.append(data.A, t, axis=0)
+    b = np.append(data.x_hat, [1.0], axis=0)
     res = nnls(A, b)
     return res[0]/np.sum(res[0])
 
-def fit_mmse(atlas, sample, sigma, p01, p11, stop_thresh, max_iter, min_proportion,
+def fit_mmse(methylome, atlas, sigma, p01, p11, stop_thresh, max_iter, min_proportion, concentration,
              true_sigma=None, true_assignments=None):
     """
-    Fit mixture model with sequencing errors (MMSE) onto sample with reference atlas.
+    Fit mixture model with sequencing errors (MMSE) onto data with reference data.
     Wrapper function to access Rust implementation.
 
+    :param methylome: path to sample methylome to fit
     :param atlas: path to reference atlas
-    :param sample: path to sample methylome to fit
     :param p01: sequencing miscall rate
     :param p11: sequencing correct call rate
     :param stop_thresh: threshold for stopping iterations
     :param max_iter: maximum number of iterations
     :param min_proportion: minimum proportion of a cell type in the mixture
     :return: fitted mixture model
     """
     # initialize MMSE model
-    mmse = MMSE(sample, atlas, sigma, p01, p11)
+    mmse = MMSE(methylome, atlas, sigma, p01, p11, concentration)
     if true_sigma is not None and true_assignments is not None:
         mmse.evaluate(stop_thresh, max_iter, min_proportion, true_sigma, true_assignments)
     else:
         mmse.optimize(stop_thresh, max_iter, min_proportion)
     return mmse.cell_type_proportions()
```

### Comparing `nanomix-0.1.1/python/nanomix/tests/test_assign.py` & `nanomix-0.2.0/python/nanomix/tests/test_assign.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 parent_dir = os.path.dirname(script_dir)
 sys.path.append(parent_dir)
 
 from main import *
 
+script_dir = os.path.dirname(os.path.realpath(__file__))
 methylome = os.path.join(script_dir, 'test_data', 'test_methylome.tsv')
 atlas = os.path.join(script_dir, 'test_data', 'test_atlas.tsv')
 sigma_path = os.path.join(script_dir, 'test_data', 'test_sigma.tsv')
 true_assignments = []
 
 class TestMain(unittest.TestCase):
```

### Comparing `nanomix-0.1.1/python/nanomix/tests/test_data/39Bisulfite.tsv` & `nanomix-0.2.0/python/nanomix/tests/test_data/39Bisulfite.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-chr	start	end	adipocyte	endothelial_cell	colon_fibroblasts	heart_fibroblasts	dermal_fibroblast	skeletal_muscle	smooth_muscle	heart_cardiomyocyte	bone_osteoblast	oligodendrocyte	neuron	hepatocyte	pancreas_duct	pancreas_acinar	pancreas_delta	pancreas_beta	pancreas_alpha	kidney_epithelial	thyroid_epithelial	fallopian_epithelial	ovary_epithelial	erythrocyte_progenitor	T-cell	NK-cell	monocyte	granulocyte	B-cell	epiderminal_keratinocyte	head_neck_epithelial	lung_epithelial	prostate_epithelial	bladder_epithelial	breast_luminal	breast_basal	lung_alveolar_epithelial	gallbladder	gastric_epithelial	colon_epithelial	small_int_epithelial
+chr	start	end	adipocyte	endothelial_cell	colon_fibroblasts	heart_fibroblasts	dermal_fibroblast	skeletal_muscle	smooth_muscle	heart_cardiomyocyte	bone_osteoblast	oligodendrocyte	neuron	hepatocyte	pancreas_duct	pancreas_acinar	pancreas_delta	pancreas_beta	pancreas_alpha	kidney	thyroid	fallopian	ovary	erythrocyte_progenitor	T-cell	NK-cell	monocyte	granulocyte	B-cell	epiderminal_keratinocyte	head_neck	lung	prostate	bladder	breast_luminal	breast_basal	lung_alveolar	gallbladder	gastric	colon	small_intestine
 chr1	1066168	1066385	0.71	0.81	0.78	0.80	0.84	0.85	0.67	0.91	0.73	0.94	0.94	0.89	0.93	0.81	0.89	0.89	0.92	0.80	0.73	0.00	0.64	0.80	0.87	0.94	0.92	0.92	0.85	0.94	0.87	0.82	0.94	0.82	0.96	0.96	0.75	0.79	0.92	0.73	0.50
 chr1	1071849	1072048	0.86	0.86	0.79	0.86	0.78	0.85	0.83	0.95	0.81	0.83	0.56	0.92	0.94	0.76	0.86	0.84	0.80	0.93	0.91	0.92	0.94	0.78	0.83	0.89	0.92	0.91	0.90	0.87	0.85	0.90	0.93	0.93	0.79	0.10	0.94	0.92	0.94	0.94	0.82
 chr1	1179392	1179548	0.88	0.91	0.76	0.83	0.90	0.87	0.86	0.95	0.79	0.93	0.89	0.93	0.97	0.91	0.90	0.94	0.93	0.62	0.76	0.88	0.83	0.80	0.93	0.97	0.93	0.94	0.05	0.95	0.88	0.90	0.95	0.96	0.98	0.96	0.96	0.92	0.96	0.94	0.96
 chr1	1196563	1196734	0.74	0.75	0.67	0.70	0.66	0.74	0.61	0.77	0.63	0.93	0.87	0.93	0.90	0.90	0.77	0.82	0.88	0.89	0.89	0.11	0.11	0.66	0.90	0.91	0.93	0.95	0.83	0.91	0.85	0.87	0.90	0.88	0.88	0.95	0.90	0.91	0.89	0.85	0.76
 chr1	1262136	1262432	0.94	0.94	0.95	0.94	0.95	0.93	0.91	0.92	0.93	0.95	0.95	0.97	0.98	0.95	0.95	0.95	0.95	0.97	0.96	0.96	0.95	0.05	0.96	0.97	0.97	0.98	0.97	0.86	0.95	0.94	0.96	0.95	0.96	0.83	0.95	0.95	0.93	0.87	0.88
 chr1	1299934	1300105	0.91	0.91	0.74	0.82	0.92	0.72	0.67	0.91	0.85	0.64	0.60	0.96	0.94	0.85	0.82	0.82	0.89	0.87	0.94	0.03	0.69	0.72	0.86	0.94	0.93	0.92	0.68	0.86	0.86	0.84	0.92	0.91	0.96	0.91	0.87	0.90	0.88	0.90	0.84
 chr1	1343575	1344011	0.90	0.93	0.89	0.89	0.87	0.66	0.88	0.93	0.79	0.93	0.93	0.14	0.95	0.88	0.90	0.92	0.94	0.90	0.95	0.94	0.94	0.83	0.94	0.97	0.96	0.96	0.95	0.84	0.90	0.91	0.95	0.93	0.92	0.93	0.94	0.65	0.81	0.94	0.86
@@ -393,15 +393,14 @@
 chr1	119006353	119006565	0.43	0.09	0.10	0.24	0.76	0.34	0.09	0.03	0.63	0.06	0.05	0.10	0.07	0.05	0.06	0.09	0.08	0.08	0.06	0.06	0.10	0.04	0.12	0.09	0.08	0.06	0.14	0.03	0.08	0.08	0.13	0.12	0.12	0.12	0.08	0.05	0.07	0.08	0.10
 chr1	119084631	119084817	0.58	0.74	0.87	0.35	0.08	0.80	0.70	0.94	0.87	0.96	0.90	0.98	0.95	0.96	0.95	0.96	0.98	0.95	0.96	0.98	0.96	0.78	0.95	0.96	0.97	0.96	0.97	0.85	0.92	0.96	0.87	0.95	0.97	0.78	0.97	0.94	0.97	0.97	0.97
 chr1	119441444	119441662	0.81	0.76	0.80	0.10	0.84	0.70	0.55	0.89	0.81	0.93	0.93	0.96	0.88	0.85	0.84	0.84	0.91	0.95	0.94	0.94	0.86	0.57	0.87	0.92	0.90	0.90	0.88	0.63	0.93	0.96	0.91	0.78	0.79	0.87	0.94	0.93	0.89	0.93	0.93
 chr1	119799594	119799845	0.88	0.86	0.86	0.77	0.81	0.75	0.76	0.89	0.32	0.94	0.94	0.84	0.93	0.05	0.91	0.95	0.97	0.96	0.95	0.97	0.93	0.63	0.86	0.89	0.90	0.79	0.91	0.94	0.95	0.95	0.97	0.97	0.97	0.96	0.93	0.92	0.80	0.95	0.90
 chr1	148809167	148809417	0.66	0.76	0.87	0.56	0.89	0.81	0.69	0.93	0.92	0.34	0.07	0.90	0.99	0.86	0.92	0.89	0.94	0.95	0.92	0.97	0.94	0.67	0.95	0.96	0.95	0.97	0.98	0.88	0.94	0.95	0.94	0.86	0.98	0.97	0.95	0.78	0.86	0.89	0.86
 chr1	149932823	149933208	0.96	0.95	0.90	0.90	0.95	0.92	0.89	0.97	0.90	0.94	0.92	0.97	0.98	0.85	0.94	0.94	0.96	0.96	0.93	0.96	0.95	0.74	0.93	0.96	0.96	0.97	0.94	0.92	0.93	0.95	0.95	0.96	0.96	0.94	0.95	0.93	0.96	0.07	0.40
 chr1	150176924	150177198	0.57	0.80	0.74	0.78	0.78	0.73	0.71	0.95	0.80	0.90	0.81	0.87	0.90	0.68	0.89	0.91	0.89	0.84	0.90	0.87	0.87	0.59	0.90	0.95	0.16	0.37	0.94	0.88	0.71	0.84	0.91	0.83	0.92	0.94	0.89	0.92	0.90	0.94	0.94
-chr1	150729792	150729946	0.78	0.90	0.85	0.71	0.93	0.78	0.84	0.98	0.82	0.94	0.92	0.99	0.99	0.87	0.92	0.92	0.98	0.92	0.93	0.94	0.94	0.88	0.97	0.99	0.97	0.96	0.97	0.00	0.73	0.91	0.93	0.97	0.88	0.91	0.65	NA	0.97	0.97	0.97
 chr1	150776192	150776427	0.85	0.91	0.82	0.88	0.58	0.85	0.75	0.98	0.88	0.92	0.94	0.97	0.97	0.89	0.94	0.95	0.97	0.94	0.91	0.96	0.78	0.72	0.92	0.96	0.67	0.78	0.93	0.89	0.92	0.66	0.90	0.87	0.96	0.96	0.07	0.97	0.78	0.90	0.93
 chr1	150791487	150792044	0.79	0.94	0.91	0.87	0.86	0.88	0.81	0.93	0.83	0.93	0.95	0.93	0.97	0.94	0.96	0.96	0.97	0.95	0.94	0.93	0.92	0.69	0.93	0.92	0.24	0.44	0.95	0.93	0.94	0.95	0.94	0.93	0.97	0.97	0.94	0.95	0.96	0.95	0.94
 chr1	151062393	151062653	0.91	0.96	0.93	0.92	0.93	0.92	0.89	0.95	0.93	0.95	0.29	0.97	0.96	0.84	0.97	0.98	0.98	0.96	0.94	0.97	0.94	0.79	0.96	0.97	0.97	0.98	0.97	0.93	0.95	0.96	0.97	0.96	0.98	0.95	0.95	0.97	0.94	0.93	0.92
 chr1	151330137	151330662	0.69	0.85	0.77	0.73	0.32	0.74	0.63	0.93	0.82	0.90	0.85	0.93	0.96	0.90	0.95	0.95	0.94	0.90	0.94	0.93	0.95	0.78	0.94	0.93	0.94	0.93	0.93	0.91	0.87	0.91	0.93	0.91	0.89	0.93	0.94	0.96	0.93	0.94	0.95
 chr1	151709676	151710166	0.88	0.89	0.83	0.79	0.89	0.84	0.73	0.94	0.76	0.74	0.25	0.92	0.91	0.74	0.68	0.76	0.59	0.75	0.88	0.89	0.87	0.65	0.88	0.91	0.95	0.96	0.89	0.89	0.87	0.80	0.93	0.91	0.96	0.96	0.86	0.87	0.89	0.93	0.81
 chr1	151711596	151711796	0.85	0.86	0.77	0.75	0.74	0.81	0.75	0.90	0.80	0.93	0.16	0.95	0.94	0.88	0.74	0.67	0.66	0.94	0.75	0.90	0.93	0.72	0.88	0.96	0.94	0.95	0.83	0.89	0.80	0.89	0.95	0.93	0.96	0.93	0.95	0.97	0.96	0.98	0.97
 chr1	151769129	151769353	0.90	0.90	0.85	0.86	0.83	0.87	0.86	0.92	0.72	0.91	0.93	0.92	0.88	0.87	0.92	0.91	0.89	0.93	0.36	0.90	0.93	0.80	0.95	0.95	0.93	0.95	0.96	0.91	0.91	0.79	0.75	0.84	0.95	0.95	0.06	0.52	0.89	0.77	0.95
@@ -3239,15 +3238,14 @@
 chr8	4698951	4699102	0.88	0.85	0.89	0.06	0.80	0.84	0.37	0.90	0.44	0.91	0.95	0.72	0.85	0.65	0.83	0.82	0.75	0.83	0.95	0.91	0.83	0.59	0.91	0.94	0.91	0.93	0.94	0.93	0.92	0.92	0.90	0.91	0.83	0.86	0.84	0.89	0.88	0.94	0.95
 chr8	6575371	6575976	0.95	0.96	0.93	0.94	0.94	0.94	0.90	0.78	0.90	0.98	0.97	0.96	0.97	0.95	0.96	0.95	0.95	0.97	0.95	0.97	0.96	0.15	0.92	0.94	0.95	0.93	0.95	0.91	0.93	0.95	0.97	0.93	0.98	0.97	0.95	0.95	0.96	0.95	0.94
 chr8	6609079	6609546	0.76	0.90	0.92	0.89	0.32	0.69	0.82	0.98	0.93	0.96	0.95	0.97	0.96	0.91	0.94	0.93	0.95	0.94	0.95	0.95	0.93	0.81	0.95	0.96	0.96	0.97	0.96	0.93	0.95	0.96	0.95	0.95	0.98	0.96	0.96	0.97	0.97	0.97	0.96
 chr8	6737850	6738339	0.94	0.96	0.96	0.94	0.95	0.92	0.91	0.97	0.95	0.95	0.96	0.97	0.98	0.95	0.87	0.96	0.98	0.91	0.94	0.98	0.96	0.70	0.95	0.98	0.97	0.96	0.97	0.91	0.97	0.97	0.99	0.97	0.97	0.98	0.98	0.92	0.08	0.95	0.95
 chr8	6753890	6754242	0.83	0.89	0.89	0.87	0.82	0.82	0.82	0.92	0.81	0.93	0.96	0.96	0.96	0.92	0.94	0.94	0.96	0.66	0.91	0.01	0.66	0.78	0.88	0.88	0.86	0.80	0.85	0.94	0.93	0.86	0.94	0.93	0.95	0.91	0.75	0.95	0.92	0.93	0.92
 chr8	6775106	6775292	0.92	0.94	0.91	0.89	0.90	0.85	0.84	0.95	0.82	0.93	0.95	0.94	0.96	0.93	0.97	0.94	0.92	0.97	0.96	0.97	0.69	0.92	0.89	0.94	0.96	0.97	0.93	0.92	0.96	0.96	0.96	0.95	0.92	0.95	0.95	0.12	0.97	0.94	0.92
 chr8	6957340	6957503	0.90	0.88	0.87	0.64	0.76	0.72	0.52	0.92	0.78	0.90	0.95	0.83	0.96	0.76	0.91	0.90	0.87	0.93	0.90	0.95	0.91	0.62	0.85	0.91	0.87	0.08	0.89	0.88	0.93	0.95	0.96	0.88	0.94	0.93	0.88	0.93	0.92	0.91	0.90
-chr8	8222716	8223086	0.57	0.92	0.91	0.90	0.93	NA	0.84	0.96	0.00	0.92	0.87	0.95	0.93	0.89	0.90	0.79	0.85	0.87	0.60	0.92	0.90	0.69	0.91	0.93	0.92	0.95	0.96	0.91	0.84	0.95	0.84	0.74	0.97	0.62	0.91	0.93	0.95	0.93	0.89
 chr8	8714786	8714965	0.76	0.88	0.87	0.69	0.48	0.72	0.66	0.91	0.72	0.95	0.95	0.94	0.97	0.85	0.91	0.90	0.87	0.96	0.95	0.92	0.96	0.62	0.87	0.92	0.96	0.95	0.95	0.80	0.74	0.82	0.68	0.92	0.03	0.75	0.94	0.98	0.95	0.93	0.92
 chr8	8854393	8854586	0.97	0.95	0.91	0.96	0.96	0.95	0.93	0.97	0.95	0.97	0.96	0.96	0.96	0.95	0.97	0.96	0.98	0.22	0.59	0.96	0.75	0.94	0.97	0.98	0.96	0.96	0.67	0.94	0.97	0.97	0.97	0.97	0.97	0.97	0.97	0.95	0.97	0.97	0.96
 chr8	9009579	9009812	0.95	0.95	0.91	0.86	0.92	0.83	0.90	0.93	0.91	0.95	0.96	0.97	0.97	0.94	0.93	0.96	0.96	0.89	0.92	0.92	0.94	0.76	0.96	0.96	0.98	0.96	0.96	0.94	0.86	0.13	0.94	0.92	0.97	0.95	0.94	0.94	0.95	0.96	0.95
 chr8	9133287	9133869	0.82	0.92	0.93	0.85	0.95	0.85	0.90	0.95	0.16	0.95	0.96	0.82	0.98	0.93	0.96	0.96	0.97	0.91	0.96	0.98	0.96	0.66	0.94	0.97	0.97	0.97	0.94	0.90	0.96	0.96	0.95	0.96	0.90	0.83	0.96	0.96	0.95	0.96	0.94
 chr8	9274158	9274361	0.95	0.94	0.88	0.79	0.85	0.94	0.75	0.98	0.91	0.95	0.96	0.97	0.98	0.88	0.95	0.95	0.92	0.96	0.94	0.95	0.95	0.69	0.91	0.92	0.95	0.96	0.91	0.27	0.91	0.96	0.96	0.95	0.88	0.96	0.96	0.95	0.94	0.92	0.94
 chr8	9629705	9629978	0.95	0.95	0.87	0.95	0.97	0.95	0.92	0.97	0.90	0.85	0.95	0.92	0.69	0.96	0.94	0.94	0.96	0.97	0.95	0.98	0.84	0.86	0.97	0.97	0.97	0.96	0.97	0.93	0.95	0.96	0.98	0.96	0.96	0.96	0.98	0.15	0.91	0.97	0.97
 chr8	9884810	9885049	0.94	0.93	0.89	0.75	0.84	0.92	0.77	0.94	0.84	0.91	0.96	0.90	0.94	0.78	0.90	0.90	0.89	0.95	0.92	0.90	0.90	0.71	0.93	0.95	0.95	0.96	0.93	0.05	0.85	0.95	0.89	0.88	0.12	0.13	0.94	0.93	0.93	0.94	0.95
@@ -3520,15 +3518,14 @@
 chr8	140621091	140621277	0.91	0.92	0.86	0.87	0.88	0.39	0.87	0.84	0.91	0.05	0.82	0.97	0.94	0.88	0.93	0.90	0.93	0.89	0.95	0.93	0.89	0.83	0.91	0.92	0.96	0.95	0.92	0.87	0.89	0.91	0.95	0.96	0.95	0.93	0.93	0.94	0.91	0.90	0.89
 chr8	141148322	141148511	0.95	0.93	0.89	0.90	0.90	0.84	0.91	0.95	0.92	0.96	0.73	0.91	0.97	0.94	0.89	0.09	0.69	0.71	0.97	0.94	0.87	0.62	0.96	0.94	0.94	0.89	0.92	0.88	0.85	0.95	0.95	0.88	0.96	0.97	0.95	0.95	0.92	0.96	0.94
 chr8	141158426	141158623	0.63	0.78	0.82	0.88	0.93	0.58	0.84	0.94	0.89	0.94	0.69	0.91	0.97	0.85	0.90	0.95	0.94	0.80	0.82	0.93	0.86	0.75	0.95	0.98	0.96	0.94	0.86	0.86	0.57	0.09	0.89	0.90	0.97	0.96	0.71	0.90	0.95	0.96	0.88
 chr8	141212343	141212659	0.83	0.87	0.88	0.88	0.88	0.79	0.85	0.59	0.86	0.95	0.95	0.92	0.95	0.95	0.93	0.94	0.94	0.94	0.95	0.97	0.96	0.84	0.93	0.88	0.81	0.17	0.94	0.89	0.91	0.91	0.93	0.95	0.93	0.94	0.91	0.89	0.89	0.95	0.95
 chr8	141400427	141400689	0.85	0.89	0.90	0.91	0.31	0.70	0.74	0.92	0.89	0.95	0.92	0.83	0.97	0.85	0.85	0.77	0.62	0.89	0.96	0.97	0.95	0.71	0.93	0.96	0.96	0.94	0.93	0.90	0.94	0.94	0.95	0.93	0.97	0.98	0.93	0.90	0.95	0.94	0.88
 chr8	141516704	141516957	0.04	0.04	0.08	0.02	0.03	0.06	0.02	0.02	0.05	0.05	0.84	0.04	0.04	0.02	0.07	0.13	0.06	0.03	0.04	0.03	0.06	0.07	0.12	0.15	0.11	0.14	0.12	0.04	0.05	0.04	0.04	0.08	0.03	0.02	0.06	0.04	0.06	0.12	0.13
 chr8	141715917	141716144	0.08	0.08	0.13	0.04	0.09	0.07	0.07	0.05	0.05	0.05	0.85	0.09	0.06	0.04	0.35	0.66	0.56	0.04	0.08	0.07	0.10	0.06	0.19	0.10	0.12	0.10	0.19	0.08	0.11	0.09	0.08	0.12	0.10	0.06	0.10	0.07	0.10	0.31	0.37
-chr8	141740768	141741070	0.79	0.78	0.71	0.50	NA	0.69	0.54	0.81	0.00	0.83	0.69	0.83	0.91	0.71	0.86	0.83	0.82	0.87	0.88	NA	0.90	0.56	0.83	0.64	0.96	0.82	0.87	NA	0.87	0.91	0.94	0.86	0.84	0.88	0.77	0.89	0.85	0.89	0.93
 chr8	142322671	142322827	0.95	0.95	0.92	0.83	0.92	0.90	0.78	0.97	0.86	0.29	0.91	0.96	0.98	0.97	0.98	0.98	0.98	0.97	0.97	0.98	0.97	0.75	0.95	0.96	0.85	0.73	0.95	0.93	0.90	0.92	0.96	0.93	0.68	0.10	0.96	0.94	0.97	0.97	0.97
 chr8	143320571	143321107	0.76	0.90	0.90	0.88	0.93	0.89	0.80	0.95	0.89	0.95	0.93	0.93	0.96	0.94	0.91	0.92	0.91	0.95	0.95	0.96	0.96	0.85	0.95	0.96	0.96	0.94	0.96	0.80	0.83	0.93	0.95	0.94	0.81	0.16	0.95	0.91	0.95	0.95	0.92
 chr8	143335509	143335732	0.75	0.82	0.84	0.86	0.87	0.83	0.76	0.96	0.81	0.95	0.96	0.06	0.94	0.79	0.96	0.93	0.95	0.67	0.93	0.96	0.95	0.84	0.93	0.89	0.85	0.79	0.96	0.92	0.91	0.91	0.95	0.91	0.91	0.93	0.93	0.78	0.92	0.93	0.86
 chr8	143374854	143375295	0.77	0.87	0.84	0.74	0.32	0.79	0.67	0.95	0.69	0.94	0.83	0.96	0.96	0.91	0.94	0.95	0.97	0.94	0.96	0.95	0.95	0.73	0.92	0.92	0.93	0.86	0.90	0.91	0.88	0.87	0.94	0.92	0.96	0.95	0.94	0.94	0.93	0.93	0.73
 chr8	143390095	143390325	0.88	0.90	0.83	0.79	0.89	0.88	0.87	0.95	0.69	0.94	0.94	0.07	0.90	0.73	0.89	0.94	0.93	0.87	0.91	0.88	0.81	0.85	0.88	0.92	0.93	0.94	0.91	0.86	0.87	0.91	0.95	0.90	0.92	0.95	0.88	0.91	0.89	0.77	0.83
 chr8	143438492	143439130	0.92	0.95	0.89	0.92	0.92	0.94	0.87	0.96	0.92	0.94	0.94	0.97	0.95	0.94	0.92	0.23	0.87	0.94	0.94	0.96	0.94	0.81	0.94	0.96	0.97	0.97	0.94	0.89	0.90	0.92	0.95	0.95	0.98	0.96	0.96	0.94	0.95	0.95	0.95
 chr8	143439189	143439438	0.87	0.92	0.86	0.92	0.87	0.92	0.85	0.96	0.88	0.95	0.68	0.97	0.96	0.96	0.59	0.02	0.29	0.94	0.95	0.97	0.96	0.86	0.96	0.96	0.97	0.95	0.96	0.94	0.95	0.96	0.93	0.95	0.97	0.96	0.96	0.95	0.96	0.81	0.92
@@ -5951,15 +5948,14 @@
 chr16	29337402	29337689	0.91	0.94	0.69	0.94	0.89	0.91	0.91	0.98	0.90	0.96	0.95	0.97	0.97	0.93	0.94	0.95	0.96	0.96	0.96	0.97	0.96	0.73	0.95	0.95	0.70	0.96	0.03	0.92	0.91	0.90	0.96	0.95	0.95	0.93	0.93	0.95	0.96	0.96	0.97
 chr16	29342706	29342959	0.96	0.95	0.92	0.91	0.91	0.90	0.92	0.96	0.92	0.96	0.95	0.97	0.95	0.88	0.93	0.94	0.97	0.96	0.95	0.93	0.94	0.67	0.91	0.94	0.94	0.96	0.93	0.02	0.07	0.56	0.86	0.83	0.79	0.81	0.91	0.95	0.95	0.92	0.91
 chr16	29343445	29344051	0.94	0.92	0.91	0.89	0.93	0.86	0.89	0.92	0.90	0.93	0.96	0.96	0.95	0.92	0.93	0.92	0.94	0.93	0.94	0.93	0.91	0.73	0.95	0.95	0.87	0.92	0.71	0.03	0.07	0.50	0.82	0.92	0.83	0.85	0.80	0.95	0.95	0.95	0.94
 chr16	29346604	29347237	0.92	0.94	0.67	0.89	0.95	0.91	0.90	0.94	0.91	0.95	0.97	0.97	0.96	0.91	0.95	0.95	0.95	0.95	0.94	0.95	0.95	0.56	0.84	0.83	0.62	0.86	0.07	0.91	0.94	0.95	0.96	0.97	0.97	0.95	0.95	0.95	0.97	0.97	0.95
 chr16	29633733	29634109	0.94	0.90	0.90	0.82	0.89	0.95	0.81	0.96	0.80	0.94	0.95	0.97	0.91	0.85	0.88	0.86	0.84	0.95	0.92	0.02	0.22	0.76	0.93	0.94	0.82	0.92	0.92	0.90	0.90	0.92	0.95	0.90	0.97	0.97	0.91	0.93	0.92	0.94	0.94
 chr16	29654736	29654910	0.89	0.91	0.90	0.80	0.90	0.89	0.79	0.96	0.77	0.94	0.91	0.96	0.93	0.81	0.92	0.91	0.91	0.95	0.92	0.95	0.95	0.10	0.93	0.95	0.85	0.87	0.94	0.88	0.90	0.91	0.95	0.93	0.90	0.93	0.91	0.89	0.92	0.95	0.94
 chr16	29814412	29814964	0.86	0.82	0.86	0.78	0.79	0.89	0.62	0.94	0.82	0.88	0.22	0.97	0.94	0.93	0.96	0.95	0.98	0.93	0.97	0.90	0.94	0.79	0.96	0.97	0.93	0.93	0.96	0.86	0.90	0.88	0.93	0.91	0.96	0.92	0.86	0.84	0.90	0.81	0.86
-chr16	30282545	30283105	0.90	0.94	0.89	0.88	0.90	0.88	0.84	0.96	NA	0.96	0.95	0.97	0.97	0.93	0.92	0.95	0.96	0.97	0.89	0.71	0.84	0.87	0.96	0.96	0.96	0.97	0.91	0.87	0.95	0.93	0.93	0.95	0.97	0.97	0.93	0.97	0.87	0.04	0.84
 chr16	30417069	30417278	0.88	0.92	0.94	0.90	0.90	0.91	0.90	0.87	0.83	0.89	0.22	0.96	0.97	0.91	0.83	0.79	0.62	0.96	0.93	0.94	0.93	0.79	0.96	0.97	0.96	0.95	0.97	0.84	0.85	0.88	0.86	0.88	0.89	0.83	0.91	0.91	0.89	0.87	0.85
 chr16	30444466	30445012	0.92	0.96	0.89	0.95	0.93	0.90	0.95	0.96	0.92	0.93	0.94	0.17	0.95	0.90	0.97	0.96	0.97	0.95	0.95	0.98	0.97	0.88	0.95	0.97	0.96	0.97	0.92	0.94	0.96	0.95	0.96	0.97	0.96	0.89	0.97	0.83	0.87	0.90	0.91
 chr16	30590032	30590193	0.93	0.94	0.92	0.93	0.92	0.91	0.91	0.96	0.91	0.95	0.95	0.96	0.96	0.95	0.91	0.95	0.94	0.95	0.94	0.96	0.95	0.84	0.96	0.95	0.96	0.97	0.95	0.92	0.94	0.94	0.97	0.96	0.96	0.96	0.94	0.93	0.94	0.69	0.20
 chr16	30709949	30710337	0.90	0.90	0.88	0.91	0.86	0.78	0.88	0.88	0.88	0.92	0.93	0.96	0.95	0.91	0.89	0.86	0.89	0.95	0.94	0.95	0.95	0.85	0.94	0.95	0.73	0.20	0.94	0.90	0.92	0.91	0.96	0.95	0.97	0.89	0.95	0.95	0.94	0.94	0.93
 chr16	30715283	30715434	0.81	0.92	0.87	0.90	0.93	0.84	0.92	0.96	0.92	0.93	0.94	0.94	0.95	0.96	0.93	0.94	0.94	0.96	0.95	0.97	0.93	0.85	0.91	0.84	0.17	0.24	0.81	0.94	0.93	0.95	0.96	0.94	0.96	0.86	0.93	0.93	0.93	0.93	0.94
 chr16	30910770	30910970	0.79	0.86	0.79	0.73	0.63	0.81	0.73	0.91	0.64	0.84	0.91	0.90	0.90	0.72	0.79	0.80	0.78	0.89	0.83	0.91	0.92	0.63	0.86	0.89	0.92	0.91	0.87	0.04	0.10	0.57	0.75	0.78	0.86	0.75	0.82	0.85	0.83	0.91	0.90
 chr16	30946810	30947237	0.91	0.92	0.91	0.90	0.90	0.91	0.89	0.92	0.87	0.91	0.75	0.96	0.92	0.89	0.68	0.04	0.67	0.93	0.93	0.93	0.92	0.90	0.96	0.95	0.96	0.95	0.95	0.89	0.85	0.85	0.91	0.94	0.93	0.85	0.90	0.87	0.91	0.94	0.93
```

### Comparing `nanomix-0.1.1/python/nanomix/tests/test_deconvolute.py` & `nanomix-0.2.0/python/nanomix/tests/test_deconvolute.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,70 +6,71 @@
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 parent_dir = os.path.dirname(script_dir)
 sys.path.append(parent_dir)
 
 from main import *
 
+script_dir = os.path.dirname(os.path.realpath(__file__))
 methylome = os.path.join(script_dir, 'test_data', 'test_methylome.tsv')
 atlas = os.path.join(script_dir, 'test_data', 'test_atlas.tsv')
 sigma_path = os.path.join(script_dir, 'test_data', 'test_sigma.tsv')
 
 class TestMain(unittest.TestCase):
 
     @classmethod
-    def setUpClass(cls):
-        # Write sigma
+    def setupclass(cls):
+        # write sigma
         sigma = [0.3, 0.7]
         coverage = 100
-        # Write an atlas
+        # write an atlas
         with open(atlas, 'w') as f:
             f.write('chr\tstart\tend')
             for i in range(len(sigma)):
                 f.write(f'\tcell{i}')
             f.write('\n')
             for i in range(len(sigma)):
                 f.write(f'chr1\t{i*100}\t{i*100+99}')
                 for j in range(len(sigma)):
                     if i == j:
                         f.write('\t0.99')
                     else:
                         f.write('\t0.01')
                 f.write('\n')
-        # Simulate a methylome
+        # simulate a methylome
         with open(methylome, 'w') as f:
             f.write('chr\tstart\tend\ttotal_calls\tmodified_calls\n')
             for i in range(len(sigma)):
                 # simulate n reads for every region
                 for _ in range(coverage):
                     # choose a cell type wighted by sigma
                     cell_type = np.random.choice(len(sigma), p=sigma)
                     if cell_type == i:
                         f.write(f'chr1\t{i*100}\t{i*100+99}\t1\t1\n')
                     else:
                         f.write(f'chr1\t{i*100}\t{i*100+99}\t1\t0\n')
 
-    def test_llse(self):
-        # Test deconvolute function
-        cell_type_proportions = deconvolute(methylome, atlas, 'llse')
+    # def test_llse(self):
+        # # test deconvolute function
+        # cell_type_proportions = deconvolute(methylome, atlas, 'llse')
 
-        # check that the cell_type proportion values are close
-        self.assertAlmostEqual(cell_type_proportions['cell1'], 0.7, places=1)
+        # # check that the cell_type proportion values are close
+        # self.assertAlmostEqual(cell_type_proportions['cell1'], 0.7, places=1)
 
-    def test_nnls(self):
-        cell_type_proportions = deconvolute(methylome, atlas, 'nnls')
+    # def test_nnls(self):
+        # cell_type_proportions = deconvolute(methylome, atlas, 'nnls')
 
-        # check that the cell_type proportion values are close
-        self.assertAlmostEqual(cell_type_proportions['cell1'], 0.7, places=1)
+        # # check that the cell_type proportion values are close
+        # self.assertAlmostEqual(cell_type_proportions['cell1'], 0.7, places=1)
 
-    def test_llsp(self):
-        cell_type_proportions = deconvolute(methylome, atlas, 'llsp')
+    # def test_llsp(self):
+        # cell_type_proportions = deconvolute(methylome, atlas, 'llsp')
 
-        # check that the cell_type proportion values are close
-        self.assertAlmostEqual(cell_type_proportions['cell1'], 0.7, places=1)
+        # # check that the cell_type proportion values are close
+        # self.assertAlmostEqual(cell_type_proportions['cell1'], 0.7, places=1)
 
     def test_mmse(self):
         cell_type_proportions = deconvolute(methylome, atlas, 'mmse')
 
         # check that the cell_type proportion values are close
         self.assertAlmostEqual(cell_type_proportions['cell1'], 0.7, places=1)
```

### Comparing `nanomix-0.1.1/python/nanomix/tests/test_evaluate.py` & `nanomix-0.2.0/python/nanomix/tests/test_evaluate.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 script_dir = os.path.dirname(os.path.realpath(__file__))
 parent_dir = os.path.dirname(script_dir)
 sys.path.append(parent_dir)
 
 from main import *
 from tools import *
 
+script_dir = os.path.dirname(os.path.realpath(__file__))
 methylome = os.path.join(script_dir, 'test_data', 'test_methylome.tsv')
 atlas = os.path.join(script_dir, 'test_data', 'test_atlas.tsv')
 sigma_path = os.path.join(script_dir, 'test_data', 'test_sigma.tsv')
 
 class TestMain(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
```

### Comparing `nanomix-0.1.1/python/nanomix/tests/test_simulate.py` & `nanomix-0.2.0/python/nanomix/tests/test_simulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 parent_dir = os.path.dirname(script_dir)
 sys.path.append(parent_dir)
 
 from main import *
 
+script_dir = os.path.dirname(os.path.realpath(__file__))
 methylome = os.path.join(script_dir, 'test_data', 'test_methylome.tsv')
 atlas = os.path.join(script_dir, 'test_data', 'test_atlas.tsv')
 sigma_path = os.path.join(script_dir, 'test_data', 'test_sigma.tsv')
 
 class TestMain(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
@@ -49,18 +50,18 @@
                     if cell_type == i:
                         f.write(f'chr1\t{i*100}\t{i*100+99}\t1\t1\n')
                     else:
                         f.write(f'chr1\t{i*100}\t{i*100+99}\t1\t0\n')
 
     def test_simulate(self):
         # Test simulate function
-        simulate(methylome, atlas, sigma_path, 200, 5, 0.0, 1.0)
+        simulate(atlas, sigma_path, 200, 5, 0.0, 1.0)
 
         # check that the cell_type proportions are close to sigma
         # Tissues are enumerated as 0 and 1. so the average of them should be the proportion of tissue2
-        with open(methylome, 'r') as f:
-            lines = f.readlines()
-            cell_types = [int(line.split('\t')[-1].strip()) for line in lines[1:]]
-        self.assertAlmostEqual(sum(cell_types)/len(cell_types), 0.7, places=1)
+        # with open(methylome, 'r') as f:
+            # lines = f.readlines()
+            # cell_types = [int(line.split('\t')[-1].strip()) for line in lines[1:]]
+        # self.assertAlmostEqual(sum(cell_types)/len(cell_types), 0.7, places=1)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `nanomix-0.1.1/Cargo.lock` & `nanomix-0.2.0/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
+name = "approx"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi",
  "libc",
@@ -43,14 +52,20 @@
  "lazy_static",
  "memchr",
  "regex-automata",
  "serde",
 ]
 
 [[package]]
+name = "bytemuck"
+version = "1.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c041d3eab048880cb0b86b256447da3f18859a163c3b8d8893f4e6368abe6393"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
@@ -120,14 +135,25 @@
 [[package]]
 name = "fuchsia-cprng"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06f77d526c1a601b7c4cdd98f54b5eaabffc14d5f2f0296febdc7f357c6d3ba"
 
 [[package]]
+name = "getrandom"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
@@ -162,24 +188,39 @@
 [[package]]
 name = "libc"
 version = "0.2.138"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db6d7e329c562c5dfab7a46a2afabc8b987ab9a4834c9d1ca04dc54c1546cef8"
 
 [[package]]
+name = "libm"
+version = "0.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+
+[[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "logaddexp"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "25958fead7442dae498f9d2d54223b763cf219523dc1490e154b9e645dbfe24d"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "matrixmultiply"
 version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dcad67dcec2d58ff56f6292582377e6921afdf3bfbd533e26fb8900ae575e002"
 dependencies = [
  "rawpointer 0.1.0",
 ]
@@ -205,27 +246,58 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "nanomix"
+name = "nalgebra"
+version = "0.29.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d506eb7e08d6329505faa8a3a00a5dcc6de9f76e0c77e4b75763ae3c770831ff"
+dependencies = [
+ "approx",
+ "matrixmultiply 0.3.2",
+ "nalgebra-macros",
+ "num-complex",
+ "num-rational",
+ "num-traits",
+ "rand 0.8.5",
+ "rand_distr",
+ "simba",
+ "typenum",
+]
+
+[[package]]
+name = "nalgebra-macros"
 version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01fcc0b8149b4632adc89ac3b7b31a12fb6099a0317a4eb2ebff574ef7de7218"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "nanomix"
+version = "0.2.0"
 dependencies = [
  "clap",
  "crossbeam-channel",
  "crossbeam-utils",
  "csv",
  "intervaltree",
+ "logaddexp",
  "ndarray",
  "probability",
  "pyo3",
- "rand",
+ "rand 0.5.6",
  "rulinalg",
+ "statrs",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
@@ -275,20 +347,32 @@
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
+name = "num-rational"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
+ "libm",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
@@ -313,14 +397,26 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
+name = "paste"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d01a5bd0424d00070b0098dd17ebca6f961a959dead1dbcbbbc1d1cd8d3deeba"
+
+[[package]]
+name = "ppv-lite86"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+
+[[package]]
 name = "probability"
 version = "0.15.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec2a43b46675065a24d11f19f8e088abaf07eb38e5eda0115a217758aabf82dd"
 dependencies = [
  "random",
  "special",
@@ -414,14 +510,35 @@
  "fuchsia-cprng",
  "libc",
  "rand_core 0.3.1",
  "winapi",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "libc",
+ "rand_chacha",
+ "rand_core 0.6.4",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core 0.6.4",
+]
+
+[[package]]
 name = "rand_core"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a6fdeb83b075e8266dcc8762c22776f6877a63111121f5f8c7411e5be7eed4b"
 dependencies = [
  "rand_core 0.4.2",
 ]
@@ -429,14 +546,33 @@
 [[package]]
 name = "rand_core"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c33a3c44ca05fa6f1807d8e6743f3824e8509beca625669633be0acbdf509dc"
 
 [[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
+name = "rand_distr"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
+dependencies = [
+ "num-traits",
+ "rand 0.8.5",
+]
+
+[[package]]
 name = "random"
 version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97d13a3485349981c90c79112a11222c3e6e75de1d52b87a7525b3bf5361420f"
 
 [[package]]
 name = "rawpointer"
@@ -478,26 +614,48 @@
 [[package]]
 name = "ryu"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4501abdff3ae82a1c1b477a17252eb69cee9e66eb915c1abaa4f44d873df9f09"
 
 [[package]]
+name = "safe_arch"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
+dependencies = [
+ "bytemuck",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
 version = "1.0.150"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e326c9ec8042f1b5da33252c8a37e9ffbd2c9bef0155215b6e6c80c790e05f91"
 
 [[package]]
+name = "simba"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f0b7840f121a46d63066ee7a99fc81dcabbc6105e437cae43528cea199b5a05f"
+dependencies = [
+ "approx",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "wide",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "special"
@@ -505,14 +663,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24a65e074159b75dcf173a4733ab2188baac24967b5c8ec9ed87ae15fcbc7636"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "statrs"
+version = "0.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d08e5e1748192713cc281da8b16924fb46be7b0c2431854eadc785823e5696e"
+dependencies = [
+ "approx",
+ "lazy_static",
+ "nalgebra",
+ "num-traits",
+ "rand 0.8.5",
+]
+
+[[package]]
 name = "strsim"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ea5119cdb4c55b55d432abb513a0429384878c15dde60cc77b1c99de1a95a6a"
 
 [[package]]
 name = "syn"
@@ -537,14 +708,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
+name = "typenum"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
 
 [[package]]
 name = "unicode-width"
@@ -561,14 +738,30 @@
 [[package]]
 name = "vec_map"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
 
 [[package]]
+name = "wasi"
+version = "0.11.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+
+[[package]]
+name = "wide"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "feff0a412894d67223777b6cc8d68c0dab06d52d95e9890d5f2d47f10dd9366c"
+dependencies = [
+ "bytemuck",
+ "safe_arch",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
```

### Comparing `nanomix-0.1.1/PKG-INFO` & `nanomix-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: nanomix
-Version: 0.1.1
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas~=1.5.2
 Requires-Dist: pyranges==0.0.120
 Requires-Dist: numpy~=1.24.1
 Requires-Dist: scipy~=1.10.0
+Requires-Dist: matplotlib
+Requires-Dist: ray
 License-File: LICENSE
 Summary: Methods for cell type deconvolution from Oxford Nanopore methylation calling
 Keywords: nanopore,methylation,deconvolution
 Author-email: Jonathan Broadbent <jonbroad15@gmail.com>, Jared Simpson <jsimpson@oicr.on.ca>
 Maintainer-email: Jonathan Broadbent <jonbroad15@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -22,77 +24,85 @@
 
 
 ## Installation
 This package is available on PyPI
 ```
 pip install nanomix
 ```
-or alternatively on Conda:
+Alternatively you can install from source. Installing from source requires [maturin](https://github.com/PyO3/maturin)
 ```
-conda install nanomix
-```
-Installing from source requires [maturin](https://github.com/PyO3/maturin)
-```
-conda install maturin
+pip install maturin
 git clone https://github.com/Jonbroad15/nanomix.git
 cd nanomix
 maturin develop
 ```
 
 ## Usage
+### Reference Atlas
+Deconvolution determines the mixture proportion based on methylation propensities of previously resolved sequencing runs of purified reference cells across the genome. This information is collated into an *atlas*. We suggest using the atlas from [Loyfer et. al](https://www.biorxiv.org/content/10.1101/2022.01.24.477547v1.full) which we have curated and labelled as `39Bisulfite.tsv` and is set for default. Their tool [wgbstools](https://github.com/nloyfer/wgbs_tools) also provides the means to create an atlas suited to the cell types you are interested in.
+
+### Deconvolution
 To deconvolute a sequencing run, one must simply provide `nanomix` with a methylome. We define a methylome as a `tsv` file with columns `{chr, start, end, total_calls, modified_calls}`. Such a file can be created from a `.bam` file using our associated program, [mbtools](https://github.com/jts/mbtools)
-Then the mixture proportion can be found by calling:
 ```
-nanomix deconvolute <METHYLOME>
+mbtools region-frequency -r ATLAS.tsv SAMPLE.bam > METHYLOME.tsv
 ```
-
-### Reference Atlas
-Deconvolution determines the mixture proportion based on methylation propensities of previously resolved sequencing runs of purified reference cells across the genome. This information is collated into an *atlas*. We suggest using the atlas from [Loyfer et. al](https://www.biorxiv.org/content/10.1101/2022.01.24.477547v1.full) which we have curated and labelled as `39Bisulfite.tsv` and is set for default. Their tool [wgbstools](https://github.com/nloyfer/wgbs_tools) also provides the means to create an atlas suited to the cell types you are interested in.
+Then the mixture proportion can be found by calling:
 ```
-nanomix deconvolute <METHYLOME> -a <ATLAS>
+nanomix deconvolute -a ATLAS.tsv METHYLOME.tsv
 ```
 
 ### Model
 We provide four deconvolution models
 
-- **llse (default):**   log-likelihood with sequencing errors. Maximize the likelihood of the methylome, atlas and sigma
+- **llse (default):**   log-likelihood with sequencing errors. Maximize the likelihood of sigma
                     by assuming modification calls follow a binomial distribution. Good for sequencing data with high error
-                    rate and non-uniform coverage distribution. (Oxford Nanopore)
+                    rate. (Oxford Nanopore)
 - **nnls:**             non-negative least squares. Minimize the squared error between the methylome and what we expect for
                     the methylome (given sigma and the atlas). Recommended for fast deconvolution of methylomes with high
                     coverage. (Methylation Arrays)
+- **llsp:**             log-likelihood with sequencing perfect. Same as llse, without error modelling. Useful for differentiating the
+                    effect of sequencing errors on deconvolution loss and accuracy.
 - **mmse:**             mixture model with sequencing errors. Also follows a binomial distribution, but softly assigns fragments
                     to cell-types. Optimization uses expectation maximization (slower than above). Recommended for high resolution
                     deconvolution (many cell types) and an atlas with large regions of grouped CpGs.
-- **llsp:**             log-likelihood with sequencing perfect. Same as llse, without error modelling. Useful for differentiating the
-                    effect of sequencing errors on deconvolution loss and accuracy.
 Select a model by:
 ```
-nanomix deconvolute <METHYLOME> -m <MODEL>
+nanomix deconvolute -m MODEL METHYLOME.tsv 
+```
+The **mmse model is distinct** in that it works by assigning reads to cell types. To this effect, one would need a methylome where every row represents a read and columns contain `{read_id, chr, start, end, total_calls, modified_calls}`, this also be constructed from a `.bam` file with [mbtools](https://github.com/jts/mbtools)
+```
+mbtools read-frequency SAMPLE.bam > METHYLOME.tsv
+nanomix deconvolute -m mmse METHYLOME.tsv
 ```
 For more info on other option hparams, run
 ```
 nanomix deconvolute -h
 ```
 
 ### Assign fragments
 Our tools also allows you to assign fragments in the methylome to cell types in the atlas based off of the deconvoluted sigma vector.
 ```
-nanomix assign <METHYLOME> -s <SIGMA> 
+nanomix assign -s SIGMA.tsv METHYLOME.tsv 
 ```
 ### Simulate 
 We provide functionality to simulate methylomes of complex cell mixtures given a `sigma.tsv` file that indicates the cell\_type in the first column and the corresponding proportion in the second column. All the proportions must add up to 1 and the cell-types must be the same as those in the supplied reference atlas. To simulate a methylome:
 ```
-nanomix simulate <SIGMA>
+nanomix simulate -a ATLAS.tsv SIGMA.tsv
 ```
 
 ### Evaluate
 Simulating data provides true cell-type assignments in the last column of the methylome. We can evaluate the performance of a models deconvolution on this methylome. This will output the deconvolution loss (euclidean distance between true and predicted sigma vector) and the read assignment accuracy at confidence levels from 0.5 to 0.9.
 ```
-nanomix evaluate <METHYLOME>
+nanomix evaluate -a ATLAS.tsv METHYLOME.tsv
 ```
 
+### Plot
+You can plot a list of deconvolution mixtures by providing them to the plot function. This will produce a stacked bar plot.
+```
+nanomix plot -o NAME.png *sigma.tsv
+```
+![exampledeconvplot](Images/example_deconvolution_plot.png)
```

