# Comparing `tmp/lilio-0.3.1.tar.gz` & `tmp/lilio-0.4.0.tar.gz`

## Comparing `lilio-0.3.1.tar` & `lilio-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,59 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 lilio-0.3.1/.bumpversion.cfg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lilio-0.3.1/.editorconfig
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 lilio-0.3.1/.mlc-config.json
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 lilio-0.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 lilio-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 lilio-0.3.1/CITATION.cff
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/Makefile
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/README.dev.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/changelog_link.rst
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/conf.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/index.rst
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/make.bat
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/project_setup.md
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/readme_link.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/_templates/.gitignore
--rw-r--r--   0        0        0   138815 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/assets/images/ai4s2s_logo.png
--rw-r--r--   0        0        0   327414 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/assets/images/calendar_concept.png
--rw-r--r--   0        0        0   766637 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/assets/images/lilio_logo.png
--rw-r--r--   0        0        0    14674 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/notebooks/all_about_the_calendar.ipynb
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/notebooks/calendar_shorthands.ipynb
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/notebooks/tutorial_calendar_shifter.ipynb
--rw-r--r--   0        0        0     8643 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/notebooks/tutorial_resampling_data.ipynb
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 lilio-0.3.1/docs/notebooks/tutorial_traintest.ipynb
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/__init__.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/_bokeh_plots.py
--rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/_plot.py
--rw-r--r--   0        0        0    25075 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/calendar.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/calendar_shifter.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/calendar_shorthands.py
--rw-r--r--   0        0        0    13582 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/resampling.py
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/traintest.py
--rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 lilio-0.3.1/lilio/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilio-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0    16880 2020-02-02 00:00:00.000000 lilio-0.3.1/tests/test_calendar.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 lilio-0.3.1/tests/test_calendar_shifter.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 lilio-0.3.1/tests/test_plots.py
--rw-r--r--   0        0        0    13433 2020-02-02 00:00:00.000000 lilio-0.3.1/tests/test_resample.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 lilio-0.3.1/tests/test_traintest.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 lilio-0.3.1/.gitignore
--rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 lilio-0.3.1/LICENSE
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 lilio-0.3.1/README.md
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 lilio-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 lilio-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 lilio-0.4.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lilio-0.4.0/.editorconfig
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 lilio-0.4.0/.flake8
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 lilio-0.4.0/.howfairis.yml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 lilio-0.4.0/.mlc-config.json
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 lilio-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 lilio-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 lilio-0.4.0/CITATION.cff
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/README.dev.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/changelog_link.rst
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/conf.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/dask_integration.md
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/index.rst
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/project_setup.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/readme_link.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/_templates/.gitignore
+-rw-r--r--   0        0        0   138815 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/ai4s2s_logo.png
+-rw-r--r--   0        0        0   327414 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/calendar_concept.png
+-rw-r--r--   0        0        0    35523 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/dask_client_example.png
+-rw-r--r--   0        0        0   192258 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/lilio_logo.png
+-rw-r--r--   0        0        0   766637 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/lilio_logo_highres.png
+-rw-r--r--   0        0        0   118768 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/lilio_logo_no_text.svg
+-rw-r--r--   0        0        0   120438 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/lilio_logo_square.svg
+-rw-r--r--   0        0        0   258644 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/lilio_logo_wide.png
+-rw-r--r--   0        0        0   120116 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/assets/images/lilio_logo_wide.svg
+-rw-r--r--   0        0        0    15401 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/notebooks/all_about_the_calendar.ipynb
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/notebooks/calendar_shorthands.ipynb
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/notebooks/tutorial_calendar_shifter.ipynb
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/notebooks/tutorial_resampling_data.ipynb
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 lilio-0.4.0/docs/notebooks/tutorial_traintest.ipynb
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/__init__.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/_attrs.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/_bokeh_plots.py
+-rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/_plot.py
+-rw-r--r--   0        0        0    25315 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/calendar.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/calendar_shifter.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/calendar_shorthands.py
+-rw-r--r--   0        0        0    13756 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/resampling.py
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/traintest.py
+-rw-r--r--   0        0        0    12280 2020-02-02 00:00:00.000000 lilio-0.4.0/lilio/utils.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0    16880 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_calendar.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_calendar_shifter.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_plots.py
+-rw-r--r--   0        0        0    15891 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_resample.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_traintest.py
+-rw-r--r--   0        0        0   395496 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_data/era5_dummy_2000.nc
+-rw-r--r--   0        0        0   459445 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_data/era5_dummy_2001.nc
+-rw-r--r--   0        0        0   459445 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_data/era5_dummy_2002.nc
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 lilio-0.4.0/tests/test_data/generate_test_data.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 lilio-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11359 2020-02-02 00:00:00.000000 lilio-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 lilio-0.4.0/README.md
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 lilio-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 lilio-0.4.0/PKG-INFO
```

### Comparing `lilio-0.3.1/.bumpversion.cfg` & `lilio-0.4.0/.bumpversion.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.1
+current_version = 0.4.0
 
 [comment]
 comment = The contents of this file cannot be merged with that of pyproject.toml until https://github.com/c4urself/bump2version/issues/42 is resolved
 
 [bumpversion:file:lilio/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `lilio-0.3.1/.mlc-config.json` & `lilio-0.4.0/.mlc-config.json`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/CHANGELOG.md` & `lilio-0.4.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
 ## [Unreleased]
 
+## 0.4.0 (2023-04-21)
+### Changed
+- Bokeh >= 3.0.0 is now required for interactive plotting, instead of <= 2.4.3.
+  - Do note that dask.distributed still requires bokeh < 3.
+
+### Added
+- Lilio's resample now supports use of dask. A tutorial on how to make use of this has been added to the documentation ([#52](https://github.com/AI4S2S/lilio/pull/52)).
+- When resampling xarray data, information such as the lilio version, calendar anchor date, the exact calendar, etc. are now added to the attributes, as well as descriptions and full names for anchor_year, i_interval, and is_target ([#49](https://github.com/AI4S2S/lilio/pull/49))
+
 ## 0.3.1 (2023-02-15)
 
 ### Changed
 - `lilio.resample` will now return `xr.DataArray` if the input is `xr.DataArray`.
 - For compatibility with DataArray output, the Dataset/DataArray returned by resample now has the coordinates "left_bound" and "right_bound" instead of a single "intervals" coordinate with the "bounds" dimension.
 - If your input data has an frequency of less than _twice_ the Calendar's smallest interval length, a UserWarning will be raised.
 - If your input data has a frequency less than the Calendar's smallest interval length, a ValueError will be raised.
```

### Comparing `lilio-0.3.1/CITATION.cff` & `lilio-0.4.0/CITATION.cff`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   - 
     family-names: Alidoost
     given-names: Fakhereh
     orcid: "https://orcid.org/0000-0001-8407-6472"
     affiliation: "Netherlands eScience Center"
 
 date-released: 2022-09-02
-version: "0.3.1"
+version: "0.4.0"
 repository-code: "https://github.com/AI4S2S/lilio"
 keywords:
   - calendar
   - calendar generation
   - calendar maker
   - machine learning
   - timeseries analysis
```

### Comparing `lilio-0.3.1/docs/CODE_OF_CONDUCT.md` & `lilio-0.4.0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/CONTRIBUTING.md` & `lilio-0.4.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/Makefile` & `lilio-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/README.dev.md` & `lilio-0.4.0/docs/README.dev.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # `lilio` developer documentation
 
 If you're looking for user documentation, go [here](readme_link.rst).
 
 ## Development install
+For a full development enviroment run the commands below.
+
+*Note that this is optional:* if you already have `hatch` in your main environment, this setup is not needed, as you can use the `hatch` environments to run all commands.
 
 ```shell
 # Create a virtual environment, e.g. with
 python3 -m venv env_name
 
 # activate virtual environment
 source env_name/bin/activate
@@ -23,15 +26,15 @@
 python3 -m pip install --no-cache-dir --editable .[dev]
 ```
 
 Afterwards check that the install directory is present in the `PATH` environment variable.
 
 ## Running the tests
 
-Running tests has been configured using `hatch`, and can be started by running:
+Lilio uses `pytest` for unit testing. Running tests has been configured using `hatch`, and can be started by running:
 
 ```shell
 hatch run test
 ```
 
 In addition to just running the tests to see if they pass, they can be used for coverage statistics, i.e. to determine how much of the package's code is actually executed during tests.
 Inside the package directory, run:
@@ -40,15 +43,15 @@
 hatch run coverage
 ```
 
 This runs tests and prints the results to the command line, as well as storing the result in a `coverage.xml` file (for analysis by, e.g. SonarCloud).
 
 ## Running linters locally
 
-For linting and code style we use `flake8`, `black` and `isort`. We additionally use `mypy` to check the type hints.
+For linting and code style we use `ruff`, `black` and `isort`. We additionally use `mypy` to check the type hints.
 All tools can simply be run by doing:
 
 ```shell
 hatch run lint
 ```
 
 To easily comply with `black` and `isort`, you can also run:
@@ -64,68 +67,46 @@
 
 ```shell
 hatch run docs:build
 ```
 
 The documentation will be in `docs/_build/html`.
 
+You can also make use of the [sphinx-autobuild](https://pypi.org/project/sphinx-autobuild/) plugin to show a live preview of the documentation, which can make developing the documentation a bit easier.
+
 ## Versioning
 
 Bumping the version across all files is done with [bumpversion](https://github.com/c4urself/bump2version), e.g.
 
 ```shell
 bumpversion major
 bumpversion minor
 bumpversion patch
 ```
 
 ## Making a release
 
-This section describes how to make a release in 3 parts:
-
-1. preparation
-1. making a release on PyPI
-1. making a release on GitHub
+This section describes how to make a release in 3 parts: preparation, release and validation.
 
-### (1/3) Preparation
+### Preparation
 
-1. Update the <CHANGELOG.md> (don't forget to update links at bottom of page)
-2. Verify that the information in `CITATION.cff` is correct, and that `.zenodo.json` contains equivalent data
+1. Update the `CHANGELOG.md` file
+2. Verify that the information in `CITATION.cff` is correct
 3. Make sure the [version has been updated](#versioning).
 4. Run the unit tests with `hatch run test`
 
-### (2/3) PyPI
+### Making the GitHub release
 
-First prepare a new directory, for example:
-```shell
-cd $(mktemp -d lilio.XXXXXX)
-```
+Make a release and tag on GitHub.com. This will:
 
-A fresh git clone ensures the release has the state of origin/main branch
+ - trigger Zenodo into making a snapshot of your repository and sticking a DOI on it.
+ - start a GitHub action that builds and uploads the new version to [PyPI](https://pypi.org/project/lilio/).
+    - Which should trigger [conda-forge](https://anaconda.org/conda-forge/lilio) to update the package as well.
 
-```shell
-git clone https://github.com/AI4S2S/lilio .
-```
 
-In a your terminal, with an activated environment which has [`hatch`](https://hatch.pypa.io/latest/) installed do:
-
-```shell
-pip install hatch --upgrade
-hatch build
-```
-
-If the build was succesfull, publish it to [PyPI's test servers](https://test.pypi.org/). Note that your credentials are different between test.pypi.org and pypy.org.
-```shell
-hatch publish --repo test
-```
-
-Visit [https://test.pypi.org/project/lilio](https://test.pypi.org/project/lilio) and
-verify that your package was uploaded successfully.
-
-Now we can publish to PyPI:
-```
-hatch publish
-```
+### Validation
 
-### (3/3) GitHub
+After making the release, you should check that:
 
-Don't forget to also make a [release on GitHub](https://github.com/AI4S2S/lilio/releases/new). If your repository uses the GitHub-Zenodo integration this will also trigger Zenodo into making a snapshot of your repository and sticking a DOI on it.
+1. The [Zenodo page](https://doi.org/10.5281/zenodo.7620212) is updated
+1. The [publishing action](https://github.com/AI4S2S/lilio/actions/workflows/python-publish.yml) ran successfully, and that `pip install lilio` installs the new version.
+1. The [conda-forge package](https://anaconda.org/conda-forge/lilio) is updated, and can be installed using conda.
```

### Comparing `lilio-0.3.1/docs/conf.py` & `lilio-0.4.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 author = "Yang Liu"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "0.3.1"
+version = "0.4.0"
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom
@@ -103,15 +103,15 @@
     "**": [
         "globaltoc.html",
         "relations.html",  # needs 'show_related': True theme option to display
         "searchbox.html",
     ]
 }
 
-# html_logo = "./assets/images/ai4s2s_logo.png"
+html_logo = "./assets/images/lilio_logo_wide.png"
 
 # -- Options for Intersphinx
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "matplotlib": ("https://matplotlib.org/stable/", None),
```

### Comparing `lilio-0.3.1/docs/index.rst` & `lilio-0.4.0/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     notebooks/tutorial_traintest.ipynb
     notebooks/tutorial_calendar_shifter.ipynb
 
 .. toctree::
     :caption: Technical information
     :maxdepth: 2
 
+    Scaling up Lilio with Dask <dask_integration.md>
     Developer Readme <README.dev.md>
     Contributing guide <contributing_link>
     Changelog <CHANGELOG.md>
     API reference <autoapi/index.rst>
 
 .. toctree::
     :caption: Quick links
```

### Comparing `lilio-0.3.1/docs/make.bat` & `lilio-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/project_setup.md` & `lilio-0.4.0/docs/project_setup.md`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/assets/images/ai4s2s_logo.png` & `lilio-0.4.0/docs/assets/images/ai4s2s_logo.png`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/assets/images/calendar_concept.png` & `lilio-0.4.0/docs/assets/images/calendar_concept.png`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/assets/images/lilio_logo.png` & `lilio-0.4.0/docs/assets/images/lilio_logo_highres.png`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/notebooks/all_about_the_calendar.ipynb` & `lilio-0.4.0/docs/notebooks/all_about_the_calendar.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933431484295846%*

 * *Differences: {"'cells'": "{27: {'source': {insert: [(2, 'The basic building block of the Calendar is the "*

 * *            '**Interval**. Intervals have three properties: the **type** (target or precursor), '*

 * *            'the **length**, and the **gap**. The gap is defined as the gap between this interval '*

 * *            'and the preceding interval of the same type (or the anchor, if this interval is the '*

 * *            "first one).\\n'), (3, '\\n'), (4, 'The length and gap are set in the same way. The "*

 * *            'most commo […]*

```diff
@@ -269,15 +269,17 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### The `Interval` building block \ud83e\uddf1\n",
                 "\n",
-                "The basic building block of the Calendar is the **Interval**. Intervals have three properties: the type (target or precursor), the length, and the gap. The gap is defined as the gap between this interval and the preceding interval of the same type (or the anchor, if this interval is the first one)."
+                "The basic building block of the Calendar is the **Interval**. Intervals have three properties: the **type** (target or precursor), the **length**, and the **gap**. The gap is defined as the gap between this interval and the preceding interval of the same type (or the anchor, if this interval is the first one).\n",
+                "\n",
+                "The length and gap are set in the same way. The most common way is to use a pandas-like frequency string (for example, \"10d\" for ten days, \"2W\" for two weeks, or \"3M\" for three months). Let's set the length to five days and the gap to a month:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -305,14 +307,32 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "If you are feeling adventurous, you can set the length and gap using a pandas.DateOffset compatible dictionary. This allows you to combine day, week, and month lengths:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "iv.length = {\"months\": 1, \"weeks\": 2}\n",
+                "iv.length_dateoffset  # shows the length as a pandas.DateOffset object."
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "### All about anchors \u2693\n",
                 "\n",
                 "As said before, the anchor date is one of the basic elements of the calendar. Up to now we have just showcased setting the anchor as a date (\"MM-DD\"), however, there are some alternative options.\n",
                 "\n",
                 "If you are interested in *only* months, it is possible to create a calendar revolving solely around calendar months. The anchor can be defined as an *English* month name (e.g., \"January\" or the short name \"Jan\"). This is equivalent to setting the anchor to the first day of that month. For example:"
             ]
         },
@@ -490,15 +510,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.5 (tags/v3.10.5:f377153, Jun  6 2022, 16:14:13) [MSC v.1929 64 bit (AMD64)]"
+            "version": "3.10.5"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "1ad84d851b7a3d072f2b3778c2795859f5c348aba25460fe1ff63101a851e075"
             }
         }
```

### Comparing `lilio-0.3.1/docs/notebooks/calendar_shorthands.ipynb` & `lilio-0.4.0/docs/notebooks/calendar_shorthands.ipynb`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/notebooks/tutorial_calendar_shifter.ipynb` & `lilio-0.4.0/docs/notebooks/tutorial_calendar_shifter.ipynb`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/docs/notebooks/tutorial_resampling_data.ipynb` & `lilio-0.4.0/docs/notebooks/tutorial_resampling_data.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999468537414966%*

 * *Differences: {"'cells'": "{10: {'source': {insert: [(2, 'Resampling works the same for an `xarray` "*

 * *            "`Dataset`.\\n'), (3, 'Note that you can use dask arrays as well, for lower memory use "*

 * *            'and distributed computation. For more info see the '*

 * *            "[documentation](https://lilio.readthedocs.io/en/latest/dask_integration.html).\\n'), "*

 * *            '(4, \'\\n\'), (5, "Let\'s make an example dataset with latitude and longitude '*

 * *            'coordinates:")], delete: [2]}}}'}*

```diff
@@ -122,15 +122,18 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Resampling `xarray` data\n",
                 "\n",
-                "Resampling works the same for an `xarray` `Dataset`. Let's make an example dataset with latitude and longitude coordinates:"
+                "Resampling works the same for an `xarray` `Dataset`.\n",
+                "Note that you can use dask arrays as well, for lower memory use and distributed computation. For more info see the [documentation](https://lilio.readthedocs.io/en/latest/dask_integration.html).\n",
+                "\n",
+                "Let's make an example dataset with latitude and longitude coordinates:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `lilio-0.3.1/docs/notebooks/tutorial_traintest.ipynb` & `lilio-0.4.0/docs/notebooks/tutorial_traintest.ipynb`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/lilio/__init__.py` & `lilio-0.4.0/lilio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,29 @@
     2020         -1            [2020-07-04, 2020-12-31)
                   1            [2020-12-31, 2021-06-29)
     dtype: interval
 
 """
 
 import logging
-from . import calendar_shifter
-from . import traintest
+from lilio import calendar_shifter
+from lilio import traintest
 from .calendar import Calendar
 from .calendar import Interval
 from .calendar_shorthands import daily_calendar
 from .calendar_shorthands import monthly_calendar
 from .calendar_shorthands import weekly_calendar
 from .resampling import resample
 
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __author__ = "Yang Liu"
 __email__ = "y.liu@esciencecenter.nl"
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 __all__ = [
     "Calendar",
     "Interval",
     "resample",
     "daily_calendar",
     "monthly_calendar",
```

### Comparing `lilio-0.3.1/lilio/_bokeh_plots.py` & `lilio-0.4.0/lilio/_bokeh_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ._plot import generate_plot_data
 
 
 if typing.TYPE_CHECKING:
     from lilio.calendar import Calendar
 
 
-def _generate_rectangle(figure: plotting.Figure, source: plotting.ColumnDataSource):
+def _generate_rectangle(figure: plotting.figure, source: plotting.ColumnDataSource):
     """Add intervals to the figure as rectangles.
 
     Args:
         figure: Bokeh figure in which the rectangles should be added.
         source: Bokeh source data containing the required parameters.
 
     Returns:
@@ -35,28 +35,28 @@
 
 def _bokeh_visualization(
     calendar: "Calendar",
     n_years: int,
     relative_dates: bool,
     add_yticklabels: bool = True,
     **kwargs,
-) -> plotting.Figure:
+) -> plotting.figure:
     """Visualization routine for generating a calendar visualization with Bokeh.
 
     Args:
         calendar: Mapped calendar which should be visualized.
         n_years: Number of years which should be displayed (most recent years only).
         relative_dates: If False, absolute dates will be used. If True, each anchor year
                         is aligned by the anchor date, so that all anchor years line up
                         vertically.
         add_yticklabels: If the years should be displayed on the y-axis ticks.
         **kwargs: Keyword arguments that should be passed to Bokeh's plotting.figure.
 
     Returns:
-        plotting.Figure
+        plotting.figure
     """
     if add_yticklabels:
         tooltips = [
             ("Interval", "@desc"),
             ("Size", "@width_days days"),
             ("Type", "@type"),
         ]
@@ -90,19 +90,19 @@
 
     figure.xaxis.axis_label = (
         "Days relative to anchor date" if relative_dates else "Date"
     )
     figure.yaxis.axis_label = "Anchor year"
 
     if relative_dates:
-        figure.x_range.start = (
-            np.min(data["x"]) - data["width"][np.argmin(data["x"])] / 2 - 14  # type: ignore
+        figure.x_range.start = (  # type: ignore
+            np.min(data["x"]) - data["width"][np.argmin(data["x"])] / 2 - 14
         )
-        figure.x_range.end = (
-            np.max(data["x"]) + data["width"][np.argmax(data["x"])] / 2 + 14  # type: ignore
+        figure.x_range.end = (  # type: ignore
+            np.max(data["x"]) + data["width"][np.argmax(data["x"])] / 2 + 14
         )
 
     if add_yticklabels:
         figure.yaxis.ticker = [int(x) for x in intervals.index.to_list()]
     else:
         figure.yaxis.ticker = []
```

### Comparing `lilio-0.3.1/lilio/_plot.py` & `lilio-0.4.0/lilio/_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,29 +200,32 @@
 
     ax.set_xlabel("Days before anchor date" if relative_dates else "Date")
     ax.set_ylabel("Anchor year")
 
     if relative_dates:
         ax.set_xlim(
             (
-                np.min(data["x"]) - data["width"][np.argmin(data["x"])] / 2 - 5,  # type: ignore
-                np.max(data["x"]) + data["width"][np.argmax(data["x"])] / 2 + 5,  # type: ignore
+                # type: ignore
+                np.min(data["x"]) - data["width"][np.argmin(data["x"])] / 2 - 5,
+                # type: ignore
+                np.max(data["x"]) + data["width"][np.argmax(data["x"])] / 2 + 5,
             )
         )
     else:
         formatter = mdates.DateFormatter("%Y-%m-%d")
         ax.xaxis.set_major_formatter(formatter)
         ax.set_xlim(
             (
                 intervals.stack().values.min().left - pd.Timedelta(days=2),
                 intervals.stack().values.max().right + pd.Timedelta(days=2),
             )
         )
 
-    ax.set_ylim([intervals.index.min() - 0.5, intervals.index.max() + 0.5])  # type: ignore
+    # type: ignore
+    ax.set_ylim([intervals.index.min() - 0.5, intervals.index.max() + 0.5])
     ax.set_yticks([int(x) for x in intervals.index.to_list()])
 
     if not add_yticklabels:
         ax.set_yticklabels([])
 
     # Add a custom legend to explain to users what the colors mean
     if add_legend:
```

### Comparing `lilio-0.3.1/lilio/calendar.py` & `lilio-0.4.0/lilio/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from typing import List
 from typing import Literal
 from typing import Tuple
 from typing import Union
 import pandas as pd
 import xarray as xr
 from pandas.tseries.offsets import DateOffset
-from . import _plot
-from . import utils
+from lilio import _plot
+from lilio import utils
 
 
 _MappingYears = Tuple[Literal["years"], int, int]
 _MappingData = Tuple[Literal["data"], pd.Timestamp, pd.Timestamp]
 
 
 class Interval:
@@ -156,16 +156,18 @@
         to easily construct basic calendars with only a few parameters, but do not have
         the flexibility that this calendar builder module provides.
 
         Args:
             anchor: String denoting the anchor date. The following inputs are valid:
                     - "MM-DD" for a month and day. E.g. "12-31".
                     - "MM" for only a month, e.g. "4" for March.
-                    - English names and abbreviations of months. E.g. "December" or "jan".
-                    - "Www" for a week number, e.g. "W05" for the fifth week of the year.
+                    - English names and abbreviations of months. E.g. "December" or
+                        "jan".
+                    - "Www" for a week number, e.g. "W05" for the fifth week of the
+                        year.
                     - "Www-D" for a week number plus day of week. E.g. "W01-4" for the
                         first thursday of the year.
             allow_overlap: If overlapping intervals between years is allowed or not.
                 Default behaviour is False, which means that anchor years will be
                 skipped to avoid data being shared between anchor years.
             mapping: Calendar mapping. Input in the form: ("years", 2000, 2020) or
                 ("data", pd.Timestamp("2000-01-01"), pd.Timestamp("2020-01-01")). The
@@ -247,16 +249,16 @@
         """Add one or more intervals to the calendar.
 
         The interval can be a target or a precursor, and can be defined by its length,
         a possible gap between this interval and the preceding interval.
 
         Args:
             role: Either a 'target' or 'precursor' interval(s).
-            length: The length of the interval(s), in a format of '5d' for five days, '2W'
-                for two weeks, or '1M' for one month.
+            length: The length of the interval(s), in a format of '5d' for five days,
+                '2W' for two weeks, or '1M' for one month.
             gap: The gap between this interval and the preceding target/precursor
                 interval. Same format as the length argument.
             n: The number of intervals which should be added to the calendar. Defaults
                 to 1.
         """
         if not isinstance(n, int):
             raise ValueError(
@@ -518,15 +520,16 @@
     def _rename_intervals(self, intervals: pd.DataFrame) -> pd.DataFrame:
         """Add target labels to the header row of the intervals.
 
         Args:
             intervals (pd.Dataframe): Dataframe with intervals.
 
         Returns:
-            pd.Dataframe: Dataframe with target periods labelled, sorted by i_interval value.
+            pd.Dataframe: Dataframe with target periods labelled, sorted by their
+                i_interval value.
         """
         # rename precursors
         intervals = intervals.rename(
             columns={
                 i: self.n_targets - i - 1
                 for i in range(self.n_targets, len(intervals.columns))
             }
@@ -546,15 +549,17 @@
                 "Cannot retrieve intervals without map_years or "
                 "map_to_data having configured the calendar."
             )
         if self._mapping == "data":
             self._set_year_range_from_timestamps()
 
         year_range = range(
-            self._last_year, self._first_year - 1, -(self._get_skip_nyears() + 1)  # type: ignore
+            self._last_year,  # type: ignore
+            self._first_year - 1,  # type: ignore
+            -(self._get_skip_nyears() + 1),  # type: ignore
         )
 
         intervals = pd.concat([self._map_year(year) for year in year_range], axis=1).T
 
         intervals = self._rename_intervals(intervals)
 
         intervals.index.name = "anchor_year"
@@ -618,18 +623,19 @@
                 fit within the plot.
             interactive: If False, matplotlib will be used for the visualization. If
                 True, bokeh will be used.
             relative_dates: Toggles if the intervals should be displayed relative to the
                 anchor date, or as absolute dates.
             show_length: Toggles if the frequency of the intervals should be displayed.
                 Defaults to False (Matplotlib plotter only).
-            add_legend: Toggles if a legend should be added to the plot (Matplotlib only)
+            add_legend: Toggles if a legend should be added to the plot (Matplotlib
+                only)
             ax: Matplotlib axis object to plot the visualization into.
-            **bokeh_kwargs: Keyword arguments to pass to Bokeh's plotting.Figure. See
-                https://docs.bokeh.org/en/2.4.2/docs/reference/plotting/figure.html
+            **bokeh_kwargs: Keyword arguments to pass to Bokeh's plotting.figure. See
+                https://docs.bokeh.org/en/latest/docs/reference/plotting/figure.html
                 for a list of possible keyword arguments.
         """
         calendar = copy.deepcopy(self)
         if calendar._mapping is None:  # pylint: disable=protected-access
             calendar.map_years(2000, 2000)
             if not relative_dates:
                 print(
@@ -647,29 +653,31 @@
         if interactive:
             utils.assert_bokeh_available()
             # pylint: disable=import-outside-toplevel
             from ._bokeh_plots import bokeh_visualization
 
             if ax is not None:
                 warnings.warn(
-                    "ax is only a valid keyword argument for the non-interactive "
-                    "matplotlib backend. Bokeh's figure can be controlled by passing "
-                    "Bokeh Figure keyword arguments (e.g. width=800).",
+                    "\n  ax is only a valid keyword argument for the non-interactive"
+                    "\n  matplotlib backend. Bokeh's figure can be controlled by"
+                    "\n  passing Bokeh figure keyword arguments (e.g. width=800).",
                     UserWarning,
+                    stacklevel=1,
                 )
             bokeh_visualization(
                 calendar, n_years, relative_dates, add_yticklabels, **bokeh_kwargs
             )
         else:
             if bokeh_kwargs:
                 warnings.warn(
-                    "kwargs for bokeh have been passed to visualize(), but the "
-                    "matplotlib backend does not support these. Use the 'ax' kwarg "
-                    "instead to control the generated figure.",
+                    "\n  kwargs for bokeh have been passed to visualize(), but the"
+                    "\n  matplotlib backend does not support these. Use the 'ax' kwarg"
+                    "\n  instead to control the generated figure.",
                     UserWarning,
+                    stacklevel=1,
                 )
 
             _plot.matplotlib_visualization(
                 calendar,
                 n_years,
                 relative_dates,
                 show_length,
```

### Comparing `lilio-0.3.1/lilio/calendar_shifter.py` & `lilio-0.4.0/lilio/calendar_shifter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Calendar shifter to create staggered calendars."""
 import copy
 from typing import Dict
 from typing import List
 from typing import Union
 import xarray as xr
-from . import calendar
-from . import utils
+from lilio import calendar
+from lilio import utils
 from .resampling import resample
 
 
 def _gap_shift(
     interval: calendar.Interval, shift: Union[str, Dict[str, int]]
 ) -> Dict[str, int]:
     """Shift a calendar interval's gap property by the given amount.
```

### Comparing `lilio-0.3.1/lilio/calendar_shorthands.py` & `lilio-0.4.0/lilio/calendar_shorthands.py`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/lilio/resampling.py` & `lilio-0.4.0/lilio/resampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """The implementation of the resampling methods for use with the Calendar."""
 import typing
 from typing import Callable
+from typing import List
 from typing import Literal
 from typing import Union
 from typing import overload
 import numpy as np
 import pandas as pd
 import xarray as xr
+from lilio import utils
+from lilio._attrs import add_attrs
 from lilio.calendar import Calendar
-from . import utils
 
 
 # List of numpy statistical methods, with a single input argument and a single output.
 ResamplingMethod = Literal[
     "mean",
     "min",
     "max",
@@ -110,15 +112,16 @@
 
 def _contains(interval_index: pd.IntervalIndex, timestamps) -> np.ndarray:
     """Check elementwise if the intervals contain the timestamps.
 
     Will return a boolean array of the shape (n_timestamps, n_intervals).
 
     Args:
-        interval_index: An IntervalIndex containing all intervals that should be checked.
+        interval_index: An IntervalIndex containing all intervals that should be
+            checked.
         timestamps: A 1-D array containing
 
     Returns:
         np.ndarray: 2-D mask array
     """
     if interval_index.closed_left:
         a = np.greater_equal(timestamps, interval_index.left.values[np.newaxis].T)
@@ -164,15 +167,14 @@
         for i, row in enumerate(contains_matrix):
             resampled_data[i] = resampling_method(input_data[colname].values[row])
         data[colname] = resampled_data
 
     return data
 
 
-# pylint: disable=too-many-locals
 def _resample_dataset(
     calendar: Calendar,
     input_data: xr.Dataset,
     how: Union[ResamplingMethod, Callable[[np.ndarray], np.ndarray]],
 ) -> xr.Dataset:
     """Resample xarray data.
 
@@ -188,58 +190,57 @@
             these intervals.
     """
     resampling_method = getattr(np, how) if isinstance(how, str) else how
     data = calendar.flat.to_xarray().rename("interval")
     data = data.to_dataset()
     data = data.stack(anch_int=("anchor_year", "i_interval"))
 
+    intervals = pd.IntervalIndex(data["interval"].values)
+    timesteps = input_data["time"].to_numpy()
+
+    indices_list: List[np.ndarray] = [np.ndarray(0)] * len(intervals)
+    for i in range(len(intervals)):
+        row = _contains(intervals[[i]], timesteps)[0]
+        indices_list[i] = np.argwhere(row).T[0]
+
     # Separate data with time dims (should be resampled), from data without time dims
-    #   (which does not need resampling). Otherwise stacking ALL dims together will
-    #   cause the stacked dimension become needlessly large, making resampling slow.
+    #   (which does not need resampling).
     input_data_time = input_data[
         [var for var in input_data.data_vars if "time" in input_data[var].dims]
     ]
     input_data_nontime = input_data[
         [var for var in input_data.data_vars if "time" not in input_data[var].dims]
     ]
 
-    stacking_dims = list(input_data_time.dims.keys())
-    stacking_dims.remove("time")
-    if stacking_dims:  # There might not be extra dims to stack!
-        input_data_time = input_data_time.stack(allstack=stacking_dims)
-
-    da_coords = {"anch_int": data["anch_int"]}
-    if stacking_dims:
-        da_coords["allstack"] = input_data_time["allstack"]
+    data_list = [xr.Dataset] * len(intervals)
+    for i in range(len(intervals)):
+        data_list[i] = xr.apply_ufunc(
+            resampling_method,
+            input_data_time.isel(time=indices_list[i]),
+            input_core_dims=[["time"]],
+            output_core_dims=[[]],
+            vectorize=True,
+            dask="parallelized",  # only does something when data is a Dask array
+            dask_gufunc_kwargs={"allow_rechunk": True},  # Same as above
+        )
 
-    contains_matrix = _contains(
-        pd.IntervalIndex(data["interval"].values), input_data_time["time"].values
-    )
+    if utils.is_dask_array(input_data_time):
+        import dask
 
-    resampled_vars = [xr.DataArray] * len(input_data_time.data_vars)
-    for i, var in enumerate(input_data_time.data_vars):
-        size_input = input_data_time[var].shape[1] if stacking_dims else 1
-        resampled_data = np.zeros((contains_matrix.shape[0], size_input))
-
-        # Note: while looping, contains_matrix will have a size of
-        # (n_intervals * n_anchor_years), making it the most reliably small dim.
-        _data = input_data_time[var].values
-        for j, row in enumerate(contains_matrix):
-            resampled_data[j, :] = resampling_method(_data[row], axis=0)
-
-        resampled_data = np.squeeze(resampled_data)  # in case of (1, n) resampled data
-
-        resampled_vars[i] = xr.DataArray(  # type: ignore
-            data=resampled_data, coords=da_coords
-        ).rename(var)
+        # Note: the * before data_list unpacks the list into separate arguments
+        #   and passes these concurrently to dask.compute. This triggers dask to
+        #   compute all the sub-datasets concurrently.
+        input_data_resampled = xr.concat(dask.compute(*data_list), dim="anch_int")
+    else:
+        input_data_resampled = xr.concat(data_list, dim="anch_int")  # type: ignore
 
     if input_data_nontime.data_vars:
-        data = xr.merge([data, input_data_nontime] + resampled_vars)
+        data = xr.merge([data, input_data_nontime, input_data_resampled])
     else:
-        data = xr.merge([data] + resampled_vars)
+        data = xr.merge([data, input_data_resampled])
 
     data = data.unstack()
     data = utils.convert_interval_to_bounds(data)
     data = data.transpose("anchor_year", "i_interval", ...)
     return data.sortby("anchor_year", "i_interval")
 
 
@@ -351,9 +352,15 @@
         resampled_data = _resample_dataset(calendar, input_data, how)
 
     utils.check_empty_intervals(resampled_data)
 
     resampled_data = _mark_target_period(resampled_data)
 
     if isinstance(input_data, xr.DataArray):
-        return resampled_data[da_name]
+        resampled_dataarray = resampled_data[da_name]
+        resampled_dataarray.attrs = input_data.attrs
+        add_attrs(resampled_dataarray, calendar)
+        return resampled_dataarray
+    if isinstance(input_data, xr.Dataset):
+        resampled_data.attrs = input_data.attrs
+        add_attrs(resampled_data, calendar)
     return resampled_data
```

### Comparing `lilio-0.3.1/lilio/traintest.py` & `lilio-0.4.0/lilio/traintest.py`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/lilio/utils.py` & `lilio-0.4.0/lilio/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,25 @@
         raise ValueError("The input data is neither a pandas or xarray object")
     if isinstance(data, (pd.Series, pd.DataFrame)):
         check_time_dim_pandas(data)
     elif isinstance(data, (xr.DataArray, xr.Dataset)):
         check_time_dim_xarray(data)
 
 
+def is_dask_array(data: Union[xr.DataArray, xr.Dataset]) -> bool:
+    """Checks if the xarray dataset/array has any dask arrays."""
+    if isinstance(data, xr.DataArray):
+        return False if data.chunks is None else True
+
+    if any([data[var].chunks is not None for var in list(data.variables)]):
+        return True
+    else:
+        return False
+
+
 def check_time_dim_xarray(data) -> None:
     """Check if an xarray data has a time dimensions with time data."""
     if "time" not in data.dims:
         raise ValueError(
             "The input DataArray/Dataset does not contain a `time` dimension"
         )
     if not xr.core.common.is_np_datetime_like(data["time"].dtype):  # type: ignore
@@ -73,16 +84,17 @@
         if not any(
             data[var].isnull().any(dim=["i_interval", "anchor_year"]).all()
             for var in time_vars
         ):
             return None
 
     warnings.warn(
-        "The input data could not fully cover the calendar's intervals. "
-        "Intervals without available data will contain NaN values."
+        "\n  The input data could not fully cover the calendar's intervals."
+        "\n  Intervals without available data will contain NaN values.",
+        stacklevel=1,
     )
     return None
 
 
 def infer_input_data_freq(
     data: Union[pd.Series, pd.DataFrame, xr.DataArray, xr.Dataset]
 ) -> pd.Timedelta:
@@ -150,18 +162,19 @@
             " Please make the Calendar's intervals larger, or use data of a higher time"
             " resolution."
             f"\nInfered data frequency: {str(data_freq)} < calendar frequency "
             f"{str(calendar_freq)}"
         )
     if calendar_freq < 2 * data_freq:
         warnings.warn(
-            "The input data frequency is very close to the Calendar's frequency. "
-            "This could lead to issues like aliasing or incorrect resampling. "
-            "If possible: make the Calendar's intervals larger, or use data of a higher"
-            " time resolution."
+            "\n  The input data frequency is very close to the Calendar's frequency."
+            "\n  This could lead to issues like aliasing or incorrect resampling."
+            "\n  If possible: make the Calendar's intervals larger, or use data of a"
+            "\n  higher time resolution.",
+            stacklevel=1,
         )
 
 
 def convert_interval_to_bounds(data: xr.Dataset) -> xr.Dataset:
     """Convert pandas intervals to bounds in a xarray Dataset.
 
     pd.Interval objects cannot be written to netCDF. To allow writing the
```

### Comparing `lilio-0.3.1/tests/test_calendar.py` & `lilio-0.4.0/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/tests/test_calendar_shifter.py` & `lilio-0.4.0/tests/test_calendar_shifter.py`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/tests/test_plots.py` & `lilio-0.4.0/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/tests/test_resample.py` & `lilio-0.4.0/tests/test_resample.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 """
 import tempfile
 from pathlib import Path
 import numpy as np
 import pandas as pd
 import pytest
 import xarray as xr
+from dask.distributed import Client
 from lilio import Calendar
 from lilio import daily_calendar
 from lilio import monthly_calendar
 from lilio import resample
 from lilio.resampling import VALID_METHODS
+from . import data_folder
+
+
+TEST_DATA_DIR = data_folder
 
 
 class TestResample:
     """Test resampling, general tests for how=mean."""
 
     # Define all required inputs as fixtures:
     @pytest.fixture
@@ -205,14 +210,53 @@
 
     def test_missing_intervals_dataset(self, dummy_calendar, dummy_dataset):
         dataset, _ = dummy_dataset
         cal = dummy_calendar.map_years(2020, 2025)
         with pytest.warns(UserWarning):
             resample(cal, dataset)
 
+    def test_dataset_attrs(self, dummy_calendar, dummy_dataset):
+        dataset, _ = dummy_dataset
+        dataset.attrs = {"history": "test_history", "other_attrs": "abc"}
+        cal = dummy_calendar.map_years(2020, 2025)
+        resampled = resample(cal, dataset)
+
+        expected_attrs = [
+            "lilio_version",
+            "lilio_calendar_anchor_date",
+            "lilio_calendar_code",
+        ]
+
+        assert "test_history" in resampled.attrs["history"]
+        assert "other_attrs" in resampled.attrs.keys()
+        for att in expected_attrs:
+            assert att in resampled.attrs.keys()
+
+    def test_dataarray_attrs(self, dummy_calendar, dummy_dataarray):
+        """This is a copy of the previous test, but with dataarray input.
+
+        Sadly, fixtures aren't compatible with parameterize. Refactoring the fixtures
+        could solve this.
+        """
+        dataarray, _ = dummy_dataarray
+        dataarray.attrs = {"history": "test_history", "other_attrs": "abc"}
+        cal = dummy_calendar.map_years(2020, 2025)
+        resampled = resample(cal, dataarray)
+
+        expected_attrs = [
+            "lilio_version",
+            "lilio_calendar_anchor_date",
+            "lilio_calendar_code",
+        ]
+
+        assert "test_history" in resampled.attrs["history"]
+        assert "other_attrs" in resampled.attrs.keys()
+        for att in expected_attrs:
+            assert att in resampled.attrs.keys()
+
 
 TOO_LOW_FREQ_ERR = r".*lower time resolution than the calendar.*"
 TOO_LOW_FREQ_WARN = r".*input data frequency is very close to the Calendar's freq.*"
 
 
 class TestResampleChecks:
     @pytest.fixture
@@ -329,7 +373,34 @@
         cal = dummy_calendar.map_to_data(data)
         resample(cal, data, how=np.mean)
 
     def test_func_input_dataset(self, dummy_calendar, dummy_dataset):
         data, _ = dummy_dataset
         cal = dummy_calendar.map_to_data(data)
         resample(cal, data, how=np.mean)
+
+
+class TestResampleDask:
+    """Test resampling, general tests for how=mean."""
+
+    # Define all required inputs as fixtures:
+    @pytest.fixture
+    def dummy_calendar(self):
+        return daily_calendar(anchor="10-15", length="7d", n_precursors=1)
+
+    @pytest.fixture
+    def dummy_dataset(self):
+        return xr.open_mfdataset(
+            TEST_DATA_DIR.glob("*.nc"),
+            parallel=False,  # See: https://github.com/pydata/xarray/issues/7079
+            chunks={"time": 30, "longitude": -1, "latitude": -1},
+            engine="netcdf4",
+        )
+
+    def test_dask_resample(self, dummy_dataset, dummy_calendar):
+        """Just asssert that resampling w/ dask runs fine."""
+        client = Client(n_workers=2, threads_per_worker=2)
+        assert dummy_dataset["t2m"].chunks is not None
+        cal = dummy_calendar
+        cal.map_years(2001, 2001)
+        resample(cal, dummy_dataset)
+        client.close()
```

### Comparing `lilio-0.3.1/tests/test_traintest.py` & `lilio-0.4.0/tests/test_traintest.py`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/LICENSE` & `lilio-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lilio-0.3.1/README.md` & `lilio-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 # lilio: Calendar generator for machine learning with timeseries data
 
 <img align="right" width="160" alt="Logo" src="https://raw.githubusercontent.com/AI4S2S/lilio/main/docs/assets/images/lilio_logo.png">
 
 
-[![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/AI4S2S/lilio)
+<!--[![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/AI4S2S/lilio) -->
 [![github license badge](https://img.shields.io/github/license/AI4S2S/lilio)](https://github.com/AI4S2S/lilio)
-[![rsd badge](https://img.shields.io/badge/rsd-lilio-blue)](https://research-software-directory.org/software/lilio)
+[![rsd badge](https://img.shields.io/badge/RSD-lilio-blue)](https://research-software-directory.org/software/lilio)
 [![DOI](https://zenodo.org/badge/588084019.svg)](https://zenodo.org/badge/latestdoi/588084019)
-[![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
-[![Documentation Status](https://readthedocs.org/projects/ai4s2s/badge/?version=latest)](https://ai4s2s.readthedocs.io/en/latest/?badge=latest)
+[![SQAaaS badge shields.io](https://img.shields.io/badge/sqaaas%20software-gold-yellow)](https://api.eu.badgr.io/public/assertions/P3scOSLyQVWzzsjq0Ueycw "SQAaaS gold badge achieved")
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![Documentation Status](https://readthedocs.org/projects/ai4s2s/badge/?version=stable)](https://lilio.readthedocs.io/en/stable/?badge=stable)
 [![build](https://github.com/AI4S2S/lilio/actions/workflows/build.yml/badge.svg)](https://github.com/AI4S2S/lilio/actions/workflows/build.yml)
-[![sonarcloud](https://github.com/AI4S2S/lilio/actions/workflows/sonarcloud.yml/badge.svg)](https://github.com/AI4S2S/lilio/actions/workflows/sonarcloud.yml)
 [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=AI4S2S_lilio&metric=coverage)](https://sonarcloud.io/dashboard?id=AI4S2S_lilio)
+<!--[![sonarcloud](https://github.com/AI4S2S/lilio/actions/workflows/sonarcloud.yml/badge.svg)](https://github.com/AI4S2S/lilio/actions/workflows/sonarcloud.yml) -->
 
 A python package for generating calendars to resample timeseries into training and target data for machine learning. Named after [the inventor](https://en.wikipedia.org/wiki/Aloysius_Lilius) of the [Gregorian Calendar](https://en.wikipedia.org/wiki/Gregorian_calendar).
 
 Lilio was originally designed for use in [`s2spy`](https://github.com/AI4S2S/s2spy), a high-level python package integrating expert knowledge and artificial intelligence to boost (sub) seasonal forecasting.
 
 ## Installation
 [![workflow pypi badge](https://img.shields.io/pypi/v/lilio.svg?colorB=blue)](https://pypi.python.org/project/lilio/)
 [![supported python versions](https://img.shields.io/pypi/pyversions/lilio)](https://pypi.python.org/project/lilio/)
+[![conda-forge](https://anaconda.org/conda-forge/lilio/badges/version.svg)](https://anaconda.org/conda-forge/lilio)
 
 To install the latest release of lilio, do:
 ```console
 python3 -m pip install lilio
 ```
 
+Lilio is also available on conda-forge. If you use conda, do:
+```console
+conda install -c conda-forge lilio
+```
+
 To install the in-development version from the GitHub repository, do:
 
 ```console
 python3 -m pip install git+https://github.com/AI4S2S/lilio.git
 ```
 
 ### Configure the package for development and testing
@@ -106,20 +113,17 @@
 For detailed information on using `lilio` package, visit the [documentation page](https://lilio.readthedocs.io/en/latest/) hosted at Readthedocs.
 
 ## Contributing
 
 If you want to contribute to the development of lilio,
 have a look at the [contribution guidelines](docs/CONTRIBUTING.md).
 
-<!--
 ## How to cite us
-[![RSD](https://img.shields.io/badge/rsd-s2spy-00a3e3.svg)](https://research-software-directory.org/software/s2spy)
-<!-- [![DOI](https://zenodo.org/badge/DOI/<replace-with-created-DOI>.svg)](https://doi.org/<replace-with-created-DOI>)
-
-TODO: add links to zenodo and rsd.
-More information will follow soon.
+[![rsd badge](https://img.shields.io/badge/RSD-lilio-blue)](https://research-software-directory.org/software/lilio)
+[![DOI](https://zenodo.org/badge/588084019.svg)](https://zenodo.org/badge/latestdoi/588084019)
 
--->
+Please use the Zenodo DOI to cite this package if you used it in your research.
 
-## Credits
+## Acknowledgements
+This package was developed by the Netherlands eScience Center and Vrije Universiteit Amsterdam under Netherlands eScience Center grant NLESC.OEC.2021.005.
 
-This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [NLeSC/python-template](https://github.com/NLeSC/python-template).
+The package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [NLeSC/python-template](https://github.com/NLeSC/python-template).
```

### Comparing `lilio-0.3.1/pyproject.toml` & `lilio-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -69,26 +69,27 @@
   "hatch",
   "ruff",
   "isort",
   "black",
   "mypy",
   "pytest",
   "pytest-cov",
+  "dask[distributed]",
 ]
 docs = [  # Required for ReadTheDocs
   "myst_parser",
   "sphinx",
   "sphinx_rtd_theme",
   "sphinx-autoapi",
   "coverage[toml]",
   "nbsphinx",
   "ipykernel",
 ]
 bokeh = [
-  "bokeh < 3.0.0",
+  "bokeh >= 3.0.0",
 ]
 
 [tool.hatch.envs.default]
 features = ["dev", "bokeh"]
 
 [tool.hatch.envs.default.scripts]
 lint = [
@@ -124,33 +125,33 @@
 
 [tool.ruff]
 select = [
   "E",  # pycodestyle
   "F",  # pyflakes
   "B",  # flake8-bugbear
   "D",  # pydocstyle
-  "C",  # mccabe complexity
+  "C90",  # mccabe complexity
 #  "I",  # isort (autosort not working correctly, disabled for now).
   "N",  # PEP8-naming
   "UP",  # pyupgrade (upgrade syntax to current syntax)
   "PLE",  # Pylint error https://github.com/charliermarsh/ruff#error-ple
   "PLR",  # Pylint refactor (e.g. too-many-arguments)
   "PLW",  # Pylint warning (useless-else-on-loop)
 ]
 extend-select = [
   "D401",  # First line should be in imperative mood
   "D400",  # First line should end in a period.
   "D404",  # First word of the docstring should not be 'This'
+  "TID252",  # No relative imports (not pep8 compliant)
 ]
 ignore = [
-  "E501",  # Line length: fails on many docstrings (needs fixing).
   "PLR2004",  # magic value used in comparsion (i.e. `if ndays == 28: month_is_feb`).
 ]
 # Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F"]
+fixable = ["A", "B", "C90", "D", "E", "F", "TID252"]
 unfixable = []
 line-length = 88
 exclude = ["docs", "build"]
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 target-version = "py38"
```

### Comparing `lilio-0.3.1/PKG-INFO` & `lilio-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilio
-Version: 0.3.1
+Version: 0.4.0
 Summary: python package for generating calendars for machine learning timeseries analysis.
 Author: Yang Liu, Bart Schilperoort, Peter Kalverla, Jannes van Ingen, Sem Vijverberg
 Author-email: y.liu@esciencecenter.nl
 Maintainer-email: Yang Liu <y.liu@esciencecenter.nl>, Bart Schilperoort <b.schilperoort@esciencecenter.nl>, Peter Kalverla <b.schilperoort@esciencecenter.nl>, Jannes van Ingen <jannes.van.ingen@s2s-ai.com>, Sem Vijverberg <sem.vijverberg@vu.nl>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: calendar,calendar generation,calendar maker,machine learning,timeseries analysis
@@ -22,18 +22,19 @@
 Requires-Dist: matplotlib
 Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: xarray
 Provides-Extra: bokeh
-Requires-Dist: bokeh<3.0.0; extra == 'bokeh'
+Requires-Dist: bokeh>=3.0.0; extra == 'bokeh'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bump2version; extra == 'dev'
+Requires-Dist: dask[distributed]; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: docs
@@ -47,37 +48,44 @@
 Description-Content-Type: text/markdown
 
 # lilio: Calendar generator for machine learning with timeseries data
 
 <img align="right" width="160" alt="Logo" src="https://raw.githubusercontent.com/AI4S2S/lilio/main/docs/assets/images/lilio_logo.png">
 
 
-[![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/AI4S2S/lilio)
+<!--[![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/AI4S2S/lilio) -->
 [![github license badge](https://img.shields.io/github/license/AI4S2S/lilio)](https://github.com/AI4S2S/lilio)
-[![rsd badge](https://img.shields.io/badge/rsd-lilio-blue)](https://research-software-directory.org/software/lilio)
+[![rsd badge](https://img.shields.io/badge/RSD-lilio-blue)](https://research-software-directory.org/software/lilio)
 [![DOI](https://zenodo.org/badge/588084019.svg)](https://zenodo.org/badge/latestdoi/588084019)
-[![fair-software badge](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
-[![Documentation Status](https://readthedocs.org/projects/ai4s2s/badge/?version=latest)](https://ai4s2s.readthedocs.io/en/latest/?badge=latest)
+[![SQAaaS badge shields.io](https://img.shields.io/badge/sqaaas%20software-gold-yellow)](https://api.eu.badgr.io/public/assertions/P3scOSLyQVWzzsjq0Ueycw "SQAaaS gold badge achieved")
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![Documentation Status](https://readthedocs.org/projects/ai4s2s/badge/?version=stable)](https://lilio.readthedocs.io/en/stable/?badge=stable)
 [![build](https://github.com/AI4S2S/lilio/actions/workflows/build.yml/badge.svg)](https://github.com/AI4S2S/lilio/actions/workflows/build.yml)
-[![sonarcloud](https://github.com/AI4S2S/lilio/actions/workflows/sonarcloud.yml/badge.svg)](https://github.com/AI4S2S/lilio/actions/workflows/sonarcloud.yml)
 [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=AI4S2S_lilio&metric=coverage)](https://sonarcloud.io/dashboard?id=AI4S2S_lilio)
+<!--[![sonarcloud](https://github.com/AI4S2S/lilio/actions/workflows/sonarcloud.yml/badge.svg)](https://github.com/AI4S2S/lilio/actions/workflows/sonarcloud.yml) -->
 
 A python package for generating calendars to resample timeseries into training and target data for machine learning. Named after [the inventor](https://en.wikipedia.org/wiki/Aloysius_Lilius) of the [Gregorian Calendar](https://en.wikipedia.org/wiki/Gregorian_calendar).
 
 Lilio was originally designed for use in [`s2spy`](https://github.com/AI4S2S/s2spy), a high-level python package integrating expert knowledge and artificial intelligence to boost (sub) seasonal forecasting.
 
 ## Installation
 [![workflow pypi badge](https://img.shields.io/pypi/v/lilio.svg?colorB=blue)](https://pypi.python.org/project/lilio/)
 [![supported python versions](https://img.shields.io/pypi/pyversions/lilio)](https://pypi.python.org/project/lilio/)
+[![conda-forge](https://anaconda.org/conda-forge/lilio/badges/version.svg)](https://anaconda.org/conda-forge/lilio)
 
 To install the latest release of lilio, do:
 ```console
 python3 -m pip install lilio
 ```
 
+Lilio is also available on conda-forge. If you use conda, do:
+```console
+conda install -c conda-forge lilio
+```
+
 To install the in-development version from the GitHub repository, do:
 
 ```console
 python3 -m pip install git+https://github.com/AI4S2S/lilio.git
 ```
 
 ### Configure the package for development and testing
@@ -154,20 +162,17 @@
 For detailed information on using `lilio` package, visit the [documentation page](https://lilio.readthedocs.io/en/latest/) hosted at Readthedocs.
 
 ## Contributing
 
 If you want to contribute to the development of lilio,
 have a look at the [contribution guidelines](docs/CONTRIBUTING.md).
 
-<!--
 ## How to cite us
-[![RSD](https://img.shields.io/badge/rsd-s2spy-00a3e3.svg)](https://research-software-directory.org/software/s2spy)
-<!-- [![DOI](https://zenodo.org/badge/DOI/<replace-with-created-DOI>.svg)](https://doi.org/<replace-with-created-DOI>)
-
-TODO: add links to zenodo and rsd.
-More information will follow soon.
+[![rsd badge](https://img.shields.io/badge/RSD-lilio-blue)](https://research-software-directory.org/software/lilio)
+[![DOI](https://zenodo.org/badge/588084019.svg)](https://zenodo.org/badge/latestdoi/588084019)
 
--->
+Please use the Zenodo DOI to cite this package if you used it in your research.
 
-## Credits
+## Acknowledgements
+This package was developed by the Netherlands eScience Center and Vrije Universiteit Amsterdam under Netherlands eScience Center grant NLESC.OEC.2021.005.
 
-This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [NLeSC/python-template](https://github.com/NLeSC/python-template).
+The package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [NLeSC/python-template](https://github.com/NLeSC/python-template).
```

