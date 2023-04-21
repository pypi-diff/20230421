# Comparing `tmp/crispr_library_prep-0.1.5.tar.gz` & `tmp/crispr_library_prep-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_library_prep-0.1.5.tar", max compression
+gzip compressed data, was "crispr_library_prep-0.1.6.tar", max compression
```

## Comparing `crispr_library_prep-0.1.5.tar` & `crispr_library_prep-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       57 2023-04-19 13:40:06.389263 crispr_library_prep-0.1.5/crispr_library_prep/__init__.py
--rw-r--r--   0        0        0    20871 2023-04-19 19:18:12.491573 crispr_library_prep-0.1.5/crispr_library_prep/CrisprLibraryPrep.py
--rw-r--r--   0        0        0      529 2023-04-19 20:02:22.646430 crispr_library_prep-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 15:47:11.053642 crispr_library_prep-0.1.5/README.md
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.5/setup.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-04-19 13:40:06.389263 crispr_library_prep-0.1.6/crispr_library_prep/__init__.py
+-rw-r--r--   0        0        0    21663 2023-04-21 15:59:57.934068 crispr_library_prep-0.1.6/crispr_library_prep/CrisprLibraryPrep.py
+-rw-r--r--   0        0        0      529 2023-04-21 16:06:24.918333 crispr_library_prep-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:47:11.053642 crispr_library_prep-0.1.6/README.md
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.6/setup.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.6/PKG-INFO
```

### Comparing `crispr_library_prep-0.1.5/crispr_library_prep/CrisprLibraryPrep.py` & `crispr_library_prep-0.1.6/crispr_library_prep/CrisprLibraryPrep.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 import matplotlib.pyplot as plt
 from scipy.stats import hypergeom, _distn_infrastructure
 from typing import Union, List, Mapping, Tuple, Optional, Any
 from typeguard import typechecked
 import pandas as pd
 from functools import partial
 import multiprocessing
+import time
 
 ### CONSTANTS
 _GENOME_CONC_PG = 6.6
 _PG_TO_NG = 0.001
 _GENOME_CONC_NG = _GENOME_CONC_PG * _PG_TO_NG
 _UG_TO_NG = 1000
 
 @typechecked
 def simulate_gRNA_library_prep(guide_library_size: int, PCR1_input_ug: float, MOI: float,  perfection_rate: float, genome_conc_ng: float = _GENOME_CONC_NG, _PCR1_input_number_duplicate:float = 1, PCR1_cycles: int = 5, _PCR1_purification_yield: float = 0.6,
                               _PCR1_purification_eluted_volume: int = 50, _PCR2_input_volume: float = 22.5,
                               PCR2_cycles:int = 7, _PCR2_purification_yield: float = 0.6,
-                              _total_target_reads: int = 150000, plot=True):
+                              _total_target_reads: Union[int, np.int32] = 150000, plot=True):
+    _total_target_reads = int(_total_target_reads)
+
     '''
     PCR1 input
     '''
     _PCR1_input_number_molecules: float = (((PCR1_input_ug*_UG_TO_NG)/genome_conc_ng)) * MOI
     _PCR1_input_guide_coverage: float = ((_PCR1_input_number_molecules*perfection_rate)/_PCR1_input_number_duplicate)/guide_library_size
     #print(_PCR1_input_guide_coverage)
     '''
@@ -66,19 +69,16 @@
     num_dups_in_PCR2_input_VALUES_LEFT_QUANTILE, num_dups_in_PCR2_input_VALUES_RIGHT_QUANTILE = hypergeom.interval(0.99, population_size, success_size, trial_count)
 
     num_dups_in_PCR2_input_VALUES_LEFT_QUANTILE: int = int(num_dups_in_PCR2_input_VALUES_LEFT_QUANTILE)
     num_dups_in_PCR2_input_VALUES_RIGHT_QUANTILE: int = int(num_dups_in_PCR2_input_VALUES_RIGHT_QUANTILE)
     #print(f"Considering PCR duplicates in range: {num_dups_in_PCR2_input_VALUES_LEFT_QUANTILE} to {num_dups_in_PCR2_input_VALUES_RIGHT_QUANTILE}")
 
     num_dups_in_PCR2_input_VALUES: np.ndarray  = np.arange(num_dups_in_PCR2_input_VALUES_LEFT_QUANTILE, num_dups_in_PCR2_input_VALUES_RIGHT_QUANTILE)
-
     # For each x-value in the interval of interest, get the probability of that number of rarities in the PCR1 input
     num_dups_in_PCR2_input_PROB: np.ndarray = num_dups_in_PCR2_input_DIST.pmf(num_dups_in_PCR2_input_VALUES)
-
-    
     '''
     PCR2 amplification
     '''
     _PCR2_product_number_molecules: float = _PCR2_input_number_molecules * 2**PCR2_cycles
     num_dups_in_PCR2_prod_VALUES: np.ndarray = num_dups_in_PCR2_input_VALUES * 2**PCR2_cycles
     
     '''
@@ -89,28 +89,28 @@
 
     '''
         NGS
     '''
     population_size: int = int(_PCR2_product_purified_number_molecules)
     success_sizes: np.ndarray = num_dups_in_PCR2_prod_purified_VALUES.astype(int)
     trial_count: int = _total_target_reads
-
     num_dups_in_NGS_input_2D_DIST: np.ndarray = np.asarray([hypergeom(population_size, success_size, trial_count) for success_size in success_sizes]) # for each potential amount of duplicates of a PCR1 input molecule, get distribution of number of duplicates in reads
-    num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES: np.ndarray = np.arange(0, 1000) # number of reads per input molecule
+
+    ngs_duplicate_threshold = 15
+    num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES: np.ndarray = np.arange(0, ngs_duplicate_threshold) # number of reads per input molecule
     num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS: np.ndarray = np.asarray([sum([num_dups_in_NGS_input_2D_DIST[i].pmf(num_reads_per_input) *  num_dups_in_PCR2_input_PROB[i] for i in range(len(num_dups_in_PCR2_input_PROB))]) for num_reads_per_input in num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES])
     
-    average_num_of_duplicates_per_PCR1_input_molecule: float = sum(num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS[np.where(np.isin(num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES,np.arange(2,1000)))[0]] * (np.arange(2,1000)-1)) * _PCR1_input_number_molecules
+    #average_num_of_duplicates_per_PCR1_input_molecule: float = sum(num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS[np.where(np.isin(num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES,np.arange(2,ngs_duplicate_threshold)))[0]] * (np.arange(2,ngs_duplicate_threshold)-1)) * _PCR1_input_number_molecules
     
-    num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES_ZT: np.ndarray = num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES[1:]
-    num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS_ZT: np.ndarray = num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS[1:]
+    #num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES_ZT: np.ndarray = num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES[1:]
+    #num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS_ZT: np.ndarray = num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS[1:]
     
-
     # Plot the hypergeometric distribution for number of duplicates in PCR1 input
     if plot:
-        threshold=15
+        threshold=ngs_duplicate_threshold
         fig = plt.figure()
         ax = fig.add_subplot(111)
         ax.plot(num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES[:threshold], num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS[:threshold], 'bo', label="Exact Hypergeometric")
         ax.vlines(num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_VALUES[:threshold], 0, num_dups_in_NGS_input_1D_DIST_MARGINAL_NGS_PROBS[:threshold], lw=2)
         ax.set_xlabel('Number of average reads per\nPCR1 input molecule')
         ax.set_ylabel('Probability')
         ax.set_title("Number of Reads per PCR1 Input Molecule\nread coverage = {}".format(_total_target_reads))
@@ -137,22 +137,31 @@
 
     # Calculate the interpolation and return
     return total_reads_targets_np[target_coverage_indices[0]]  - ((total_reads_targets_np[target_coverage_indices[0]] - total_reads_targets_np[target_coverage_indices[1]]) * (guide_coverages_np[target_coverage_indices[0]] - target_coverage)/(guide_coverages_np[target_coverage_indices[0]] - guide_coverages_np[target_coverage_indices[1]]))
 
 
 # TODO 20230417 - For target_coverage_percentage, a future step is to determine the inflection point manually by either the simulation result or from solving the hypergeometric distribution (which is definitely possible) 
 @typechecked
-def get_target_coverage(gDNA_amount: float, moi: float, sample_name:str, perfection_rate: float, guide_library_size:int, genome_conc_ng: float = _GENOME_CONC_NG, target_coverage_input=None, target_coverage_percentage: float=0.70, read_intervals_count: int= 20):
+def get_target_coverage(gDNA_amount: float, moi: float, sample_name:str, perfection_rate: float, guide_library_size:int, genome_conc_ng: float = _GENOME_CONC_NG, target_coverage_input=None, target_coverage_percentage: float=0.70, read_intervals_count: int= 20, cores=1):
 
     PCR1_input_coverage = (((((gDNA_amount*_UG_TO_NG)/genome_conc_ng)*moi))*perfection_rate)/guide_library_size
     target_coverage_suggested = PCR1_input_coverage * target_coverage_percentage
     max_reads = PCR1_input_coverage * guide_library_size * 5
     
     # Retrieve list of reads to pass into simulation then run simulation
-    total_reads_targets_res = np.arange(max_reads/read_intervals_count, max_reads, max_reads/read_intervals_count)
+    total_reads_targets_res = np.arange(max_reads/read_intervals_count, max_reads, max_reads/read_intervals_count).astype(int)
+
+    simulate_gRNA_library_prep_p = partial(simulate_gRNA_library_prep, guide_library_size = guide_library_size, PCR1_input_ug = gDNA_amount, MOI = moi, perfection_rate=perfection_rate, genome_conc_ng=genome_conc_ng, plot=False)
+    if cores == 1:
+         guide_coverages_res = [simulate_gRNA_library_prep_p(_total_target_reads=total_reads) for total_reads in total_reads_targets_res]
+    else:
+        with multiprocessing.Pool(processes=cores) as pool:
+            guide_coverages_res = pool.map(simulate_gRNA_library_prep_p, total_reads_targets_res)
+            
+
     guide_coverages_res = [simulate_gRNA_library_prep(guide_library_size = guide_library_size, PCR1_input_ug = gDNA_amount, MOI = moi,
                                     _total_target_reads=int(total_reads), perfection_rate=perfection_rate, genome_conc_ng=genome_conc_ng, plot=False) for total_reads in total_reads_targets_res]
     
     # Get the reads for the target coverage
     get_target_coverage_linear_interop_p = partial(get_target_coverage_linear_interop, np.asarray(guide_coverages_res), np.asarray(total_reads_targets_res))
 
     target_read_amount_suggested = get_target_coverage_linear_interop_p(target_coverage=target_coverage_suggested)
@@ -201,17 +210,16 @@
     gDNA_amount_tests = np.arange(max_gDNA_amount/gDNA_intervals_count, max_gDNA_amount, max_gDNA_amount/gDNA_intervals_count)
     
     # Add the max gDNA and ideal gDNA amount
     gDNA_amount_tests = np.append(gDNA_amount_tests, max_gDNA_amount)
     if (ideal_gDNA_amount is not None) and (ideal_gDNA_amount not in gDNA_amount_tests):
         gDNA_amount_tests = np.append(gDNA_amount_tests, ideal_gDNA_amount)
     
-
     # Perform simulation for each gDNA test and visualize
-    get_target_coverage_p = partial(get_target_coverage, moi=moi, sample_name=sample_name, perfection_rate=perfection_rate, guide_library_size=guide_library_size, genome_conc_ng=genome_conc_ng, target_coverage_input=target_coverage_input, target_coverage_percentage=target_coverage_percentage, read_intervals_count=read_intervals_count)
+    get_target_coverage_p = partial(get_target_coverage, moi=moi, sample_name=sample_name, perfection_rate=perfection_rate, guide_library_size=guide_library_size, genome_conc_ng=genome_conc_ng, target_coverage_input=target_coverage_input, target_coverage_percentage=target_coverage_percentage, read_intervals_count=read_intervals_count, cores=1)
 
     if cores == 1:
         print(gDNA_amount_tests)
         target_coverage_result_list = [get_target_coverage_p(gDNA_amount=gDNA_amount_test) for gDNA_amount_test in gDNA_amount_tests]
     else:
         with multiprocessing.Pool(processes=cores) as pool:
             target_coverage_result_list = pool.map(get_target_coverage_p, gDNA_amount_tests)
```

### Comparing `crispr_library_prep-0.1.5/pyproject.toml` & `crispr_library_prep-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crispr-library-prep"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Basheer Becerra <bbecerr@outlook.com>"]
 readme = "README.md"
 packages = [{include = "crispr_library_prep"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `crispr_library_prep-0.1.5/setup.py` & `crispr_library_prep-0.1.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'numpy>=1.23,<2.0',
  'pandas>=1.5.3,<2.0.0',
  'scipy>=1.10.1,<2.0.0',
  'typeguard>=3.0.2,<4.0.0']
 
 setup_kwargs = {
     'name': 'crispr-library-prep',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
     'long_description': '',
     'author': 'Basheer Becerra',
     'author_email': 'bbecerr@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `crispr_library_prep-0.1.5/PKG-INFO` & `crispr_library_prep-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crispr-library-prep
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Basheer Becerra
 Author-email: bbecerr@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

