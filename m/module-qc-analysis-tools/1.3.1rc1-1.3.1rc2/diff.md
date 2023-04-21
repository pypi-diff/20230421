# Comparing `tmp/module_qc_analysis_tools-1.3.1rc1.tar.gz` & `tmp/module_qc_analysis_tools-1.3.1rc2.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.1rc1.tar` & `module_qc_analysis_tools-1.3.1rc2.tar`

### file list

```diff
@@ -1,31 +1,37 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0    23808 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/globals.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0    21042 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    34380 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/LICENSE
--rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/README.md
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/pyproject.toml
--rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/MINIMUM_HEALTH.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/PIXEL_FAILURE.py
+-rw-r--r--   0        0        0    23808 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/TUNING_PERFORMANCE.py
+-rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     5382 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0    21307 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    34380 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/LICENSE
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/README.md
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/pyproject.toml
+-rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc2/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.1rc1/.gitlab-ci.yml` & `module_qc_analysis_tools-1.3.1rc2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/.pre-commit-config.yaml` & `module_qc_analysis_tools-1.3.1rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/tbump.toml` & `module_qc_analysis_tools-1.3.1rc2/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 7263 3122 0a0a  t = "1.3.1rc1"..
+00000010: 7420 3d20 2231 2e33 2e31 7263 3222 0a0a  t = "1.3.1rc2"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
-00000150: 2e33 2e31 7263 3120 e286 9220 7b6e 6577  .3.1rc1 ... {new
+00000150: 2e33 2e31 7263 3220 e286 9220 7b6e 6577  .3.1rc2 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/globals.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,38 +30,73 @@
     "--input-meas",
     help="path to the input measurement file or directory containing input measurement files.",
     exists=True,
     file_okay=True,
     readable=True,
     resolve_path=True,
 )
+OPTIONS["input_yarr_config"]: Path = typer.Option(
+    "info.json",
+    "-i",
+    "--input-yarr-config",
+    help="path to the json config file containing paths to YARR scan outputs. Run analysis-load-yarr-scans.py to generate.",
+    exists=True,
+    file_okay=True,
+    readable=True,
+    resolve_path=True,
+)
+OPTIONS["input_yarr_scans"]: Path = typer.Option(
+    None,
+    "-i",
+    "--input-yarr-scans",
+    help="path to the json config file containing paths to YARR scan outputs. Run analysis-load-yarr-scans.py to generate.",
+    exists=True,
+    readable=True,
+    resolve_path=True,
+)
 OPTIONS["output_dir"]: Path = typer.Option(
     "outputs",
     "-o",
     "--output-dir",
     help="output directory",
     exists=False,
     writable=True,
 )
 OPTIONS["qc_criteria"]: Path = typer.Option(
     str(data / "analysis_cuts.json"),
     "-q",
     "--qc-criteria",
-    help="path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)",
+    help="path to json file with QC selection criteria",
+    exists=True,
+    file_okay=True,
+    readable=True,
+    resolve_path=True,
+)
+OPTIONS["pixel_classification"]: Path = typer.Option(
+    str(data / "pixel_classification.json"),
+    "-p",
+    "--pixel-failure-config",
+    help="path to json file with pixel failure selection criteria",
     exists=True,
     file_okay=True,
     readable=True,
     resolve_path=True,
 )
 OPTIONS["layer"]: str = typer.Option(
     "Unknown",
     "-l",
     "--layer",
     help="Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2 (default)",
 )
+OPTIONS["moduleSN"]: str = typer.Option(
+    "Unknown",
+    "-m",
+    "--moduleSN",
+    help="Module serial number",
+)
 OPTIONS["permodule"]: bool = typer.Option(
     False, help="Store results in one file per module (default: one file per chip)"
 )
 OPTIONS["fit_method"]: FitMethod = typer.Option(
     FitMethod.numpy, "-f", "--fit-method", help="fitting method"
 )
 OPTIONS["nchips"]: int = typer.Option(
@@ -137,7 +172,48 @@
     "--config-type",
     help="The config type to be modified. E.g. E.g. L2_warm/l2_cold.",
 )
 OPTIONS["override"]: bool = typer.Option(
     False,
     help="Update chip configuration even if the chip failed QC",
 )
+OPTIONS["output_yarr"]: str = typer.Option(
+    None,
+    "-o",
+    "--output-yarr",
+    help="output directory to put info.json which will be used as input to YARR scan analysis",
+    exists=False,
+    writable=True,
+    resolve_path=True,
+)
+OPTIONS["digitalscan"]: Path = typer.Option(
+    None,
+    "-ds",
+    "--digital-scan",
+    help="path to the digital scan output directory to use in YARR analysis",
+    exists=True,
+    readable=True,
+)
+OPTIONS["analogscan"]: Path = typer.Option(
+    None,
+    "-as",
+    "--analog-scan",
+    help="path to the analog scan output directory to use in YARR analysis",
+    exists=True,
+    readable=True,
+)
+OPTIONS["thresholdscan_hr"]: Path = typer.Option(
+    None,
+    "-hr",
+    "--threshold-scan-hr",
+    help="path to the threshold scan (high-range) output directory to use in YARR analysis",
+    exists=True,
+    readable=True,
+)
+OPTIONS["thresholdscan_hd"]: Path = typer.Option(
+    None,
+    "-hd",
+    "--threshold-scan-hd",
+    help="path to the threshold scan (high-def) output directory to use in YARR analysis",
+    exists=True,
+    readable=True,
+)
```

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 from module_qc_analysis_tools.cli.ADC_CALIBRATION import main as adc_calibration
 from module_qc_analysis_tools.cli.ANALOG_READBACK import main as analog_readback
 from module_qc_analysis_tools.cli.globals import CONTEXT_SETTINGS
 from module_qc_analysis_tools.cli.INJECTION_CAPACITANCE import (
     main as injection_capacitance,
 )
 from module_qc_analysis_tools.cli.IV_MEASURE import main as iv_measure
+from module_qc_analysis_tools.cli.load_yarr_scans import main as load_yarr_scans
 from module_qc_analysis_tools.cli.MASS_MEASUREMENT import main as mass
+from module_qc_analysis_tools.cli.MINIMUM_HEALTH import main as minimum_health
 from module_qc_analysis_tools.cli.overwrite_config import main as overwrite_config
+from module_qc_analysis_tools.cli.PIXEL_FAILURE import main as pixel_failure
 from module_qc_analysis_tools.cli.SLDO import main as sldo
+from module_qc_analysis_tools.cli.TUNING_PERFORMANCE import main as tuning_performance
 from module_qc_analysis_tools.cli.update_chip_config import main as update_chip_config
 from module_qc_analysis_tools.cli.VCAL_CALIBRATION import main as vcal_calibration
 from module_qc_analysis_tools.cli.VISUAL_INSPECTION import main as visual_inspection
 
 # subcommands
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 app_analysis = typer.Typer(context_settings=CONTEXT_SETTINGS)
@@ -52,10 +56,14 @@
 app_analysis.command("sldo")(sldo)
 app_analysis.command("vcal-calibration")(vcal_calibration)
 app_analysis.command("mass-measurement")(mass)
 app_analysis.command("iv-measure")(iv_measure)
 app_analysis.command("visual-inspection")(visual_inspection)
 app_config.command("overwrite")(overwrite_config)
 app_config.command("update")(update_chip_config)
+app_config.command("load-yarr-scans")(load_yarr_scans)
+app_config.command("minimum-health")(minimum_health)
+app_config.command("tuning-performance")(tuning_performance)
+app_config.command("pixel-failure")(pixel_failure)
 
 # for generating documentation using mkdocs-click
 typer_click_object = typer.main.get_command(app)
```

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'MINIMUM_HEALTH'": "OrderedDict([('BAD_ANALOG_INTEGRATED', [0, 153.6]), "*

 * *                     "('THRESHOLD_FAILED_FITS_INDEPENDENT', [0, 1536]), ('HIGH_ENC_INDEPENDENT', "*

 * *                     '[0, 1536])])',*

 * * "'PIXEL_FAILURE'": "OrderedDict([('ELECTRICALLY_FAILED', [0, 153.6])])",*

 * * "'TUNING_PERFORMANCE'": "OrderedDict([('UNTUNED_THRESHOLD_MEAN', [1700, 2700]), "*

 * *                         "('UNTUNED_THRESHOLD_FAILED_FITS', [0, 1536]), "*

 * *                         "('UNTUNED_THRESHOLD_SIGMA', [0, 400]), ('TU […]*

```diff
@@ -168,14 +168,34 @@
     "INJECTION_CAPACITANCE": {
         "INJ_CAPACITANCE": [
             6.74,
             9.0
         ]
     },
     "MASS_MEASUREMENT": {},
+    "MINIMUM_HEALTH": {
+        "BAD_ANALOG_INTEGRATED": [
+            0,
+            153.6
+        ],
+        "HIGH_ENC_INDEPENDENT": [
+            0,
+            1536
+        ],
+        "THRESHOLD_FAILED_FITS_INDEPENDENT": [
+            0,
+            1536
+        ]
+    },
+    "PIXEL_FAILURE": {
+        "ELECTRICALLY_FAILED": [
+            0,
+            153.6
+        ]
+    },
     "SLDO": {
         "SLDO_IINA": {
             "LOne": [
                 0.681,
                 0.735
             ],
             "LTwo": [
@@ -288,14 +308,54 @@
             ],
             "LZero": [
                 1.09,
                 1.11
             ]
         }
     },
+    "TUNING_PERFORMANCE": {
+        "TUNED_TDAC_MEAN": [
+            -1,
+            1
+        ],
+        "TUNED_TDAC_SIGMA": [
+            8.5,
+            12.5
+        ],
+        "TUNED_THRESHOLD_MEAN": {
+            "LOne": [
+                1350,
+                1650
+            ],
+            "LTwo": [
+                1350,
+                1650
+            ],
+            "LZero": [
+                900,
+                1100
+            ]
+        },
+        "TUNED_THRESHOLD_SIGMA": [
+            0,
+            50
+        ],
+        "UNTUNED_THRESHOLD_FAILED_FITS": [
+            0,
+            1536
+        ],
+        "UNTUNED_THRESHOLD_MEAN": [
+            1700,
+            2700
+        ],
+        "UNTUNED_THRESHOLD_SIGMA": [
+            0,
+            400
+        ]
+    },
     "VCAL_CALIBRATION": {
         "VCAL_HIGH_OFFSET": [
             -23,
             17
         ],
         "VCAL_HIGH_SLOPE": [
             0.16,
```

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 log.setLevel("INFO")
 
 
 def format_text():
     return " {:^30}: {:^20}: {:^20}: {:^5}"
 
 
+def format_text_short():
+    return " {:^30}: {:^20}:"
+
+
 def print_output_pass(key, results, lower_bound, upper_bound):
     txt = format_text()
     log.info(
         bcolors.OKGREEN
         + txt.format(
             key,
             round(results, 4),
@@ -41,14 +45,19 @@
             f"[{lower_bound}, {upper_bound}]",
             "FAIL",
         )
         + bcolors.ENDC
     )
 
 
+def print_output_neutral(key, results):
+    txt = format_text_short()
+    log.info(bcolors.WARNING + txt.format(key, round(results, 4)) + bcolors.ENDC)
+
+
 def get_layer(layer):
     layers = {"L0": "LZero", "L1": "LOne", "L2": "LTwo"}
     return layers.get(layer)
 
 
 def check_layer(layer):
     possible_layers = ["L0", "L1", "L2"]
@@ -231,19 +240,20 @@
     log.info(txt.format("Parameter", "Analysis result", "QC criteria", "Pass"))
     log.info(
         "--------------------------------------------------------------------------------------"
     )
 
     for key in results:
         if not qc_selections.get(key):
-            log.warning(
+            log.debug(
                 bcolors.WARNING
                 + f" Selection for {key} not found in QC file! Skipping."
                 + bcolors.ENDC
             )
+            print_output_neutral(key, results.get(key))
             continue
         check_qc_selections.pop(key)
 
         # Handle AR_NOMINAL_SETTINGS in completely different function, for now...
         if key == "AR_NOMINAL_SETTINGS":
             passes_qc_test = perform_qc_analysis_AR_NOMINAL_SETTINGS(
                 test_type,
```

### Comparing `module_qc_analysis_tools-1.3.1rc1/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-1.3.1rc2/src/module_qc_analysis_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/tests/test_cli.py` & `module_qc_analysis_tools-1.3.1rc2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/.gitignore` & `module_qc_analysis_tools-1.3.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/LICENSE` & `module_qc_analysis_tools-1.3.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc1/README.md` & `module_qc_analysis_tools-1.3.1rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v1.3.1rc1
+# module-qc-analysis-tools v1.3.1rc2
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -49,15 +49,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc1
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc2
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

### Comparing `module_qc_analysis_tools-1.3.1rc1/pyproject.toml` & `module_qc_analysis_tools-1.3.1rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 description = "Module qc analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
     "matplotlib",
-    "module-qc-data-tools >= 1.0.3",
+    "module-qc-data-tools >= 1.0.4",
     "typer",
     "importlib_resources>=1.4.0; python_version < '3.9'",  # for resources
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -42,14 +42,18 @@
 analysis-SLDO = "module_qc_analysis_tools.cli.SLDO:app"
 analysis-VCAL-CALIBRATION = "module_qc_analysis_tools.cli.VCAL_CALIBRATION:app"
 analysis-MASS-MEASUREMENT = "module_qc_analysis_tools.cli.MASS_MEASUREMENT:app"
 analysis-IV-MEASURE = "module_qc_analysis_tools.cli.IV_MEASURE:app"
 analysis-VISUAL-INSPECTION = "module_qc_analysis_tools.cli.VISUAL_INSPECTION:app"
 analysis-overwrite-config = "module_qc_analysis_tools.cli.overwrite_config:app"
 analysis-update-chip-config = "module_qc_analysis_tools.cli.update_chip_config:app"
+analysis-load-yarr-scans = "module_qc_analysis_tools.cli.load_yarr_scans:app"
+analysis-MINIMUM-HEALTH = "module_qc_analysis_tools.cli.MINIMUM_HEALTH:app"
+analysis-TUNING-PERFORMANCE = "module_qc_analysis_tools.cli.TUNING_PERFORMANCE:app"
+analysis-PIXEL-FAILURE = "module_qc_analysis_tools.cli.PIXEL_FAILURE:app"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
```

### Comparing `module_qc_analysis_tools-1.3.1rc1/PKG-INFO` & `module_qc_analysis_tools-1.3.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.1rc1
+Version: 1.3.1rc2
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -29,20 +29,20 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
-Requires-Dist: module-qc-data-tools>=1.0.3
+Requires-Dist: module-qc-data-tools>=1.0.4
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.1rc1
+# module-qc-analysis-tools v1.3.1rc2
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -89,15 +89,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc1
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc2
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

