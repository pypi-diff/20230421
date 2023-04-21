# Comparing `tmp/era5cli-1.3.2.tar.gz` & `tmp/era5cli-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/era5cli/era5cli/dist/.tmp-43fa3l0z/era5cli-1.3.2.tar", last modified: Tue Dec 13 14:32:53 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `era5cli-1.3.2.tar` & `era5cli-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-13 14:32:53.000000 era5cli-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (116)     3075 2022-12-13 14:32:37.000000 era5cli-1.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2694 2022-12-13 14:32:37.000000 era5cli-1.3.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (116)    11359 2022-12-13 14:32:37.000000 era5cli-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       84 2022-12-13 14:32:37.000000 era5cli-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3288 2022-12-13 14:32:53.000000 era5cli-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2017 2022-12-13 14:32:37.000000 era5cli-1.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-13 14:32:53.000000 era5cli-1.3.2/era5cli/
--rw-r--r--   0 runner    (1001) docker     (116)       61 2022-12-13 14:32:37.000000 era5cli-1.3.2/era5cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      693 2022-12-13 14:32:37.000000 era5cli-1.3.2/era5cli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15349 2022-12-13 14:32:37.000000 era5cli-1.3.2/era5cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    17443 2022-12-13 14:32:37.000000 era5cli-1.3.2/era5cli/fetch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2352 2022-12-13 14:32:37.000000 era5cli-1.3.2/era5cli/info.py
--rw-r--r--   0 runner    (1001) docker     (116)    15178 2022-12-13 14:32:37.000000 era5cli-1.3.2/era5cli/inputref.py
--rw-r--r--   0 runner    (1001) docker     (116)     5537 2022-12-13 14:32:37.000000 era5cli-1.3.2/era5cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-13 14:32:53.000000 era5cli-1.3.2/era5cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3288 2022-12-13 14:32:53.000000 era5cli-1.3.2/era5cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      414 2022-12-13 14:32:53.000000 era5cli-1.3.2/era5cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-13 14:32:53.000000 era5cli-1.3.2/era5cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       45 2022-12-13 14:32:53.000000 era5cli-1.3.2/era5cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       36 2022-12-13 14:32:53.000000 era5cli-1.3.2/era5cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2022-12-13 14:32:53.000000 era5cli-1.3.2/era5cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      173 2022-12-13 14:32:37.000000 era5cli-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       39 2022-12-13 14:32:37.000000 era5cli-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-13 14:32:53.000000 era5cli-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1748 2022-12-13 14:32:37.000000 era5cli-1.3.2/setup.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 era5cli-1.4.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 era5cli-1.4.0/CITATION.cff
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 era5cli-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 era5cli-1.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 era5cli-1.4.0/readthedocs.yml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/.codecov.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/workflows/cffconvert.yml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/workflows/test_and_build.yml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 era5cli-1.4.0/.github/workflows/test_codecov.yml
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/contribute.md
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/development_era5cli.md
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/formulating_requests.md
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/gen_reference_pages.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/general_development.md
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/getting_started.md
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/hourly_monthly.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/index.md
+-rw-r--r--   0        0        0   107756 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/assets/era5cli_favicon.png
+-rw-r--r--   0        0        0    96539 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/assets/era5cli_logo_colors.png
+-rw-r--r--   0        0        0   135504 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/assets/era5cli_logo_colors_border.png
+-rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/assets/era5cli_logo_white.svg
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/reference/arguments.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/reference/cli_usage.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/reference/variables.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 era5cli-1.4.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/__version__.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/_request_size.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/cli.py
+-rw-r--r--   0        0        0    21049 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/fetch.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/info.py
+-rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/inputref.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/key_management.py
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/utils.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/__init__.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/common.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/config.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/info.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 era5cli-1.4.0/era5cli/args/periods.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     9834 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_config.py
+-rw-r--r--   0        0        0    21778 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_fetch.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_info.py
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_integration.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 era5cli-1.4.0/tests/test_version.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 era5cli-1.4.0/.gitignore
+-rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 era5cli-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 era5cli-1.4.0/README.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 era5cli-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 era5cli-1.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `era5cli-1.3.2/CITATION.cff` & `era5cli-1.4.0/CITATION.cff`

 * *Files 5% similar despite different names*

```diff
@@ -78,18 +78,23 @@
     given-names: Stefan
     orcid: https://orcid.org/0000-0002-5821-2060
   -
     affiliation: "Environment and Climate Change Canada"
     family-names: Malinina
     given-names: Elizaveta
     orcid: https://orcid.org/0000-0002-4102-2877
+  -
+    affiliation: "Netherlands eScience Center"
+    family-names: Schilperoort
+    given-names: Bart
+    orcid: https://orcid.org/0000-0003-4487-9822
 
 cff-version: 1.2.0
 date-released: 2022-12-13
 doi: 10.5281/zenodo.3252665
 keywords:
   - "ERA5"
 license: Apache-2.0
 message: "If you use this software, please cite it using these metadata."
 repository-code: "https://github.com/ewatercycle/era5cli"
 title: era5cli
-version: 1.3.2
+version: "1.4.0"
```

### Comparing `era5cli-1.3.2/LICENSE` & `era5cli-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `era5cli-1.3.2/README.rst` & `era5cli-1.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,33 @@
-era5cli
-=======
-.. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
-    :target: https://opensource.org/licenses/Apache-2.0
-    :alt: License
+<img align="right" width="150" alt="Logo" src="docs/assets/era5cli_logo_colors_border.png">
 
-.. image:: https://readthedocs.org/projects/era5cli/badge/?version=latest
-    :target: https://era5cli.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
 
-.. image:: https://github.com/eWaterCycle/era5cli/actions/workflows/test_codecov.yml/badge.svg
-   :target: https://github.com/eWaterCycle/era5cli/actions/workflows/test_codecov.yml
-   :alt: Github Actions
+[![github license badge](https://img.shields.io/github/license/eWaterCycle/era5cli)](https://github.com/eWaterCycle/era5cli)
+[![rsd badge](https://img.shields.io/badge/RSD-era5cli-blue)](https://research-software-directory.org/software/era5cli)
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3252665.svg)](https://doi.org/10.5281/zenodo.3252665)
 
-.. image:: https://codecov.io/gh/eWaterCycle/era5cli/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/eWaterCycle/era5cli
-   :alt: Test coverage
+[![Documentation Status](https://readthedocs.org/projects/era5cli/badge/?version=stable)](https://lilio.readthedocs.io/en/stable/?badge=stable)
+[![build](https://github.com/eWaterCycle/era5cli/actions/workflows/test_and_build.yml/badge.svg)](https://github.com/eWaterCycle/era5cli/actions/workflows/test_and_build.yml)
+[![Test Coverage](https://codecov.io/gh/eWaterCycle/era5cli/branch/main/graph/badge.svg?token=qeZXgGASBK)](https://codecov.io/gh/eWaterCycle/era5cli)
+[![PyPI](https://badge.fury.io/py/era5cli.svg)](https://badge.fury.io/py/era5cli)
 
-.. image:: https://badge.fury.io/py/era5cli.svg
-    :target: https://badge.fury.io/py/era5cli
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3252665.svg
-   :target: https://doi.org/10.5281/zenodo.3252665
+A command line interface to download ERA5 data from the [Copernicus Climate Data Store](<https://climate.copernicus.eu/>).
 
-.. image:: https://img.shields.io/badge/rsd-era5cli-00a3e3.svg
-   :target: https://www.research-software.nl/software/era5cli
-   :alt: Research Software Directory Badge
+<hr>
 
-.. image:: https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow
-   :target: https://fair-software.eu
+With `era5cli` you can:
 
-.. inclusion-marker-start-do-not-remove
+ - Download meteorological data in GRIB/NetCDF, including ERA5 data from the preliminary back extension, and ERA5-Land data.
+ - List and retrieve information on available variables and pressure levels
+ - Select multiple variables for several months and years
+ - Split outputs by years (and optionally months), producing a separate files instead of merging them in one file
+ - Download multiple files at once
+ - Extract data for a sub-region of the globe
 
-A command line interface to download ERA5 data from the `Copernicus Climate Data Store <https://climate.copernicus.eu/>`_.
+<hr>
 
-With era5cli you can:
+Free software: Apache Software License 2.0
 
-- download meteorological data in GRIB/NetCDF, including ERA5 data from the preliminary back extension, and ERA5-Land data.
-- list and retrieve information on available variables and pressure levels
-- select multiple variables for several months and years
-- split outputs by years, producing a separate file for every year instead of merging them in one file
-- download multiple files at once
-- extract data for a sub-region of the globe
+Documentation: https://era5cli.readthedocs.io
 
-.. inclusion-marker-end-do-not-remove
-
-| Free software: Apache Software License 2.0
-| Documentation: https://era5cli.readthedocs.io
```

### Comparing `era5cli-1.3.2/era5cli/fetch.py` & `era5cli-1.4.0/era5cli/fetch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Fetch ERA5 variables."""
 
-import os
+import itertools
 import logging
-
+import os
 import cdsapi
 from pathos.threading import ThreadPool as Pool
-
 import era5cli.inputref as ref
 import era5cli.utils
+from era5cli import key_management
+from era5cli._request_size import TooLargeRequestError
+from era5cli._request_size import request_too_large
 
 
 class Fetch:
     """Fetch ERA5 data using cdsapi.
 
     Parameters
     ----------
@@ -73,45 +75,63 @@
         dryrun: bool
             Whether to print the cdsapi request to the screen,
             or make the request to start downloading the data.
             `dryrun = True` will print the request to stdout. By default,
             the data will be downloaded.
         prelimbe: bool
             Whether to download the preliminary back extension (1950-1978).
-            Note that in this case, `years` nust be between 1950 and
+            Note that in this case, `years` must be between 1950 and
             1978. `prelimbe = True` is incompatible with `land = True`.
         land: bool
             Whether to download data from the ERA5-Land dataset.
             Note that the ERA5-Land dataset starts in 1981.
             `land = True` is incompatible with the use of
             `prelimbe = True` and `ensemble = True`.
+        overwrite: bool
+            Whether to overwrite existing files or not.
+            Setting `overwrite = True` will make
+            era5cli overwrite existing files. By default,
+            you will be prompted if a file already exists, with
+            the question if you want to overwrite it or not.
+        dashed_vars: bool
+            Whether to use dashed variable names in the output
+            files, or the normal names ('temperature-of-snow-layer'
+            instead of 'temperature_of_snow_layer').
     """
-    def __init__(self,
-                 years: list,
-                 months: list,
-                 days: list,
-                 hours: list,
-                 variables: list,
-                 outputformat: str,
-                 outputprefix: str,
-                 period: str,
-                 ensemble: bool,
-                 area=None,
-                 statistics=None,
-                 synoptic=None,
-                 pressurelevels=None,
-                 merge=False,
-                 threads=None,
-                 prelimbe=False,
-                 land=False):
+
+    def __init__(
+        self,
+        years: list,
+        months: list,
+        days: list,
+        hours: list,
+        variables: list,
+        outputformat: str,
+        outputprefix: str,
+        period: str,
+        ensemble: bool,
+        area=None,
+        statistics=None,
+        synoptic=None,
+        pressurelevels=None,
+        splitmonths=False,
+        merge=False,
+        threads=None,
+        prelimbe=False,
+        land=False,
+        overwrite=False,
+        dashed_vars=False,
+    ):
         """Initialization of Fetch class."""
+        self._get_login()  # Get login info from config file.
+
         self.months = era5cli.utils._zpad_months(months)
         """list(str): List of zero-padded strings of months
         (e.g. ['01', '02',..., '12'])."""
-        if period == 'monthly':
+        if period == "monthly":
             self.days = None
         else:
             self.days = era5cli.utils._zpad_days(days)
             """list(str): List of zero-padded strings of days
             (e.g. ['01', '02',..., '31'])."""
 
         self.hours = era5cli.utils._format_hours(hours)
@@ -129,14 +149,16 @@
         """str: File format of output file."""
         self.years = years
         """list(int): List of years."""
         self.outputprefix = outputprefix
         """str: Prefix of output filename."""
         self.threads = threads
         """int: number of parallel threads to use for downloading."""
+        self.splitmonths = splitmonths
+        """bool: Split request per month, can avoid Too Large Request error."""
         self.merge = merge
         """bool: Merge yearly output files if True."""
         self.period = period
         """str: Frequency of output data (monthly or daily)."""
         self.ensemble = ensemble
         """bool: Whether to download high resolution realisation
         (HRES) or a reduced resolution ten member ensemble
@@ -152,14 +174,54 @@
         (synoptic=False)."""
         self.prelimbe = prelimbe
         """bool: Whether to select from the ERA5 preliminary back
         extension which supports years from 1950 to 1978"""
         self.land = land
         """bool: Whether to download from the ERA5-Land
         dataset."""
+        self.overwrite = overwrite
+        """bool: Whether to overwrite existing files."""
+        self.dashed_vars = dashed_vars
+        """bool: Whether to use dashed variable names in the output
+        files, or the normal names."""
+
+        if self.merge and self.splitmonths:
+            raise ValueError(
+                "\nThe commands '--merge' and '--splitmonths' are not compatible with"
+                "\neach other. Please pick one of the two."
+            )
+
+        if self.prelimbe:
+            logging.warning(
+                "\n  The years of the ERA5 preliminary back extension (1950 - 1978) are"
+                "\n  now included in the main ERA5 products. The `--prelimbe` argument"
+                "\n  will be deprecated in a future release."
+                "\n  Please update your workflow accordingly."
+            )
+
+        vars = list(self.variables)  # Use list() to avoid copying by reference
+        if "geopotential" in vars and pressurelevels == ["surface"]:
+            vars.remove("geopotential")
+        if any([var in ref.PLVARS for var in vars]):
+            print(pressurelevels)
+            self._check_levels()
+
+        if self.period == "hourly" and request_too_large(self):
+            raise TooLargeRequestError(
+                "\n  Your request is too large for the CDS API."
+                "\n  Consider splitting up your request in months, "
+                "\n  by using '--splitmonths True'."
+                "\n  For more info see 'era5cli hourly --help'."
+            )
+
+    def _get_login(self):
+        # First check if the config exists, and guide the user if it does not.
+        key_management.check_era5cli_config()
+        # Only then load the keys (as they should be there now).
+        self.url, self.key = key_management.load_era5cli_config()
 
     def fetch(self, dryrun=False):
         """Split calls and fetch results.
 
         Parameters
         ----------
         dryrun: bool
@@ -167,98 +229,127 @@
             files will be downloaded. For a dryrun the cdsapi request will
             be written to stdout.
         """
         self.dryrun = dryrun
         # define extension output filename
         self._extension()
         # define fetch call depending on split argument
-        if not self.merge:
-            # split by variable and year
+
+        if self.splitmonths:
+            self._split_variable_yr_month()
+        elif not self.merge:
             self._split_variable_yr()
         else:
-            # split by variable
             self._split_variable()
 
     def _extension(self):
         """Set filename extension."""
-        if self.outputformat.lower() == 'netcdf':
+        if self.outputformat.lower() == "netcdf":
             self.ext = "nc"
-        elif self.outputformat.lower() == 'grib':
-            self.ext = 'grb'
+        elif self.outputformat.lower() == "grib":
+            self.ext = "grb"
         else:
-            raise ValueError('Unknown outputformat: {}'.format(
-                self.outputformat))
+            raise ValueError(f"Unknown outputformat: {self.outputformat}")
 
     def _process_areaname(self):
         (lat_max, lon_min, lat_min, lon_max) = [round(c) for c in self.area]
 
         def lon(x):
             return f"{x}E" if x >= 0 else f"{abs(x)}W"
 
         def lat(y):
             return f"{y}N" if y >= 0 else f"{abs(y)}S"
 
         name = f"_{lon(lon_min)}-{lon(lon_max)}_{lat(lat_min)}-{lat(lat_max)}"
         return name
 
-    def _define_outputfilename(self, var, years):
+    def _define_outputfilename(self, var, years, month=None):
         """Define output filename."""
         start, end = years[0], years[-1]
 
-        prefix = (f"{self.outputprefix}-land"
-                  if self.land else self.outputprefix)
-        yearblock = f"{start}-{end}" if not start == end else f"{start}"
-        fname = f"{prefix}_{var}_{yearblock}_{self.period}"
+        prefix = f"{self.outputprefix}-land" if self.land else self.outputprefix
+
+        yearblock = f"{start}-{end}" if start != end else f"{start}"
+
+        varname = var.replace("_", "-") if self.dashed_vars else var
+
+        fname = f"{prefix}_{varname}_{yearblock}"
+
+        if month is not None:
+            fname += f"-{month}"
+        fname += f"_{self.period}"
+
         if self.area:
             fname += self._process_areaname()
         if self.ensemble:
             fname += "_ensemble"
         if self.statistics:
             fname += "_statistics"
         if self.synoptic:
             fname += "_synoptic"
         fname += f".{self.ext}"
         return fname
 
     def _split_variable(self):
         """Split by variable."""
         outputfiles = [
-            self._define_outputfilename(var, self.years)
-            for var in self.variables
+            self._define_outputfilename(var, self.years) for var in self.variables
         ]
+        if not self.overwrite:
+            era5cli.utils.assert_outputfiles_not_exist(outputfiles)
+
         years = len(outputfiles) * [self.years]
-        if not self.threads:
-            pool = Pool()
-        else:
-            pool = Pool(nodes=self.threads)
+
+        pool = Pool(nodes=self.threads) if self.threads else Pool()
         pool.map(self._getdata, self.variables, years, outputfiles)
 
     def _split_variable_yr(self):
         """Fetch variable split by variable and year."""
         outputfiles = []
         variables = []
         for var in self.variables:
-            outputfiles += ([
-                self._define_outputfilename(var, [yr]) for yr in self.years
-            ])
+            outputfiles += [self._define_outputfilename(var, [yr]) for yr in self.years]
             variables += len(self.years) * [var]
+
+        if not self.overwrite:
+            era5cli.utils.assert_outputfiles_not_exist(outputfiles)
+
         years = len(self.variables) * self.years
-        if not self.threads:
-            pool = Pool()
-        else:
-            pool = Pool(nodes=self.threads)
+
+        pool = Pool(nodes=self.threads) if self.threads else Pool()
         pool.map(self._getdata, variables, years, outputfiles)
 
+    def _split_variable_yr_month(self):
+        """Fetch variable split by variable, year, and month."""
+        outputfiles = []
+        variables = []
+        years = []
+        months = []
+
+        for var, year, month in itertools.product(
+            self.variables, self.years, self.months
+        ):
+            outputfiles += [self._define_outputfilename(var, [year, year], month)]
+            variables += [var]
+            years += [year]
+            months += [month]
+
+        if not self.overwrite:
+            era5cli.utils.assert_outputfiles_not_exist(outputfiles)
+
+        pool = Pool(nodes=self.threads) if self.threads else Pool()
+        pool.map(self._getdata, variables, years, outputfiles, months)
+
     def _product_type(self):
         """Construct the product type name from the options."""
-        assert not (self.land and self.ensemble), (
-                'ERA5-Land does not contain Ensemble statistics.'
-            )
+        assert not (
+            self.land and self.ensemble
+        ), "ERA5-Land does not contain Ensemble statistics."
 
-        if self.period == 'hourly' and self.ensemble and self.statistics:
+        if self.period == "hourly" and self.ensemble and self.statistics:
             # The only configuration to return a list
             return [
                 "ensemble_members",
                 "ensemble_mean",
                 "ensemble_spread",
             ]
 
@@ -294,128 +385,138 @@
         return producttype
 
     def _check_levels(self):
         """Retrieve pressure level info for request"""
         if not self.pressure_levels:
             raise ValueError(
                 "Requested 3D variable(s), but no pressure levels specified."
-                "Aborting.")
+                "Aborting."
+            )
         if not all(level in ref.PLEVELS for level in self.pressure_levels):
             raise ValueError(
-                f"Invalid pressure levels. Allowed values are: {ref.PLEVELS}")
+                f"Invalid pressure levels. Allowed values are: {ref.PLEVELS}"
+            )
 
     def _check_variable(self, variable):
         """Check variable available and compatible with other inputs."""
         # if land then the variable must be in era5 land
         if self.land:
             if variable not in ref.ERA5_LAND_VARS:
                 raise ValueError(
                     f"Variable {variable} is not available in ERA5-Land.\n"
-                    f"Choose from {ref.ERA5_LAND_VARS}")
+                    f"Choose from {ref.ERA5_LAND_VARS}"
+                )
         elif variable in ref.PLVARS + ref.SLVARS:
-            if self.period == "monthly":
-                if variable in ref.MISSING_MONTHLY_VARS:
-                    header = ("There is no monthly data available for the "
-                              "following variables:\n")
-                    raise ValueError(
-                        era5cli.utils._print_multicolumn(
-                            header, ref.MISSING_MONTHLY_VARS))
+            if self.period == "monthly" and variable in ref.MISSING_MONTHLY_VARS:
+                header = (
+                    "There is no monthly data available for the "
+                    "following variables:\n"
+                )
+                raise ValueError(
+                    era5cli.utils.print_multicolumn(header, ref.MISSING_MONTHLY_VARS)
+                )
         else:
-            raise ValueError("Invalid variable name: {}".format(variable))
+            raise ValueError(f"Invalid variable name: {variable}")
 
     def _check_area(self):
         """Confirm that area parameters are correct."""
         (lat_max, lon_min, lat_min, lon_max) = self.area
-        if not (-90 <= lat_max <= 90 and -90 <= lat_min <= 90
-                and -180 <= lon_min <= 180 and -180 <= lon_max <= 180
-                and lat_max > lat_min and lon_max != lon_min):
+        if not (
+            -90 <= lat_max <= 90
+            and -90 <= lat_min <= 90
+            and -180 <= lon_min <= 180
+            and -180 <= lon_max <= 180
+            and lat_max > lat_min
+            and lon_max != lon_min
+        ):
             raise ValueError(
                 "Provide coordinates as lat_max lon_min lat_min lon_max. "
                 "Latitude must be in range -180,+180 and "
-                "longitude must be in range -90,+90.")
+                "longitude must be in range -90,+90."
+            )
 
     def _parse_area(self):
         """Parse area parameters to accepted coordinates."""
         self._check_area()
         area = [round(coord, ndigits=2) for coord in self.area]
         if self.area != area:
-            print(
-                f"NB: coordinates {self.area} rounded down to two decimals.\n")
+            print(f"NB: coordinates {self.area} rounded down to two decimals.\n")
         return area
 
     def _build_name(self, variable):
         """Build up name of dataset to use"""
 
         name = "reanalysis-era5"
 
         # report to user in case of ambiguous vars
         if (variable in ref.PLVARS) and (variable in ref.SLVARS):
             instruction_pressure = (
                 "Getting variable from pressure level data. To get the "
                 "surface variable instead, add `--levels surface` or "
-                "`levels=['surface']` to the request.\n")
+                "`levels=['surface']` to the request.\n"
+            )
             instruction_surface = (
                 "Getting variable from surface level data. To get the "
                 "pressure variable instead, omit `--levels surface` or "
-                "`levels=['surface']` from the request.\n")
+                "`levels=['surface']` from the request.\n"
+            )
             if self.pressure_levels == ["surface"]:
                 instruction = instruction_surface
             else:
                 instruction = instruction_pressure
-            logging.warning(f"The variable name '{variable}' is ambiguous. "
-                            f"{instruction}")
+            logging.warning(
+                f"The variable name '{variable}' is ambiguous. {instruction}"
+            )
 
         if self.land:
             name += "-land"
-        # workaround for deprecated variable 'orography'
         elif variable == "orography":
             variable = "geopotential"
             name += "-single-levels"
             logging.warning(
-                "The variable 'orography' has been deprecated by CDS. Use "
-                "`--variables geopotential --levels surface` going forward. "
-                "The current query has been changed accordingly.")
+                "\n  The variable 'orography' has been deprecated by CDS. Use"
+                "\n  `--variables geopotential --levels surface` going forward."
+                "\n  The current query has been changed accordingly."
+            )
         elif self.pressure_levels == ["surface"]:
             name += "-single-levels"
-        # the order of the following conditions is important!
-        # please do not switch them
         elif variable in ref.PLVARS:
             name += "-pressure-levels"
         elif variable in ref.SLVARS:
             name += "-single-levels"
         else:
-            raise ValueError("Invalid variable name: {}".format(variable))
+            raise ValueError(f"Invalid variable name: {variable}")
 
         if self.period == "monthly":
             name += "-monthly-means"
 
         if self.prelimbe:
             if self.land:
                 raise ValueError(
                     "Back extension not available for ERA5-Land. "
-                    "ERA5-Land data is available from 1950 on.")
+                    "ERA5-Land data is available from 1950 on."
+                )
             name += "-preliminary-back-extension"
         return name, variable
 
-    def _build_request(self, variable, years):
+    def _build_request(self, variable, years, months=None):
         """Build the download request for the retrieve method of cdsapi."""
         self._check_variable(variable)
 
         name, variable = self._build_name(variable)
 
         request = {
-            'variable': variable,
-            'year': years,
-            'month': self.months,
-            'time': self.hours,
-            'format': self.outputformat
+            "variable": variable,
+            "year": years,
+            "month": self.months if months is None else months,
+            "time": self.hours,
+            "format": self.outputformat,
         }
 
         if "pressure-levels" in name:
-            self._check_levels()
             request["pressure_level"] = self.pressure_levels
 
         if self.area:
             request["area"] = self._parse_area()
 
         product_type = self._product_type()
         if product_type is not None:
@@ -425,22 +526,26 @@
             request["day"] = self.days
 
         return (name, request)
 
     def _exit(self):
         pass
 
-    def _getdata(self, variables: list, years: list, outputfile: str):
+    def _getdata(self, variables: list, years: list, outputfile: str, months=None):
         """Fetch variables using cds api call."""
-        name, request = self._build_request(variables, years)
+        name, request = self._build_request(variables, years, months)
+
         if self.dryrun:
             print(name, request, outputfile)
         else:
             queueing_message = (
-                os.linesep, "Download request is being queued at Copernicus.",
+                os.linesep,
+                "Download request is being queued at Copernicus.",
                 os.linesep,
                 "It can take some time before downloading starts, ",
-                "please do not kill this process in the meantime.", os.linesep)
-            connection = cdsapi.Client()
+                "please do not kill this process in the meantime.",
+                os.linesep,
+            )
+            connection = cdsapi.Client(url=self.url, key=self.key, verify=True)
             print("".join(queueing_message))  # print queueing message
             connection.retrieve(name, request, outputfile)
-            era5cli.utils._append_history(name, request, outputfile)
+            era5cli.utils.append_history(name, request, outputfile)
```

### Comparing `era5cli-1.3.2/era5cli/info.py` & `era5cli-1.4.0/era5cli/info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Print ERA5 information on available variables and levels."""
 
 import era5cli.inputref as ref
-from era5cli.utils import _print_multicolumn
+from era5cli.utils import print_multicolumn
 
 
 class Info:
     """Print ERA5 information on available variables and levels.
 
     Parameters
     ----------
@@ -34,35 +34,35 @@
             self.infotype = "list"
         except KeyError:
             self.infotype = []
             for valname, vallist in ref.REFDICT.items():
                 if self.infoname in vallist:
                     self.infotype.append(valname)
         if len(self.infotype) == 0:
-            raise ValueError('Unknown value for reference argument.')
+            raise ValueError("Unknown value for reference argument.")
 
     def list(self):
         """Print a list of available variables or pressure levels.
 
         Prints a list of available variables or pressure levels. The output is
         printed in multiple columns if the size of the terminal supports it.
         """
         self._define_table_header()
-        _print_multicolumn(self.header, self.infolist)
+        print_multicolumn(self.header, self.infolist)
 
     def vars(self):
         """Return the  variable name or pressure level.
 
         Print in which list the given variable occurs.
         """
-        lists = ', '.join(self.infotype)
-        print("{} is in the list(s): {}".format(self.infoname, lists))
+        lists = ", ".join(self.infotype)
+        print(f"{self.infoname} is in the list(s): {lists}")
 
     def _define_table_header(self):
         """Define table header."""
         hdict = {
-            'levels': 'pressure levels',
-            '2Dvars': '2D variables',
-            '3Dvars': '3D variables',
-            'land': 'ERA5-land variables'
+            "levels": "pressure levels",
+            "2Dvars": "2D variables",
+            "3Dvars": "3D variables",
+            "land": "ERA5-land variables",
         }
-        self.header = "Available {}:".format(hdict[self.infoname])
+        self.header = f"Available {hdict[self.infoname]}:"
```

### Comparing `era5cli-1.3.2/era5cli/utils.py` & `era5cli-1.4.0/era5cli/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Utility functions."""
 
+import datetime
 import shutil
+import textwrap
+from pathlib import Path
+from typing import List
 import prettytable
 from netCDF4 import Dataset
-from pathlib import Path
-import datetime
-import textwrap
-
 import era5cli
 from era5cli.__version__ import __version__ as era5cliversion
 
 
 def _zpadlist(values: list, inputtype: str, minval: int, maxval: int) -> list:
     """Return a list of zero padded strings and perform input checks.
 
@@ -37,18 +37,16 @@
     Raises
     ------
     AssertionError
         If any value in the list is not within `minval<=value<=maxval`.
     """
     returnlist = []
     for value in values:
-        assert (int(value) >= minval), (
-            'invalid value specified for {}: {}'.format(inputtype, value))
-        assert (int(value) <= maxval), (
-            'invalid value specified for {}: {}'.format(inputtype, value))
+        assert int(value) >= minval, f"invalid value specified for {inputtype}: {value}"
+        assert int(value) <= maxval, f"invalid value specified for {inputtype}: {value}"
         returnlist += [str(int(value)).zfill(2)]
     return returnlist
 
 
 def _zpad_days(values: list) -> list:
     """Return a list of zero padded strings.
 
@@ -62,15 +60,15 @@
         List of month numbers (1-31).
 
     Returns
     -------
     list(str)
         List of zero-padded strings of months (e.g. ['01', '02',..., '31']).
     """
-    return _zpadlist(values, 'days', 1, 31)
+    return _zpadlist(values, "days", 1, 31)
 
 
 def _zpad_months(values: list) -> list:
     """Return a list of zero padded strings.
 
     Returns a list of zero padded strings of month numbers from a list of
     input months. Invalid month numbers (e.g. outside of 1-12) will raise
@@ -82,15 +80,15 @@
         List of month numbers (1-12).
 
     Returns
     -------
     list(str)
         List of zero-padded strings of months (e.g. ['01', '02',..., '12']).
     """
-    return _zpadlist(values, 'months', 1, 12)
+    return _zpadlist(values, "months", 1, 12)
 
 
 def _format_hours(values: list) -> list:
     """Return a list of xx:00 formated time strings.
 
     Returns a list xx:00 formated time strings from a list of input hours.
     Invalid iput hours (e.g. outside of 0-23) will raise an exception.
@@ -104,69 +102,66 @@
     -------
     list(str)
         List of xx:00 formatted time strings (e.g. ['00:00', '01:00', ...,
         '23:00']).
     """
     returnlist = []
     for value in values:
-        assert (int(value) >= 0), (
-            'invalid value specified for hours: {}'.format(value))
-        assert (int(value) <= 23), (
-            'invalid value specified for hours: {}'.format(value))
-        returnlist += ["{}:00".format(str(value).zfill(2))]
+        assert int(value) >= 0, f"invalid value specified for hours: {value}"
+        assert int(value) <= 23, f"invalid value specified for hours: {value}"
+        returnlist += [f"{str(value).zfill(2)}:00"]
     return returnlist
 
 
-def _print_multicolumn(header: str, info: list):
+def print_multicolumn(header: str, info: list):
     """Print a list of strings in several columns.
 
     Parameters
     ----------
     header: str
         Table header string.
     info: list()
         Data to be printed.
     """
     # get size of terminal window
-    columns, rows = shutil.get_terminal_size(fallback=(80, 24))
+    columns, _ = shutil.get_terminal_size(fallback=(80, 24))
     # maximum width of string in list
-    maxwidth = max([len(str(x)) for x in info])
+    maxwidth = max(len(str(x)) for x in info)
     # calculate number of columns that fit on screen
     ncols = columns // (maxwidth + 2)
     # calculate number of rows
-    nrows = - ((-len(info)) // ncols)
+    nrows = -((-len(info)) // ncols)
     # the number of columns may be reducible for that many rows.
-    ncols = - ((-len(info)) // nrows)
+    ncols = -((-len(info)) // nrows)
     table = prettytable.PrettyTable([str(x) for x in range(ncols)])
     table.title = header
     table.header = False
-    table.align = 'l'
+    table.align = "l"
     table.hrules = prettytable.NONE
     table.vrules = prettytable.NONE
-    chunks = [info[i:i + nrows] for i in
-              range(0, len(info), nrows)]
-    chunks[-1].extend('' for i in range(nrows - len(chunks[-1])))
+    chunks = [info[i : i + nrows] for i in range(0, len(info), nrows)]
+    chunks[-1].extend("" for _ in range(nrows - len(chunks[-1])))
     chunks = zip(*chunks)
     for chunk in chunks:
         table.add_row(chunk)
     print(table)
 
 
-def _append_history(name, request, fname):
+def append_history(name, request, fname):
     """Append era5cli version information.
 
     Parameters
     ----------
     fname: str
         Filename.
     """
     dtime = datetime.datetime.now(tz=datetime.timezone.utc).strftime(
-        "%Y-%m-%d %H:%M:%S %Z")
-    appendtxt = "{} by {} {}: {} {}".format(dtime, era5cli.__name__,
-                                            era5cliversion, name, request)
+        "%Y-%m-%d %H:%M:%S %Z"
+    )
+    appendtxt = f"{dtime} by {era5cli.__name__} {era5cliversion}: {name} {request}"
     extension = Path(fname).suffix
     if extension == ".nc":
         _append_netcdf_history(fname, appendtxt)
 
 
 def _append_netcdf_history(ncfile: str, appendtxt: str):
     """Append era5cli version and download command to netCDF history.
@@ -175,15 +170,55 @@
     ----------
     ncfile: str
         Filename of netCDF file.
     appendtxt: str
         Text to append to history of netCDF file.
     """
     # open netCDF file rw and append to history
-    ncfile = Dataset(ncfile, 'r+')
+    ncfile = Dataset(ncfile, "r+")
     try:
-        ncfile.history = textwrap.dedent('''\
-            {}
-            {}'''.format(appendtxt, ncfile.history))
+        ncfile.history = textwrap.dedent(
+            f"""\
+            {appendtxt}
+            {ncfile.history}"""
+        )
     except AttributeError:
         ncfile.history = appendtxt
     ncfile.close()
+
+
+def strtobool(value: str) -> bool:
+    """Convert a string to a boolean. Required to have a true/false arg in argparse.
+
+    For example: `--flag True` or `--flag False`.
+
+    Functions the same as:
+    https://github.com/pypa/distutils/blob/4435cec31b8eb5712aa8bf993bea3f07051c24d8/distutils/util.py#L340-L353
+    However, distutils will be deprecated in future Python versions.
+    """
+    trues = ["true", "t", "yes", "y", "1"]
+    falses = ["false", "f", "no", "n", "0"]
+
+    if value.lower() in trues:
+        return True
+    if value.lower() in falses:
+        return False
+    raise ValueError(
+        "Could not convert string to boolean. Valid inputs are:"
+        f"{trues} and {falses} (case insensitive)."
+    )
+
+
+def assert_outputfiles_not_exist(outputfiles: List[str]) -> None:
+    """Check if files already exist, and prompt the user if they do."""
+    if any(Path(file).exists() for file in outputfiles):
+        answer = input(
+            "\n  Some file(s) that will be downloaded already exist in this folder."
+            "\n  Do you want to overwrite them? (Y/N)"
+            "\n  Tip: to skip this flag, use `--overwrite`."
+            "\n"
+        )
+        if answer.lower() in ["n", "no", "nope"]:
+            raise FileExistsError(
+                "\n  One or more files already exist in this folder."
+                "\n  Please remove them, or change to a different folder to continue"
+            )
```

