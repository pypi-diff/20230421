# Comparing `tmp/amirispy-1.1.4.tar.gz` & `tmp/amirispy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amirispy-1.1.4.tar", last modified: Fri Feb 24 11:00:00 2023, max compression
+gzip compressed data, was "amirispy-1.2.tar", last modified: Fri Apr 21 13:24:36 2023, max compression
```

## Comparing `amirispy-1.1.4.tar` & `amirispy-1.2.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 11:00:00.699225 amirispy-1.1.4/
--rw-rw-rw-   0        0        0       42 2022-10-28 14:04:41.000000 amirispy-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6277 2023-02-24 11:00:00.699225 amirispy-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5707 2023-02-24 10:50:38.000000 amirispy-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-02-24 11:00:00.699225 amirispy-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1520 2023-02-24 10:51:57.000000 amirispy-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:00:00.652397 amirispy-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-02-24 11:00:00.652397 amirispy-1.1.4/src/amirispy/
--rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.1.4/src/amirispy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:00:00.668037 amirispy-1.1.4/src/amirispy/scripts/
--rw-rw-rw-   0        0        0      182 2022-11-04 09:40:34.000000 amirispy-1.1.4/src/amirispy/scripts/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-02-24 10:50:38.000000 amirispy-1.1.4/src/amirispy/scripts/amiris.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:00:00.668037 amirispy-1.1.4/src/amirispy/scripts/resources/
--rw-rw-rw-   0        0        0      331 2022-10-28 13:24:56.000000 amirispy-1.1.4/src/amirispy/scripts/resources/fameSetup.yaml
-drwxrwxrwx   0        0        0        0 2023-02-24 11:00:00.683585 amirispy-1.1.4/src/amirispy/scripts/subcommands/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:38:53.000000 amirispy-1.1.4/src/amirispy/scripts/subcommands/__init__.py
--rw-rw-rw-   0        0        0     1711 2022-11-04 09:43:46.000000 amirispy-1.1.4/src/amirispy/scripts/subcommands/compare.py
--rw-rw-rw-   0        0        0     5797 2023-02-24 10:50:38.000000 amirispy-1.1.4/src/amirispy/scripts/subcommands/install.py
--rw-rw-rw-   0        0        0     3007 2023-02-20 13:58:47.000000 amirispy-1.1.4/src/amirispy/scripts/subcommands/run.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:00:00.699225 amirispy-1.1.4/src/amirispy/source/
--rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.1.4/src/amirispy/source/__init__.py
--rw-rw-rw-   0        0        0     5079 2023-02-24 10:50:38.000000 amirispy-1.1.4/src/amirispy/source/cli.py
--rw-rw-rw-   0        0        0     5671 2022-11-04 09:43:46.000000 amirispy-1.1.4/src/amirispy/source/file_comparison.py
--rw-rw-rw-   0        0        0     2105 2023-02-08 15:01:04.000000 amirispy-1.1.4/src/amirispy/source/files.py
--rw-rw-rw-   0        0        0     2641 2023-02-07 15:32:49.000000 amirispy-1.1.4/src/amirispy/source/logs.py
--rw-rw-rw-   0        0        0      828 2023-02-07 15:47:53.000000 amirispy-1.1.4/src/amirispy/source/util.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:00:00.668037 amirispy-1.1.4/src/amirispy.egg-info/
--rw-rw-rw-   0        0        0     6277 2023-02-24 11:00:00.000000 amirispy-1.1.4/src/amirispy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-02-24 11:00:00.000000 amirispy-1.1.4/src/amirispy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 11:00:00.000000 amirispy-1.1.4/src/amirispy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-02-24 11:00:00.000000 amirispy-1.1.4/src/amirispy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-24 11:00:00.000000 amirispy-1.1.4/src/amirispy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-02-24 11:00:00.000000 amirispy-1.1.4/src/amirispy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-24 11:00:00.000000 amirispy-1.1.4/src/amirispy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.735850 amirispy-1.2/
+-rw-rw-rw-   0        0        0       42 2022-10-28 14:04:41.000000 amirispy-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7801 2023-04-21 13:24:36.735850 amirispy-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7212 2023-04-21 13:23:31.000000 amirispy-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 13:24:36.735850 amirispy-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1550 2023-04-21 13:23:31.000000 amirispy-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.691769 amirispy-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.698765 amirispy-1.2/src/amirispy/
+-rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.2/src/amirispy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.709765 amirispy-1.2/src/amirispy/scripts/
+-rw-rw-rw-   0        0        0      182 2022-11-04 09:40:34.000000 amirispy-1.2/src/amirispy/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2017 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/scripts/amiris.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.713765 amirispy-1.2/src/amirispy/scripts/resources/
+-rw-rw-rw-   0        0        0      331 2022-10-28 13:24:56.000000 amirispy-1.2/src/amirispy/scripts/resources/fameSetup.yaml
+drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.718764 amirispy-1.2/src/amirispy/scripts/subcommands/
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:38:53.000000 amirispy-1.2/src/amirispy/scripts/subcommands/__init__.py
+-rw-rw-rw-   0        0        0     4659 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/scripts/subcommands/batch.py
+-rw-rw-rw-   0        0        0     1711 2022-11-04 09:43:46.000000 amirispy-1.2/src/amirispy/scripts/subcommands/compare.py
+-rw-rw-rw-   0        0        0     5797 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/scripts/subcommands/install.py
+-rw-rw-rw-   0        0        0     1420 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/scripts/subcommands/run.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.734843 amirispy-1.2/src/amirispy/source/
+-rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.2/src/amirispy/source/__init__.py
+-rw-rw-rw-   0        0        0     6431 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/source/cli.py
+-rw-rw-rw-   0        0        0     4080 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/source/fameio_calls.py
+-rw-rw-rw-   0        0        0     5671 2022-11-04 09:43:46.000000 amirispy-1.2/src/amirispy/source/file_comparison.py
+-rw-rw-rw-   0        0        0     2103 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/source/files.py
+-rw-rw-rw-   0        0        0     2641 2023-02-07 15:32:49.000000 amirispy-1.2/src/amirispy/source/logs.py
+-rw-rw-rw-   0        0        0      828 2023-02-07 15:47:53.000000 amirispy-1.2/src/amirispy/source/util.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.706758 amirispy-1.2/src/amirispy.egg-info/
+-rw-rw-rw-   0        0        0     7801 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/top_level.txt
```

### Comparing `amirispy-1.1.4/PKG-INFO` & `amirispy-1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: amirispy
-Version: 1.1.4
-Summary: Python tools for the electricity market model AMIRIS
-Home-page: https://gitlab.com/dlr-ve/esy/amiris/amiris-py
-Author: Christoph Schimeczek, Felix Nitsch
-Author-email: amiris@dlr.de
-License: Apache License 2.0
-Keywords: AMIRIS,agent-based modelling
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 <!-- SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 
 [![PyPI version](https://badge.fury.io/py/amirispy.svg)](https://badge.fury.io/py/amirispy)
 [![PyPI license](https://img.shields.io/pypi/l/amirispy.svg)](https://badge.fury.io/py/amirispy)
 [![pipeline status](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/badges/main/pipeline.svg)](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/commits/main)
@@ -46,14 +30,15 @@
 
 
 ## Usage
 Currently, there are three distinct commands available:
 
 - `amiris install`: installation of the [latest AMIRIS version](https://gitlab.com/dlr-ve/esy/amiris/amiris) and [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) to your computer
 - `amiris run`: perform a full workflow by compiling the `.pb` file from your `scenario.yaml`, executing AMIRIS, and converting results
+- `amiris batch`: perform multiple runs each with scenario compilation, AMIRIS execution, and results extraction
 - `amiris comparison`: compare the results of two different AMIRIS runs to check them for their equivalence
 
 
 ### `amiris install`
 Downloads and installs the latest open access AMIRIS instance and accompanying examples.
 
 | Option               | Action                                                                                                                                                       |
@@ -66,30 +51,41 @@
 
 ### `amiris run`
 Compile scenario, execute AMIRIS, and extract results.
 
 | Option               | Action                                                    |
 |----------------------|-----------------------------------------------------------|
 | `-j` or `--jar`      | Path to `amiris-core_<version>-jar-with-dependencies.jar` |
-| `-s` or `--scenario` | Path to `scenario.yaml`                                   |
+| `-s` or `--scenario` | Path to a scenario yaml-file                              |
 | `-o` or `--output`   | Directory to write output to                              |
 
 
+### `amiris batch`
+Perform multiple runs - each with scenario compilation, AMIRIS execution, and results extraction
+
+| Option                | Action                                                                        |
+|-----------------------|-------------------------------------------------------------------------------|
+| `-j` or `--jar`       | Path to `amiris-core_<version>-jar-with-dependencies.jar`                     |
+| `-s` or `--scenarios` | Path to single or list of: scenario yaml-files or their enclosing directories |
+| `-o` or `--output`    | Directory to write output to                                                  |
+| `-r` or `--recursive` | Option to recursively search in provided Path for scenario (default: False)   |
+| `-p` or `--pattern`   | Optional name pattern that scenario files searched for must match             |
+
+
 ### `amiris compare`
 Compare if results of two AMIRIS runs and equivalent.
 
-| Option               | Action                                         |
-|----------------------|------------------------------------------------|
-| `-e` or `--expected` | Path to folder with expected results           |
-| `-t` or `--test`     | Path to folder with results to test            |
-| `-i` or `--ignore`   | Optional list of file names to not be compared |
+| Option               | Action                                                            |
+|----------------------|-------------------------------------------------------------------|
+| `-e` or `--expected` | Path to folder with expected result .csv files                    |
+| `-t` or `--test`     | Path to folder with results files (.csv) to test  for equivalence |
+| `-i` or `--ignore`   | Optional list of file names not to be compared                    |
 
 
 ### Help
-
 You reach the help menu at any point using `-h` or `--help` which gives you a list of all available options, e.g.:
 
 `amiris --help`
 
 
 ### Logging
 You may define a logging level or optional log file as **first** arguments in your workflow using any of the following arguments:
@@ -97,20 +93,22 @@
 | Option               | Action                                                                                                            |
 |----------------------|-------------------------------------------------------------------------------------------------------------------|
 | `-l` or `--log`      | Sets the logging level. Default is `error`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.  |
 | `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.        |
 
 Example: `amiris --log debug --logfile my/log/file.txt install`
 
+## Cite AMIRIS-Py
+If you use AMIRIS-Py for academic work, please cite:
+
+Christoph Schimeczek, Kristina Nienhaus, Ulrich Frey, Evelyn Sperber, Seyedfarzad Sarfarazi, Felix Nitsch, Johannes Kochems & A. Achraf El Ghazi (2023). AMIRIS: Agent-based Market model for the Investigation of Renewable and Integrated energy Systems. Journal of Open Source Software. doi: [10.21105/joss.05041](https://doi.org/10.21105/joss.05041)
 
 ## Contributing
 Please see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Available Support
 This is a purely scientific project by (at the moment) one research group. 
 Thus, there is no paid technical support available.
 
 If you experience any trouble with AMIRIS, you may contact the developers at the [openMod-Forum](https://forum.openmod.org/tag/amiris) or via [amiris@dlr.de](mailto:amiris@dlr.de).
 Please report bugs and make feature requests by filing issues following the provided templates (see also [CONTRIBUTING](CONTRIBUTING.md)).
 For substantial enhancements, we recommend that you contact us via [amiris@dlr.de](mailto:amiris@dlr.de) for working together on the code in common projects or towards common publications and thus further develop AMIRIS.
-
-
```

### Comparing `amirispy-1.1.4/README.md` & `amirispy-1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: amirispy
+Version: 1.2
+Summary: Python tools for the electricity market model AMIRIS
+Home-page: https://gitlab.com/dlr-ve/esy/amiris/amiris-py
+Author: Christoph Schimeczek, Felix Nitsch
+Author-email: amiris@dlr.de
+License: Apache License 2.0
+Keywords: AMIRIS,agent-based modelling
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 <!-- SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 
 [![PyPI version](https://badge.fury.io/py/amirispy.svg)](https://badge.fury.io/py/amirispy)
 [![PyPI license](https://img.shields.io/pypi/l/amirispy.svg)](https://badge.fury.io/py/amirispy)
 [![pipeline status](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/badges/main/pipeline.svg)](https://gitlab.com/dlr-ve/esy/amiris/amiris-py/commits/main)
@@ -30,14 +47,15 @@
 
 
 ## Usage
 Currently, there are three distinct commands available:
 
 - `amiris install`: installation of the [latest AMIRIS version](https://gitlab.com/dlr-ve/esy/amiris/amiris) and [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) to your computer
 - `amiris run`: perform a full workflow by compiling the `.pb` file from your `scenario.yaml`, executing AMIRIS, and converting results
+- `amiris batch`: perform multiple runs each with scenario compilation, AMIRIS execution, and results extraction
 - `amiris comparison`: compare the results of two different AMIRIS runs to check them for their equivalence
 
 
 ### `amiris install`
 Downloads and installs the latest open access AMIRIS instance and accompanying examples.
 
 | Option               | Action                                                                                                                                                       |
@@ -50,30 +68,41 @@
 
 ### `amiris run`
 Compile scenario, execute AMIRIS, and extract results.
 
 | Option               | Action                                                    |
 |----------------------|-----------------------------------------------------------|
 | `-j` or `--jar`      | Path to `amiris-core_<version>-jar-with-dependencies.jar` |
-| `-s` or `--scenario` | Path to `scenario.yaml`                                   |
+| `-s` or `--scenario` | Path to a scenario yaml-file                              |
 | `-o` or `--output`   | Directory to write output to                              |
 
 
+### `amiris batch`
+Perform multiple runs - each with scenario compilation, AMIRIS execution, and results extraction
+
+| Option                | Action                                                                        |
+|-----------------------|-------------------------------------------------------------------------------|
+| `-j` or `--jar`       | Path to `amiris-core_<version>-jar-with-dependencies.jar`                     |
+| `-s` or `--scenarios` | Path to single or list of: scenario yaml-files or their enclosing directories |
+| `-o` or `--output`    | Directory to write output to                                                  |
+| `-r` or `--recursive` | Option to recursively search in provided Path for scenario (default: False)   |
+| `-p` or `--pattern`   | Optional name pattern that scenario files searched for must match             |
+
+
 ### `amiris compare`
 Compare if results of two AMIRIS runs and equivalent.
 
-| Option               | Action                                         |
-|----------------------|------------------------------------------------|
-| `-e` or `--expected` | Path to folder with expected results           |
-| `-t` or `--test`     | Path to folder with results to test            |
-| `-i` or `--ignore`   | Optional list of file names to not be compared |
+| Option               | Action                                                            |
+|----------------------|-------------------------------------------------------------------|
+| `-e` or `--expected` | Path to folder with expected result .csv files                    |
+| `-t` or `--test`     | Path to folder with results files (.csv) to test  for equivalence |
+| `-i` or `--ignore`   | Optional list of file names not to be compared                    |
 
 
 ### Help
-
 You reach the help menu at any point using `-h` or `--help` which gives you a list of all available options, e.g.:
 
 `amiris --help`
 
 
 ### Logging
 You may define a logging level or optional log file as **first** arguments in your workflow using any of the following arguments:
@@ -81,18 +110,24 @@
 | Option               | Action                                                                                                            |
 |----------------------|-------------------------------------------------------------------------------------------------------------------|
 | `-l` or `--log`      | Sets the logging level. Default is `error`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.  |
 | `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.        |
 
 Example: `amiris --log debug --logfile my/log/file.txt install`
 
+## Cite AMIRIS-Py
+If you use AMIRIS-Py for academic work, please cite:
+
+Christoph Schimeczek, Kristina Nienhaus, Ulrich Frey, Evelyn Sperber, Seyedfarzad Sarfarazi, Felix Nitsch, Johannes Kochems & A. Achraf El Ghazi (2023). AMIRIS: Agent-based Market model for the Investigation of Renewable and Integrated energy Systems. Journal of Open Source Software. doi: [10.21105/joss.05041](https://doi.org/10.21105/joss.05041)
 
 ## Contributing
 Please see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Available Support
 This is a purely scientific project by (at the moment) one research group. 
 Thus, there is no paid technical support available.
 
 If you experience any trouble with AMIRIS, you may contact the developers at the [openMod-Forum](https://forum.openmod.org/tag/amiris) or via [amiris@dlr.de](mailto:amiris@dlr.de).
 Please report bugs and make feature requests by filing issues following the provided templates (see also [CONTRIBUTING](CONTRIBUTING.md)).
 For substantial enhancements, we recommend that you contact us via [amiris@dlr.de](mailto:amiris@dlr.de) for working together on the code in common projects or towards common publications and thus further develop AMIRIS.
+
+
```

### Comparing `amirispy-1.1.4/setup.py` & `amirispy-1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from setuptools import find_packages, setup
 
 __author__ = [
-    "Christoph Schimeczek", # noqa
-    "Felix Nitsch", # noqa
+    "Christoph Schimeczek",  # noqa
+    "Felix Nitsch",  # noqa
 ]
 __copyright__ = "Copyright 2022, German Aerospace Center (DLR)"
 
 __license__ = "Apache License 2.0"
 __maintainer__ = "Christoph Schimeczek"  # noqa
 __email__ = "amiris@dlr.de"
 __status__ = "Production"
@@ -20,36 +20,35 @@
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
-    name="amirispy", # noqa
-    version="1.1.4",
+    name="amirispy",  # noqa
+    version="1.2",
     description="Python tools for the electricity market model AMIRIS",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["AMIRIS", "agent-based modelling"],
     url="https://gitlab.com/dlr-ve/esy/amiris/amiris-py",
     author=", ".join(__author__),
     author_email=__email__,
     license=__license__,
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     entry_points={
         "console_scripts": [
-            "amiris=amirispy.scripts:amiris", # noqa
+            "amiris=amirispy.scripts:amiris",  # noqa
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    install_requires=[
-        "pandas", "wget", "fameio>=1.6.1"
-    ],
+    install_requires=["pandas", "wget", "fameio>=1.8"],
+    extras_require={"dev": ["pytest>=7.2"]},
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
 )
```

### Comparing `amirispy-1.1.4/src/amirispy/scripts/amiris.py` & `amirispy-1.2/src/amirispy/scripts/amiris.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,37 +4,50 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import logging as log
 
 from amirispy.scripts.subcommands.compare import compare_results
 from amirispy.scripts.subcommands.run import run_amiris
+from amirispy.scripts.subcommands.batch import batch_run_amiris
 from amirispy.scripts.subcommands.install import install_amiris
-from amirispy.source.cli import arg_handling_run, Command, CompareOptions, InstallOptions, RunOptions, GeneralOptions
+from amirispy.source.cli import (
+    arg_handling_run,
+    Command,
+    CompareOptions,
+    InstallOptions,
+    RunOptions,
+    BatchOptions,
+    GeneralOptions,
+)
 from amirispy.source.logs import set_up_logger, log_and_print
 
 
 def amiris_cli() -> None:
     """Calls sub-commands with appropriate arguments as returned by the command line parser"""
 
     command, options = arg_handling_run()
     set_up_logger(options[GeneralOptions.LOG], options[GeneralOptions.LOGFILE])
     if command is Command.INSTALL:
-        log.info("Starting install script")
+        log_and_print("Starting install script")
         install_amiris(
             options[InstallOptions.URL],
             options[InstallOptions.TARGET],
             options[InstallOptions.FORCE],
             options[InstallOptions.MODE],
         )
         log_and_print(f"Installation setup to '{options[InstallOptions.TARGET]}' complete")
     elif command is Command.RUN:
-        log.info("Start running AMIRIS")
+        log_and_print("Start running AMIRIS")
         run_amiris(options)
         log_and_print(f"Successfully executed AMIRIS. See your results in '{options[RunOptions.OUTPUT]}'")
+    elif command is Command.BATCH:
+        log_and_print("Start running AMIRIS batch run")
+        batch_run_amiris(options)
+        log_and_print(f"Successfully executed AMIRIS. See your results in '{options[BatchOptions.OUTPUT]}'")
     elif command is Command.COMPARE:
-        log.info("Starting comparison script")
+        log_and_print("Starting comparison script")
         compare_results(options[CompareOptions.EXPECTED], options[CompareOptions.TEST], options[CompareOptions.IGNORE])
 
 
 if __name__ == "__main__":
     amiris_cli()
```

### Comparing `amirispy-1.1.4/src/amirispy/scripts/subcommands/compare.py` & `amirispy-1.2/src/amirispy/scripts/subcommands/compare.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.1.4/src/amirispy/scripts/subcommands/install.py` & `amirispy-1.2/src/amirispy/scripts/subcommands/install.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.1.4/src/amirispy/scripts/subcommands/run.py` & `amirispy-1.2/src/amirispy/source/fameio_calls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,118 @@
 # SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import logging as log
-import os
 import subprocess
 from pathlib import Path
+from typing import Dict
 
-from fameio.scripts import make_config, convert_results
-from fameio.source.cli import Options, ResolveOptions
+from fameio.scripts.convert_results import run as convert_results
+from fameio.scripts.make_config import run as make_config
+from fameio.source.cli import Options, ResolveOptions, MergingOptions
 
-from amirispy.source.cli import GeneralOptions, RunOptions
+from amirispy.source.cli import BatchOptions, GeneralOptions, RunOptions
 from amirispy.source.files import ensure_folder_exists, check_if_write_access
-from amirispy.source.logs import log_error_and_raise
-from amirispy.source.util import check_java_installation
 
-_ERR_NOT_A_FILE = "Specified Path '{}' does not point to an existing file."
 
+def determine_all_paths(
+    scenario_yaml: Path, working_directory: Path, options: Dict, batch: bool = False
+) -> Dict[str, Path]:
+    """
+    Determines all Paths for the given scenario file and working directory
+
+    Args:
+        scenario_yaml: path to the scenario file
+        working_directory: the base working directory
+        options: amiris-py command line options
+        batch: bool which is True when to determine paths for batch runs (default: False)
 
-def run_amiris(options: dict) -> None:
+    Returns:
+        Dictionary containing all Paths to final results and temporary files
     """
-    Compile scenario to protobuf using fameio.scripts.make_config,
-    execute AMIRIS,
-    and extract results using fameio.scripts.convert_results
+    paths = {
+        "SCENARIO_FILE": scenario_yaml if scenario_yaml.is_absolute() else working_directory.joinpath(scenario_yaml),
+        "SCENARIO_DIRECTORY": scenario_yaml.parent,
+        "BASE_NAME": scenario_yaml.stem,
+        "INPUT_PB": working_directory.joinpath("input.pb"),
+        "OUTPUT_PB": working_directory.joinpath("output.pb"),
+    }
+
+    jar_option = BatchOptions.JAR if batch else RunOptions.JAR
+    output_option = BatchOptions.OUTPUT if batch else RunOptions.OUTPUT
+    paths.update(
+        {
+            "JAR_FILE": options[jar_option],
+            "SETUP_FILE": Path(options[jar_option].parents[0], "fameSetup.yaml"),
+            "RESULT_FOLDER": Path(options[output_option], scenario_yaml.stem),
+        }
+    )
+
+    return paths
+
+
+def compile_input(options: dict, paths: Dict[str, Path]) -> None:
+    """
+    Creates protobuf file using given `options` and `paths`
 
     Args:
-        options:
-            RunOptions.JAR: Path to amiris-core_<version>-jar-with-dependencies.jar
-            RunOptions.SCENARIO: Path to scenario.yaml
-            RunOptions.OUTPUT: Directory to write output to
-            GeneralOptions.LOG: Logging level gathered by CLI
-            GeneralOptions.LOGFILE: Path to log_file gathered by CLI
+        options: for logging
+        paths: to given input and output files
 
     Returns:
         None
     """
-    check_java_installation(raise_exception=True)
-    origin_wd = Path.cwd()
-
     fameio_input_config = {
         Options.LOG_LEVEL: options[GeneralOptions.LOG],
         Options.LOG_FILE: options[GeneralOptions.LOGFILE],
-        Options.OUTPUT: f"{origin_wd}/input.pb",
+        Options.OUTPUT: paths["INPUT_PB"],
     }
+    log.info("Creating binary protobuf input file: `{protobuf_file_path}` from scenario `{scenario_file}`")
+    make_config(paths["SCENARIO_FILE"].resolve(), fameio_input_config)
 
-    path_to_scenario: Path = options[RunOptions.SCENARIO]
-    if not path_to_scenario.is_file():
-        log_error_and_raise(ValueError(_ERR_NOT_A_FILE.format(path_to_scenario)))
-    scenario_wd = path_to_scenario.parents[0]
-
-    check_if_write_access(origin_wd)
-    os.chdir(scenario_wd)
-    log.info("Converting binary protobuf file")
-    make_config(path_to_scenario.name, fameio_input_config)
-    os.chdir(origin_wd)
-
-    path_to_jar = options[RunOptions.JAR]
-    jar_wd = path_to_jar.parents[0]
-    fame_setup_path = Path(jar_wd, "fameSetup.yaml")
 
-    input_pb = fameio_input_config[Options.OUTPUT]
+def call_amiris(paths: Dict[str, Path]) -> None:
+    """
+    Run AMIRIS using given paths
 
-    call = 'java -jar "{}" -f "{}" -s "{}"'.format(path_to_jar, input_pb, fame_setup_path)
-    log.info("Starting AMIRIS")
+    Args:
+        paths: to all required files
+
+    Returns:
+        None
+    """
+    call = 'java -jar "{}" -f "{}" -s "{}"'.format(paths["JAR_FILE"], paths["INPUT_PB"], paths["SETUP_FILE"])
+    log.info(f"Calling AMIRIS with {paths['SCENARIO_FILE']}")
     subprocess.run(call, shell=True, check=True)
 
-    output_folder = options[RunOptions.OUTPUT]
+
+def compile_output(options: Dict, paths: Dict[str, Path]) -> None:
+    """
+    Conducts to conversion of AMIRIS output to CSV files based on given options and paths
+
+    Args:
+        options: for logging
+        paths: to given input and output files
+
+    Returns:
+        None
+    """
     fameio_output_config = {
         Options.LOG_LEVEL: options[GeneralOptions.LOG],
         Options.LOG_FILE: options[GeneralOptions.LOGFILE],
         Options.AGENT_LIST: None,
-        Options.OUTPUT: output_folder,
+        Options.OUTPUT: paths["RESULT_FOLDER"],
         Options.SINGLE_AGENT_EXPORT: False,
         Options.MEMORY_SAVING: False,
         Options.RESOLVE_COMPLEX_FIELD: ResolveOptions.SPLIT,
+        Options.TIME_MERGING: {
+            MergingOptions.FOCAL_POINT: 0,
+            MergingOptions.STEPS_BEFORE: 1800,
+            MergingOptions.STEPS_AFTER: 1799,
+        },
     }
 
-    path_to_amiris_pb_result = "output.pb"
-    ensure_folder_exists(output_folder)
-    check_if_write_access(output_folder)
+    ensure_folder_exists(paths["RESULT_FOLDER"])
+    check_if_write_access(paths["RESULT_FOLDER"])
     log.info("Converting protobuf to csv files")
-    convert_results(path_to_amiris_pb_result, fameio_output_config)
+    convert_results(paths["OUTPUT_PB"].resolve(), fameio_output_config)
```

### Comparing `amirispy-1.1.4/src/amirispy/source/cli.py` & `amirispy-1.2/src/amirispy/source/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,23 @@
 INSTALL_HELP = "Downloads and installs latest open access AMIRIS instance"
 INSTALL_URL_MODEL_HELP = "URL to download AMIRIS model from (default: latest AMIRIS artifact)"
 INSTALL_TARGET_HELP = "Folder to install 'amiris-core_<version>-jar-with-dependencies.jar' to (default: './')"
 INSTALL_FORCE_HELP = "Force install to overwrite existing AMIRIS installation and/or examples (default: False)"
 INSTALL_MODE_HELP = "Choose to install model and examples `all` (default), only `model`, or only `examples`"
 RUN_HELP = "Compile scenario, execute AMIRIS, and extract results"
 RUN_JAR_HELP = "Path to 'amiris-core_<version>-jar-with-dependencies.jar'"
-RUN_SCENARIO_HELP = "Path to 'scenario.yaml'"
+RUN_SCENARIO_HELP = "Path to a scenario yaml-file"
 RUN_OUTPUT_HELP = "Directory to write output to"
+BATCH_HELP = (
+    "Batch mode to perform multiple runs each with scenario compilation, AMIRIS execution, and results extraction"
+)
+BATCH_SCENARIO_HELP = "Path to single or list of: scenario yaml-files or their enclosing directories"
+BATCH_RECURSIVE_HELP = "Option to recursively search in provided Path for scenario (default: False)"
+DEFAULT_PATTERN = "*.y*ml"
+BATCH_PATTERN_HELP = f"Optional name pattern that scenario files searched for must match (default: '{DEFAULT_PATTERN}')"
 COMPARE_HELP = "Compare if results of two AMIRIS runs and equivalent"
 COMPARE_EXPECTED_HELP = "Path to folder with expected results"
 COMPARE_TEST_HELP = "Path to folder with results to test"
 COMPARE_IGNORE_HELP = "Optional list of file names to not be compared"
 URL_LATEST_AMIRIS = "https://gitlab.com/dlr-ve/esy/amiris/amiris/-/jobs/artifacts/main/download?job=deploy:jdk8"
 
 
@@ -39,14 +46,15 @@
 
 class Command(Enum):
     """Specifies command to execute"""
 
     RUN = auto()
     INSTALL = auto()
     COMPARE = auto()
+    BATCH = auto()
 
 
 class CompareOptions(Enum):
     """Options for command `compare`"""
 
     EXPECTED = auto()
     TEST = auto()
@@ -66,15 +74,30 @@
     """Options for command `run`"""
 
     JAR = auto()
     SCENARIO = auto()
     OUTPUT = auto()
 
 
-Options = {Command.COMPARE: CompareOptions, Command.RUN: RunOptions, Command.INSTALL: InstallOptions}
+class BatchOptions(Enum):
+    """Options for command `batch`"""
+
+    JAR = auto()
+    SCENARIOS = auto()
+    OUTPUT = auto()
+    RECURSIVE = auto()
+    PATTERN = auto()
+
+
+Options = {
+    Command.COMPARE: CompareOptions,
+    Command.RUN: RunOptions,
+    Command.INSTALL: InstallOptions,
+    Command.BATCH: BatchOptions,
+}
 
 
 def arg_handling_run() -> Tuple[Command, Dict[Enum, Any]]:
     """Handles command line arguments for `amiris` and returns `command` and its options `args`"""
 
     parent_parser = argparse.ArgumentParser(prog="amiris", description=AMIRIS_PARSER)
     parent_parser.add_argument("-lf", "--logfile", type=Path, required=False, help=AMIRIS_LOG_FILE_HELP)
@@ -100,14 +123,21 @@
         help=INSTALL_MODE_HELP,
     )
     run_parser = subparsers.add_parser("run", help=RUN_HELP)
     run_parser.add_argument("--jar", "-j", type=Path, required=True, help=RUN_JAR_HELP)
     run_parser.add_argument("--scenario", "-s", type=Path, required=True, help=RUN_SCENARIO_HELP)
     run_parser.add_argument("--output", "-o", type=Path, default=Path("./"), help=RUN_OUTPUT_HELP)
 
+    batch_parser = subparsers.add_parser("batch", help=BATCH_HELP)
+    batch_parser.add_argument("--jar", "-j", type=Path, required=True, help=RUN_JAR_HELP)
+    batch_parser.add_argument("--scenarios", "-s", nargs="+", type=Path, required=True, help=BATCH_SCENARIO_HELP)
+    batch_parser.add_argument("--output", "-o", type=Path, default=Path("./"), help=RUN_OUTPUT_HELP)
+    batch_parser.add_argument("--recursive", "-r", default=False, action="store_true", help=BATCH_RECURSIVE_HELP)
+    batch_parser.add_argument("--pattern", "-p", type=str, default=DEFAULT_PATTERN, help=BATCH_PATTERN_HELP)
+
     compare_parser = subparsers.add_parser("compare", help=COMPARE_HELP)
     compare_parser.add_argument("--expected", "-e", type=Path, required=True, help=COMPARE_EXPECTED_HELP)
     compare_parser.add_argument("--test", "-t", type=Path, required=True, help=COMPARE_TEST_HELP)
     compare_parser.add_argument("--ignore", "-i", required=False, help=COMPARE_IGNORE_HELP)
 
     args = vars(parent_parser.parse_args())
```

### Comparing `amirispy-1.1.4/src/amirispy/source/file_comparison.py` & `amirispy-1.2/src/amirispy/source/file_comparison.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.1.4/src/amirispy/source/files.py` & `amirispy-1.2/src/amirispy/source/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         None
 
     Raises:
         ValueError: if path is an existing file
     """
     if path.is_file():
         log_error_and_raise(ValueError(_ERR_NOT_A_FOLDER.format(path)))
-
     if not path.is_dir():
         path.mkdir(parents=True)
 
 
 def check_if_write_access(path: Path) -> None:
     """Raises Error if no writing access to `path`"""
     if not os.access(path, os.W_OK):
```

### Comparing `amirispy-1.1.4/src/amirispy/source/logs.py` & `amirispy-1.2/src/amirispy/source/logs.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.1.4/src/amirispy/source/util.py` & `amirispy-1.2/src/amirispy/source/util.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.1.4/src/amirispy.egg-info/PKG-INFO` & `amirispy-1.2/src/amirispy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: amirispy
-Version: 1.1.4
+Version: 1.2
 Summary: Python tools for the electricity market model AMIRIS
 Home-page: https://gitlab.com/dlr-ve/esy/amiris/amiris-py
 Author: Christoph Schimeczek, Felix Nitsch
 Author-email: amiris@dlr.de
 License: Apache License 2.0
 Keywords: AMIRIS,agent-based modelling
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 <!-- SPDX-FileCopyrightText: 2022 German Aerospace Center <amiris@dlr.de>
 
 SPDX-License-Identifier: Apache-2.0 -->
 
 [![PyPI version](https://badge.fury.io/py/amirispy.svg)](https://badge.fury.io/py/amirispy)
 [![PyPI license](https://img.shields.io/pypi/l/amirispy.svg)](https://badge.fury.io/py/amirispy)
@@ -46,14 +47,15 @@
 
 
 ## Usage
 Currently, there are three distinct commands available:
 
 - `amiris install`: installation of the [latest AMIRIS version](https://gitlab.com/dlr-ve/esy/amiris/amiris) and [examples](https://gitlab.com/dlr-ve/esy/amiris/examples) to your computer
 - `amiris run`: perform a full workflow by compiling the `.pb` file from your `scenario.yaml`, executing AMIRIS, and converting results
+- `amiris batch`: perform multiple runs each with scenario compilation, AMIRIS execution, and results extraction
 - `amiris comparison`: compare the results of two different AMIRIS runs to check them for their equivalence
 
 
 ### `amiris install`
 Downloads and installs the latest open access AMIRIS instance and accompanying examples.
 
 | Option               | Action                                                                                                                                                       |
@@ -66,30 +68,41 @@
 
 ### `amiris run`
 Compile scenario, execute AMIRIS, and extract results.
 
 | Option               | Action                                                    |
 |----------------------|-----------------------------------------------------------|
 | `-j` or `--jar`      | Path to `amiris-core_<version>-jar-with-dependencies.jar` |
-| `-s` or `--scenario` | Path to `scenario.yaml`                                   |
+| `-s` or `--scenario` | Path to a scenario yaml-file                              |
 | `-o` or `--output`   | Directory to write output to                              |
 
 
+### `amiris batch`
+Perform multiple runs - each with scenario compilation, AMIRIS execution, and results extraction
+
+| Option                | Action                                                                        |
+|-----------------------|-------------------------------------------------------------------------------|
+| `-j` or `--jar`       | Path to `amiris-core_<version>-jar-with-dependencies.jar`                     |
+| `-s` or `--scenarios` | Path to single or list of: scenario yaml-files or their enclosing directories |
+| `-o` or `--output`    | Directory to write output to                                                  |
+| `-r` or `--recursive` | Option to recursively search in provided Path for scenario (default: False)   |
+| `-p` or `--pattern`   | Optional name pattern that scenario files searched for must match             |
+
+
 ### `amiris compare`
 Compare if results of two AMIRIS runs and equivalent.
 
-| Option               | Action                                         |
-|----------------------|------------------------------------------------|
-| `-e` or `--expected` | Path to folder with expected results           |
-| `-t` or `--test`     | Path to folder with results to test            |
-| `-i` or `--ignore`   | Optional list of file names to not be compared |
+| Option               | Action                                                            |
+|----------------------|-------------------------------------------------------------------|
+| `-e` or `--expected` | Path to folder with expected result .csv files                    |
+| `-t` or `--test`     | Path to folder with results files (.csv) to test  for equivalence |
+| `-i` or `--ignore`   | Optional list of file names not to be compared                    |
 
 
 ### Help
-
 You reach the help menu at any point using `-h` or `--help` which gives you a list of all available options, e.g.:
 
 `amiris --help`
 
 
 ### Logging
 You may define a logging level or optional log file as **first** arguments in your workflow using any of the following arguments:
@@ -97,14 +110,18 @@
 | Option               | Action                                                                                                            |
 |----------------------|-------------------------------------------------------------------------------------------------------------------|
 | `-l` or `--log`      | Sets the logging level. Default is `error`. Options are `debug`, `info`, `warning`, `warn`, `error`, `critical`.  |
 | `-lf` or `--logfile` | Sets the logging file. Default is `None`. If `None` is provided, all logs get only printed to the console.        |
 
 Example: `amiris --log debug --logfile my/log/file.txt install`
 
+## Cite AMIRIS-Py
+If you use AMIRIS-Py for academic work, please cite:
+
+Christoph Schimeczek, Kristina Nienhaus, Ulrich Frey, Evelyn Sperber, Seyedfarzad Sarfarazi, Felix Nitsch, Johannes Kochems & A. Achraf El Ghazi (2023). AMIRIS: Agent-based Market model for the Investigation of Renewable and Integrated energy Systems. Journal of Open Source Software. doi: [10.21105/joss.05041](https://doi.org/10.21105/joss.05041)
 
 ## Contributing
 Please see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Available Support
 This is a purely scientific project by (at the moment) one research group. 
 Thus, there is no paid technical support available.
```

### Comparing `amirispy-1.1.4/src/amirispy.egg-info/SOURCES.txt` & `amirispy-1.2/src/amirispy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 src/amirispy.egg-info/not-zip-safe
 src/amirispy.egg-info/requires.txt
 src/amirispy.egg-info/top_level.txt
 src/amirispy/scripts/__init__.py
 src/amirispy/scripts/amiris.py
 src/amirispy/scripts/resources/fameSetup.yaml
 src/amirispy/scripts/subcommands/__init__.py
+src/amirispy/scripts/subcommands/batch.py
 src/amirispy/scripts/subcommands/compare.py
 src/amirispy/scripts/subcommands/install.py
 src/amirispy/scripts/subcommands/run.py
 src/amirispy/source/__init__.py
 src/amirispy/source/cli.py
+src/amirispy/source/fameio_calls.py
 src/amirispy/source/file_comparison.py
 src/amirispy/source/files.py
 src/amirispy/source/logs.py
 src/amirispy/source/util.py
```

