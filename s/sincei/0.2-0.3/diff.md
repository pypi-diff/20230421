# Comparing `tmp/sincei-0.2.tar.gz` & `tmp/sincei-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sincei-0.2.tar", last modified: Tue Feb  7 18:36:07 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sincei-0.2.tar` & `sincei-0.3.tar`

### file list

```diff
@@ -1,48 +1,32 @@
-drwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)        0 2023-02-07 18:36:07.489312 sincei-0.2/
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     1068 2023-02-03 12:54:15.000000 sincei-0.2/LICENCE.txt
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     2055 2023-02-07 18:36:07.489312 sincei-0.2/PKG-INFO
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     1595 2023-02-06 11:19:54.000000 sincei-0.2/README.md
-drwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)        0 2023-02-07 18:36:07.485312 sincei-0.2/bin/
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)      125 2023-02-03 11:20:29.000000 sincei-0.2/bin/scBulkCoverage
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)      125 2023-02-03 11:20:11.000000 sincei-0.2/bin/scClusterCells
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)      126 2023-02-03 11:19:51.000000 sincei-0.2/bin/scCombineCounts
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)      120 2023-02-03 11:19:36.000000 sincei-0.2/bin/scCountQC
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)      123 2023-02-03 11:19:17.000000 sincei-0.2/bin/scCountReads
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)      127 2023-02-03 11:18:55.000000 sincei-0.2/bin/scFilterBarcodes
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)      124 2023-02-03 11:18:34.000000 sincei-0.2/bin/scFilterStats
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)      116 2023-02-03 11:18:17.000000 sincei-0.2/bin/scJSD
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)     2135 2023-02-03 10:52:07.000000 sincei-0.2/bin/sincei
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)       38 2023-02-07 18:36:07.489312 sincei-0.2/setup.cfg
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)     3272 2023-02-07 18:31:28.000000 sincei-0.2/setup.py
-drwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)        0 2023-02-07 18:36:07.489312 sincei-0.2/sincei/
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     2575 2023-02-03 16:18:30.000000 sincei-0.2/sincei/Clustering.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     5169 2023-02-03 16:18:30.000000 sincei-0.2/sincei/FragmentFFT.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     5014 2023-02-03 16:18:30.000000 sincei-0.2/sincei/GetStats.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)    21586 2023-02-03 16:18:30.000000 sincei-0.2/sincei/ParserCommon.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)    53644 2023-02-03 16:18:30.000000 sincei-0.2/sincei/ReadCounter.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     2835 2023-02-03 16:18:30.000000 sincei-0.2/sincei/RegionQuery.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     8676 2023-02-03 16:18:30.000000 sincei-0.2/sincei/Utilities.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)    12996 2023-02-03 16:18:30.000000 sincei-0.2/sincei/WriteBedGraph.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)      110 2023-02-03 16:18:29.000000 sincei-0.2/sincei/__init__.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     6439 2023-02-03 16:18:30.000000 sincei-0.2/sincei/_deprecated.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)       20 2023-02-03 18:41:31.000000 sincei-0.2/sincei/_version.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     6107 2023-02-03 16:18:30.000000 sincei-0.2/sincei/multimodalClustering.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)    16229 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scBAMops.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)    20755 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scBulkCoverage.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)     6188 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scClusterCells.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)     4811 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scCombineCounts.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)     9602 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scCountQC.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)     8078 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scCountReads.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)     7441 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scFilterBarcodes.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)    11667 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scFilterStats.py
--rwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)     5212 2023-02-03 16:18:30.000000 sincei-0.2/sincei/scJSD.py
-drwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)        0 2023-02-07 18:36:07.489312 sincei-0.2/sincei/test/
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)        0 2023-02-03 16:41:56.000000 sincei-0.2/sincei/test/__init__.py
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)      421 2023-02-03 17:23:54.000000 sincei-0.2/sincei/test/test_tools.py
-drwxrwxr-x   0 vbhardwaj  (1000) vbhardwaj  (1000)        0 2023-02-07 18:36:07.489312 sincei-0.2/sincei.egg-info/
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)     2055 2023-02-07 18:36:07.000000 sincei-0.2/sincei.egg-info/PKG-INFO
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)      876 2023-02-07 18:36:07.000000 sincei-0.2/sincei.egg-info/SOURCES.txt
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)        1 2023-02-07 18:36:07.000000 sincei-0.2/sincei.egg-info/dependency_links.txt
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)        1 2023-02-03 10:34:20.000000 sincei-0.2/sincei.egg-info/not-zip-safe
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)      146 2023-02-07 18:36:07.000000 sincei-0.2/sincei.egg-info/requires.txt
--rw-rw-r--   0 vbhardwaj  (1000) vbhardwaj  (1000)        7 2023-02-07 18:36:07.000000 sincei-0.2/sincei.egg-info/top_level.txt
+-rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 sincei-0.3/sincei/ExponentialFamily.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 sincei-0.3/sincei/FragmentFFT.py
+-rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 sincei-0.3/sincei/GLMPCA.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 sincei-0.3/sincei/GetStats.py
+-rw-r--r--   0        0        0    21422 2020-02-02 00:00:00.000000 sincei-0.3/sincei/ParserCommon.py
+-rw-r--r--   0        0        0    52482 2020-02-02 00:00:00.000000 sincei-0.3/sincei/ReadCounter.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 sincei-0.3/sincei/RegionQuery.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 sincei-0.3/sincei/TopicModels.py
+-rw-r--r--   0        0        0     8624 2020-02-02 00:00:00.000000 sincei-0.3/sincei/Utilities.py
+-rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 sincei-0.3/sincei/WriteBedGraph.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 sincei-0.3/sincei/__init__.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 sincei-0.3/sincei/_deprecated.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sincei-0.3/sincei/_version.py
+-rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 sincei-0.3/sincei/multimodalClustering.py
+-rwxr-xr-x   0        0        0    16039 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scBAMops.py
+-rwxr-xr-x   0        0        0    20499 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scBulkCoverage.py
+-rwxr-xr-x   0        0        0     7812 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scClusterCells.py
+-rwxr-xr-x   0        0        0     4748 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scCombineCounts.py
+-rwxr-xr-x   0        0        0     9502 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scCountQC.py
+-rwxr-xr-x   0        0        0     8048 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scCountReads.py
+-rwxr-xr-x   0        0        0     7377 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scFilterBarcodes.py
+-rwxr-xr-x   0        0        0    11377 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scFilterStats.py
+-rwxr-xr-x   0        0        0     5176 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scJSD.py
+-rwxr-xr-x   0        0        0      385 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scPlotRegion
+-rwxr-xr-x   0        0        0     2126 2020-02-02 00:00:00.000000 sincei-0.3/sincei/sincei.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sincei-0.3/sincei/test/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 sincei-0.3/sincei/test/test_tools.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sincei-0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 sincei-0.3/LICENCE.txt
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sincei-0.3/README.md
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 sincei-0.3/pyproject.toml
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 sincei-0.3/PKG-INFO
```

### Comparing `sincei-0.2/LICENCE.txt` & `sincei-0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `sincei-0.2/README.md` & `sincei-0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 
-<img src="./docs/content/images/sincei.png" alt="sincei logo" style="height: 200px; width:400px;"/>
-
 ## sincei: A user-friendly toolkit for QC, counting, clustering and plotting of single-cell (epi)genomics data.
 
-[![DOI](https://zenodo.org/badge/271841139.svg)](https://zenodo.org/badge/latestdoi/271841139)
-
- - **Documentation**: [![Documentation Status](https://readthedocs.org/projects/sincei/badge/?version=latest)](https://sincei.readthedocs.io/en/latest/?badge=latest)
- - **Source code**: [![test](https://github.com/vivekbhr/sincei/actions/workflows/test.yml/badge.svg)](https://github.com/vivekbhr/sincei/actions/workflows/test.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![DOI](https://zenodo.org/badge/271841139.svg)](https://zenodo.org/badge/latestdoi/271841139) [![Documentation Status](https://readthedocs.org/projects/sincei/badge/?version=latest)](https://sincei.readthedocs.io/en/latest/?badge=latest) [![PyPI Version](https://img.shields.io/pypi/v/sincei.svg?style=plastic)](https://pypi.org/project/sincei/) [![test](https://github.com/vivekbhr/sincei/actions/workflows/test.yml/badge.svg)](https://github.com/vivekbhr/sincei/actions/workflows/test.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+## [Full Documentation](http://sincei.rtfd.io/).
 
 ## Installation
 
 sincei is a command line toolkit based on python3, and can be installed using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html).
 
 Create a new conda environment and install sincei stable release from github using:
 
 ```
-cd <your_programs_folder>
-conda create -n sincei -c conda-forge -c bioconda scanpy deeptools
+conda create -n sincei -c anaconda python=3.8
 conda activate sincei
-(sincei): pip install --editable=git+https://github.com/vivekbhr/sincei.git@master#egg=sincei
+(sincei): pip install sincei
 ```
 
-For the development version, try:
+For the latest development version, try:
 
 ```
-(sincei): pip install --editable=git+https://github.com/vivekbhr/sincei.git@develop#egg=sincei
+(sincei): pip install git+https://github.com/vivekbhr/sincei.git@develop#egg=sincei
 ```
 
 ## Usage
 
 **Get the tool list with `sincei --help`**
 
 Each tool begins with the prefix sc<tool_name>, such as:
 
- $ scBulkCoverage -b file1.bam -g groupinfo.txt -o coverage
+ $ scBulkCoverage -b file1.bam -i groupinfo.txt -o coverage
+
 
-## [Full Documentation](http://sincei.rtfd.io/).
```

### Comparing `sincei-0.2/bin/sincei` & `sincei-0.3/sincei/sincei.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import argparse
 import sys
 import os
+
 ## own functions
-#scriptdir=os.path.abspath(os.path.join(__file__, "../../sincei"))
-#sys.path.append(scriptdir)
+# scriptdir=os.path.abspath(os.path.join(__file__, "../../sincei"))
+# sys.path.append(scriptdir)
 from sincei._version import __version__
 
 
 def parse_arguments(args=None):
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="""
@@ -30,26 +31,25 @@
     scCombineCounts         [WIP] Concatenate/merge the counts from different samples/batches or modalities
     scClusterCells          Perform dimensionality reduction and clustering on the output of scCountReads.
     scBulkCoverage          Get pseudo-bulk coverage per group using a user-supplied cell->group mapping (output of scClusterCells).
     scBAMops                Modify a BAM file to group cells (using cell barcodes), or filter/shift mapped reads.
     scFindMarkers           [WIP] Find marker genes per group, given the output of scCountReads and a user-defined group.
     scFeaturePlot           [WIP] Plot the counts for a given feature on a UMAP or on a (IGV-style) genomic-track.
 
-""".format(__version__))
-
+""".format(
+            __version__
+        ),
+    )
 
     return parser
 
 
 def process_args(args=None):
     args = parse_arguments().parse_args(args)
 
     return args
 
 
 def main(args=None):
     if args is None and len(sys.argv) == 1:
         args = ["--help"]
     process_args(args)
-
-if __name__ == "__main__":
-    main()
```

### Comparing `sincei-0.2/sincei/FragmentFFT.py` & `sincei-0.3/sincei/FragmentFFT.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,15 @@
     fig = plt.figure()
     ax1 = fig.add_subplot(1, 1, 1)
 
     outdict = dict.fromkeys(fragment_len_dict.keys())
     for barcode in outdict.keys():
         fragment_len = fragment_len_dict[barcode]
 
-        n, bins, patches = ax1.hist(
-            fragment_len, bins=100, color="orange", range=(0, 1000), alpha=0.3
-        )
+        n, bins, patches = ax1.hist(fragment_len, bins=100, color="orange", range=(0, 1000), alpha=0.3)
         # calculating fft
         dflist = []
         for num in range(80, 101, 1):
             dflist.append(ffttable(n[10:num]))
         d2 = pd.concat(dflist, ignore_index=True)
         d2 = d2.sort_values(by=["freq"], ascending=False)
         outdict[barcode] = d2
@@ -145,20 +143,16 @@
         max_y_pos = 1 / d2.loc[d2.value.idxmax(), "freq"]
         mean_value = np.mean(d2.value)
 
         ## color barcodes where max periodicity is not between 120 and 160, or 240 and 320
         p1 = range(120, 160, 1)
         p2 = range(240, 320, 1)
 
-        mononuc_periodicity = np.mean(
-            d2.loc[[int(x) in p1 for x in 1 / d2.freq], "value"]
-        )
-        dinuc_periodicity = np.mean(
-            d2.loc[[int(x) in p2 for x in 1 / d2.freq], "value"]
-        )
+        mononuc_periodicity = np.mean(d2.loc[[int(x) in p1 for x in 1 / d2.freq], "value"])
+        dinuc_periodicity = np.mean(d2.loc[[int(x) in p2 for x in 1 / d2.freq], "value"])
 
         # if int(mean_value) in p1:
         #    col='red'
         # elif int(mean_value) in p2:
         #    col='blue'
         # else:
         col = "grey"
```

### Comparing `sincei-0.2/sincei/GetStats.py` & `sincei-0.3/sincei/GetStats.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,15 @@
     o = []
     for fname in args.bamfiles:
         fh = bamHandler.openBam(fname)
         chromUse = utilities.mungeChromosome(chrom, fh.references)
         prev_pos = set()
         lpos = None
         ## initiate a dict with all values to keep per read
-        info_list = (
-            []
-        )  # dict.fromkeys(['barcode', 'position', 'duplicate', 'GCcontent', 'strand'])
+        info_list = []  # dict.fromkeys(['barcode', 'position', 'duplicate', 'GCcontent', 'strand'])
 
         for read in fh.fetch(chromUse, start, end):
             ## general filtering
             if read.pos < start:
                 # ensure that we never double count (in case distanceBetweenBins == 0)
                 continue
             if read.flag & 4:
@@ -85,18 +83,15 @@
             if blackList and blackList.findOverlaps(
                 chrom,
                 read.reference_start,
                 read.reference_start + read.infer_query_length(always=False) - 1,
             ):
                 continue
             if args.motifFilter:
-                test = [
-                    checkMotifs(read, chrom, twoBitGenome, m[0], m[1])
-                    for m in args.motifFilter
-                ]
+                test = [checkMotifs(read, chrom, twoBitGenome, m[0], m[1]) for m in args.motifFilter]
                 # if none given motif found, return true
                 if not any(test):
                     continue
 
             # now collect info
             info = [None for n in range(0, 8)]
             info[0] = chromUse
@@ -126,17 +121,15 @@
                 else:
                     info[4] = abs(float(lpos - read.reference_start))
                 ## also add the distance of this read to previous pos
 
             lpos = read.reference_start
             prev_pos.add(tup)
 
-            info[5] = checkGCcontent(
-                read, args.GCcontentFilter[0], args.GCcontentFilter[1], returnGC=True
-            )
+            info[5] = checkGCcontent(read, args.GCcontentFilter[0], args.GCcontentFilter[1], returnGC=True)
             # filterRNAstrand
             info[6] = read.is_reverse
             if args.getReadID:
                 info[7] = read.query_name
             info_list.append(info)
         fh.close()
```

### Comparing `sincei-0.2/sincei/ParserCommon.py` & `sincei-0.3/sincei/ParserCommon.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
             "-b",
             metavar="FILE1 FILE2",
             help="List of indexed bam files separated by spaces.",
             nargs="+",
             required=True,
         )
     elif "bamfile" in opts:
-        group.add_argument(
-            "--bamfile", "-b", metavar="FILE", help="Indexed BAM file", required=True
-        )
+        group.add_argument("--bamfile", "-b", metavar="FILE", help="Indexed BAM file", required=True)
     if "whitelist" in opts:
         group.add_argument(
             "--whitelist",
             "-w",
             help="A single-column file containing the whitelist of barcodes to be used",
             metavar="TXT",
             default=None,
@@ -58,16 +56,15 @@
             required=True,
         )
 
     if "BED" in opts:
         group.add_argument(
             "--BED",
             help=show_or_hide(
-                "Limits the coverage analysis to "
-                "the regions specified in these files.",
+                "Limits the coverage analysis to " "the regions specified in these files.",
                 "BED",
                 suppress_args,
             ),
             metavar="FILE1.bed FILE2.bed",
             nargs="+",
             required=True if "BED" in requiredOpts else False,
         )
@@ -95,25 +92,19 @@
     return parser
 
 
 def otherOptions(args=None):
     parser = argparse.ArgumentParser(add_help=False)
     group = parser.add_argument_group("Other options")
 
-    group.add_argument(
-        "--help", "-h", action="help", help="show this help message and exit"
-    )
+    group.add_argument("--help", "-h", action="help", help="show this help message and exit")
 
-    group.add_argument(
-        "--verbose", "-v", help="Set to see processing messages.", action="store_true"
-    )
+    group.add_argument("--verbose", "-v", help="Set to see processing messages.", action="store_true")
 
-    group.add_argument(
-        "--version", action="version", version="%(prog)s {}".format(__version__)
-    )
+    group.add_argument("--version", action="version", version="%(prog)s {}".format(__version__))
 
     return parser
 
 
 def plotOptions(args=None):
     parser = argparse.ArgumentParser(add_help=False)
     group = parser.add_argument_group("Plot options")
@@ -366,16 +357,15 @@
     parser = argparse.ArgumentParser(add_help=False)
     group = parser.add_argument_group("Read Processing Options")
 
     group.add_argument(
         "--minMappingQuality",
         metavar="INT",
         help=show_or_hide(
-            "If set, only reads that have a mapping "
-            "quality score of at least this are considered.",
+            "If set, only reads that have a mapping " "quality score of at least this are considered.",
             "minMappingQuality",
             suppress_args,
         ),
         type=int,
     )
 
     group.add_argument(
@@ -426,16 +416,15 @@
         type=int,
         required=False,
     )
 
     group.add_argument(
         "--maxFragmentLength",
         help=show_or_hide(
-            "The maximum fragment length needed for read/pair "
-            "inclusion. (Default: %(default)s)",
+            "The maximum fragment length needed for read/pair " "inclusion. (Default: %(default)s)",
             "maxFragmentLength",
             suppress_args,
         ),
         metavar="INT",
         default=0,
         type=int,
         required=False,
@@ -562,17 +551,15 @@
     elif string == "max":
         # use all available processors
         numberOfProcessors = availProc
     else:
         try:
             numberOfProcessors = int(string)
         except ValueError:
-            raise argparse.ArgumentTypeError(
-                "{} is not a valid number of processors".format(string)
-            )
+            raise argparse.ArgumentTypeError("{} is not a valid number of processors".format(string))
 
         except Exception as e:
             raise argparse.ArgumentTypeError(
                 "the given value {} is not valid. "
                 "Error message: {}\nThe number of "
                 "available processors in your "
                 "computer is {}.".format(string, e, availProc)
@@ -614,17 +601,15 @@
     ## Labels
     if args.groupTag:
         # in case of --groupTag, use args.labels as groups
         if len(args.bamfiles) > 1:
             print("Only a single BAM file is allowed when --groupTag is specified.")
             exit(0)
         if not args.labels:
-            print(
-                "Please indicate the sample groups to be processed from the BAM file with --labels"
-            )
+            print("Please indicate the sample groups to be processed from the BAM file with --labels")
             exit(0)
     else:
         if args.labels and len(args.bamfiles) != len(args.labels):
             print(
                 "The number of labels does not match the number of bam files. "
                 "This is only allowed if a single BAM file is provided and --groupTag is specified."
             )
```

### Comparing `sincei-0.2/sincei/ReadCounter.py` & `sincei-0.3/sincei/ReadCounter.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,17 +278,15 @@
                 verbose=verbose,
             )
             if extendReads is True:
                 # try to guess fragment length if the bam file contains paired end reads
                 if frag_len_dict:
                     self.defaultFragmentLength = int(frag_len_dict["median"])
                 else:
-                    exit(
-                        "*ERROR*: library is not paired-end. Please provide an extension length."
-                    )
+                    exit("*ERROR*: library is not paired-end. Please provide an extension length.")
                 if verbose:
                     print(
                         (
                             "Fragment length based on paired en data "
                             "estimated to be {}".format(frag_len_dict["median"])
                         )
                     )
@@ -297,19 +295,15 @@
                 sys.stderr.write(
                     "*WARNING*: read extension is smaller than read length (read length = {}). "
                     "Reads will not be extended.\n".format(int(read_len_dict["median"]))
                 )
                 self.defaultFragmentLength = "read length"
 
             elif extendReads > 2000:
-                exit(
-                    "*ERROR*: read extension must be smaller that 2000. Value give: {} ".format(
-                        extendReads
-                    )
-                )
+                exit("*ERROR*: read extension must be smaller that 2000. Value give: {} ".format(extendReads))
             else:
                 self.defaultFragmentLength = int(extendReads)
 
         else:
             self.defaultFragmentLength = "read length"
 
         self.numberOfProcessors = numberOfProcessors
@@ -344,17 +338,15 @@
             self.out_file_for_raw_data = out_file_for_raw_data
         else:
             self.save_data = False
             self.out_file_for_raw_data = None
 
         # check that wither numberOfSamples or stepSize are set
         if numberOfSamples is None and stepSize is None and bedFile is None:
-            raise ValueError(
-                "either stepSize, numberOfSamples or bedFile have to be set"
-            )
+            raise ValueError("either stepSize, numberOfSamples or bedFile have to be set")
 
         if self.defaultFragmentLength != "read length":
             self.maxPairedFragmentLength = 4 * self.defaultFragmentLength
         else:
             self.maxPairedFragmentLength = 1000
         if self.maxFragmentLength > 0:
             self.maxPairedFragmentLength = self.maxFragmentLength
@@ -379,25 +371,21 @@
         # the following values are empirical
         if self.stepSize is None:
             if self.region is None:
                 self.stepSize = max(int(float(genomeSize) / self.numberOfSamples), 1)
             else:
                 # compute the step size, based on the number of samples
                 # and the length of the region studied
-                (chrom, start, end) = mapReduce.getUserRegion(chromSizes, self.region)[
-                    :3
-                ]
+                (chrom, start, end) = mapReduce.getUserRegion(chromSizes, self.region)[:3]
                 self.stepSize = max(int(float(end - start) / self.numberOfSamples), 1)
 
         # number of samples is better if large
         if np.mean(chrLengths) < self.stepSize and self.bedFile is None:
             min_num_of_samples = int(genomeSize / np.mean(chrLengths))
-            raise ValueError(
-                "numberOfSamples has to be bigger than {} ".format(min_num_of_samples)
-            )
+            raise ValueError("numberOfSamples has to be bigger than {} ".format(min_num_of_samples))
 
         max_mapped = 0
         if len(self.mappedList) > 0:
             max_mapped = max(self.mappedList)
 
         # If max_mapped is 0 (i.e., bigWig input), set chunkSize to a multiple of binLength and use every bin
         if max_mapped == 0:
@@ -428,17 +416,15 @@
                 y = pyBigWig.open(x)
             # check whether the BAM file has the tags needed
             checkBAMtag(y, x, self.cellTag)
             if self.groupTag:
                 checkBAMtag(y, x, self.groupTag)
             bamFilesHandles.append(y)
 
-        chromsizes, non_common = deeptools.utilities.getCommonChrNames(
-            bamFilesHandles, verbose=self.verbose
-        )
+        chromsizes, non_common = deeptools.utilities.getCommonChrNames(bamFilesHandles, verbose=self.verbose)
 
         # skip chromosome in the list. This is usually for the
         # X chromosome which may have either one copy  in a male sample
         # or a mixture of male/female and is unreliable.
         # Also the skip may contain heterochromatic regions and
         # mitochondrial DNA
         if len(self.chrsToSkip):
@@ -447,17 +433,15 @@
         chrNames, chrLengths = list(zip(*chromsizes))
 
         genomeSize = sum(chrLengths)
 
         chunkSize = None
         if self.bedFile is None:
             if self.genomeChunkSize is None:
-                chunkSize = self.get_chunk_length(
-                    bamFilesHandles, genomeSize, chromsizes, chrLengths
-                )
+                chunkSize = self.get_chunk_length(bamFilesHandles, genomeSize, chromsizes, chrLengths)
             else:
                 chunkSize = self.genomeChunkSize
 
         [bam_h.close() for bam_h in bamFilesHandles]
 
         if self.verbose:
             print("step size is {}".format(self.stepSize))
@@ -609,34 +593,30 @@
         if bed_regions_list is not None:
             # print(bed_regions_list)
             # bed/gtf file is provided
             # in this case the <name> column entry can be optionally saved in the output
             regionNames = [x[2] for x in bed_regions_list]
             if self.bed_and_bin:
                 # further binning needs to be done inside the bed/gtf file (metagene counting, or computeMatrix bins)
-                transcriptsToConsider.append(
-                    [(x[1][0][0], x[1][0][1], self.binLength) for x in bed_regions_list]
-                )
+                transcriptsToConsider.append([(x[1][0][0], x[1][0][1], self.binLength) for x in bed_regions_list])
             else:
                 # simply take the whole regions
                 transcriptsToConsider = [x[1] for x in bed_regions_list]
         else:
             regionNames = None
             # genome-wide binning is needed
             if self.stepSize == self.binLength:
                 # simple tiling of chromosome
                 transcriptsToConsider.append([(start, end, self.binLength)])
             else:
                 # tiling with some stepsize
                 for i in range(start, end, self.stepSize):
                     if i + self.binLength > end:
                         break
-                    if blackList is not None and blackList.findOverlaps(
-                        chrom, i, i + self.binLength
-                    ):
+                    if blackList is not None and blackList.findOverlaps(chrom, i, i + self.binLength):
                         continue
                     transcriptsToConsider.append([(i, i + self.binLength)])
 
         #        if self.save_data:
         #            _file = open(deeptools.utilities.getTempFileName(suffix='.bed'), 'w+t')
         #            _file_name = _file.name
         #        else:
@@ -696,17 +676,15 @@
             else:
                 for exon in trans:
                     for startPos in range(exon[0], exon[1], exon[2]):
                         if idx >= subnum_reads_per_bin.shape[0]:
                             # At the end of chromosomes (or due to blacklisted regions), there are bins smaller than the bin size
                             # Counts there are added to the bin before them, but range() will still try to include them.
                             break
-                        name = "{}_{}_{}::{}".format(
-                            chrom, startPos, min(startPos + exon[2], exon[1]), bedname
-                        )
+                        name = "{}_{}_{}::{}".format(chrom, startPos, min(startPos + exon[2], exon[1]), bedname)
                         regionList.append(name)
                         # _file.write(name+"\n")
                         idx += 1
 
         # save region data as text (if the mtx file is asked)
         if self.save_data:
             _file = open(deeptools.utilities.getTempFileName(suffix=".bed"), "w+t")
@@ -732,17 +710,15 @@
                     start,
                     end,
                 )
             )
 
         return subnum_reads_per_bin, _file_name, regionList
 
-    def get_coverage_of_region(
-        self, bamHandle, chrom, regions, fragmentFromRead_func=None
-    ):
+    def get_coverage_of_region(self, bamHandle, chrom, regions, fragmentFromRead_func=None):
         r"""
         Returns a numpy array that corresponds to the number of reads
         that overlap with each tile.
 
         >>> test = Tester()
         >>> import pysam
         >>> c = CountReadsPerBin([], stepSize=1, extendReads=300)
@@ -781,17 +757,15 @@
             for reg in regions:
                 nbins += (reg[1] - reg[0]) // reg[2]
                 if (reg[1] - reg[0]) % reg[2] > 0:
                     nbins += 1
         # coverages = np.zeros(nbins, dtype='float64')
         ## instead of an array, the coverages object is a dict with keys = barcodes, values = np arrays
         coverages = {}
-        if (
-            self.groupTag and self.groupLabels
-        ):  # multi-sample BAM input, use the reconstructed labels
+        if self.groupTag and self.groupLabels:  # multi-sample BAM input, use the reconstructed labels
             for b in self.groupLabels:
                 coverages[b] = np.zeros(nbins, dtype="float64")
         else:
             for b in self.barcodes:
                 coverages[b] = np.zeros(nbins, dtype="float64")
 
         if self.defaultFragmentLength == "read length":
@@ -843,68 +817,56 @@
             try:
                 if chrom not in bamHandle.references:
                     raise NameError("chromosome {} not found in bam file".format(chrom))
             except:
                 # bigWig input, currently unUSED
                 if bamHandle.chroms(chrom):
                     _ = np.array(
-                        bamHandle.stats(
-                            chrom, regStart, regEnd, type="mean", nBins=nRegBins
-                        ),
+                        bamHandle.stats(chrom, regStart, regEnd, type="mean", nBins=nRegBins),
                         dtype=np.float,
                     )
                     _[np.isnan(_)] = 0.0
                     _ = _ * tileSize
                     coverages[bc] += _
                     continue
                 else:
                     raise NameError(
-                        "chromosome {} not found in bigWig file with chroms {}".format(
-                            chrom, bamHandle.chroms()
-                        )
+                        "chromosome {} not found in bigWig file with chroms {}".format(chrom, bamHandle.chroms())
                     )
 
             prev_pos = set()
             lpos = None  # of previous processed read pair
 
             for read in bamHandle.fetch(chrom, regStart, regEnd):
                 if read.is_unmapped:
                     continue
                 if self.minMappingQuality and read.mapq < self.minMappingQuality:
                     continue
 
                 # filter reads based on SAM flag
-                if (
-                    self.samFlag_include
-                    and read.flag & self.samFlag_include != self.samFlag_include
-                ):
+                if self.samFlag_include and read.flag & self.samFlag_include != self.samFlag_include:
                     continue
                 if self.samFlag_exclude and read.flag & self.samFlag_exclude != 0:
                     continue
 
                 # Fragment lengths
                 tLen = deeptools.utilities.getTLen(read)
                 if self.minFragmentLength > 0 and tLen < self.minFragmentLength:
                     continue
                 if self.maxFragmentLength > 0 and tLen > self.maxFragmentLength:
                     continue
 
                 # Motif filter
                 if self.motifFilter:
-                    test = [
-                        checkMotifs(read, chrom, twoBitGenome, m[0], m[1])
-                        for m in self.motifFilter
-                    ]
+                    test = [checkMotifs(read, chrom, twoBitGenome, m[0], m[1]) for m in self.motifFilter]
                     if not any(test):
                         continue
                 # GC content filter
                 if self.GCcontentFilter:
-                    if not checkGCcontent(
-                        read, self.GCcontentFilter[0], self.GCcontentFilter[1]
-                    ):
+                    if not checkGCcontent(read, self.GCcontentFilter[0], self.GCcontentFilter[1]):
                         continue
 
                 # Aligned fraction filter
                 if self.minAlignedFraction:
                     if not checkAlignedFraction(read, self.minAlignedFraction):
                         continue
 
@@ -912,41 +874,29 @@
                 try:
                     bc = read.get_tag(self.cellTag)
                     if self.groupTag:
                         grp = read.get_tag(self.groupTag)
                         new_bc = "::".join([grp, bc])  # new barcode tag = sample+bc tag
                         if new_bc not in self.groupLabels:
                             if self.verbose:
-                                print(
-                                    "Encountered group: {}, not in provided labels. skipping..".format(
-                                        grp
-                                    )
-                                )
+                                print("Encountered group: {}, not in provided labels. skipping..".format(grp))
                             continue
                     else:
                         new_bc = bc
                 except KeyError:
                     continue
                 # also keep a counter for barcodes not in whitelist?
                 if bc not in self.barcodes:
                     if self.verbose:
-                        print(
-                            "Encountered barcode: {}, not in provided whitelist. skipping..".format(
-                                bc
-                            )
-                        )
+                        print("Encountered barcode: {}, not in provided whitelist. skipping..".format(bc))
                     continue
                 # get rid of duplicate reads with same barcode, startpos and optionally, endpos/umi
                 if self.duplicateFilter:
                     tup = getDupFilterTuple(read, new_bc, self.duplicateFilter)
-                    if (
-                        lpos is not None
-                        and lpos == read.reference_start
-                        and tup in prev_pos
-                    ):
+                    if lpos is not None and lpos == read.reference_start and tup in prev_pos:
                         continue
                     if lpos != read.reference_start:
                         prev_pos.clear()
                     lpos = read.reference_start
                     prev_pos.add(tup)
 
                 # since reads can be split (e.g. RNA-seq reads) each part of the
@@ -1216,22 +1166,18 @@
                     fragmentEnd = read.reference_end
                 else:
                     fragmentStart = read.reference_start
                     fragmentEnd = read.reference_start + self.defaultFragmentLength
 
         if self.center_read:
             fragmentCenter = fragmentEnd - (fragmentEnd - fragmentStart) / 2
-            fragmentStart = int(
-                fragmentCenter - read.infer_query_length(always=False) / 2
-            )
+            fragmentStart = int(fragmentCenter - read.infer_query_length(always=False) / 2)
             fragmentEnd = fragmentStart + read.infer_query_length(always=False)
 
-        assert (
-            fragmentStart < fragmentEnd
-        ), "fragment start greater than fragment" "end for read {}".format(
+        assert fragmentStart < fragmentEnd, "fragment start greater than fragment" "end for read {}".format(
             read.query_name
         )
         return [(fragmentStart, fragmentEnd)]
 
     def getSmoothRange(self, tileIndex, tileSize, smoothRange, maxPosition):
         r"""
         Given a tile index position and a tile size (length), return the a new indices
```

### Comparing `sincei-0.2/sincei/RegionQuery.py` & `sincei-0.3/sincei/RegionQuery.py`

 * *Files identical despite different names*

### Comparing `sincei-0.2/sincei/Utilities.py` & `sincei-0.3/sincei/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 import numpy as np
 import sys
 
 
 def checkBAMtag(bam, name, tag):
     bctag = [read.has_tag(tag) for read in bam.head(1000)]
     if not any(bctag):
-        sys.stderr.write(
-            "WARNING: Input file {} seems to lack the tag {}. Output might be empty. \n".format(
-                name, tag
-            )
-        )
+        sys.stderr.write("WARNING: Input file {} seems to lack the tag {}. Output might be empty. \n".format(name, tag))
     return None
 
 
 def checkMotifs(read, chrom, genome, readMotif, refMotif):
     """
     Check whether a given motif is present in the read and the corresponding reference genome.
     For example, in MNAse (scChIC-seq) data, we expect the reads to have an 'A' at the 5'-end,
```

### Comparing `sincei-0.2/sincei/WriteBedGraph.py` & `sincei-0.3/sincei/WriteBedGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,26 +132,22 @@
 
         """
         # self.__dict__["smoothLength"] = smoothLength
         getStats = len(self.mappedList) < len(self.bamFilesList)
         bam_handles = []
         for x in self.bamFilesList:
             if getStats:
-                bam, mapped, unmapped, stats = bamHandler.openBam(
-                    x, returnStats=True, nThreads=self.numberOfProcessors
-                )
+                bam, mapped, unmapped, stats = bamHandler.openBam(x, returnStats=True, nThreads=self.numberOfProcessors)
                 self.mappedList.append(mapped)
                 self.statsList.append(stats)
             else:
                 bam = bamHandler.openBam(x)
             bam_handles.append(bam)
 
-        genome_chunk_length = getGenomeChunkLength(
-            bam_handles, self.binLength, self.mappedList
-        )
+        genome_chunk_length = getGenomeChunkLength(bam_handles, self.binLength, self.mappedList)
         # check if both bam files correspond to the same species
         # by comparing the chromosome names:
         chrom_names_and_size, non_common = getCommonChrNames(bam_handles, verbose=False)
 
         if self.region:
             # in case a region is used, append the tilesize
             self.region += ":{}".format(self.binLength)
@@ -237,17 +233,15 @@
             if format == "bigwig":
                 bedGraphToBigWig(
                     chrom_names_and_size,
                     [bg_out],
                     "{}_{}.bw".format(out_file_prefix, cl),
                 )
 
-    def writeBedGraph_worker(
-        self, chrom, start, end, func_to_call, func_args, bed_regions_list=None
-    ):
+    def writeBedGraph_worker(self, chrom, start, end, func_to_call, func_args, bed_regions_list=None):
         r"""Writes a bedgraph based on the read coverage per group of cells, indicated by cluster_info data frame.
 
         The given func is called to compute the desired bedgraph value
         using the funcArgs
 
         Parameters
         ----------
@@ -290,18 +284,15 @@
         >>> f = open(tempFile[3], 'r')
         >>> f.readlines()
         ['3R\t0\t100\t0\n', '3R\t100\t200\t1\n']
         >>> f.close()
         >>> os.remove(tempFile[3])
         """
         if start > end:
-            raise NameError(
-                "start position ({0}) bigger "
-                "than end position ({1})".format(start, end)
-            )
+            raise NameError("start position ({0}) bigger " "than end position ({1})".format(start, end))
         coverage, _, r = self.count_reads_in_region(chrom, start, end)
 
         ## get groups (clusters)
         cluster_info = self.clusterInfo
         clusters = cluster_info.cluster.unique().tolist()
         tempfilenames = dict.fromkeys(clusters)
         ## sum up tilecoverage group-wise
@@ -328,28 +319,20 @@
                     previous_value = value
 
                 elif previous_value == value:
                     writeEnd = min(writeEnd + self.binLength, end)
 
                 elif previous_value != value:
                     if not np.isnan(previous_value):
-                        _file.write(
-                            line_string.format(
-                                chrom, writeStart, writeEnd, previous_value
-                            )
-                        )
+                        _file.write(line_string.format(chrom, writeStart, writeEnd, previous_value))
                     previous_value = value
                     writeStart = writeEnd
                     writeEnd = min(writeStart + self.binLength, end)
 
             # write remaining value if not a nan
-            if (
-                previous_value is not None
-                and writeStart != end
-                and not np.isnan(previous_value)
-            ):
+            if previous_value is not None and writeStart != end and not np.isnan(previous_value):
                 _file.write(line_string.format(chrom, writeStart, end, previous_value))
 
             tempfilenames[cl] = _file.name
             _file.close()
 
         return chrom, start, end, tempfilenames
```

### Comparing `sincei-0.2/sincei/_deprecated.py` & `sincei-0.3/sincei/_deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,20 +133,16 @@
 
     G : igraph object
         Graph object.
     """
 
     # cluster on cel-topic dist
     _distances = pairwise_distances(cell_topic.iloc[:, 1:], metric=distance_metric)
-    knn_indices, knn_distances = _get_indices_distances_from_dense_matrix(
-        _distances, nk
-    )
-    distances, connectivities = _compute_connectivities_umap(
-        knn_indices, knn_distances, _distances.shape[0], nk
-    )
+    knn_indices, knn_distances = _get_indices_distances_from_dense_matrix(_distances, nk)
+    distances, connectivities = _compute_connectivities_umap(knn_indices, knn_distances, _distances.shape[0], nk)
 
     if modularityAlg == "leiden":
         if connectivity_graph:
             G = get_igraph_from_adjacency(connectivities, directed=True)
         else:
             G = get_igraph_from_adjacency(distances, directed=True)
         partition = la.find_partition(
```

### Comparing `sincei-0.2/sincei/multimodalClustering.py` & `sincei-0.3/sincei/multimodalClustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import igraph as ig
 import leidenalg as la
 from scipy import sparse
 
 import sys
 
 # own modules
-from sincei.Clustering import LSA_gensim
+from sincei.TopicModels import TOPICMODEL
 from sincei._deprecated import cluster_LSA
 
 # umap.__version__ : should be >= 0.5.1
 
 ## literature on multi-graph clustering
 """
 https://github.com/crisbodnar/regularised-spectral-clustering
@@ -55,72 +55,59 @@
     mode1_adata : AnnData
         AnnData object for mode 1
     mode2_adata : AnnData
         AnnData object for mode 2
     """
 
     # subset RNA anndata
-    mode1_adata = mode1_adata[
-        [
-            i
-            for i, v in enumerate(mode1_adata.obs[column_key])
-            if v in mode2_adata.obs.index
-        ]
-    ]
+    mode1_adata = mode1_adata[[i for i, v in enumerate(mode1_adata.obs[column_key]) if v in mode2_adata.obs.index]]
     # re-compute distances/clusters/umap
     sc.pp.neighbors(mode1_adata, n_neighbors=nK)
     sc.tl.louvain(mode1_adata)
     sc.tl.umap(mode1_adata, min_dist=0.5, spread=5, init_pos="random", random_state=42)
     # get graph
     G_rna = get_igraph_from_adjacency(mode1_adata.obsp["connectivities"], directed=True)
 
     # subset chic anndata
     # mode2_adata=mode2_adata[[i for i,v in enumerate(mode2_adata.obs_names.to_list()) if v in set(mode1_adata.obs[column_key])]]
     mode2_adata = mode2_adata[mode1_adata.obs[column_key].tolist()]
     # re-do LSA
     mtx = sparse.csr_matrix(mode2_adata.X.transpose())
-    corpus_lsi, cell_topic = LSA_gensim(
+    dat = TOPICMODEL(
         mtx,
         list(mode2_adata.obs.index),
         list(mode2_adata.var.index),
         nTopics=20,
         smartCode="lfu",
     )
+    dat.runLSA()
+    cell_topic = dat.get_cell_topic()
+
     # get graph
-    chic_umap, G_chic = cluster_LSA(
-        cell_topic, modularityAlg="leiden", resolution=1, nk=nK
-    )
+    chic_umap, G_chic = cluster_LSA(cell_topic, modularityAlg="leiden", resolution=1, nk=nK)
     mode2_adata.obsm["X_pca"] = cell_topic
     mode2_adata.obsm["X_umap"] = chic_umap
     # leiden multi-layer clustering
     optimiser = la.Optimiser()
     part_rna = la.ModularityVertexPartition(G_rna)
     part_chic = la.ModularityVertexPartition(G_chic)
     #
     # part_rna = la.CPMVertexPartition(G_rna, resolution=res_layer1)
     # part_chic = la.CPMVertexPartition(G_chic, resolution=res_layer2)
-    optimiser.optimise_partition_multiplex(
-        [part_rna, part_chic], layer_weights=[2, 1], n_iterations=-1
-    )
+    optimiser.optimise_partition_multiplex([part_rna, part_chic], layer_weights=[2, 1], n_iterations=-1)
     print("Detected clusters: ", set(part_chic.membership))
     chic_umap["cluster_multi"] = part_chic.membership
 
     # merge RNA and ChIC UMAPs
-    rna_umap = pd.DataFrame(
-        mode1_adata.obsm["X_umap"], columns=["RNA_UMAP1", "RNA_UMAP2"]
-    )
+    rna_umap = pd.DataFrame(mode1_adata.obsm["X_umap"], columns=["RNA_UMAP1", "RNA_UMAP2"])
     rna_umap.index = mode1_adata.obs.index
     rna_umap["cluster_mode1"] = mode1_adata.obs.louvain
     rna_umap[column_key] = mode1_adata.obs[column_key]
-    multi_umap = rna_umap.merge(
-        chic_umap, left_index=False, right_index=True, left_on=column_key
-    )
-    multi_umap["cluster_mode1"] = [
-        int(x) for x in multi_umap["cluster_mode1"].to_list()
-    ]
+    multi_umap = rna_umap.merge(chic_umap, left_index=False, right_index=True, left_on=column_key)
+    multi_umap["cluster_mode1"] = [int(x) for x in multi_umap["cluster_mode1"].to_list()]
 
     return multi_umap, mode1_adata, mode2_adata
 
 
 ## run aligned UMAPs between two dfs with PCs
 def umap_aligned(pca_mode1, pca_mode2, nK=15, distance_metric="eucledian"):
     r"""
```

### Comparing `sincei-0.2/sincei/scBAMops.py` & `sincei-0.3/sincei/scBAMops.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 
 ## UPDATE: add group tag to BAM file based on a 2-columns mapping file (barcode -> group)
 
 
 def parseArguments():
     internalParser = get_args()
     ioParser = ParserCommon.inputOutputOptions(opts=["bamfile", "groupInfo", "outFile"])
-    bamParser = ParserCommon.bamOptions(
-        suppress_args=["binSize", "distanceBetweenBins"]
-    )
+    bamParser = ParserCommon.bamOptions(suppress_args=["binSize", "distanceBetweenBins"])
     filterParser = ParserCommon.filterOptions()
     readParser = ParserCommon.readOptions(suppress_args=["extendReads", "centerReads"])
     otherParser = ParserCommon.otherOptions()
     parser = argparse.ArgumentParser(
         parents=[
             ioParser,
             internalParser,
@@ -186,24 +184,21 @@
         total += 1
 
         bc = read.get_tag(args.cellTag)
         if isinstance(args.groupInfo, pd.DataFrame):
             smpl = read.get_tag(args.groupTag)
             try:
                 tag_to_add = args.groupInfo.loc[
-                    (args.groupInfo["sample"] == smpl)
-                    & (args.groupInfo["barcode"] == bc),
+                    (args.groupInfo["sample"] == smpl) & (args.groupInfo["barcode"] == bc),
                     "cluster",
                 ].values.item()
                 read.set_tag(args.outTagName, tag_to_add, value_type="Z", replace=True)
             except:
                 if args.verbose:
-                    sys.stderr.write(
-                        "Encountered read tags not in groupInfo file, skipped.."
-                    )
+                    sys.stderr.write("Encountered read tags not in groupInfo file, skipped..")
                 nFiltered += 1
                 if ofiltered:
                     ofiltered.write(read)
                 continue
 
         ## -- begin filtering -- ##
         if read.flag & 4:
@@ -215,18 +210,15 @@
 
         if args.minMappingQuality and read.mapq < args.minMappingQuality:
             nFiltered += 1
             if ofiltered:
                 ofiltered.write(read)
             continue
 
-        if (
-            args.samFlagInclude
-            and read.flag & args.samFlagInclude != args.samFlagInclude
-        ):
+        if args.samFlagInclude and read.flag & args.samFlagInclude != args.samFlagInclude:
             nFiltered += 1
             if ofiltered:
                 ofiltered.write(read)
             continue
         if args.samFlagExclude and read.flag & args.samFlagExclude != 0:
             nFiltered += 1
             if ofiltered:
@@ -255,27 +247,23 @@
             if lpos != read.reference_start:
                 prev_pos.clear()
             lpos = read.reference_start
             prev_pos.add(tup)
 
         # remove reads with low/high GC content
         if args.GCcontentFilter:
-            if not checkGCcontent(
-                read, args.GCcontentFilter[0], args.GCcontentFilter[1]
-            ):
+            if not checkGCcontent(read, args.GCcontentFilter[0], args.GCcontentFilter[1]):
                 nFiltered += 1
                 if ofiltered:
                     ofiltered.write(read)
                 continue
 
         # remove reads that don't pass the motif filter
         if args.motifFilter:
-            if not checkMotifs(
-                read, chrom, twoBitGenome, args.motifFilter[0], args.motifFilter[1]
-            ):
+            if not checkMotifs(read, chrom, twoBitGenome, args.motifFilter[0], args.motifFilter[1]):
                 nFiltered += 1
                 if ofiltered:
                     ofiltered.write(read)
                 continue
 
         # filterRNAstrand
         if args.filterRNAstrand:
@@ -387,17 +375,15 @@
         if len(args.shift) not in [2, 4]:
             sys.exit("The --shift option can accept either 2 or 4 values only.")
         if len(args.shift) == 2:
             args.shift.extend([-args.shift[1], -args.shift[0]])
     elif args.ATACshift:
         args.shift = [4, -5, 5, -4]
 
-    bam, mapped, unmapped, stats = openBam(
-        args.bamfile, returnStats=True, nThreads=args.numberOfProcessors
-    )
+    bam, mapped, unmapped, stats = openBam(args.bamfile, returnStats=True, nThreads=args.numberOfProcessors)
     total = mapped + unmapped
     chrom_sizes = [(x, y) for x, y in zip(bam.references, bam.lengths)]
     chromDict = {x: y for x, y in zip(bam.references, bam.lengths)}
 
     # if motifFilter is given, convert the input to list
     if args.motifFilter:
         if not args.genome2bit:
```

### Comparing `sincei-0.2/sincei/scBulkCoverage.py` & `sincei-0.3/sincei/scBulkCoverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 from sincei import ParserCommon
 from sincei import WriteBedGraph
 
 debug = 0
 
 
 def parseArguments():
-    io_args = ParserCommon.inputOutputOptions(
-        opts=["bamfiles", "groupInfo", "outFilePrefix"]
-    )
+    io_args = ParserCommon.inputOutputOptions(opts=["bamfiles", "groupInfo", "outFilePrefix"])
     bam_args = ParserCommon.bamOptions(default_opts={"binSize": 100})
     read_args = ParserCommon.readOptions()
     filter_args = ParserCommon.filterOptions()
     other_args = ParserCommon.otherOptions()
     parser = argparse.ArgumentParser(
         parents=[io_args, get_args(), bam_args, filter_args, read_args, other_args],
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -173,46 +171,39 @@
     df_not_in_labels = set(df["sample"]).difference(set(args.labels))
     if bool(df_not_in_labels):
         sys.stderr.write(
             "Some (or all) of the samples indicated in the groupInfo file "
             "are absent from the bam file labels! \n"
             "Mismatched samples are: {} \n".format(df_not_in_labels)
         )
+        df = df.loc[df["sample"].isin(set(args.labels)),]
     elif bool(labels_not_in_df):
         sys.stderr.write(
             "Some (or all) of the samples indicated in --labels "
             "are absent from the in the groupInfo file! \n"
             "Mismatched samples are: {} \n".format(labels_not_in_df)
         )
 
     # make another df, containing union of all barcodes, and in the same order per sample
     barcodes = df["barcode"].unique().tolist()
-    sm = list(
-        itertools.chain.from_iterable(
-            itertools.repeat(lab, len(barcodes)) for lab in args.labels
-        )
-    )
+    sm = list(itertools.chain.from_iterable(itertools.repeat(lab, len(barcodes)) for lab in args.labels))
     bc = barcodes * len(args.labels)
     groupInfo = pd.DataFrame({"sample": sm, "barcode": bc})
-    groupInfo.index = groupInfo[["sample", "barcode"]].apply(
-        lambda x: "::".join(x), axis=1
-    )
+    groupInfo.index = groupInfo[["sample", "barcode"]].apply(lambda x: "::".join(x), axis=1)
     groupInfo = pd.merge(
         groupInfo,
         df["cluster"],
         how="left",
         left_index=True,
         right_index=True,
         sort=False,
     )
     groupInfo = groupInfo.reset_index()[["sample", "barcode", "cluster"]]
     # re-construct new labels (sample+bc)
-    newlabels = [
-        "::".join([x, y]) for x, y in zip(groupInfo["sample"], groupInfo["barcode"])
-    ]
+    newlabels = ["::".join([x, y]) for x, y in zip(groupInfo["sample"], groupInfo["barcode"])]
     # Normalization options
     scale_factor = args.scaleFactor
     func_args = {"scaleFactor": args.scaleFactor}
 
     coverageAsFrequency = False
     if not args.ignoreForNormalization:
         args.ignoreForNormalization = []
@@ -238,17 +229,15 @@
                 blackListFileName=args.blackListFileName,
                 numberOfProcessors=args.numberOfProcessors,
                 verbose=args.verbose,
             )
             for file in args.bamfiles
         ]
         if any([x[0] is None for x in fraglengths]):
-            sys.exit(
-                "*Error*: For the --MNAse function a paired end library is required. "
-            )
+            sys.exit("*Error*: For the --MNAse function a paired end library is required. ")
 
         # Set some default fragment length bounds
         if args.minFragmentLength == 0:
             args.minFragmentLength = 130
         if args.maxFragmentLength == 0:
             args.maxFragmentLength = 200
 
@@ -284,17 +273,15 @@
     elif args.Offset:
         if len(args.Offset) > 1:
             if args.Offset[0] == 0:
                 sys.exit(
                     "*Error*: An offset of 0 isn't allowed, since offsets are 1-based positions inside each alignment."
                 )
             if args.Offset[1] > 0 and args.Offset[1] < args.Offset[0]:
-                sys.exit(
-                    "'Error*: The right side bound is less than the left-side bound. This is inappropriate."
-                )
+                sys.exit("'Error*: The right side bound is less than the left-side bound. This is inappropriate.")
         else:
             if args.Offset[0] == 0:
                 sys.exit(
                     "*Error*: An offset of 0 isn't allowed, since offsets are 1-based positions inside each alignment."
                 )
         wr = OffsetFragment(
             args.bamfiles,
@@ -412,40 +399,34 @@
                 if read.is_reverse:
                     foo = (read.next_reference_start, read.reference_start)
                     if foo[0] < foo[1]:
                         blocks.insert(0, foo)
                 else:
                     foo = (
                         read.reference_end,
-                        read.reference_end
-                        + abs(read.template_length)
-                        - read.infer_query_length(),
+                        read.reference_end + abs(read.template_length) - read.infer_query_length(),
                     )
                     if foo[0] < foo[1]:
                         blocks.append(foo)
 
             # Extend using the default fragment length
             else:
                 if read.is_reverse:
                     foo = (
-                        read.reference_start
-                        - self.defaultFragmentLength
-                        + read.infer_query_length(),
+                        read.reference_start - self.defaultFragmentLength + read.infer_query_length(),
                         read.reference_start,
                     )
                     if foo[0] < 0:
                         foo = (0, foo[1])
                     if foo[0] < foo[1]:
                         blocks.insert(0, foo)
                 else:
                     foo = (
                         read.reference_end,
-                        read.reference_end
-                        + self.defaultFragmentLength
-                        - read.infer_query_length(),
+                        read.reference_end + self.defaultFragmentLength - read.infer_query_length(),
                     )
                     if foo[0] < foo[1]:
                         blocks.append(foo)
 
         stretch = []
         # For the sake of simplicity, convert [(10, 20), (30, 40)] to [10, 11, 12, 13, ..., 40]
         # Then subset accordingly
@@ -469,17 +450,15 @@
             return rv
         if read.is_reverse:
             foo = foo[::-1]
 
         # Convert the stretch back to a list of tuples
         foo = np.array(foo)
         d = foo[1:] - foo[:-1]
-        idx = (
-            np.argwhere(d > 1).flatten().tolist()
-        )  # This now holds the interval bounds as a list
+        idx = np.argwhere(d > 1).flatten().tolist()  # This now holds the interval bounds as a list
         idx.append(-1)
         last = 0
         rv = []
         for i in idx:
             rv.append((foo[last].astype("int"), foo[i].astype("int") + 1))
             last = i + 1
```

### Comparing `sincei-0.2/sincei/scClusterCells.py` & `sincei-0.3/sincei/scClusterCells.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import sys
 import os
+import copy
 import argparse
 import numpy as np
 import pandas as pd
+import torch
 from scipy import sparse, io
 from sklearn.preprocessing import binarize
 
 # plotting
 import matplotlib
 import matplotlib.pyplot as plt
 
@@ -23,21 +25,20 @@
 
 
 ## own Functions
 # scriptdir=os.path.abspath(os.path.join(__file__, "../../sincei"))
 # sys.path.append(scriptdir)
 
 from sincei import ParserCommon
-from sincei.Clustering import LSA_gensim
+from sincei.TopicModels import TOPICMODEL
+from sincei.GLMPCA import GLMPCA, EXPONENTIAL_FAMILY_DICT
 
 
 def parseArguments():
-    io_args = ParserCommon.inputOutputOptions(
-        opts=["loomfile", "outFile"], requiredOpts=["outFile"]
-    )
+    io_args = ParserCommon.inputOutputOptions(opts=["loomfile", "outFile"], requiredOpts=["outFile"])
     plot_args = ParserCommon.plotOptions()
     other_args = ParserCommon.otherOptions()
 
     parser = argparse.ArgumentParser(
         parents=[io_args, get_args(), plot_args, other_args],
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,  # argparse.RawDescriptionHelpFormatter,
         description="""
@@ -74,20 +75,29 @@
         "to the existing cluster of cells.",
     )
 
     general.add_argument(
         "--method",
         "-m",
         type=str,
-        choices=["LSA"],
+        choices=["LSA", "LDA", "glmPCA"],
         default="LSA",
         help="The dimentionality reduction method for clustering. (Default: %(default)s)",
     )
 
     general.add_argument(
+        "--glmPCAfamily",
+        "-gf",
+        type=str,
+        choices=EXPONENTIAL_FAMILY_DICT.keys(),
+        default="poisson",
+        help="The choice of exponential family distribution to use for glmPCA method. (Default: %(default)s)",
+    )
+
+    general.add_argument(
         "--binarize",
         action="store_true",
         help="Binarize the counts per region before dimentionality reduction (only for LSA/LDA)",
     )
 
     general.add_argument(
         "--nPrinComps",
@@ -122,59 +132,93 @@
 
 
 def main(args=None):
     args = parseArguments().parse_args(args)
 
     adata = sc.read_loom(args.input, obs_names="obs_names", var_names="var_names")
 
-    ## LSA and clustering based on gensim
-    mtx = sparse.csr_matrix(adata.X.transpose())
+    mtx = sparse.csr_matrix(adata.X.copy().transpose())  # features x cells
+    cells = copy.deepcopy(adata.obs_names.to_list())
+    regions = copy.deepcopy(adata.var_names.to_list())
+
     if args.binarize:
         mtx = binarize(mtx, copy=True)
-    corpus_lsi, cell_topic, corpus_tfidf = LSA_gensim(
-        mtx,
-        list(adata.obs.index),
-        list(adata.var.index),
-        nTopics=args.nPrinComps,
-        smartCode="lfu",
-    )
 
-    ## update the anndata object, drop cells which are not in the anndata
-    adata = adata[cell_topic.index]
-    adata.obsm["X_pca"] = np.asarray(cell_topic.iloc[:, 1 : args.nPrinComps])
+    if args.method == "LSA":
+        ## LSA using gensim
+        model_object = TOPICMODEL(
+            mtx,
+            cells,
+            regions,
+            n_topics=args.nPrinComps,
+            smart_code="lfu",
+        )
+        model_object.runLSA()
+        cell_topic = model_object.get_cell_topic(pop_sparse_cells=True)
+        ## update the anndata object, drop cells which are not in the anndata, drop 1st PC
+        adata = adata[cell_topic.index]
+        adata.obsm["X_pca"] = np.asarray(cell_topic.iloc[:, 1 : args.nPrinComps])
+
+    elif args.method == "LDA":
+        ## LDA using gensim
+        model_object = TOPICMODEL(
+            mtx,
+            cells,
+            regions,
+            n_topics=args.nPrinComps,
+            n_passes=2,
+            n_workers=4,
+        )
+        model_object.runLDA()
+        cell_topic = model_object.get_cell_topic(pop_sparse_cells=True)
+        ## update the anndata object, drop cells which are not in the anndata, drop 1st PC
+        adata = adata[cell_topic.index]
+        adata.obsm["X_pca"] = np.asarray(cell_topic.iloc[:, 1 : args.nPrinComps])
+
+    elif args.method == "glmPCA":
+        # convert mtx to torch tensor
+        mtx = torch.tensor(mtx.todense())  # feature*cell tensor
+
+        ## glmPCA using mctorch
+        model_object = GLMPCA(
+            n_pc=args.nPrinComps,
+            family=args.glmPCAfamily,
+        )
+        model_object.fit(mtx)
+        cell_pcs = model_object.saturated_loadings_.detach().numpy()
+
+        ## update the anndata object
+        adata.obsm["X_pca"] = np.asarray(cell_pcs)
+
     sc.pp.neighbors(adata, use_rep="X_pca", n_neighbors=args.nNeighbors)
     sc.tl.leiden(adata, resolution=args.clusterResolution)
     sc.tl.paga(adata)
     sc.pl.paga(adata, plot=False, threshold=0.1)
     sc.tl.umap(adata, min_dist=0.1, spread=5, init_pos="paga")
 
     adata.write_loom(args.outFile, write_obsm_varm=True)
 
     if args.outFileUMAP:
         ## plot UMAP
-        fig = sc.pl.umap(
-            adata, color="leiden", legend_loc="on data", return_fig=True, show=False
-        )
+        fig = sc.pl.umap(adata, color="leiden", legend_loc="on data", return_fig=True, show=False)
         fig.savefig(args.outFileUMAP, dpi=200, format=args.plotFileFormat)
         prefix = args.outFileUMAP.split(".")[0]
-        umap_lsi = pd.DataFrame(
-            adata.obsm["X_umap"], columns=["UMAP1", "UMAP2"], index=adata.obs.index
-        )
+        umap_lsi = pd.DataFrame(adata.obsm["X_umap"], columns=["UMAP1", "UMAP2"], index=adata.obs.index)
         umap_lsi["cluster"] = adata.obs["leiden"]
         umap_lsi.to_csv(prefix + ".tsv", sep="\t", index_label="cell_id")
         # plt.rcParams['font.size'] = 8.0
         # convert cm values to inches
         # fig = plt.figure(figsize=(args.plotWidth / 2.54, args.plotHeight / 2.54))
         # fig.suptitle('LSA-UMAP', y=(1 - (0.06 / args.plotHeight)))
         # plt.scatter(umap_lsi.UMAP1, umap_lsi.UMAP2, s=5, alpha = 0.8, c=[sns.color_palette()[x] for x in list(umap_lsi.cluster)])
         # plt.tight_layout()
         # plt.savefig(args.outFileUMAP, dpi=200, format=args.plotFileFormat)
         # plt.close()
 
     # save if asked
     if args.outFileTrainedModel:
-        corpus_lsi.save(args.outFileTrainedModel)
+        model_object.lsi_model.save(args.outFileTrainedModel)
     #    if args.outGraph:
     # 'The output file for the Graph object (lgl format) which can be used for further clustering/integration.'
     #        graph.write_lgl(args.outGraph)
 
     return 0
```

### Comparing `sincei-0.2/sincei/scCombineCounts.py` & `sincei-0.3/sincei/scCombineCounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import scanpy as sc
 
 
 ## own Functions
 # scriptdir=os.path.abspath(os.path.join(__file__, "../../sincei"))
 # sys.path.append(scriptdir)
 from sincei import ParserCommon
-from sincei.Clustering import LSA_gensim
 
 
 def parseArguments():
     other_args = ParserCommon.otherOptions()
 
     parser = argparse.ArgumentParser(
         parents=[get_args(), other_args],
@@ -102,18 +101,15 @@
         print("The number of labels does not match the number of input files.")
         sys.exit(1)
     if not args.labels:
         if args.smartLabels:
             args.labels = smartLabels(args.input)
         else:
             args.labels = [os.path.basename(x) for x in args.input]
-    adata_list = [
-        sc.read_loom(x, obs_names="obs_names", var_names="var_names")
-        for x in args.input
-    ]
+    adata_list = [sc.read_loom(x, obs_names="obs_names", var_names="var_names") for x in args.input]
 
     ## concatenate labels and match chrom, start, end
     var_list = []
     var_cols = ["chrom", "start", "end"]
     for lab, ad in zip(args.labels, adata_list):
         obs = ad.obs_names.to_list()
         lab = [lab] * len(obs)
```

### Comparing `sincei-0.2/sincei/scCountQC.py` & `sincei-0.3/sincei/scCountQC.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,24 @@
     # 1. regions
     if bad_chrom:
         adata = adata[:, ~adata.var.chrom.isin(bad_chrom)]
     if filter_region_dict:
         for key in filter_region_dict.keys():
             adata = adata[
                 :,
-                (adata.var[key] >= filter_region_dict[key][0])
-                & (adata.var[key] <= filter_region_dict[key][1]),
+                (adata.var[key] >= filter_region_dict[key][0]) & (adata.var[key] <= filter_region_dict[key][1]),
             ]
 
     # 2. Cells
     if bad_cells:
         adata = adata[~adata.obs.index.isin(bad_cells)]
     if filter_cell_dict:
         for key in filter_cell_dict.keys():
             adata = adata[
-                (adata.obs[key] >= filter_cell_dict[key][0])
-                & (adata.obs[key] <= filter_cell_dict[key][1]),
+                (adata.obs[key] >= filter_cell_dict[key][0]) & (adata.obs[key] <= filter_cell_dict[key][1]),
                 :,
             ]
 
     return adata
 
 
 """
@@ -201,27 +199,21 @@
         obs_tsv = mat + ".cells.tsv"
         var_tsv = mat + ".regions.tsv"
         adata.obs.to_csv(obs_tsv, sep="\t", index_label="cell_id")
         adata.var.to_csv(var_tsv, sep="\t", index_label="feature_id")
 
     # if --describe is asked, only print the numeric vars and obs columns
     if args.describe:
-        is_num_col = [
-            (pd.api.types.is_float_dtype(x) | pd.api.types.is_integer_dtype(x))
-            for x in adata.obs.dtypes
-        ]
+        is_num_col = [(pd.api.types.is_float_dtype(x) | pd.api.types.is_integer_dtype(x)) for x in adata.obs.dtypes]
         cols = adata.obs.loc[:, is_num_col]
         sys.stdout.write("\n Cell metrics: \n")
         sys.stdout.write("Total cells: {} \n".format(adata.shape[0]))
         print(pd.DataFrame({"min": cols.min(), "max": cols.max()}))
 
-        is_num_row = [
-            (pd.api.types.is_float_dtype(x) | pd.api.types.is_integer_dtype(x))
-            for x in adata.var.dtypes
-        ]
+        is_num_row = [(pd.api.types.is_float_dtype(x) | pd.api.types.is_integer_dtype(x)) for x in adata.var.dtypes]
         rows = adata.var.loc[:, is_num_row]
         sys.stdout.write("\n Feature metrics: \n")
         sys.stdout.write("Total features: {} \n".format(adata.shape[1]))
         print(pd.DataFrame({"min": rows.min(), "max": rows.max()}))
         exit()
 
     if args.filterCellArgs:
```

### Comparing `sincei-0.2/sincei/scCountReads.py` & `sincei-0.3/sincei/scCountReads.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,17 +69,15 @@
         parents=[
             ParserCommon.inputOutputOptions(
                 opts=["bamfiles", "barcodes", "outFilePrefix", "BED"],
                 requiredOpts=["barcodes", "outFilePrefix"],
                 suppress_args=["BED"],
             ),
             parserCommon.gtf_options(suppress=True),
-            ParserCommon.bamOptions(
-                default_opts={"binSize": 10000, "distanceBetweenBins": 0}
-            ),
+            ParserCommon.bamOptions(default_opts={"binSize": 10000, "distanceBetweenBins": 0}),
             read_args,
             filter_args,
             get_args(),
             other_args,
         ],
         help="The reads are counted in bins of equal size. The bin size and distance between bins can be adjusted.",
         add_help=False,
```

### Comparing `sincei-0.2/sincei/scFilterBarcodes.py` & `sincei-0.3/sincei/scFilterBarcodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 # scriptdir=os.path.abspath(os.path.join(__file__, "../../sincei"))
 # sys.path.append(scriptdir)
 from sincei.Utilities import *
 from sincei import ParserCommon
 
 
 def parseArguments():
-    io_args = ParserCommon.inputOutputOptions(
-        opts=["bamfile", "whitelist", "outfile"], requiredOpts=["bamfile"]
-    )
+    io_args = ParserCommon.inputOutputOptions(opts=["bamfile", "whitelist", "outFile"], requiredOpts=["bamfile"])
     bam_args = ParserCommon.bamOptions(
         suppress_args=["labels", "smartLabels", "distanceBetweenBins", "region"],
         default_opts={"binSize": 100000},
     )
     other_args = ParserCommon.otherOptions()
 
     parser = argparse.ArgumentParser(
@@ -74,17 +72,15 @@
         required=False,
     )
 
     general.add_argument(
         "--minMappingQuality",
         "-mq",
         metavar="INT",
-        help="If set, only reads that have a mapping "
-        "quality score of at least this are "
-        "considered.",
+        help="If set, only reads that have a mapping " "quality score of at least this are " "considered.",
         type=int,
     )
 
     general.add_argument(
         "--rankPlot",
         "-rp",
         type=parserCommon.writableFile,
@@ -166,17 +162,15 @@
 
     # open barcode file and read the content in a list
     if args.whitelist:
         with open(args.whitelist, "r") as f:
             barcodes = f.read().splitlines()
         args.whitelist = barcodes
 
-    bhs = bamHandler.openBam(
-        args.bamfile, returnStats=True, nThreads=args.numberOfProcessors
-    )[0]
+    bhs = bamHandler.openBam(args.bamfile, returnStats=True, nThreads=args.numberOfProcessors)[0]
     chrom_sizes = list(zip(bhs.references, bhs.lengths))
     bhs.close()
 
     # Get the remaining metrics
     res = mapReduce(
         [args],
         getFiltered_worker,
@@ -214,17 +208,15 @@
             marker="o",
             color="grey",
             markersize=6,
         )
         ax.set_xlabel("Barcode Rank", fontsize=15)
         ax.set_ylabel("No. of nonzero bins (log10)", fontsize=15)
         ax.set_title("Ranked counts (#bins) for detected Barcodes", fontsize=15)
-        plt.xticks(
-            np.arange(0, max(df["count"]), int(max(df["count_rank"]) / 10)), fontsize=10
-        )
+        plt.xticks(np.arange(0, max(df["count"]), int(max(df["count_rank"]) / 10)), fontsize=10)
         plt.yticks(np.arange(0, 4, 0.1), fontsize=10)
 
         # Annotation
         if args.minCount:
             plt.axhline(args.minCount, color="r")
 
         fig.tight_layout()
@@ -242,9 +234,9 @@
     if args.outFile is None:
         of = sys.stdout
     else:
         of = open(args.outFile, "w")
 
     for x in final_set:
         of.write(str(x) + "\n")
-    df.to_csv("~/programs/sincei/test_df.csv")
+    # df.to_csv("~/programs/sincei/test_df.csv")
     return 0
```

### Comparing `sincei-0.2/sincei/scFilterStats.py` & `sincei-0.3/sincei/scFilterStats.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 from sincei.Utilities import *
 from sincei import ParserCommon
 
 
 def parseArguments():
     filterParser = ParserCommon.filterOptions()
 
-    io_args = ParserCommon.inputOutputOptions(
-        opts=["bamfiles", "barcodes", "outFile"], requiredOpts=["barcodes"]
-    )
+    io_args = ParserCommon.inputOutputOptions(opts=["bamfiles", "barcodes", "outFile"], requiredOpts=["barcodes"])
     bam_args = ParserCommon.bamOptions(
         suppress_args=["region"],
         default_opts={"binSize": 100000, "distanceBetweenBins": 1000000},
     )
     filter_args = ParserCommon.filterOptions()
     read_args = ParserCommon.readOptions(
         suppress_args=[
@@ -144,18 +142,15 @@
             if read.flag & 4:
                 # Ignore unmapped reads, they were counted already
                 continue
 
             if args.minMappingQuality and read.mapq < args.minMappingQuality:
                 filtered[bc] = 1
                 minMapq[bc] += 1
-            if (
-                args.samFlagInclude
-                and read.flag & args.samFlagInclude != args.samFlagInclude
-            ):
+            if args.samFlagInclude and read.flag & args.samFlagInclude != args.samFlagInclude:
                 filtered[bc] = 1
                 samFlagInclude[bc] += 1
             if args.samFlagExclude and read.flag & args.samFlagExclude != 0:
                 filtered[bc] = 1
                 samFlagExclude[bc] += 1
 
             if args.minAlignedFraction:
@@ -171,19 +166,15 @@
             ):
                 filtered[bc] = 1
                 blacklisted[bc] += 1
 
             ## Duplicates
             if args.duplicateFilter:
                 tup = getDupFilterTuple(read, bc, args.duplicateFilter)
-                if (
-                    lpos is not None
-                    and lpos == read.reference_start
-                    and tup in prev_pos
-                ):
+                if lpos is not None and lpos == read.reference_start and tup in prev_pos:
                     filtered[bc] = 1
                     internalDupes[bc] += 1
                 if lpos != read.reference_start:
                     prev_pos.clear()
                 lpos = read.reference_start
                 prev_pos.add(tup)
             if read.is_duplicate:
@@ -191,26 +182,21 @@
                 externalDupes[bc] += 1
             if read.is_paired and read.mate_is_unmapped:
                 filtered[bc] = 1
                 singletons[bc] += 1
 
             ## remove reads with low/high GC content
             if args.GCcontentFilter:
-                if not checkGCcontent(
-                    read, args.GCcontentFilter[0], args.GCcontentFilter[1]
-                ):
+                if not checkGCcontent(read, args.GCcontentFilter[0], args.GCcontentFilter[1]):
                     filtered[bc] = 1
                     filterGC[bc] += 1
 
             ## remove reads that don't pass the motif filter
             if args.motifFilter:
-                test = [
-                    checkMotifs(read, chrom, twoBitGenome, m[0], m[1])
-                    for m in args.motifFilter
-                ]
+                test = [checkMotifs(read, chrom, twoBitGenome, m[0], m[1]) for m in args.motifFilter]
                 # if none given motif found, return true
                 if not any(test):
                     filtered[bc] = 1
                     filterMotifs[bc] += 1
 
             # filterRNAstrand
             if args.filterRNAstrand:
@@ -279,17 +265,15 @@
 
     if args.outFile is None:
         of = sys.stdout
     else:
         of = open(args.outFile, "w")
 
     for bam in args.bamfiles:
-        x = bamHandler.openBam(bam, returnStats=True, nThreads=args.numberOfProcessors)[
-            0
-        ]
+        x = bamHandler.openBam(bam, returnStats=True, nThreads=args.numberOfProcessors)[0]
         chrom_sizes = list(zip(x.references, x.lengths))
 
         checkBAMtag(x, bam, args.cellTag)
         if args.groupTag:
             checkBAMtag(x, bam, args.groupTag)
             sys.stderr.write("--groupTag is not implemented for scFilterStats yet! \n")
             exit(1)
@@ -322,21 +306,17 @@
         "Singletons",
         "Wrong_strand",
         "Wrong_motif",
         "Unwanted_GC_content",
         "Low_aligned_fraction",
     ]
 
-    final_df = pd.DataFrame(
-        data=np.concatenate(final_array), index=rowLabels, columns=colLabels
-    )
+    final_df = pd.DataFrame(data=np.concatenate(final_array), index=rowLabels, columns=colLabels)
     ## since stats are approximate, present results as %
-    final_df.iloc[:, 1:] = (
-        final_df.iloc[:, 1:].div(final_df.Total_sampled, axis=0) * 100
-    )
+    final_df.iloc[:, 1:] = final_df.iloc[:, 1:].div(final_df.Total_sampled, axis=0) * 100
 
     if args.outFile is not None:
         final_df.to_csv(args.outFile, sep="\t")
     else:
         print(final_df)
 
     return 0
```

### Comparing `sincei-0.2/sincei/scJSD.py` & `sincei-0.3/sincei/scJSD.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,16 @@
 
 
 def parseArguments(args=None):
     io_args = ParserCommon.inputOutputOptions(
         opts=["bamfiles", "barcodes", "outFile"],
         requiredOpts=["bamfiles", "barcodes", "outFile"],
     )
-    bam_args = ParserCommon.bamOptions(
-        suppress_args=["region", "distanceBetweenBins"], default_opts={"binSize": 10000}
-    )
-    read_args = ParserCommon.readOptions(
-        suppress_args=["filterRNAstrand", "extendReads", "centerReads"]
-    )
+    bam_args = ParserCommon.bamOptions(suppress_args=["region", "distanceBetweenBins"], default_opts={"binSize": 10000})
+    read_args = ParserCommon.readOptions(suppress_args=["filterRNAstrand", "extendReads", "centerReads"])
     filter_args = ParserCommon.filterOptions(
         suppress_args=[
             "motifFilter",
             "genome2bit",
             "GCcontentFilter",
             "minAlignedFraction",
         ]
@@ -85,16 +81,15 @@
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="This tool samples regions in the genome from BAM files "
         "and compares the cumulative read coverages for each cell on those regions. "
         "to a synthetic cell with poisson distributed reads using Jansson Shannon Distance. "
         "Cells with high enrichment of signals show a higher JSD compared to cells whose signal "
         "is homogenously distrubuted.",
         conflict_handler="resolve",
-        usage="An example usage is: plotFingerprint -b treatment.bam control.bam "
-        "-plot fingerprint.png",
+        usage="An example usage is: plotFingerprint -b treatment.bam control.bam " "-plot fingerprint.png",
         add_help=False,
     )
 
     return parser
 
 
 def main(args=None):
```

