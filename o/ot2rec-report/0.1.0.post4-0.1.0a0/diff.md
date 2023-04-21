# Comparing `tmp/ot2rec_report-0.1.0.post4.tar.gz` & `tmp/ot2rec_report-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ot2rec_report-0.1.0.post4.tar", last modified: Fri Apr 21 17:02:38 2023, max compression
+gzip compressed data, was "ot2rec_report-0.1.0a0.tar", last modified: Wed Mar 29 18:10:42 2023, max compression
```

## Comparing `ot2rec_report-0.1.0.post4.tar` & `ot2rec_report-0.1.0a0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:02:38.623910 ot2rec_report-0.1.0.post4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-21 17:02:38.623910 ot2rec_report-0.1.0.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 17:02:38.623910 ot2rec_report-0.1.0.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:02:38.619910 ot2rec_report-0.1.0.post4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:02:38.619910 ot2rec_report-0.1.0.post4/src/ot2rec_report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:02:38.623910 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_aretomo_align.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_aretomo_header.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_aretomo_recon.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_ctffind.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_ctfsim.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_excludebadtilts.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_imod_align.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_imod_header.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_imod_recon.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_main.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_mc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_rlf_deconv.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_savu_recon.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_warp.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/workflow_diagram.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-21 17:02:27.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:02:38.619910 ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-21 17:02:38.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-21 17:02:38.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:02:38.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 17:02:38.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:02:38.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-21 17:02:38.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 17:02:38.000000 ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:10:42.418419 ot2rec_report-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-29 18:10:42.418419 ot2rec_report-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 18:10:42.418419 ot2rec_report-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:10:42.414419 ot2rec_report-0.1.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:10:42.414419 ot2rec_report-0.1.0a0/src/ot2rec_report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:10:42.418419 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_aretomo_align.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_aretomo_header.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_aretomo_recon.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_ctffind.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_ctfsim.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_excludebadtilts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_imod_align.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_imod_header.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_imod_recon.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_main.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_mc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_rlf_deconv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_savu_recon.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_warp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/templates/workflow_diagram.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-29 18:10:23.000000 ot2rec_report-0.1.0a0/src/ot2rec_report/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:10:42.414419 ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-29 18:10:42.000000 ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-29 18:10:42.000000 ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:10:42.000000 ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-29 18:10:42.000000 ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:10:42.000000 ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-29 18:10:42.000000 ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 18:10:42.000000 ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/top_level.txt
```

### Comparing `ot2rec_report-0.1.0.post4/LICENSE` & `ot2rec_report-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/PKG-INFO` & `ot2rec_report-0.1.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ot2rec_report
-Version: 0.1.0.post4
+Version: 0.1.0a0
 Summary: Generate reports for Ot2Rec
 Home-page: https://github.com/rosalindfranklininstitute/ot2rec_report.git
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ot2Rec Report
```

### Comparing `ot2rec_report-0.1.0.post4/README.md` & `ot2rec_report-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/setup.py` & `ot2rec_report-0.1.0a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from pathlib import Path
 
 # read contents of readme
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
 setup(
-    version="0.1.0post4",
+    version="0.1.0a",
     name="ot2rec_report",
     description="Generate reports for Ot2Rec",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rosalindfranklininstitute/ot2rec_report.git",
     include_package_data=True,
     packages=find_packages("src"),
```

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/main.py` & `ot2rec_report-0.1.0a0/src/ot2rec_report/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 def read_ipynb(filename):
     fn = pkg_resources.resource_filename("ot2rec_report.templates", filename)
 
     with open(fn, "r") as f:
         return json.load(f)
 
 
-def main(args=None):
+def main():
     lookup_dict = {
         "workflow_diagram": read_ipynb("workflow_diagram.ipynb"),
         "motioncor2": read_ipynb("report_mc.ipynb"),
         "warp": read_ipynb("report_warp.ipynb"),
         "ctffind": read_ipynb("report_ctffind.ipynb"),
         "ctfsim": read_ipynb("report_ctfsim.ipynb"),
         "exclude_bad_tilts": read_ipynb("report_excludebadtilts.ipynb"),
@@ -90,16 +90,15 @@
         "aretomo_header": read_ipynb("report_aretomo_header.ipynb"),
         "aretomo_align": read_ipynb("report_aretomo_align.ipynb"),
         "aretomo_recon": read_ipynb("report_aretomo_recon.ipynb"),
         "savu_recon": read_ipynb("report_savu_recon.ipynb"),
         "rlf_deconv": read_ipynb("report_rlf_deconv.ipynb"),
     }
 
-    if args is None:
-        args = get_args_o2r_report.show(run=True)
+    args = get_args_o2r_report.show(run=True)
 
     final_nb = dc(read_ipynb("report_main.ipynb"))
     node_list = [i.name for i in args.processes.value]
 
     # Check if AreTomo has been used
     at_list = list(i for i, s in enumerate(node_list) if "aretomo" in s)
     at_used = len(at_list) > 0
```

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_aretomo_align.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_aretomo_align.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_aretomo_header.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_aretomo_header.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_aretomo_recon.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_imod_recon.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9036368868400119%*

 * *Differences: {"'cells'": "{1: {'id': '5f17516c-b77c-4b95-a903-cc50fc4baf50', 'metadata': {replace: "*

 * *            "OrderedDict()}, 'source': ['### Tomographic Reconstruction (IMOD)\\n', "*

 * *            "'Reconstruction was performed with IMOD BatchRunTomo.']}, 2: {'id': "*

 * *            "'44d2077d-956d-47d2-9c0c-873c581e987b', 'metadata': {'slideshow': {'slide_type': "*

 * *            "'slide'}, delete: ['tags']}, 'source': {insert: [(0, 'from IPython.display import "*

 * *            'Markdown as md\\n\'), (2, \'printmd(f" Reconstruc […]*

```diff
@@ -1,98 +1,105 @@
 {
     "cells": [
         {
-            "cell_type": "markdown",
-            "id": "dc30f8f7-6f34-420d-8ef8-d11c56698a5c",
-            "metadata": {
-                "slideshow": {
-                    "slide_type": "slide"
-                }
-            },
-            "source": [
-                "### Tomographic Reconstruction (AreTomo)"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e7a30837",
+            "id": "f77a586f",
             "metadata": {
-                "slideshow": {
-                    "slide_type": "subslide"
-                },
                 "tags": [
                     "raises-exception",
                     "hide"
                 ]
             },
             "outputs": [],
             "source": [
-                "def get_aretomo_params():\n",
-                "    \"\"\"Print out relevant AreTomo setup parameters\"\"\"\n",
-                "    aretomo_yaml = f\"{os.getcwd()}/{proj_name}_aretomo_recon.yaml\"\n",
-                "    if os.path.isfile(aretomo_yaml) is False:\n",
-                "        aretomo_yaml = f\"{os.getcwd()}/{proj_name}_aretomo_align-recon.yaml\"\n",
-                "\n",
+                "def get_tomogram_filenames():\n",
+                "    # Get IMOD mdout\n",
                 "    try:\n",
-                "        with open(aretomo_yaml, \"r\") as f:\n",
-                "            aretomo_params = yaml.load(f.read(), Loader=yaml.FullLoader)\n",
-                "            printmd(f\"Vol Z = {aretomo_params['AreTomo_recon']['volz']}\")\n",
-                "            printmd(\n",
-                "                f\"Sample thickness = {aretomo_params['AreTomo_recon']['sample_thickness']}\"\n",
-                "            )\n",
-                "            printmd(f\"Pixel size = {aretomo_params['AreTomo_recon']['pixel_size']}\")\n",
-                "            printmd(\n",
-                "                f\"Reconstruction algorithm = {aretomo_params['AreTomo_recon']['recon_algo']}\"\n",
-                "            )\n",
-                "            printmd(f\"Bin factor = {aretomo_params['AreTomo_setup']['output_binning']}\")\n",
-                "            printmd(f\"Darktol = {aretomo_params['AreTomo_setup']['dark_tol']}\")\n",
+                "        imod_mdout = f\"{os.getcwd()}/{proj_name}_recon_mdout.yaml\"\n",
                 "    except FileNotFoundError:\n",
-                "        print(f\"{aretomo_yaml} not found, cannot retrieve AreTomo setup parameters\")\n",
+                "        print(\n",
+                "            f\"{proj_name}_recon_mdout.yaml not found, cannot find tomogram filenames.\"\n",
+                "        )\n",
+                "\n",
+                "    with open(imod_mdout, \"r\") as f:\n",
+                "        output = yaml.load(f.read(), Loader=yaml.FullLoader)\n",
+                "        tomogram_filenames = output[\"recon_output\"].values()\n",
+                "        algor = output[\"recon_algor\"] if \"recon_algor\" in output.keys() else \"WBP\"\n",
                 "\n",
+                "    return tomogram_filenames, algor\n",
+                "\n",
+                "\n",
+                "tomogram_filenames, algor = get_tomogram_filenames()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "5f17516c-b77c-4b95-a903-cc50fc4baf50",
+            "metadata": {},
+            "source": [
+                "### Tomographic Reconstruction (IMOD)\n",
+                "Reconstruction was performed with IMOD BatchRunTomo."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "44d2077d-956d-47d2-9c0c-873c581e987b",
+            "metadata": {
+                "slideshow": {
+                    "slide_type": "slide"
+                }
+            },
+            "outputs": [],
+            "source": [
+                "from IPython.display import Markdown as md\n",
                 "\n",
-                "get_aretomo_params()"
+                "printmd(f\" Reconstruction algorithm: {algor}\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "555e9de1-3ed2-4b18-a065-f465419b7148",
+            "metadata": {},
+            "source": [
+                "For more information, please see [https://bio3d.colorado.edu/imod/doc/directives.html](https://bio3d.colorado.edu/imod/doc/directives.html)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "aec1bde9",
+            "id": "6d1a9c1a",
             "metadata": {
                 "tags": [
                     "hide"
                 ]
             },
             "outputs": [],
             "source": [
-                "def get_aretomo_tomofilenames():\n",
-                "    \"\"\"Get list of tomograms from AreTomo\"\"\"\n",
-                "    aretomo_yaml = f\"{os.getcwd()}/{proj_name}_aretomo_recon.yaml\"\n",
-                "    if os.path.isfile(aretomo_yaml) is False:\n",
-                "        aretomo_yaml = f\"{os.getcwd()}/{proj_name}_aretomo_align-recon.yaml\"\n",
-                "\n",
-                "    try:\n",
-                "        with open(aretomo_yaml, \"r\") as f:\n",
-                "            aretomo_params = yaml.load(f.read(), Loader=yaml.FullLoader)\n",
-                "            tomogram_filenames = aretomo_params[\"AreTomo_setup\"][\"output_mrc\"]\n",
-                "            return tomogram_filenames\n",
-                "    except FileNotFoundError:\n",
-                "        print(f\"{aretomo_yaml} not found, cannot retrieve tomogram filenames\")\n",
-                "\n",
-                "\n",
                 "def get_central_slices(img_data):\n",
                 "    # Find central slices\n",
-                "    z_central = int(img_data.shape[0] / 2)\n",
-                "    y_central = int(img_data.shape[1] / 2)\n",
-                "    x_central = int(img_data.shape[2] / 2)\n",
+                "    z_central = img_data.shape[0] // 2\n",
+                "    x_central = img_data.shape[1] // 2\n",
+                "    y_central = img_data.shape[2] // 2\n",
+                "\n",
+                "    # Calculate number of slices to add\n",
+                "    zxy_add = (np.array(img_data.shape) * 0.0025).astype(int)\n",
+                "    zxy_add[zxy_add < 1] = 1\n",
                 "\n",
                 "    # xy, yz, xz image data\n",
-                "    xy_data = img_data[z_central, :, :]\n",
-                "    yz_data = img_data[:, y_central, :]\n",
-                "    xz_data = img_data[:, :, x_central]\n",
+                "    xy_data = img_data[z_central - zxy_add[0] : z_central + zxy_add[0], :, :].sum(\n",
+                "        axis=0\n",
+                "    )\n",
+                "    yz_data = img_data[:, x_central - zxy_add[1] : x_central + zxy_add[1], :].sum(\n",
+                "        axis=1\n",
+                "    )\n",
+                "    xz_data = img_data[:, :, y_central - zxy_add[2] : y_central + zxy_add[2]].sum(\n",
+                "        axis=2\n",
+                "    )\n",
                 "\n",
                 "    return [xy_data, yz_data, xz_data]\n",
                 "\n",
                 "\n",
                 "def show_tomogram(tomo_fname):\n",
                 "    \"\"\"tomo_fname can be 3-D .mrc, 3-D .tiff, or stack of 2-D tiffs\"\"\"\n",
                 "\n",
@@ -111,77 +118,60 @@
                 "        img_data = tifffile.imread(tomo_fname)\n",
                 "\n",
                 "    else:\n",
                 "        raise ValueError(\n",
                 "            \"Tomogram cannot be read. Please use a 3D tiff, mrc or stack of 2D Tiffs\"\n",
                 "        )\n",
                 "\n",
-                "    yz_data, xy_data, xz_data = get_central_slices(img_data)\n",
+                "    xy_data, yz_data, xz_data = get_central_slices(img_data)\n",
+                "    data_flattened = np.hstack(\n",
+                "        (xy_data.flatten(), yz_data.flatten(), xz_data.flatten())\n",
+                "    )\n",
+                "\n",
                 "    # Show central slices in xy, yz, xz\n",
-                "    plt.figure(figsize=(10, 5))\n",
+                "    plt.figure(figsize=(10, 3.5))\n",
                 "    plt.suptitle(os.path.basename(tomo_fname))\n",
                 "    titles = [\"x-y\", \"y-z\", \"x-z\"]\n",
                 "\n",
                 "    for i, data in enumerate([xy_data, yz_data, xz_data]):\n",
                 "        plt.subplot(1, 3, i + 1)\n",
                 "        plt.imshow(\n",
                 "            data,\n",
                 "            cmap=\"Greys_r\",\n",
-                "            vmin=np.percentile(data.flatten(), 10),\n",
-                "            vmax=np.percentile(data.flatten(), 90),\n",
+                "            vmin=np.percentile(data_flattened, 10),\n",
+                "            vmax=np.percentile(data_flattened, 90),\n",
                 "        )\n",
                 "        plt.title(titles[i])\n",
                 "\n",
-                "    plt.tight_layout()\n",
-                "\n",
-                "def show_tomograms_as_grid(tomo_filenames: list):\n",
-                "    nrows = math.ceil(len(tomo_filenames) / 4)\n",
-                "    plt.figure(figsize=(10, nrows*3))\n",
-                "\n",
-                "    for i, tomo in enumerate(tomo_filenames):\n",
-                "        plt.subplot(nrows, 4, i+1)\n",
-                "        with mrcfile.open(tomo) as mrc:\n",
-                "            plt.imshow(\n",
-                "                mrc.data, \n",
-                "                cmap=\"Greys_r\", \n",
-                "                # vmin=np.percentile(mrc.data.flatten(), 10),\n",
-                "                # vmax=np.percentile(mrc.data.flatten(), 90),\n",
-                "            )\n",
-                "            plt.title(os.path.basename(tomo).strip(\"_rec_projXY.mrc\"))\n",
-                "            plt.axis('off')\n",
-                "\n",
                 "    plt.tight_layout()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "aa8e6514",
+            "id": "521d9b57",
             "metadata": {
                 "slideshow": {
                     "slide_type": "subslide"
                 },
                 "tags": [
-                    "raises-exception",
-                    "hide"
+                    "hide",
+                    "raises_exception"
                 ]
             },
             "outputs": [],
             "source": [
                 "# Show thumbnails of the tomograms\n",
-                "tomogram_filenames = get_aretomo_tomofilenames()\n",
-                "xy_filenames = [f\"{os.path.splitext(f)[0]}_projXY.mrc\" for f in tomogram_filenames]\n",
-                "show_tomograms_as_grid(xy_filenames)\n",
                 "\n",
-                "print(\"\\n\\n\\n\\n\\n\\n\") # empty lines to avoid bottom being cut off in slides mode"
+                "for tomogram in tomogram_filenames:\n",
+                "    show_tomogram(tomogram)"
             ]
         }
     ],
     "metadata": {
-        "celltoolbar": "Tags",
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
@@ -189,18 +179,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.8.13"
         },
         "vscode": {
             "interpreter": {
-                "hash": "e7370f93d1d0cde622a1f8e1c04877d8463912d04d973331ad4851f04de6915a"
+                "hash": "a924c2a426d7d6d6ce3d626a5e3a7a2287a067c2124b0bdfb6641928f2c3ed0d"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_ctffind.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_ctffind.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_ctfsim.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_ctfsim.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_excludebadtilts.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_excludebadtilts.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_imod_align.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_imod_align.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_imod_header.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_imod_header.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_imod_recon.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_aretomo_recon.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9043828718081436%*

 * *Differences: {"'cells'": "{0: {'id': 'dc30f8f7-6f34-420d-8ef8-d11c56698a5c', 'metadata': {replace: "*

 * *            "OrderedDict([('slideshow', OrderedDict([('slide_type', 'slide')]))])}, 'source': "*

 * *            "['### Tomographic Reconstruction (AreTomo)']}, 1: {'id': 'e7a30837', 'metadata': "*

 * *            "{'slideshow': {'slide_type': 'subslide'}, 'tags': ['raises-exception', 'hide']}, "*

 * *            '\'source\': {insert: [(0, \'def get_aretomo_params():\\n\'), (1, \'    """Print out '*

 * *            'relevant AreTomo setup p […]*

```diff
@@ -1,105 +1,96 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f77a586f",
+            "cell_type": "markdown",
+            "id": "dc30f8f7-6f34-420d-8ef8-d11c56698a5c",
             "metadata": {
-                "tags": [
-                    "raises-exception",
-                    "hide"
-                ]
+                "slideshow": {
+                    "slide_type": "slide"
+                }
             },
-            "outputs": [],
             "source": [
-                "def get_tomogram_filenames():\n",
-                "    # Get IMOD mdout\n",
-                "    try:\n",
-                "        imod_mdout = f\"{os.getcwd()}/{proj_name}_recon_mdout.yaml\"\n",
-                "    except FileNotFoundError:\n",
-                "        print(\n",
-                "            f\"{proj_name}_recon_mdout.yaml not found, cannot find tomogram filenames.\"\n",
-                "        )\n",
-                "\n",
-                "    with open(imod_mdout, \"r\") as f:\n",
-                "        output = yaml.load(f.read(), Loader=yaml.FullLoader)\n",
-                "        tomogram_filenames = output[\"recon_output\"].values()\n",
-                "        algor = output[\"recon_algor\"] if \"recon_algor\" in output.keys() else \"WBP\"\n",
-                "\n",
-                "    return tomogram_filenames, algor\n",
-                "\n",
-                "\n",
-                "tomogram_filenames, algor = get_tomogram_filenames()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "5f17516c-b77c-4b95-a903-cc50fc4baf50",
-            "metadata": {},
-            "source": [
-                "### Tomographic Reconstruction (IMOD)\n",
-                "Reconstruction was performed with IMOD BatchRunTomo."
+                "### Tomographic Reconstruction (AreTomo)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "44d2077d-956d-47d2-9c0c-873c581e987b",
+            "id": "e7a30837",
             "metadata": {
                 "slideshow": {
-                    "slide_type": "slide"
-                }
+                    "slide_type": "subslide"
+                },
+                "tags": [
+                    "raises-exception",
+                    "hide"
+                ]
             },
             "outputs": [],
             "source": [
-                "from IPython.display import Markdown as md\n",
+                "def get_aretomo_params():\n",
+                "    \"\"\"Print out relevant AreTomo setup parameters\"\"\"\n",
+                "    aretomo_yaml = f\"{os.getcwd()}/{proj_name}_aretomo_recon.yaml\"\n",
+                "    if os.path.isfile(aretomo_yaml) is False:\n",
+                "        aretomo_yaml = f\"{os.getcwd()}/{proj_name}_aretomo_align-recon.yaml\"\n",
                 "\n",
-                "printmd(f\" Reconstruction algorithm: {algor}\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "555e9de1-3ed2-4b18-a065-f465419b7148",
-            "metadata": {},
-            "source": [
-                "For more information, please see [https://bio3d.colorado.edu/imod/doc/directives.html](https://bio3d.colorado.edu/imod/doc/directives.html)"
+                "    try:\n",
+                "        with open(aretomo_yaml, \"r\") as f:\n",
+                "            aretomo_params = yaml.load(f.read(), Loader=yaml.FullLoader)\n",
+                "            printmd(f\"Vol Z = {aretomo_params['AreTomo_recon']['volz']}\")\n",
+                "            printmd(\n",
+                "                f\"Sample thickness = {aretomo_params['AreTomo_recon']['sample_thickness']}\"\n",
+                "            )\n",
+                "            printmd(f\"Pixel size = {aretomo_params['AreTomo_recon']['pixel_size']}\")\n",
+                "            printmd(\n",
+                "                f\"Reconstruction algorithm = {aretomo_params['AreTomo_recon']['recon_algo']}\"\n",
+                "            )\n",
+                "    except FileNotFoundError:\n",
+                "        print(f\"{aretomo_yaml} not found, cannot retrieve AreTomo setup parameters\")\n",
+                "\n",
+                "\n",
+                "get_aretomo_params()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6d1a9c1a",
+            "id": "aec1bde9",
             "metadata": {
                 "tags": [
                     "hide"
                 ]
             },
             "outputs": [],
             "source": [
+                "def get_aretomo_tomofilenames():\n",
+                "    \"\"\"Get list of tomograms from AreTomo\"\"\"\n",
+                "    aretomo_yaml = f\"{os.getcwd()}/{proj_name}_aretomo_recon.yaml\"\n",
+                "    if os.path.isfile(aretomo_yaml) is False:\n",
+                "        aretomo_yaml = f\"{os.getcwd()}/{proj_name}_aretomo_align-recon.yaml\"\n",
+                "\n",
+                "    try:\n",
+                "        with open(aretomo_yaml, \"r\") as f:\n",
+                "            aretomo_params = yaml.load(f.read(), Loader=yaml.FullLoader)\n",
+                "            tomogram_filenames = aretomo_params[\"AreTomo_setup\"][\"output_mrc\"]\n",
+                "            return tomogram_filenames\n",
+                "    except FileNotFoundError:\n",
+                "        print(f\"{aretomo_yaml} not found, cannot retrieve tomogram filenames\")\n",
+                "\n",
+                "\n",
                 "def get_central_slices(img_data):\n",
                 "    # Find central slices\n",
-                "    z_central = img_data.shape[0] // 2\n",
-                "    x_central = img_data.shape[1] // 2\n",
-                "    y_central = img_data.shape[2] // 2\n",
-                "\n",
-                "    # Calculate number of slices to add\n",
-                "    zxy_add = (np.array(img_data.shape) * 0.0025).astype(int)\n",
-                "    zxy_add[zxy_add < 1] = 1\n",
+                "    z_central = int(img_data.shape[0] / 2)\n",
+                "    y_central = int(img_data.shape[1] / 2)\n",
+                "    x_central = int(img_data.shape[2] / 2)\n",
                 "\n",
                 "    # xy, yz, xz image data\n",
-                "    xy_data = img_data[z_central - zxy_add[0] : z_central + zxy_add[0], :, :].sum(\n",
-                "        axis=0\n",
-                "    )\n",
-                "    yz_data = img_data[:, x_central - zxy_add[1] : x_central + zxy_add[1], :].sum(\n",
-                "        axis=1\n",
-                "    )\n",
-                "    xz_data = img_data[:, :, y_central - zxy_add[2] : y_central + zxy_add[2]].sum(\n",
-                "        axis=2\n",
-                "    )\n",
+                "    xy_data = img_data[z_central, :, :]\n",
+                "    yz_data = img_data[:, y_central, :]\n",
+                "    xz_data = img_data[:, :, x_central]\n",
                 "\n",
                 "    return [xy_data, yz_data, xz_data]\n",
                 "\n",
                 "\n",
                 "def show_tomogram(tomo_fname):\n",
                 "    \"\"\"tomo_fname can be 3-D .mrc, 3-D .tiff, or stack of 2-D tiffs\"\"\"\n",
                 "\n",
@@ -118,60 +109,57 @@
                 "        img_data = tifffile.imread(tomo_fname)\n",
                 "\n",
                 "    else:\n",
                 "        raise ValueError(\n",
                 "            \"Tomogram cannot be read. Please use a 3D tiff, mrc or stack of 2D Tiffs\"\n",
                 "        )\n",
                 "\n",
-                "    xy_data, yz_data, xz_data = get_central_slices(img_data)\n",
-                "    data_flattened = np.hstack(\n",
-                "        (xy_data.flatten(), yz_data.flatten(), xz_data.flatten())\n",
-                "    )\n",
-                "\n",
+                "    yz_data, xy_data, xz_data = get_central_slices(img_data)\n",
                 "    # Show central slices in xy, yz, xz\n",
-                "    plt.figure(figsize=(10, 3.5))\n",
+                "    plt.figure(figsize=(10, 5))\n",
                 "    plt.suptitle(os.path.basename(tomo_fname))\n",
                 "    titles = [\"x-y\", \"y-z\", \"x-z\"]\n",
                 "\n",
                 "    for i, data in enumerate([xy_data, yz_data, xz_data]):\n",
                 "        plt.subplot(1, 3, i + 1)\n",
                 "        plt.imshow(\n",
                 "            data,\n",
                 "            cmap=\"Greys_r\",\n",
-                "            vmin=np.percentile(data_flattened, 10),\n",
-                "            vmax=np.percentile(data_flattened, 90),\n",
+                "            vmin=np.percentile(data.flatten(), 10),\n",
+                "            vmax=np.percentile(data.flatten(), 90),\n",
                 "        )\n",
                 "        plt.title(titles[i])\n",
                 "\n",
                 "    plt.tight_layout()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "521d9b57",
+            "id": "aa8e6514",
             "metadata": {
                 "slideshow": {
                     "slide_type": "subslide"
                 },
                 "tags": [
-                    "hide",
-                    "raises_exception"
+                    "raises-exception",
+                    "hide"
                 ]
             },
             "outputs": [],
             "source": [
                 "# Show thumbnails of the tomograms\n",
-                "\n",
+                "tomogram_filenames = get_aretomo_tomofilenames()\n",
                 "for tomogram in tomogram_filenames:\n",
                 "    show_tomogram(tomogram)"
             ]
         }
     ],
     "metadata": {
+        "celltoolbar": "Tags",
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
@@ -179,18 +167,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.13"
+            "version": "3.8.10"
         },
         "vscode": {
             "interpreter": {
-                "hash": "a924c2a426d7d6d6ce3d626a5e3a7a2287a067c2124b0bdfb6641928f2c3ed0d"
+                "hash": "e7370f93d1d0cde622a1f8e1c04877d8463912d04d973331ad4851f04de6915a"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_main.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_main.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999917328042328%*

 * *Differences: {"'cells'": "{1: {'source': {delete: [15]}}}"}*

```diff
@@ -36,15 +36,14 @@
                 "import seaborn as sns\n",
                 "import pandas as pd\n",
                 "from IPython.display import Markdown, display\n",
                 "from datetime import datetime\n",
                 "import ot2rec_report\n",
                 "from importlib.metadata import version\n",
                 "import pkg_resources\n",
-                "import math\n",
                 "\n",
                 "plt.rcParams.update({\"figure.max_open_warning\": 0})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_mc.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_mc.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_rlf_deconv.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_rlf_deconv.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_savu_recon.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_savu_recon.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/report_warp.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/report_warp.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/templates/workflow_diagram.ipynb` & `ot2rec_report-0.1.0a0/src/ot2rec_report/templates/workflow_diagram.ipynb`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report/utils.py` & `ot2rec_report-0.1.0a0/src/ot2rec_report/utils.py`

 * *Files identical despite different names*

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/PKG-INFO` & `ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ot2rec-report
-Version: 0.1.0.post4
+Version: 0.1.0a0
 Summary: Generate reports for Ot2Rec
 Home-page: https://github.com/rosalindfranklininstitute/ot2rec_report.git
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ot2Rec Report
```

### Comparing `ot2rec_report-0.1.0.post4/src/ot2rec_report.egg-info/SOURCES.txt` & `ot2rec_report-0.1.0a0/src/ot2rec_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

