# Comparing `tmp/module_qc_data_tools-1.0.3.tar.gz` & `tmp/module_qc_data_tools-1.0.4.tar.gz`

## Comparing `module_qc_data_tools-1.0.3.tar` & `module_qc_data_tools-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/.flake8
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/.gitlab-ci.yml
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/tbump.toml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/src/module_qc_data_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/src/module_qc_data_tools/_version.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/src/module_qc_data_tools/mux_conversion.py
--rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/src/module_qc_data_tools/qcDataFrame.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/tests/test_package.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/LICENSE
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/README.md
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/.flake8
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/tbump.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/src/module_qc_data_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/src/module_qc_data_tools/_version.py
+-rw-r--r--   0        0        0    13584 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/src/module_qc_data_tools/qcDataFrame.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/tests/test_package.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/README.md
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.4/PKG-INFO
```

### Comparing `module_qc_data_tools-1.0.3/.gitlab-ci.yml` & `module_qc_data_tools-1.0.4/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
             "python:3.9-buster",
             "python:3.10-buster",
             "python:3.11-buster",
           ]
 
 package:
   stage: build
+  variables:
+    GIT_STRATEGY: clone
   script:
     - pipx run hatch run build-check
   artifacts:
     paths:
       - dist/
 
 .deploy:
```

### Comparing `module_qc_data_tools-1.0.3/.pre-commit-config.yaml` & `module_qc_data_tools-1.0.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
     hooks:
       - id: check-json
       - id: trailing-whitespace
       # broken in old git from 2013
       # - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
-      - id: no-commit-to-branch
-        args: [--branch, main]
       - id: check-case-conflict
       - id: debug-statements
       - id: mixed-line-ending
       - id: check-symlinks
       - id: check-toml
       - id: check-yaml
       - id: requirements-txt-fixer
```

### Comparing `module_qc_data_tools-1.0.3/tbump.toml` & `module_qc_data_tools-1.0.4/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e30 2e33 220a 0a23 2045  t = "1.0.3"..# E
+00000010: 7420 3d20 2231 2e30 2e34 220a 0a23 2045  t = "1.0.4"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 312e 302e  mp version: 1.0.
-00000150: 3320 e286 9220 7b6e 6577 5f76 6572 7369  3 ... {new_versi
+00000150: 3420 e286 9220 7b6e 6577 5f76 6572 7369  4 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_data_tools-1.0.3/src/module_qc_data_tools/qcDataFrame.py` & `module_qc_data_tools-1.0.4/src/module_qc_data_tools/qcDataFrame.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,17 +80,21 @@
         json.dump(sorted_output, fp, cls=MyEncoder, indent=4)
 
 
 def load_json(path):
     with open(path) as serialized:
         inputdata = json.load(serialized)
     alldf = []
+    # Can read measurement jsons (nested list) or analysis jsons (1D list)
     for chip in inputdata:
-        for _dict in chip:
-            alldf += [outputDataFrame(_dict=_dict)]
+        if isinstance(chip, list):
+            for _dict in chip:
+                alldf += [outputDataFrame(_dict=_dict)]
+        else:
+            alldf += [outputDataFrame(_dict=chip)]
     return alldf
 
 
 def convert_name_to_serial(chipName):
     serialPrefix = "20UPGFC"  # This will change to 20UPGFW for real wafers
     try:
         chip_number = str(int(chipName, base=16))
@@ -101,14 +105,29 @@
     except Exception:
         print(
             f"Warning: Can't convert chip name ({chipName}) into serial number, setting serial number to {chipName}"
         )
         return chipName
 
 
+def convert_serial_to_name(chipSerial):
+    # Assumes prefix is of length 7 (i.e. "20UPGFC")
+    try:
+        # Remove prefix and preceding 0's
+        chipSerial = chipSerial[7:]
+        chipSerial = chipSerial.lstrip("0")
+        chipName = hex(int(chipSerial))
+    except Exception:
+        chipName = chipSerial
+        print(
+            f"Warning: Can't convert chip serial number ({chipSerial}) into name, setting chip name to {chipSerial}"
+        )
+    return chipName
+
+
 # requires the connectivity file name to be "<ATLAS_SN>_<layer>_<temperature>.json" as output from the database tool
 def get_sn_from_connectivity(fileName):
     try:
         moduleSN = os.path.basename(fileName).split("_")[0]
         check_sn_format(moduleSN)
     except Exception as e:
         print(f"Error: Cannot extract module serial number from path ({fileName}): {e}")
@@ -341,15 +360,16 @@
         self._passed = passed
 
     def set_results(self, results=None):
         if results is not None:
             self._results = results
         else:
             self._results = qcDataFrame()
-        self.set_serial_num()
+        if self._serialNumber == "Unknown":
+            self.set_serial_num()
 
     def get_results(self):
         return self._results
 
     def to_dict(self, forAnalysis=False):
         _dict = {"serialNumber": self._serialNumber, "testType": self._testType}
         if not forAnalysis:
@@ -383,8 +403,11 @@
         with open(path, "w") as fp:
             json.dump(_dict, fp, cls=MyEncoder, indent=4)
 
     def from_dict(self, _dict):
         self._serialNumber = _dict.get("serialNumber")
         self._testType = _dict.get("testType")
         self._subtestType = _dict.get("subtestType")
-        self._results = qcDataFrame(_dict=_dict.get("results"))
+        try:
+            self._results = qcDataFrame(_dict=_dict.get("results"))
+        except Exception:
+            self._results = _dict.get("results")
```

### Comparing `module_qc_data_tools-1.0.3/.gitignore` & `module_qc_data_tools-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_data_tools-1.0.3/LICENSE` & `module_qc_data_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_data_tools-1.0.3/README.md` & `module_qc_data_tools-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module QC data tools v1.0.3
+# module QC data tools v1.0.4
 
 This project contains the modules needed to write/read the data files used in
 the module QC flow. This project is to be added as a submodule in other
 projects.
 
 ## Installation
 
@@ -28,15 +28,15 @@
 ```
 
 ### via pip
 
 ```
 python -m venv venv
 source venv/bin/activate
-python -m pip install -U pip module-qc-data-tools==1.0.3
+python -m pip install -U pip module-qc-data-tools==1.0.4
 ```
 
 ## Developer
 
 ### versioning
 
 In case you need to tag the version of the code, you need to have either `hatch`
```

### Comparing `module_qc_data_tools-1.0.3/pyproject.toml` & `module_qc_data_tools-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_data_tools-1.0.3/PKG-INFO` & `module_qc_data_tools-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module_qc_data_tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Module qc data tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-data-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-data-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-data-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -32,15 +32,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: jsonschema
 Requires-Dist: numpy
 Requires-Dist: tabulate
 Description-Content-Type: text/markdown
 
-# module QC data tools v1.0.3
+# module QC data tools v1.0.4
 
 This project contains the modules needed to write/read the data files used in
 the module QC flow. This project is to be added as a submodule in other
 projects.
 
 ## Installation
 
@@ -66,15 +66,15 @@
 ```
 
 ### via pip
 
 ```
 python -m venv venv
 source venv/bin/activate
-python -m pip install -U pip module-qc-data-tools==1.0.3
+python -m pip install -U pip module-qc-data-tools==1.0.4
 ```
 
 ## Developer
 
 ### versioning
 
 In case you need to tag the version of the code, you need to have either `hatch`
```

