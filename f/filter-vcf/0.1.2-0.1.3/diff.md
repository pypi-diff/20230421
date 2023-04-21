# Comparing `tmp/filter-vcf-0.1.2.tar.gz` & `tmp/filter-vcf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter-vcf-0.1.2.tar", last modified: Tue Apr 11 12:39:57 2023, max compression
+gzip compressed data, was "filter-vcf-0.1.3.tar", last modified: Fri Apr 21 13:27:29 2023, max compression
```

## Comparing `filter-vcf-0.1.2.tar` & `filter-vcf-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0       13 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/PYPI.md
--rw-r--r--   0        0        0        0 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/process.py
--rw-r--r--   0        0        0        0 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/util/__init__.py
--rw-r--r--   0        0        0     1791 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/util/addDepth.py
--rw-r--r--   0        0        0     2015 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/util/cleanAD.py
--rw-r--r--   0        0        0     4179 2023-04-11 12:37:21.778314 filter-vcf-0.1.2/filter_vcf/util/cleanGT.py
--rw-r--r--   0        0        0     1753 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/convertChrName.py
--rw-r--r--   0        0        0      631 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/detectVcf.py
--rw-r--r--   0        0        0     1744 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/passFilter.py
--rw-r--r--   0        0        0      814 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/readVcf.py
--rw-r--r--   0        0        0      720 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/removeNonRef.py
--rw-r--r--   0        0        0      685 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/sortVcf.py
--rw-r--r--   0        0        0      781 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/filter_vcf/util/unique.py
--rw-r--r--   0        0        0      899 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3490 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/tests/decomp.vcf
--rw-r--r--   0        0        0   270284 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/tests/full.vcf
--rw-r--r--   0        0        0     1682 2023-04-11 12:37:21.782315 filter-vcf-0.1.2/tests/presorted.vcf
--rw-r--r--   0        0        0    62601 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/sample.nrm.vcf.gz
--rw-r--r--   0        0        0    38219 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/test_process.py
--rw-r--r--   0        0        0     1682 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/unsorted.vcf
--rw-r--r--   0        0        0      514 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/unsorted.vcf.gz
--rw-r--r--   0        0        0       40 2023-04-11 12:37:21.786315 filter-vcf-0.1.2/tests/vcf.txt
--rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 filter-vcf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/PYPI.md
+-rw-r--r--   0        0        0        0 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/__init__.py
+-rw-r--r--   0        0        0     1905 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/config.py
+-rw-r--r--   0        0        0      675 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/filter_vcf.py
+-rw-r--r--   0        0        0     6841 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/process.py
+-rw-r--r--   0        0        0        0 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/__init__.py
+-rw-r--r--   0        0        0     1791 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/addDepth.py
+-rw-r--r--   0        0        0     2435 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/cleanAD.py
+-rw-r--r--   0        0        0     4257 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/cleanGT.py
+-rw-r--r--   0        0        0     1753 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/convertChrName.py
+-rw-r--r--   0        0        0      631 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/detectVcf.py
+-rw-r--r--   0        0        0      814 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/readVcf.py
+-rw-r--r--   0        0        0      720 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/removeNonRef.py
+-rw-r--r--   0        0        0      779 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/sortVcf.py
+-rw-r--r--   0        0        0      781 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/unique.py
+-rw-r--r--   0        0        0     1485 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/userFilter.py
+-rw-r--r--   0        0        0      295 2023-04-21 13:25:13.939307 filter-vcf-0.1.3/filter_vcf/util/writeVcf.py
+-rw-r--r--   0        0        0      899 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3490 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/tests/decomp.vcf
+-rw-r--r--   0        0        0   270284 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/tests/full.vcf
+-rw-r--r--   0        0        0     1682 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/tests/presorted.vcf
+-rw-r--r--   0        0        0    62601 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/tests/sample.nrm.vcf.gz
+-rw-r--r--   0        0        0    38476 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/tests/test_process.py
+-rw-r--r--   0        0        0     1682 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/tests/unsorted.vcf
+-rw-r--r--   0        0        0      514 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/tests/unsorted.vcf.gz
+-rw-r--r--   0        0        0       40 2023-04-21 13:25:13.943307 filter-vcf-0.1.3/tests/vcf.txt
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 filter-vcf-0.1.3/PKG-INFO
```

### Comparing `filter-vcf-0.1.2/filter_vcf/util/addDepth.py` & `filter-vcf-0.1.3/filter_vcf/util/addDepth.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/filter_vcf/util/cleanAD.py` & `filter-vcf-0.1.3/filter_vcf/util/cleanAD.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,29 +19,37 @@
                     labels = working_line[8].split(":")
                     values = working_line[9].split(":")
                     variant_dict = dict(zip(labels, values))
 
                     gt_value = variant_dict.get("GT")
                     ad_values = variant_dict.get("AD").split(",")
 
-                    # First variant will correspond with first and second AD values
-                    if gt_value == "1/.":
+                    if len(ad_values) == 2:
                         new_ad_values = [ad_values[0], ad_values[1]]
                         variant_dict.update({"AD": ",".join(new_ad_values)})
 
                         working_line[9] = ":".join(list(variant_dict.values()))
                         vcf_with_corrected_ad.append("\t".join(working_line))
 
-                    # Second variant will correspond with first and third AD values
-                    elif gt_value == "./1":
-                        new_ad_values = [ad_values[0], ad_values[2]]
-                        variant_dict.update({"AD": ",".join(new_ad_values)})
+                    # First variant will correspond with first and second AD values
+                    else:
+                        if gt_value == "1/.":
+                            new_ad_values = [ad_values[0], ad_values[1]]
+                            variant_dict.update({"AD": ",".join(new_ad_values)})
+
+                            working_line[9] = ":".join(list(variant_dict.values()))
+                            vcf_with_corrected_ad.append("\t".join(working_line))
+
+                        # Second variant will correspond with first and third AD values
+                        elif gt_value == "./1":
+                            new_ad_values = [ad_values[0], ad_values[2]]
+                            variant_dict.update({"AD": ",".join(new_ad_values)})
 
-                        working_line[9] = ":".join(list(variant_dict.values()))
-                        vcf_with_corrected_ad.append("\t".join(working_line))
+                            working_line[9] = ":".join(list(variant_dict.values()))
+                            vcf_with_corrected_ad.append("\t".join(working_line))
 
                 else:
                     vcf_with_corrected_ad.append(line)
 
     # Concat to single string, and add newline to end
     vcf_with_corrected_ad = "\n".join(vcf_with_corrected_ad)
     vcf_with_corrected_ad = vcf_with_corrected_ad + "\n"
```

### Comparing `filter-vcf-0.1.2/filter_vcf/util/cleanGT.py` & `filter-vcf-0.1.3/filter_vcf/util/cleanGT.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 
                         working_line[9] = ":".join(list(variant_dict.values()))
                         vcf_with_corrected_gt.append("\t".join(working_line))
 
                     else:
                         vcf_with_corrected_gt.append(line)
 
+                else:
+                    vcf_with_corrected_gt.append(line)
+
     # Concat to single string, and add newline to end
     vcf_with_corrected_gt = "\n".join(vcf_with_corrected_gt)
     vcf_with_corrected_gt = vcf_with_corrected_gt + "\n"
 
     return vcf_with_corrected_gt
```

### Comparing `filter-vcf-0.1.2/filter_vcf/util/convertChrName.py` & `filter-vcf-0.1.3/filter_vcf/util/convertChrName.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/filter_vcf/util/detectVcf.py` & `filter-vcf-0.1.3/filter_vcf/util/detectVcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/filter_vcf/util/readVcf.py` & `filter-vcf-0.1.3/filter_vcf/util/readVcf.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/filter_vcf/util/removeNonRef.py` & `filter-vcf-0.1.3/filter_vcf/util/removeNonRef.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/filter_vcf/util/sortVcf.py` & `filter-vcf-0.1.3/filter_vcf/util/sortVcf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from logging import Logger
 from natsort import index_natsorted
 from fuc import pyvcf
 
 
 def sort_vcf(vcf_frame: pyvcf.VcfFrame, log: Logger) -> str:
     # Perform natural sort on CHROM, POS, REF, and ALT columns
+    if isinstance(vcf_frame, str):
+        vcf_frame = pyvcf.VcfFrame.from_string(vcf_frame)
+
     vcf_frame.df.sort_values(
         by=["CHROM", "POS", "REF", "ALT"],
         key=lambda x: np.argsort(
             index_natsorted(
                 zip(
                     vcf_frame.df["CHROM"],
                     vcf_frame.df["POS"],
```

### Comparing `filter-vcf-0.1.2/filter_vcf/util/unique.py` & `filter-vcf-0.1.3/filter_vcf/util/unique.py`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/pyproject.toml` & `filter-vcf-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "filter-vcf"
-version = "0.1.2"
+version = "0.1.3"
 description = "LifeOmic VCF filtering"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging==0.3.2",
     "vcfpy>=0.13.4",
```

### Comparing `filter-vcf-0.1.2/tests/decomp.vcf` & `filter-vcf-0.1.3/tests/decomp.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/tests/full.vcf` & `filter-vcf-0.1.3/tests/full.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/tests/presorted.vcf` & `filter-vcf-0.1.3/tests/presorted.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/tests/sample.nrm.vcf.gz` & `filter-vcf-0.1.3/tests/sample.nrm.vcf.gz`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/tests/test_process.py` & `filter-vcf-0.1.3/tests/test_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,76 @@
 import os
-import numpy as np
 import logging
 from fuc import pyvcf
 import unittest
 
 
-from filter_vcf.process import process_vcf
+from filter_vcf.filter_vcf import filter_vcf
+from filter_vcf.util.userFilter import perform_filter_vcf
 from filter_vcf.util.sortVcf import sort_vcf
 from filter_vcf.util.readVcf import read_vcf
+from filter_vcf.util.writeVcf import write_vcf
 from filter_vcf.util.addDepth import add_depth
 from filter_vcf.util.cleanAD import clean_ad
 from filter_vcf.util.cleanGT import remove_gt_dot, fix_gt_extra, clean_gt
 from filter_vcf.util.removeNonRef import filter_non_ref
 from filter_vcf.util.detectVcf import detect_vcf
 from filter_vcf.util.convertChrName import convert_chr_name
 from filter_vcf.util.unique import keep_unique_variants
-from filter_vcf.util.passFilter import pass_filter, pass_only
 
 
 class MockLog:
     def info(self, _: str):
         return None
 
     def error(self, _: str):
         return None
 
 
 mock_log = MockLog()
 
 
-def test_process():
+def test_filter_vcf():
 
     vcf_file = f"{os.path.dirname(os.path.abspath(__file__))}/sample.nrm.vcf.gz"
 
-    result = process_vcf(vcf_file, "PASS:sb")
+    result = filter_vcf(vcf_file, "PASS:sb", mock_log)
 
     os.remove(vcf_file.replace("nrm.vcf.gz", "nrm.filtered.vcf.gz"))
 
     assert result is not None
 
 
+def test_perform_filter_vcf():
+
+    vcf_for_filtering = str(
+        """##fileformat=VCFv4.0
+##fileDate=20180419
+#CHROM	POS	ID	REF	ALT	QUAL	FILTER	
+1	35885022	rs1474253187	T	C	.	PASS	
+2	44622946	rs9291422989	C	G	.	sb	
+9	30912459	rs1330713521	A	G	.	lowQ	
+11	42641414	rs1006891614	C	T	.	PASS;sb	
+12	65138464	rs1531215484	A	T	.	lowQ;sb	
+"""
+    )
+
+    filtered_vcf = perform_filter_vcf(vcf_for_filtering, "PASS:sb", mock_log)
+
+    assert filtered_vcf == str(
+        """##fileformat=VCFv4.0
+##fileDate=20180419
+#CHROM	POS	ID	REF	ALT	QUAL	FILTER	
+1	35885022	rs1474253187	T	C	.	PASS	
+2	44622946	rs9291422989	C	G	.	sb	
+11	42641414	rs1006891614	C	T	.	PASS;sb	
+"""
+    )
+
+
 def test_read_vcf():
     unsorted_vcf = read_vcf(f"{os.path.dirname(os.path.abspath(__file__))}/unsorted.vcf", mock_log)
     unsorted_vcf_gzip = read_vcf(
         f"{os.path.dirname(os.path.abspath(__file__))}/unsorted.vcf.gz", mock_log
     )
 
     assert unsorted_vcf.to_string() == unsorted_vcf_gzip.to_string()
@@ -71,14 +98,44 @@
                 cm.output,
                 [
                     f'ERROR:root:Given file "{wrong_format_file}" must be in vcf or vcf.gz format',
                 ],
             )
 
 
+def test_write_vcf():
+    os.makedirs(f"{os.path.dirname(os.path.abspath(__file__))}/tmp/", exist_ok=True)
+
+    def cleanup():
+        os.system(f"rm {os.path.dirname(os.path.abspath(__file__))}/tmp/written.vcf.gz")
+
+    working_vcf = str(
+        """##fileformat=VCFv4.0
+##fileDate=20180419
+#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
+1	35885022	rs1474253187	T	C	.	.	RS=1474253187;RSPOS=35885022;dbSNPBuildID=151;SSR=0;SAO=0;VP=0x050000020005000002000100;GENEINFO=KCNE1:3753
+2	44622946	rs929142298	C	G	.	.	RS=929142298;RSPOS=44622946;dbSNPBuildID=150;SSR=0;SAO=0;VP=0x050000000005000002000100
+9	30912459	rs1330713521	A	G	.	.	RS=1330713521;RSPOS=30912459;dbSNPBuildID=151;SSR=0;SAO=0;VP=0x050000080005000002000100;GENEINFO=GRIK1:2897
+11	42641414	rs1006891614	C	T	.	.	RS=1006891614;RSPOS=42641414;dbSNPBuildID=150;SSR=0;SAO=0;VP=0x050000000005000002000100
+"""
+    )
+
+    write_vcf(
+        working_vcf,
+        f"{os.path.dirname(os.path.abspath(__file__))}/tmp/written.vcf.gz",
+        compression=True,
+        log=mock_log,
+    )
+
+    assert (
+        os.path.exists(f"{os.path.dirname(os.path.abspath(__file__))}/tmp/written.vcf.gz") == True
+    )
+    cleanup()
+
+
 def test_sort_vcf():
     presorted_vcf = str(
         """##fileformat=VCFv4.0
 ##fileDate=20180419
 #CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
 1	35885022	rs1474253187	T	C	.	.	RS=1474253187;RSPOS=35885022;dbSNPBuildID=151;SSR=0;SAO=0;VP=0x050000020005000002000100;GENEINFO=KCNE1:3753
 1	35910077	rs1293956811	A	G	.	.	RS=1293956811;RSPOS=35910077;dbSNPBuildID=151;SSR=0;SAO=0;VP=0x050000080005000002000100;GENEINFO=RCAN1:1827
@@ -118,34 +175,30 @@
 chr1	2556714	rs4870	A	G	0.0	Benign	DP=681;TI=NM_003820.3;GI=TNFRSF14;FC=Missense;PC=K17R;DC=c.50A>G;LO=EXON;EXON=1;CI=Benign	GT:VF:AD:SB:SA:SP:SO	1/1:1.000:0,681:327/354:0/0,327/354:0
 chr1	2562891	rs2234167	G	A	0.0	Benign	DP=958;TI=NM_003820.3;GI=TNFRSF14;FC=Missense;PC=V241I;DC=c.721G>A;LO=EXON;EXON=7;CI=Benign	GT:VF:AD:SB:SA:SP:SO	0/1:0.453:524,434:417/541:234/290,183/251:4
 chr1	7677739	rs3011926	A	G	0.0	rs	DP=1359;TI=NM_015215.3;GI=CAMTA1;FC=Silent;DC=c.2914+6A>G;LO=INTRON;EXON=11	GT:VF:AD:SB:SA:SP:SO	1/1:1.000:0,1359:555/804:0/0,555/804:0
 """
     )
 
     with_dp_vcf = add_depth(no_dp_vcf, mock_log)
-    assert with_dp_vcf == (
-        (
-            str(
-                """##fileformat=VCFv4.0
+    assert with_dp_vcf == str(
+        """##fileformat=VCFv4.0
 ##fileDate=20180419
 ##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">
 ##FORMAT=<ID=VF,Number=1,Type=Float,Description="Variant Frequency">
 ##FORMAT=<ID=AD,Number=.,Type=Integer,Description="Allele Depth">
 ##FORMAT=<ID=SB,Number=1,Type=String,Description="Strand Bias with read numbers (Fw/Rv)">
 ##FORMAT=<ID=SA,Number=2,Type=String,Description="Number of 1) forward ref alleles; 2) reverse ref; 3) forward non-ref; 4) reverse non-ref alleles, used in variant calling">
 ##FORMAT=<ID=SP,Number=1,Type=Float,Description="Phred of Chi-square p-value for strand bias">
 ##FORMAT=<ID=SO,Number=1,Type=String,Description="abs(log10( (RefFw*AltRv)/(RefRv*AltFw) )) for strand bias">
 ##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read Depth">
 #CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT  CASE-ID
 chr1	2556714	rs4870	A	G	0.0	Benign	DP=681;TI=NM_003820.3;GI=TNFRSF14;FC=Missense;PC=K17R;DC=c.50A>G;LO=EXON;EXON=1;CI=Benign	GT:VF:AD:SB:SA:SP:SO:DP	1/1:1.000:0,681:327/354:0/0,327/354:0:681
 chr1	2562891	rs2234167	G	A	0.0	Benign	DP=958;TI=NM_003820.3;GI=TNFRSF14;FC=Missense;PC=V241I;DC=c.721G>A;LO=EXON;EXON=7;CI=Benign	GT:VF:AD:SB:SA:SP:SO:DP	0/1:0.453:524,434:417/541:234/290,183/251:4:958
 chr1	7677739	rs3011926	A	G	0.0	rs	DP=1359;TI=NM_015215.3;GI=CAMTA1;FC=Silent;DC=c.2914+6A>G;LO=INTRON;EXON=11	GT:VF:AD:SB:SA:SP:SO:DP	1/1:1.000:0,1359:555/804:0/0,555/804:0:1359
 """
-            )
-        )
     )
 
     prexisting_dp_vcf = str(
         """##fileformat=VCFv4.0
 ##fileDate=20180419
 ##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">
 ##FORMAT=<ID=VF,Number=1,Type=Float,Description="Variant Frequency">
@@ -158,34 +211,30 @@
 #CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT  CASE-ID
 chr1	2556714	rs4870	A	G	0.0	Benign	DP=681;TI=NM_003820.3;GI=TNFRSF14;FC=Missense;PC=K17R;DC=c.50A>G;LO=EXON;EXON=1;CI=Benign	GT:VF:AD:SB:SA:SP:SO:AD:DP	1/1:1.000:0,681:327/354:0/0,327/354:0:INF:681
 chr1	2562891	rs2234167	G	A	0.0	Benign	DP=958;TI=NM_003820.3;GI=TNFRSF14;FC=Missense;PC=V241I;DC=c.721G>A;LO=EXON;EXON=7;CI=Benign	GT:VF:AD:SB:SA:SP:SO:AD:DP	0/1:0.453:524,434:417/541:234/290,183/251:4:0.0:958
 chr1	7677739	rs3011926	A	G	0.0	rs	DP=1359;TI=NM_015215.3;GI=CAMTA1;FC=Silent;DC=c.2914+6A>G;LO=INTRON;EXON=11	GT:VF:AD:SB:SA:SP:SO:AD:DP	1/1:1.000:0,1359:555/804:0/0,555/804:0:INF:1359
 """
     )
 
-    assert add_depth(prexisting_dp_vcf, mock_log) == (
-        (
-            str(
-                """##fileformat=VCFv4.0
+    assert add_depth(prexisting_dp_vcf, mock_log) == str(
+        """##fileformat=VCFv4.0
 ##fileDate=20180419
 ##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">
 ##FORMAT=<ID=VF,Number=1,Type=Float,Description="Variant Frequency">
 ##FORMAT=<ID=AD,Number=.,Type=Integer,Description="Allele Depth">
 ##FORMAT=<ID=SB,Number=1,Type=String,Description="Strand Bias with read numbers (Fw/Rv)">
 ##FORMAT=<ID=SA,Number=2,Type=String,Description="Number of 1) forward ref alleles; 2) reverse ref; 3) forward non-ref; 4) reverse non-ref alleles, used in variant calling">
 ##FORMAT=<ID=SP,Number=1,Type=Float,Description="Phred of Chi-square p-value for strand bias">
 ##FORMAT=<ID=SO,Number=1,Type=String,Description="abs(log10( (RefFw*AltRv)/(RefRv*AltFw) )) for strand bias">
 ##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read Depth">
 #CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT  CASE-ID
 chr1	2556714	rs4870	A	G	0.0	Benign	DP=681;TI=NM_003820.3;GI=TNFRSF14;FC=Missense;PC=K17R;DC=c.50A>G;LO=EXON;EXON=1;CI=Benign	GT:VF:AD:SB:SA:SP:SO:AD:DP	1/1:1.000:0,681:327/354:0/0,327/354:0:INF:681
 chr1	2562891	rs2234167	G	A	0.0	Benign	DP=958;TI=NM_003820.3;GI=TNFRSF14;FC=Missense;PC=V241I;DC=c.721G>A;LO=EXON;EXON=7;CI=Benign	GT:VF:AD:SB:SA:SP:SO:AD:DP	0/1:0.453:524,434:417/541:234/290,183/251:4:0.0:958
 chr1	7677739	rs3011926	A	G	0.0	rs	DP=1359;TI=NM_015215.3;GI=CAMTA1;FC=Silent;DC=c.2914+6A>G;LO=INTRON;EXON=11	GT:VF:AD:SB:SA:SP:SO:AD:DP	1/1:1.000:0,1359:555/804:0/0,555/804:0:INF:1359
 """
-            )
-        )
     )
 
 
 def test_remove_gt_dot():
     vcf_with_gt_dots = str(
         """##fileformat=VCFv4.0
 ##fileDate=20180419
@@ -211,14 +260,15 @@
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	./0/1/.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	./0/0/.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	0/0/0/.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	0/0/1/.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	.|0|.|.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	.|.|0|.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	.|.|.|0:146:0,10,62,84
+chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	0/1:146:0,10,62,84
 """
     )
     vcf_with_corrected_gt = remove_gt_dot(vcf_with_gt_dots, mock_log)
     assert vcf_with_corrected_gt == str(
         """##fileformat=VCFv4.0
 ##fileDate=20180419
 ##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">
@@ -243,14 +293,15 @@
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	0/1:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	0/0:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	0/0/0/.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	0/0/1/.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	.|0|.|.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	.|.|0|.:146:0,10,62,84
 chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	.|.|.|0:146:0,10,62,84
+chrX	154766321	rs2728532	G	T	0	rs	DP=908	GT:AD:DP	0/1:146:0,10,62,84
 """
     )
 
 
 def test_fix_gt_extra():
     vcf_with_gt_extra = str(
         """##fileformat=VCFv4.0
@@ -585,57 +636,7 @@
 #CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
 1	35910077	rs1293956811	A	G	.	.	RS=1293956811;RSPOS=35910077;dbSNPBuildID=151;SSR=0;SAO=0;VP=0x050000080005000002000100;GENEINFO=RCAN1:1827
 2	44578967	rs562685327	G	A	.	.	RS=562685327;RSPOS=44578967;dbSNPBuildID=142;SSR=0;SAO=0;VP=0x050000000005000026000100
 7	46901014	rs1299817526	CCTCCGACCTCTCTGGCCCTGTGGGT	C	.	.	RS=1299817526;RSPOS=46901015;dbSNPBuildID=151;SSR=0;SAO=0;VP=0x050000080005000002000200;GENEINFO=COL18A1:80781
 9	46901014	rs1299817526	CCTCCGACCTCTCTGGCCCTGTGGGT	C	.	.	RS=1299817526;RSPOS=46901015;dbSNPBuildID=151;SSR=0;SAO=0;VP=0x050000080005000002000200;GENEINFO=COL18A1:80781
 """
     )
-
-
-def test_pass_filter():
-    vcf_for_pass_filter = str(
-        """##fileformat=VCFv4.0
-##fileDate=20180419
-#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
-chr1	27892262	.	GA	G	0.0	R8.1;lowQ	DP=891	GT:VF:AD	0/1:0.012:878,11
-chr1	35192998	.	T	A	0.0	lowQ	DP=260	GT:VF:AD	0/1:0.012:256,3
-chr1	36286551	.	C	T	0.0	.	DP=2603	GT:VF:AD	0/1:0.493:1320,1283
-chr1	36286832	.	C	T	0.0	Pass	DP=1848	GT:VF:AD	1/1:1.000:0,1848
-"""
-    )
-
-    vcf_all_pass = pass_filter(vcf_for_pass_filter, log=mock_log)
-
-    assert vcf_all_pass == str(
-        """##fileformat=VCFv4.0
-##fileDate=20180419
-#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
-chr1	27892262	.	GA	G	0.0	R8.1;lowQ;Pass	DP=891	GT:VF:AD	0/1:0.012:878,11
-chr1	35192998	.	T	A	0.0	lowQ;Pass	DP=260	GT:VF:AD	0/1:0.012:256,3
-chr1	36286551	.	C	T	0.0	Pass	DP=2603	GT:VF:AD	0/1:0.493:1320,1283
-chr1	36286832	.	C	T	0.0	Pass	DP=1848	GT:VF:AD	1/1:1.000:0,1848
-"""
-    )
-
-
-def test_pass_only():
-    vcf_for_pass_only = str(
-        """##fileformat=VCFv4.0
-##fileDate=20180419
-#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
-chr1	27892262	.	GA	G	0.0	R8.1;lowQ;Pass	DP=891	GT:VF:AD	0/1:0.012:878,11
-chr1	35192998	.	T	A	0.0	lowQ	DP=260	GT:VF:AD	0/1:0.012:256,3
-chr1	36286551	.	C	T	0.0	Pass	DP=2603	GT:VF:AD	0/1:0.493:1320,1283
-chr1	36286832	.	C	T	0.0	.	DP=1848	GT:VF:AD	1/1:1.000:0,1848
-"""
-    )
-
-    vcf_only_pass = pass_only(vcf_for_pass_only, log=mock_log)
-
-    assert vcf_only_pass == str(
-        """##fileformat=VCFv4.0
-##fileDate=20180419
-#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
-chr1	27892262	.	GA	G	0.0	R8.1;lowQ;Pass	DP=891	GT:VF:AD	0/1:0.012:878,11
-chr1	36286551	.	C	T	0.0	Pass	DP=2603	GT:VF:AD	0/1:0.493:1320,1283
-"""
-    )
```

### Comparing `filter-vcf-0.1.2/tests/unsorted.vcf` & `filter-vcf-0.1.3/tests/unsorted.vcf`

 * *Files identical despite different names*

### Comparing `filter-vcf-0.1.2/tests/unsorted.vcf.gz` & `filter-vcf-0.1.3/tests/unsorted.vcf.gz`

 * *Files identical despite different names*

