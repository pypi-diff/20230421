# Comparing `tmp/rushd-0.3.0.tar.gz` & `tmp/rushd-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rushd-0.3.0.tar", last modified: Wed Mar  1 18:18:54 2023, max compression
+gzip compressed data, was "rushd-0.4.0.tar", last modified: Fri Apr 21 13:22:50 2023, max compression
```

## Comparing `rushd-0.3.0.tar` & `rushd-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-03-01 18:18:54.822243 rushd-0.3.0/
--rw-r--r--   0 kaseylove   (501) staff       (20)     1069 2022-01-21 15:10:03.000000 rushd-0.3.0/LICENSE
--rw-r--r--   0 kaseylove   (501) staff       (20)     3762 2023-03-01 18:18:54.821886 rushd-0.3.0/PKG-INFO
--rw-r--r--   0 kaseylove   (501) staff       (20)     2857 2023-03-01 17:55:41.000000 rushd-0.3.0/README.md
--rw-r--r--   0 kaseylove   (501) staff       (20)      527 2023-03-01 18:01:20.000000 rushd-0.3.0/pyproject.toml
--rw-r--r--   0 kaseylove   (501) staff       (20)       38 2023-03-01 18:18:54.822393 rushd-0.3.0/setup.cfg
--rw-r--r--   0 kaseylove   (501) staff       (20)     1823 2023-03-01 18:03:58.000000 rushd-0.3.0/setup.py
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-03-01 18:18:54.808907 rushd-0.3.0/src/
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-03-01 18:18:54.814861 rushd-0.3.0/src/rushd/
--rw-r--r--   0 kaseylove   (501) staff       (20)      637 2023-03-01 18:01:20.000000 rushd-0.3.0/src/rushd/__init__.py
--rw-r--r--   0 kaseylove   (501) staff       (20)    14652 2023-03-01 18:03:58.000000 rushd-0.3.0/src/rushd/flow.py
--rw-r--r--   0 kaseylove   (501) staff       (20)    11309 2023-03-01 18:01:20.000000 rushd-0.3.0/src/rushd/io.py
--rw-r--r--   0 kaseylove   (501) staff       (20)     6198 2023-03-01 18:01:20.000000 rushd-0.3.0/src/rushd/well_mapper.py
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-03-01 18:18:54.817622 rushd-0.3.0/src/rushd.egg-info/
--rw-r--r--   0 kaseylove   (501) staff       (20)     3762 2023-03-01 18:18:54.000000 rushd-0.3.0/src/rushd.egg-info/PKG-INFO
--rw-r--r--   0 kaseylove   (501) staff       (20)      403 2023-03-01 18:18:54.000000 rushd-0.3.0/src/rushd.egg-info/SOURCES.txt
--rw-r--r--   0 kaseylove   (501) staff       (20)        1 2023-03-01 18:18:54.000000 rushd-0.3.0/src/rushd.egg-info/dependency_links.txt
--rw-r--r--   0 kaseylove   (501) staff       (20)      210 2023-03-01 18:18:54.000000 rushd-0.3.0/src/rushd.egg-info/requires.txt
--rw-r--r--   0 kaseylove   (501) staff       (20)        6 2023-03-01 18:18:54.000000 rushd-0.3.0/src/rushd.egg-info/top_level.txt
-drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-03-01 18:18:54.821029 rushd-0.3.0/tests/
--rw-r--r--   0 kaseylove   (501) staff       (20)    11898 2023-03-01 18:01:20.000000 rushd-0.3.0/tests/test_file_io.py
--rw-r--r--   0 kaseylove   (501) staff       (20)     3607 2023-03-01 18:01:20.000000 rushd-0.3.0/tests/test_file_moi.py
--rw-r--r--   0 kaseylove   (501) staff       (20)    18337 2023-03-01 18:03:58.000000 rushd-0.3.0/tests/test_flow.py
--rw-r--r--   0 kaseylove   (501) staff       (20)      891 2023-03-01 18:01:20.000000 rushd-0.3.0/tests/test_pandas_cache.py
--rw-r--r--   0 kaseylove   (501) staff       (20)     3274 2023-03-01 18:01:20.000000 rushd-0.3.0/tests/test_well_mapper.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.693870 rushd-0.4.0/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     1069 2022-08-30 19:04:22.000000 rushd-0.4.0/LICENSE
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3824 2023-04-21 13:22:50.693870 rushd-0.4.0/PKG-INFO
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     2856 2023-04-21 13:20:40.000000 rushd-0.4.0/README.md
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      527 2023-02-02 22:08:57.000000 rushd-0.4.0/pyproject.toml
+-rw-r--r--   0 christopher  (1000) christopher  (1000)       38 2023-04-21 13:22:50.693870 rushd-0.4.0/setup.cfg
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     1885 2023-04-21 13:13:34.000000 rushd-0.4.0/setup.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.683870 rushd-0.4.0/src/
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.687204 rushd-0.4.0/src/rushd/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      651 2023-04-19 21:24:37.000000 rushd-0.4.0/src/rushd/__init__.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    15001 2023-04-19 19:55:19.000000 rushd-0.4.0/src/rushd/flow.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    11309 2023-02-02 21:36:26.000000 rushd-0.4.0/src/rushd/io.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     6509 2023-04-21 13:09:39.000000 rushd-0.4.0/src/rushd/plot.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     6281 2023-04-19 19:55:18.000000 rushd-0.4.0/src/rushd/well_mapper.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.687204 rushd-0.4.0/src/rushd.egg-info/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3824 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/PKG-INFO
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      440 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/SOURCES.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)        1 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/dependency_links.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      210 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/requires.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)        6 2023-04-21 13:22:50.000000 rushd-0.4.0/src/rushd.egg-info/top_level.txt
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-04-21 13:22:50.690537 rushd-0.4.0/tests/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    11898 2023-02-02 22:12:16.000000 rushd-0.4.0/tests/test_file_io.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3607 2023-02-02 22:12:16.000000 rushd-0.4.0/tests/test_file_moi.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    18337 2023-03-24 17:26:34.000000 rushd-0.4.0/tests/test_flow.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      891 2023-02-02 22:12:16.000000 rushd-0.4.0/tests/test_pandas_cache.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     4469 2023-04-19 20:32:45.000000 rushd-0.4.0/tests/test_plot.py
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     3274 2023-02-02 22:12:16.000000 rushd-0.4.0/tests/test_well_mapper.py
```

### Comparing `rushd-0.3.0/LICENSE` & `rushd-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rushd-0.3.0/PKG-INFO` & `rushd-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: rushd
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package for maintaining robust, reproducible data management.
 Home-page: https://github.com/GallowayLabMIT/rushd
 Author: Christopher Johnstone, Kasey Love, Conrad Oakes
 Author-email: meson800@gmail.com
 Project-URL: Bug Tracker, https://github.com/GallowayLabMIT/rushd/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # rushd
+[![Stable documentation](https://img.shields.io/badge/Documentation-stable-blue)](https://gallowaylabmit.github.io/rushd/en/main/)
 [![PyPI-downloads](https://img.shields.io/pypi/dm/rushd)](https://pypi.org/project/rushd)
 [![PyPI-version](https://img.shields.io/pypi/v/rushd)](https://pypi.org/project/rushd)
 [![PyPI-license](https://img.shields.io/pypi/l/rushd)](https://pypi.org/project/rushd)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/rushd)](https://pypi.org/project/rushd)
 [![codecov](https://codecov.io/gh/GallowayLabMIT/rushd/branch/main/graph/badge.svg?token=ALaU8lQxt5)](https://codecov.io/gh/GallowayLabMIT/rushd)
 
 A package for maintaining robust, reproducible data management.
@@ -43,15 +45,16 @@
 
 ## Quickstart
 Simply import `rushd`!
 ```
 import rushd as rd
 ```
 
-## Complete Examples
+## Documentation
+See the documentation available at https://gallowaylabmit.github.io/rushd
 
 ## Developer install
 If you'd like to hack locally on `rushd`, after cloning this repository:
 ```
 $ git clone https://github.com/GallowayLabMIT/rushd.git
 $ cd rushd
 ```
@@ -65,20 +68,17 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
-## [0.3.0] - 2023-03-01
+## [0.4.0] - 2023-04-21
 ### Added
-- `rd.flow.load_groups_with_metadata` loads files from several folders (groups, e.g. corresponding to plates) into a single dataframe
-### Modified
-- `rd.flow.moi` properly generates plots of MOI vs fraction infected for checking calculation accuracy
-- `rd.well_mapper` properly handles metadata concatenation
+- `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
 
 ## What does the name mean?
 The name is a reference to [Ibn Rushd](https://en.wikipedia.org/wiki/Averroes), a Muslim scholar born in Córdoba who was responsible for translating and adding scholastic commentary to ancient Greek works, especially Aristotle. His translations spurred further translations into Latin and Hebrew, reigniting interest in ancient Greek works for the first time since the fall of the Roman empire.
```

### Comparing `rushd-0.3.0/README.md` & `rushd-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # rushd
+[![Stable documentation](https://img.shields.io/badge/Documentation-stable-blue)](https://gallowaylabmit.github.io/rushd/en/main/)
 [![PyPI-downloads](https://img.shields.io/pypi/dm/rushd)](https://pypi.org/project/rushd)
 [![PyPI-version](https://img.shields.io/pypi/v/rushd)](https://pypi.org/project/rushd)
 [![PyPI-license](https://img.shields.io/pypi/l/rushd)](https://pypi.org/project/rushd)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/rushd)](https://pypi.org/project/rushd)
 [![codecov](https://codecov.io/gh/GallowayLabMIT/rushd/branch/main/graph/badge.svg?token=ALaU8lQxt5)](https://codecov.io/gh/GallowayLabMIT/rushd)
 
 A package for maintaining robust, reproducible data management.
@@ -20,15 +21,16 @@
 
 ## Quickstart
 Simply import `rushd`!
 ```
 import rushd as rd
 ```
 
-## Complete Examples
+## Documentation
+See the documentation available at https://gallowaylabmit.github.io/rushd
 
 ## Developer install
 If you'd like to hack locally on `rushd`, after cloning this repository:
 ```
 $ git clone https://github.com/GallowayLabMIT/rushd.git
 $ cd rushd
 ```
@@ -42,20 +44,17 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
-## [0.3.0] - 2023-03-01
+## [0.4.0] - 2023-04-21
 ### Added
-- `rd.flow.load_groups_with_metadata` loads files from several folders (groups, e.g. corresponding to plates) into a single dataframe
-### Modified
-- `rd.flow.moi` properly generates plots of MOI vs fraction infected for checking calculation accuracy
-- `rd.well_mapper` properly handles metadata concatenation
+- `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
 
 ## What does the name mean?
 The name is a reference to [Ibn Rushd](https://en.wikipedia.org/wiki/Averroes), a Muslim scholar born in Córdoba who was responsible for translating and adding scholastic commentary to ancient Greek works, especially Aristotle. His translations spurred further translations into Latin and Hebrew, reigniting interest in ancient Greek works for the first time since the fall of the Roman empire.
```

### Comparing `rushd-0.3.0/pyproject.toml` & `rushd-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rushd-0.3.0/setup.py` & `rushd-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rushd",
-    version="0.3.0",
+    version="0.4.0",
     author="Christopher Johnstone, Kasey Love, Conrad Oakes",
     author_email="meson800@gmail.com",
     description="Package for maintaining robust, reproducible data management.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GallowayLabMIT/rushd",
     project_urls={
         "Bug Tracker": "https://github.com/GallowayLabMIT/rushd/issues",
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Utilities",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `rushd-0.3.0/src/rushd/__init__.py` & `rushd-0.4.0/src/rushd/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """## rushd: data management for humans.
 
 Collection of helper modules for maintaining
 robust, reproducible data management.
 """
-from . import flow, io  # noqa
+from . import flow, io, plot  # noqa
 from .io import infile, outfile  # noqa
 
-submodules = ["io", "flow"]
+submodules = ["io", "flow", "plot"]
 
 re_exports = [
     "infile",
     "outfile",
 ]
 # Re-exports of common functions loaded from submodules
 __all__ = submodules + re_exports
```

### Comparing `rushd-0.3.0/src/rushd/flow.py` & `rushd-0.4.0/src/rushd/flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Allows users to specify custom metadata applied via well mapping.
 Combines user data from multiple .csv files into a single DataFrame.
 """
 import re
 import warnings
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 # Support Python 3.7 by importing Literal from typing_extensions
 try:
     from typing import Literal  # type: ignore
 except ImportError:
     from typing_extensions import Literal
 
@@ -40,14 +40,47 @@
     """Error raised when there is an issue with the data groups DataFrame."""
 
 
 class MOIinputError(RuntimeError):
     """Error raised when there is an issue with the provided dataframe."""
 
 
+def load_well_metadata(yaml_path: Union[str, Path]) -> Dict[Any, Any]:
+    """Load a YAML file and convert it into a well mapping.
+
+    Parameters
+    ----------
+    yaml_path: Path to the .yaml file to use for associating metadata with well IDs.
+
+    Returns
+    -------
+    A dictionary that contains a well mapping for all metadata columns.
+    """
+    if not isinstance(yaml_path, Path):
+        yaml_path = Path(yaml_path)
+
+    with yaml_path.open() as yaml_file:
+        metadata = yaml.safe_load(yaml_file)
+        if (type(metadata) is not dict) or ("metadata" not in metadata):
+            raise YamlError(
+                "Incorrectly formatted .yaml file."
+                " All metadata must be stored under the header 'metadata'"
+            )
+        for k, v in metadata["metadata"].items():
+            if isinstance(v, dict):
+                warnings.warn(
+                    f'Metadata column "{k}" is a YAML dictionary, not a list!'
+                    " Make sure your entries under this key start with dashes."
+                    " Passing a dictionary does not allow duplicate keys and"
+                    " is sort-order-dependent.",
+                    MetadataWarning,
+                )
+    return {k: well_mapper.well_mapping(v) for k, v in metadata["metadata"].items()}
+
+
 def load_csv_with_metadata(
     data_path: Union[str, Path], yaml_path: Union[str, Path], filename_regex: Optional[str] = None
 ) -> pd.DataFrame:
     """
     Load .csv data into DataFrame with associated metadata.
 
     Generates a pandas DataFrame from a set of .csv files located at the given path,
@@ -67,37 +100,19 @@
         If not included, the filenames are assumed to follow this format (default
         export format from FlowJo): 'export_[well]_[population].csv'
 
     Returns
     -------
     A single pandas DataFrame containing all data with associated metadata.
     """
-    if not isinstance(yaml_path, Path):
-        yaml_path = Path(yaml_path)
     if not isinstance(data_path, Path):
         data_path = Path(data_path)
 
     try:
-        with yaml_path.open() as file:
-            metadata = yaml.safe_load(file)
-            if (type(metadata) is not dict) or ("metadata" not in metadata):
-                raise YamlError(
-                    "Incorrectly formatted .yaml file."
-                    " All metadata must be stored under the header 'metadata'"
-                )
-            for k, v in metadata["metadata"].items():
-                if isinstance(v, dict):
-                    warnings.warn(
-                        f'Metadata column "{k}" is a YAML dictionary, not a list!'
-                        " Make sure your entries under this key start with dashes."
-                        " Passing a dictionary does not allow duplicate keys and"
-                        " is sort-order-dependent.",
-                        MetadataWarning,
-                    )
-            metadata_map = {k: well_mapper.well_mapping(v) for k, v in metadata["metadata"].items()}
+        metadata_map = load_well_metadata(yaml_path)
     except FileNotFoundError as err:
         raise YamlError("Specified metadata YAML file does not exist!") from err
 
     # Load data from .csv files
     data_list: List[pd.DataFrame] = []
 
     for file in data_path.glob("*.csv"):
```

### Comparing `rushd-0.3.0/src/rushd/io.py` & `rushd-0.4.0/src/rushd/io.py`

 * *Files identical despite different names*

### Comparing `rushd-0.3.0/src/rushd/well_mapper.py` & `rushd-0.4.0/src/rushd/well_mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,13 +171,15 @@
                         ),
                     ):
                         # Add the non-normalized and normalized (leading zeros)
                         # versions. Adding an existing entry is a no-op, so no
                         # harm done.
                         wells.add(f"{itc_mapping[well[0]]}{well[1]}")
                         wells.add(f"{itc_mapping[well[0]]}{well[1]:02d}")
-            for well in wells:
-                if well not in output_mapping:
-                    output_mapping[well] = key
+            for parsed_well in wells:
+                if parsed_well not in output_mapping:
+                    output_mapping[parsed_well] = key
                 else:
-                    output_mapping[well] = str(output_mapping[well]) + separator + str(key)
+                    output_mapping[parsed_well] = (
+                        str(output_mapping[parsed_well]) + separator + str(key)
+                    )
     return output_mapping
```

### Comparing `rushd-0.3.0/src/rushd.egg-info/PKG-INFO` & `rushd-0.4.0/src/rushd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: rushd
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package for maintaining robust, reproducible data management.
 Home-page: https://github.com/GallowayLabMIT/rushd
 Author: Christopher Johnstone, Kasey Love, Conrad Oakes
 Author-email: meson800@gmail.com
 Project-URL: Bug Tracker, https://github.com/GallowayLabMIT/rushd/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # rushd
+[![Stable documentation](https://img.shields.io/badge/Documentation-stable-blue)](https://gallowaylabmit.github.io/rushd/en/main/)
 [![PyPI-downloads](https://img.shields.io/pypi/dm/rushd)](https://pypi.org/project/rushd)
 [![PyPI-version](https://img.shields.io/pypi/v/rushd)](https://pypi.org/project/rushd)
 [![PyPI-license](https://img.shields.io/pypi/l/rushd)](https://pypi.org/project/rushd)
 [![Supported python versions](https://img.shields.io/pypi/pyversions/rushd)](https://pypi.org/project/rushd)
 [![codecov](https://codecov.io/gh/GallowayLabMIT/rushd/branch/main/graph/badge.svg?token=ALaU8lQxt5)](https://codecov.io/gh/GallowayLabMIT/rushd)
 
 A package for maintaining robust, reproducible data management.
@@ -43,15 +45,16 @@
 
 ## Quickstart
 Simply import `rushd`!
 ```
 import rushd as rd
 ```
 
-## Complete Examples
+## Documentation
+See the documentation available at https://gallowaylabmit.github.io/rushd
 
 ## Developer install
 If you'd like to hack locally on `rushd`, after cloning this repository:
 ```
 $ git clone https://github.com/GallowayLabMIT/rushd.git
 $ cd rushd
 ```
@@ -65,20 +68,17 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
-## [0.3.0] - 2023-03-01
+## [0.4.0] - 2023-04-21
 ### Added
-- `rd.flow.load_groups_with_metadata` loads files from several folders (groups, e.g. corresponding to plates) into a single dataframe
-### Modified
-- `rd.flow.moi` properly generates plots of MOI vs fraction infected for checking calculation accuracy
-- `rd.well_mapper` properly handles metadata concatenation
+- `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
 
 ## What does the name mean?
 The name is a reference to [Ibn Rushd](https://en.wikipedia.org/wiki/Averroes), a Muslim scholar born in Córdoba who was responsible for translating and adding scholastic commentary to ancient Greek works, especially Aristotle. His translations spurred further translations into Latin and Hebrew, reigniting interest in ancient Greek works for the first time since the fall of the Roman empire.
```

### Comparing `rushd-0.3.0/tests/test_file_io.py` & `rushd-0.4.0/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `rushd-0.3.0/tests/test_file_moi.py` & `rushd-0.4.0/tests/test_file_moi.py`

 * *Files identical despite different names*

### Comparing `rushd-0.3.0/tests/test_flow.py` & `rushd-0.4.0/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `rushd-0.3.0/tests/test_pandas_cache.py` & `rushd-0.4.0/tests/test_pandas_cache.py`

 * *Files identical despite different names*

### Comparing `rushd-0.3.0/tests/test_well_mapper.py` & `rushd-0.4.0/tests/test_well_mapper.py`

 * *Files identical despite different names*

