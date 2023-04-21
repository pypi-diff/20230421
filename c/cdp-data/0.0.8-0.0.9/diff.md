# Comparing `tmp/cdp-data-0.0.8.tar.gz` & `tmp/cdp-data-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdp-data-0.0.8.tar", last modified: Mon Oct 10 23:51:19 2022, max compression
+gzip compressed data, was "cdp-data-0.0.9.tar", last modified: Tue Oct 18 17:24:23 2022, max compression
```

## Comparing `cdp-data-0.0.8.tar` & `cdp-data-0.0.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.476517 cdp-data-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.468517 cdp-data-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.468517 cdp-data-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.468517 cdp-data-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-10-10 23:51:06.000000 cdp-data-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-10-10 23:51:06.000000 cdp-data-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-10-10 23:51:06.000000 cdp-data-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-10-10 23:51:06.000000 cdp-data-0.0.8/Justfile
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-10-10 23:51:06.000000 cdp-data-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-10-10 23:51:19.476517 cdp-data-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-10-10 23:51:06.000000 cdp-data-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.468517 cdp-data-0.0.8/cdp_data/
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/cdp_data/bin/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/cdp_data/bin/research/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/bin/research/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17696 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/bin/research/cdp_councils_in_action_2022_content.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    28532 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/instances.py
--rw-r--r--   0 runner    (1001) docker     (121)    21665 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)    11651 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/plots.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/cdp_data/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/tests/test_keywords_and_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/cdp_data/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4843 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/tests/utils/test_incremental_average.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/cdp_data/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6586 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/utils/fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-10-10 23:51:06.000000 cdp-data-0.0.8/cdp_data/utils/incremental_average.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/cdp_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-10-10 23:51:19.000000 cdp-data-0.0.8/cdp_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-10-10 23:51:19.000000 cdp-data-0.0.8/cdp_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 23:51:19.000000 cdp-data-0.0.8/cdp_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-10 23:51:19.000000 cdp-data-0.0.8/cdp_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 23:51:18.000000 cdp-data-0.0.8/cdp_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-10-10 23:51:19.000000 cdp-data-0.0.8/cdp_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-10 23:51:19.000000 cdp-data-0.0.8/cdp_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   335529 2022-10-10 23:51:06.000000 cdp-data-0.0.8/docs/_static/header-keywords-over-time.png
--rw-r--r--   0 runner    (1001) docker     (121)    92650 2022-10-10 23:51:06.000000 cdp-data-0.0.8/docs/_static/seattle-keywords-over-time.png
--rwxr-xr-x   0 runner    (1001) docker     (121)     5447 2022-10-10 23:51:06.000000 cdp-data-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-10 23:51:06.000000 cdp-data-0.0.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-10-10 23:51:06.000000 cdp-data-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-10 23:51:06.000000 cdp-data-0.0.8/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.472517 cdp-data-0.0.8/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)   131019 2022-10-10 23:51:06.000000 cdp-data-0.0.8/notebooks/historical_vote_proportions.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   500991 2022-10-10 23:51:06.000000 cdp-data-0.0.8/notebooks/plot_keyword_history.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-10-10 23:51:06.000000 cdp-data-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 23:51:19.476517 cdp-data-0.0.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-10-10 23:51:06.000000 cdp-data-0.0.8/scripts/generate-readme-figs.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-10 23:51:19.476517 cdp-data-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.995241 cdp-data-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.987241 cdp-data-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.987241 cdp-data-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.991241 cdp-data-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-10-18 17:24:09.000000 cdp-data-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-10-18 17:24:09.000000 cdp-data-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-10-18 17:24:09.000000 cdp-data-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-10-18 17:24:09.000000 cdp-data-0.0.9/Justfile
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-10-18 17:24:09.000000 cdp-data-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-10-18 17:24:23.995241 cdp-data-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-10-18 17:24:09.000000 cdp-data-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.991241 cdp-data-0.0.9/cdp_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.991241 cdp-data-0.0.9/cdp_data/bin/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.991241 cdp-data-0.0.9/cdp_data/bin/research/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/bin/research/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17696 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/bin/research/cdp_councils_in_action_2022_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32550 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/instances.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23082 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11901 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/plots.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.991241 cdp-data-0.0.9/cdp_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      929 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/tests/test_keywords_and_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.991241 cdp-data-0.0.9/cdp_data/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4843 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/tests/utils/test_incremental_average.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.995241 cdp-data-0.0.9/cdp_data/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6868 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/utils/fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-10-18 17:24:09.000000 cdp-data-0.0.9/cdp_data/utils/incremental_average.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.991241 cdp-data-0.0.9/cdp_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-10-18 17:24:23.000000 cdp-data-0.0.9/cdp_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-10-18 17:24:23.000000 cdp-data-0.0.9/cdp_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 17:24:23.000000 cdp-data-0.0.9/cdp_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-18 17:24:23.000000 cdp-data-0.0.9/cdp_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 17:24:23.000000 cdp-data-0.0.9/cdp_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-10-18 17:24:23.000000 cdp-data-0.0.9/cdp_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-18 17:24:23.000000 cdp-data-0.0.9/cdp_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.995241 cdp-data-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.995241 cdp-data-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)   335529 2022-10-18 17:24:09.000000 cdp-data-0.0.9/docs/_static/header-keywords-over-time.png
+-rw-r--r--   0 runner    (1001) docker     (121)    92650 2022-10-18 17:24:09.000000 cdp-data-0.0.9/docs/_static/seattle-keywords-over-time.png
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5447 2022-10-18 17:24:09.000000 cdp-data-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-18 17:24:09.000000 cdp-data-0.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-10-18 17:24:09.000000 cdp-data-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-18 17:24:09.000000 cdp-data-0.0.9/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.995241 cdp-data-0.0.9/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (121)   131019 2022-10-18 17:24:09.000000 cdp-data-0.0.9/notebooks/historical_vote_proportions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   500991 2022-10-18 17:24:09.000000 cdp-data-0.0.9/notebooks/plot_keyword_history.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-10-18 17:24:09.000000 cdp-data-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:24:23.995241 cdp-data-0.0.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-10-18 17:24:09.000000 cdp-data-0.0.9/scripts/generate-readme-figs.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 17:24:23.995241 cdp-data-0.0.9/setup.cfg
```

### Comparing `cdp-data-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md` & `cdp-data-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md` & `cdp-data-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/.github/PULL_REQUEST_TEMPLATE.md` & `cdp-data-0.0.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/.github/workflows/ci.yml` & `cdp-data-0.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/.github/workflows/docs.yml` & `cdp-data-0.0.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/.gitignore` & `cdp-data-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/.pre-commit-config.yaml` & `cdp-data-0.0.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 
   - repo: https://github.com/PyCQA/flake8
     rev: 4.0.1
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-typing-imports>=1.9.0
-          - flake8-pyprojecttoml
+          - flake8-pyprojecttoml==0.0.1
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.971
     hooks:
       - id: mypy
```

### Comparing `cdp-data-0.0.8/CODE_OF_CONDUCT.md` & `cdp-data-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/CONTRIBUTING.md` & `cdp-data-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/Justfile` & `cdp-data-0.0.9/Justfile`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/LICENSE` & `cdp-data-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/PKG-INFO` & `cdp-data-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdp-data
-Version: 0.0.8
+Version: 0.0.9
 Summary: Data Utilities and Processing Generalized for All CDP Instances
 Author-email: "Eva Maxfield Brown, Council Data Project Contributors" <evamaxfieldbrown@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/CouncilDataProject/cdp-data
 Project-URL: Bug Tracker, https://github.com/CouncilDataProject/cdp-data/issues
 Project-URL: Documentation, https://CouncilDataProject.github.io/cdp-data
 Project-URL: User Support, https://github.com/CouncilDataProject/cdp-data/issues
```

### Comparing `cdp-data-0.0.8/README.md` & `cdp-data-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/cdp_data/bin/research/cdp_councils_in_action_2022_content.py` & `cdp-data-0.0.9/cdp_data/bin/research/cdp_councils_in_action_2022_content.py`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/cdp_data/datasets.py` & `cdp-data-0.0.9/cdp_data/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 from cdp_backend.database import models as db_models
 from cdp_backend.pipeline.transcript_model import Transcript
 from cdp_backend.utils.file_utils import resource_copy
 from dataclasses_json import dataclass_json
 from fireo.models import Model
@@ -31,197 +31,259 @@
 @dataclass
 class _VideoFetchParams:
     session_id: str
     session_key: str
     event_id: str
     video_uri: str
     parent_cache_dir: Path
+    fs: GCSFileSystem
+    raise_on_error: bool
 
 
 @dataclass_json
 @dataclass
 class _MatchingVideo:
     session_key: str
-    video_path: Path
+    video_path: Optional[Path]
 
 
 def _get_matching_video(
     fetch_params: _VideoFetchParams,
 ) -> _MatchingVideo:
-    # Handle cache dir
-    this_video_cache_dir = (
-        fetch_params.parent_cache_dir
-        / f"event-{fetch_params.event_id}"
-        / f"session-{fetch_params.session_id}"
-    )
-    # Create cache dir (Handle try except because threaded)
     try:
-        this_video_cache_dir.mkdir(parents=True, exist_ok=True)
-    except FileExistsError:
-        pass
-
-    # Download transcript if needed
-    save_path = this_video_cache_dir / "video"
-    if save_path.is_dir():
-        raise IsADirectoryError(
-            f"Video '{fetch_params.video_uri}', could not be saved because "
-            f"'{save_path}' is a directory. Delete or move the directory to a "
-            f"different location or change the target dataset cache dir."
-        )
-    elif save_path.is_file():
-        log.debug(
-            f"Skipping video '{fetch_params.video_uri}'. "
-            f"A file already exists at target save path."
-        )
-    else:
-        resource_copy(uri=fetch_params.video_uri, dst=save_path)
-
-    return _MatchingVideo(
-        session_key=fetch_params.session_key,
-        video_path=save_path,
-    )
+        # Handle cache dir
+        this_video_cache_dir = (
+            fetch_params.parent_cache_dir
+            / f"event-{fetch_params.event_id}"
+            / f"session-{fetch_params.session_id}"
+        )
+        # Create cache dir (Handle try except because threaded)
+        try:
+            this_video_cache_dir.mkdir(parents=True, exist_ok=True)
+        except FileExistsError:
+            pass
+
+        # Download transcript if needed
+        save_path = this_video_cache_dir / "video"
+        if save_path.is_dir():
+            raise IsADirectoryError(
+                f"Video '{fetch_params.video_uri}', could not be saved because "
+                f"'{save_path}' is a directory. Delete or move the directory to a "
+                f"different location or change the target dataset cache dir."
+            )
+        elif save_path.is_file():
+            log.debug(
+                f"Skipping video '{fetch_params.video_uri}'. "
+                f"A file already exists at target save path."
+            )
+        else:
+            resource_copy(uri=fetch_params.video_uri, dst=save_path)
+
+        return _MatchingVideo(
+            session_key=fetch_params.session_key,
+            video_path=save_path,
+        )
+
+    except Exception:
+        if fetch_params.raise_on_error:
+            raise FileNotFoundError(
+                f"Something went wrong while fetching the video for session: "
+                f"'{fetch_params.session_id}' from '{fetch_params.fs.project}' "
+                f"Please check if a report has already been made to GitHub "
+                f"(https://github.com/CouncilDataProject/cdp-data/issues). "
+                f"If you cannot find an open issue for this session, "
+                f"please create a new one. "
+                f"In the meantime, please try rerunning your request with "
+                f"`raise_on_error=False`"
+            )
+
+        return _MatchingVideo(
+            session_key=fetch_params.session_key,
+            video_path=None,
+        )
 
 
 @dataclass
 class _AudioFetchParams:
     session_id: str
     session_key: str
     event_id: str
     parent_cache_dir: Path
     fs: GCSFileSystem
+    raise_on_error: bool
 
 
 @dataclass_json
 @dataclass
 class _MatchingAudio:
     session_key: str
-    audio_path: Path
+    audio_path: Optional[Path]
 
 
 def _get_matching_audio(
     fetch_params: _AudioFetchParams,
 ) -> _MatchingAudio:
-    # Get any DB transcript
-    db_transcript = db_models.Transcript.collection.filter(
-        "session_ref", "==", fetch_params.session_key
-    ).get()
-
-    # Get transcript file info
-    db_transcript_file = db_transcript.file_ref.get()
-
-    # Strip the transcript details from filename
-    # Audio files are stored with the same URI as the transcript
-    # but instead of `-cdp_{version}-transcript.json`
-    # they simply end with `-audio.wav`
-    transcript_uri_parts = db_transcript_file.uri.split("/")
-    transcript_filename = transcript_uri_parts[-1]
-    uri_base = "/".join(transcript_uri_parts[:-1])
-    session_content_hash = transcript_filename[:64]
-    audio_uri = "/".join([uri_base, f"{session_content_hash}-audio.wav"])
-
-    # Handle cache dir
-    this_audio_cache_dir = (
-        fetch_params.parent_cache_dir
-        / f"event-{fetch_params.event_id}"
-        / f"session-{fetch_params.session_id}"
-    )
-    # Create cache dir (Handle try except because threaded)
     try:
-        this_audio_cache_dir.mkdir(parents=True, exist_ok=True)
-    except FileExistsError:
-        pass
-
-    # Download audio if needed
-    save_path = this_audio_cache_dir / "audio.wav"
-    if save_path.is_dir():
-        raise IsADirectoryError(
-            f"Audio '{audio_uri}', could not be saved because "
-            f"'{save_path}' is a directory. Delete or move the directory to a "
-            f"different location or change the target dataset cache dir."
-        )
-    elif save_path.is_file():
-        log.debug(
-            f"Skipping audio '{audio_uri}'. "
-            f"A file already exists at target save path."
-        )
-    else:
-        fetch_params.fs.get(audio_uri, str(save_path))
-
-    return _MatchingAudio(
-        session_key=fetch_params.session_key,
-        audio_path=save_path,
-    )
+        # Get any DB transcript
+        db_transcript = db_models.Transcript.collection.filter(
+            "session_ref", "==", fetch_params.session_key
+        ).get()
+
+        # Get transcript file info
+        db_transcript_file = db_transcript.file_ref.get()
+
+        # Strip the transcript details from filename
+        # Audio files are stored with the same URI as the transcript
+        # but instead of `-cdp_{version}-transcript.json`
+        # they simply end with `-audio.wav`
+        transcript_uri_parts = db_transcript_file.uri.split("/")
+        transcript_filename = transcript_uri_parts[-1]
+        uri_base = "/".join(transcript_uri_parts[:-1])
+        session_content_hash = transcript_filename[:64]
+        audio_uri = "/".join([uri_base, f"{session_content_hash}-audio.wav"])
+
+        # Handle cache dir
+        this_audio_cache_dir = (
+            fetch_params.parent_cache_dir
+            / f"event-{fetch_params.event_id}"
+            / f"session-{fetch_params.session_id}"
+        )
+        # Create cache dir (Handle try except because threaded)
+        try:
+            this_audio_cache_dir.mkdir(parents=True, exist_ok=True)
+        except FileExistsError:
+            pass
+
+        # Download audio if needed
+        save_path = this_audio_cache_dir / "audio.wav"
+        if save_path.is_dir():
+            raise IsADirectoryError(
+                f"Audio '{audio_uri}', could not be saved because "
+                f"'{save_path}' is a directory. Delete or move the directory to a "
+                f"different location or change the target dataset cache dir."
+            )
+        elif save_path.is_file():
+            log.debug(
+                f"Skipping audio '{audio_uri}'. "
+                f"A file already exists at target save path."
+            )
+        else:
+            fetch_params.fs.get(audio_uri, str(save_path))
+
+        return _MatchingAudio(
+            session_key=fetch_params.session_key,
+            audio_path=save_path,
+        )
+
+    except Exception:
+        if fetch_params.raise_on_error:
+            raise FileNotFoundError(
+                f"Something went wrong while fetching the video for session: "
+                f"'{fetch_params.session_id}' from '{fetch_params.fs.project}' "
+                f"Please check if a report has already been made to GitHub "
+                f"(https://github.com/CouncilDataProject/cdp-data/issues). "
+                f"If you cannot find an open issue for this session, "
+                f"please create a new one. "
+                f"In the meantime, please try rerunning your request with "
+                f"`raise_on_error=False`"
+            )
+
+        return _MatchingAudio(
+            session_key=fetch_params.session_key,
+            audio_path=None,
+        )
 
 
 @dataclass
 class _TranscriptFetchParams:
     session_id: str
     session_key: str
     event_id: str
     transcript_selection: str
     parent_cache_dir: Path
     fs: GCSFileSystem
+    raise_on_error: bool
 
 
 @dataclass_json
 @dataclass
 class _MatchingTranscript:
     session_key: str
-    transcript: db_models.Transcript
-    transcript_path: Path
+    transcript: Optional[db_models.Transcript]
+    transcript_path: Optional[Path]
 
 
 def _get_matching_db_transcript(
     fetch_params: _TranscriptFetchParams,
 ) -> _MatchingTranscript:
-    # Get DB transcript
-    db_transcript = (
-        db_models.Transcript.collection.filter(
-            "session_ref", "==", fetch_params.session_key
-        )
-        .order(f"-{fetch_params.transcript_selection}")
-        .get()
-    )
-
-    # Get transcript file info
-    db_transcript_file = db_transcript.file_ref.get()
-
-    # Handle cache dir
-    this_transcript_cache_dir = (
-        fetch_params.parent_cache_dir
-        / f"event-{fetch_params.event_id}"
-        / f"session-{fetch_params.session_id}"
-    )
-    # Create cache dir (Handle try except because threaded)
     try:
-        this_transcript_cache_dir.mkdir(parents=True, exist_ok=True)
-    except FileExistsError:
-        pass
-
-    # Download transcript if needed
-    save_path = this_transcript_cache_dir / "transcript.json"
-    if save_path.is_dir():
-        raise IsADirectoryError(
-            f"Transcript '{db_transcript_file.uri}', could not be saved because "
-            f"'{save_path}' is a directory. Delete or move the directory to a "
-            f"different location or change the target dataset cache dir."
-        )
-    elif save_path.is_file():
-        log.debug(
-            f"Skipping transcript '{db_transcript_file.uri}'. "
-            f"A file already exists at target save path."
-        )
-    else:
-        fetch_params.fs.get(db_transcript_file.uri, str(save_path))
-
-    return _MatchingTranscript(
-        session_key=fetch_params.session_key,
-        transcript=db_transcript,
-        transcript_path=save_path,
-    )
+        # Get DB transcript
+        db_transcript = (
+            db_models.Transcript.collection.filter(
+                "session_ref", "==", fetch_params.session_key
+            )
+            .order(f"-{fetch_params.transcript_selection}")
+            .get()
+        )
+
+        # Get transcript file info
+        db_transcript_file = db_transcript.file_ref.get()
+
+        # Handle cache dir
+        this_transcript_cache_dir = (
+            fetch_params.parent_cache_dir
+            / f"event-{fetch_params.event_id}"
+            / f"session-{fetch_params.session_id}"
+        )
+        # Create cache dir (Handle try except because threaded)
+        try:
+            this_transcript_cache_dir.mkdir(parents=True, exist_ok=True)
+        except FileExistsError:
+            pass
+
+        # Download transcript if needed
+        save_path = this_transcript_cache_dir / "transcript.json"
+        if save_path.is_dir():
+            raise IsADirectoryError(
+                f"Transcript '{db_transcript_file.uri}', could not be saved because "
+                f"'{save_path}' is a directory. Delete or move the directory to a "
+                f"different location or change the target dataset cache dir."
+            )
+        elif save_path.is_file():
+            log.debug(
+                f"Skipping transcript '{db_transcript_file.uri}'. "
+                f"A file already exists at target save path."
+            )
+        else:
+            fetch_params.fs.get(db_transcript_file.uri, str(save_path))
+
+        return _MatchingTranscript(
+            session_key=fetch_params.session_key,
+            transcript=db_transcript,
+            transcript_path=save_path,
+        )
+
+    except Exception:
+        if fetch_params.raise_on_error:
+            raise FileNotFoundError(
+                f"Something went wrong while fetching the video for session: "
+                f"'{fetch_params.session_id}' from '{fetch_params.fs.project}' "
+                f"Please check if a report has already been made to GitHub "
+                f"(https://github.com/CouncilDataProject/cdp-data/issues). "
+                f"If you cannot find an open issue for this session, "
+                f"please create a new one. "
+                f"In the meantime, please try rerunning your request with "
+                f"`raise_on_error=False`"
+            )
+
+        return _MatchingTranscript(
+            session_key=fetch_params.session_key,
+            transcript=None,
+            transcript_path=None,
+        )
 
 
 def _merge_dataclasses_to_df(
     data_objs: List[dataclass_json],
     df: pd.DataFrame,
     data_objs_key: str,
     df_key: str,
@@ -373,14 +435,16 @@
     store_full_metadata: bool = False,
     store_transcript: bool = False,
     transcript_selection: str = "confidence",
     store_transcript_as_csv: bool = False,
     store_video: bool = False,
     store_audio: bool = False,
     cache_dir: Optional[Union[str, Path]] = None,
+    raise_on_error: bool = True,
+    tqdm_kws: Dict[str, Any] = {},
 ) -> pd.DataFrame:
     """
     Get a dataset of sessions from a CDP infrastructure.
 
     Parameters
     ----------
     infrastructure_slug: str
@@ -424,14 +488,20 @@
         Should the session audio be requested and stored to disk and a path to the
         stored audio file be added to the returned DataFrame.
         Default: False (do not request and store the audio)
     cache_dir: Optional[Union[str, Path]]
         An optional directory path to cache the dataset. Directory is created if it
         does not exist.
         Default: "./cdp-datasets"
+    raise_on_error: bool
+        Should any failure to pull files result in an error or be ignored.
+        Default: True (raise on any failure)
+    tqdm_kws: Dict[str, Any]
+        A dictionary with extra keyword arguments to provide to tqdm progress
+        bars. Must not include the `desc` keyword argument.
 
     Returns
     -------
     dataset: pd.DataFrame
         The dataset with all additions requested.
 
     Notes
@@ -516,14 +586,15 @@
 
     # Handle basic event metadata attachment
     log.info("Attaching event metadata to each session datum")
     sessions = db_utils.load_model_from_pd_columns(
         sessions,
         join_id_col="id",
         model_ref_col="event_ref",
+        tqdm_kws=tqdm_kws,
     )
 
     # We only need to handle cache dir and more if any extras are True
     if not any(
         [
             store_full_metadata,
             store_transcript,
@@ -556,53 +627,58 @@
             [
                 _VideoFetchParams(
                     session_id=row.id,
                     session_key=row.key,
                     event_id=row.event.id,
                     video_uri=row.video_uri,
                     parent_cache_dir=cache_dir,
+                    fs=fs,
+                    raise_on_error=raise_on_error,
                 )
                 for _, row in sessions.iterrows()
             ],
             desc="Fetching videos",
+            **tqdm_kws,
         )
 
         # Merge fetched data back to session df
         sessions = _merge_dataclasses_to_df(
             data_objs=fetched_video_infos,
             df=sessions,
             data_objs_key="session_key",
             df_key="key",
-        )
+        ).dropna(subset=["video_path"])
 
     # Handle audio
     if store_audio:
         log.info("Fetching audio")
         fetched_audio_infos = thread_map(
             _get_matching_audio,
             [
                 _AudioFetchParams(
                     session_id=row.id,
                     session_key=row.key,
                     event_id=row.event.id,
                     parent_cache_dir=cache_dir,
                     fs=fs,
+                    raise_on_error=raise_on_error,
                 )
                 for _, row in sessions.iterrows()
             ],
             desc="Fetching audios",
+            **tqdm_kws,
         )
 
         # Merge fetched data back to session df
         sessions = _merge_dataclasses_to_df(
             data_objs=fetched_audio_infos,
             df=sessions,
             data_objs_key="session_key",
             df_key="key",
-        )
+        ).dropna(subset=["audio_path"])
 
     # Pull transcript info
     if store_transcript:
         log.info("Fetching transcripts")
         # Threaded get of transcript info
         fetched_transcript_infos = thread_map(
             _get_matching_db_transcript,
@@ -610,41 +686,38 @@
                 _TranscriptFetchParams(
                     session_id=row.id,
                     session_key=row.key,
                     event_id=row.event.id,
                     transcript_selection=transcript_selection,
                     parent_cache_dir=cache_dir,
                     fs=fs,
+                    raise_on_error=raise_on_error,
                 )
                 for _, row in sessions.iterrows()
             ],
             desc="Fetching transcripts",
+            **tqdm_kws,
         )
 
         # Merge fetched data back to session df
         sessions = _merge_dataclasses_to_df(
             data_objs=fetched_transcript_infos,
             df=sessions,
             data_objs_key="session_key",
             df_key="key",
-        )
-
-        def _wrapped_transcript_converter(transcript_path: Path) -> Path:
-            transcript_df = convert_transcript_to_dataframe(transcript_path)
-            dest = transcript_path.with_suffix(".csv")
-            transcript_df.to_csv(dest, index=False)
-            return dest
+        ).dropna(subset=["transcript_path"])
 
         # Handle conversion of transcripts to CSVs
         if store_transcript_as_csv:
             log.info("Converting and storing transcripts as CSVs")
             rows_with_csv_paths: List[pd.Series] = []
             for _, row in tqdm(
                 sessions.iterrows(),
                 desc="Converting and storing each transcript as a CSV",
+                **tqdm_kws,
             ):
                 # Convert
                 transcript_df = convert_transcript_to_dataframe(row["transcript_path"])
 
                 # Get storage name
                 dest = row["transcript_path"].with_suffix(".csv")
                 transcript_df.to_csv(dest, index=False)
@@ -724,14 +797,15 @@
 
 
 def get_vote_dataset(
     infrastructure_slug: str,
     start_datetime: Optional[Union[str, datetime]] = None,
     end_datetime: Optional[Union[str, datetime]] = None,
     replace_py_objects: bool = False,
+    tqdm_kws: Dict[str, Any] = {},
 ) -> pd.DataFrame:
     """
     Get a dataset of votes from a CDP infrastructure.
 
     Parameters
     ----------
     infrastructure_slug: str
@@ -743,14 +817,17 @@
         An optional datetime that the vote dataset will end at.
         Default: None (no datetime end bound on the dataset)
     replace_py_objects: bool
         Replace any non-standard Python type with standard ones to
         allow the returned data be ready for storage.
         See 'See Also' for more details.
         Default: False (keep Python objects in the DataFrame)
+    tqdm_kws: Dict[str, Any]
+        A dictionary with extra keyword arguments to provide to tqdm progress
+        bars. Must not include the `desc` keyword argument.
 
     Returns
     -------
     pd.DataFrame
         The dataset requested.
 
     See Also
@@ -781,14 +858,15 @@
 
     # Thread fetch votes for each event
     log.info("Fetching votes for each event")
     fetched_votes_frames = thread_map(
         _get_votes_for_event,
         [e.key for e in events],
         desc="Fetching votes for each event",
+        **tqdm_kws,
     )
     votes = pd.concat(fetched_votes_frames)
 
     # If no votes are found, return empty dataset
     if len(votes) == 0:
         return pd.DataFrame(
             columns=[
@@ -822,107 +900,117 @@
 
     # Thread fetch events for each vote
     log.info("Attaching event metadata to each vote datum")
     votes = db_utils.load_model_from_pd_columns(
         votes,
         join_id_col="id",
         model_ref_col="event_ref",
+        tqdm_kws=tqdm_kws,
     )
 
     # Thread fetch matters for each vote
     log.info("Attaching matter metadata to each vote datum")
     votes = db_utils.load_model_from_pd_columns(
         votes,
         join_id_col="id",
         model_ref_col="matter_ref",
+        tqdm_kws=tqdm_kws,
     )
 
     # Thread fetch event minutes items for each vote
     log.info("Attaching event minutes item metadata to each vote datum")
     votes = db_utils.load_model_from_pd_columns(
         votes,
         join_id_col="id",
         model_ref_col="event_minutes_item_ref",
+        tqdm_kws=tqdm_kws,
     )
 
     # Thread fetch people for each vote
     log.info("Attaching person metadata to each vote datum")
     votes = db_utils.load_model_from_pd_columns(
         votes,
         join_id_col="id",
         model_ref_col="person_ref",
+        tqdm_kws=tqdm_kws,
     )
 
     # Expand event models
     votes = db_utils.expand_models_from_pd_column(
         votes,
         model_col="event",
         model_attr_rename_lut={
             "id": "event_id",
             "key": "event_key",
             "body_ref": "body_ref",
             "event_datetime": "event_datetime",
             "agenda_uri": "agenda_uri",
             "minutes_uri": "minutes_uri",
         },
+        tqdm_kws=tqdm_kws,
     )
 
     # Expand matter models
     votes = db_utils.expand_models_from_pd_column(
         votes,
         model_col="matter",
         model_attr_rename_lut={
             "id": "matter_id",
             "key": "matter_key",
             "name": "matter_name",
             "matter_type": "matter_type",
             "title": "matter_title",
         },
+        tqdm_kws=tqdm_kws,
     )
 
     # Expand event minutes item models
     votes = db_utils.expand_models_from_pd_column(
         votes,
         model_col="event_minutes_item",
         model_attr_rename_lut={
             "id": "event_minutes_item_id",
             "key": "event_minutes_item_key",
             "index": "event_minutes_item_index_in_meeting",
             "decision": "event_minutes_item_overall_decision",
         },
+        tqdm_kws=tqdm_kws,
     )
 
     # Expand person models
     votes = db_utils.expand_models_from_pd_column(
         votes,
         model_col="person",
         model_attr_rename_lut={
             "id": "person_id",
             "key": "person_key",
             "name": "person_name",
         },
+        tqdm_kws=tqdm_kws,
     )
 
     # Thread fetch body for each vote
     log.info("Attaching body metadata to each vote datum")
     votes = db_utils.load_model_from_pd_columns(
         votes,
         join_id_col="id",
         model_ref_col="body_ref",
+        tqdm_kws=tqdm_kws,
     )
 
     # Expand body models
     votes = db_utils.expand_models_from_pd_column(
         votes,
         model_col="body",
         model_attr_rename_lut={
             "id": "body_id",
             "key": "body_key",
             "name": "body_name",
         },
+        tqdm_kws=tqdm_kws,
     )
 
     # Replace col values with storage ready replacements
     if replace_py_objects:
         votes = replace_dataframe_cols_with_storage_replacements(votes)
 
     return votes
```

### Comparing `cdp-data-0.0.8/cdp_data/instances.py` & `cdp-data-0.0.9/cdp_data/instances.py`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/cdp_data/keywords.py` & `cdp-data-0.0.9/cdp_data/keywords.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import logging
 from collections import Counter
 from dataclasses import dataclass
 from datetime import datetime
 from functools import partial
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import pandas as pd
 from cdp_backend.database import models as db_models
 from cdp_backend.pipeline.transcript_model import Transcript
 from cdp_backend.utils.string_utils import clean_text
 from nltk import ngrams
 from nltk.stem import SnowballStemmer
@@ -260,14 +260,15 @@
     return counts
 
 
 def _compute_ngram_usage_history(
     data: pd.DataFrame,
     ngram_size: int = 1,
     strict: bool = False,
+    tqdm_kws: Dict[str, Any] = {},
 ) -> pd.DataFrame:
     """
     Compute all ngrams usage history for the provided session dataset.
     This data can be used to plot how much of a CDP instance's discussion is comprised
     of specific keywords.
 
     Parameters
@@ -276,14 +277,17 @@
         The session dataset to process and compute history for.
     ngram_size: int
         The ngram size to use for counting and calculating usage.
         Default: 1 (unigrams)
     strict: bool
         Should all ngrams be stemmed or left unstemmed for a more strict usage history.
         Default: False (stem and clean all grams in the dataset)
+    tqdm_kws: Dict[str, Any]
+        A dictionary with extra keyword arguments to provide to tqdm progress
+        bars. Must not include the `desc` keyword argument.
 
     Returns
     -------
     ngram_history: pd.DataFrame
         A pandas DataFrame of all found ngrams (stemmed and cleaned or unstemmed and
         uncleaned) from the data and their counts for each session and their percentage
         of use as a percent of their use for the day over the sum of all other ngrams
@@ -322,14 +326,15 @@
                     session_id=row.id,
                     session_datetime=row.session_datetime,
                     transcript_path=row.transcript_path,
                 )
                 for _, row in data.iterrows()
             ],
             desc="Counting ngrams in each transcript",
+            **tqdm_kws,
         )
     )
 
     # Make a column for just date
     counts["session_date"] = pd.to_datetime(counts["session_datetime"]).dt.date
 
     # Group by gram and compute combined usage for day
@@ -353,14 +358,16 @@
 def compute_ngram_usage_history(
     infrastructure_slug: Union[str, List[str]],
     ngram_size: int = 1,
     strict: bool = False,
     start_datetime: Optional[Union[str, datetime]] = None,
     end_datetime: Optional[Union[str, datetime]] = None,
     cache_dir: Optional[Union[str, Path]] = None,
+    raise_on_error: bool = True,
+    tqdm_kws: Dict[str, Any] = {},
 ) -> pd.DataFrame:
     """
     Pull the minimal data needed for a session dataset for the provided infrastructure
     and start and end datetimes, then compute the ngram usage history DataFrame.
 
     Parameters
     ----------
@@ -378,14 +385,20 @@
     end_datetime: Optional[Union[str, datetime]]
         An optional datetime that the session dataset will end at.
         Default: None (no datetime end bound on the dataset)
     cache_dir: Optional[Union[str, Path]]
         An optional directory path to cache the dataset. Directory is created if it
         does not exist.
         Default: "./cdp-datasets"
+    raise_on_error: bool
+        Should any failure to pull files result in an error or be ignored.
+        Default: True (raise on any failure)
+    tqdm_kws: Dict[str, Any]
+        A dictionary with extra keyword arguments to provide to tqdm progress
+        bars. Must not include the `desc` keyword argument.
 
     Returns
     -------
     gram_usage: pd.DataFrame
         A pandas DataFrame of all found ngrams (stemmed and cleaned or unstemmed and
         uncleaned) from the data and their counts for each session and their percentage
         of use as a percent of their use for the day over the sum of all other ngrams
@@ -415,32 +428,37 @@
         infrastructure_slug = [infrastructure_slug]
 
     # Create dataframe for all histories
     gram_usage = []
 
     # Start collecting datasets for each infrastructure
     for infra_slug in tqdm(
-        infrastructure_slug, "Counting ngrams for each infrastructure"
+        infrastructure_slug,
+        desc="Counting ngrams for each infrastructure",
+        **tqdm_kws,
     ):
         # Get the dataset
         log.info(f"Getting session dataset for {infra_slug}")
         infra_ds = datasets.get_session_dataset(
             infrastructure_slug=infra_slug,
             start_datetime=start_datetime,
             end_datetime=end_datetime,
             store_transcript=True,
             cache_dir=cache_dir,
+            raise_on_error=raise_on_error,
+            tqdm_kws=tqdm_kws,
         )
 
         # Compute ngram usages for infra
         log.info(f"Computing ngram history for {infra_slug}")
         infra_gram_usage = _compute_ngram_usage_history(
             infra_ds,
             ngram_size=ngram_size,
             strict=strict,
+            tqdm_kws=tqdm_kws,
         )
         infra_gram_usage["infrastructure"] = infra_slug
         gram_usage.append(infra_gram_usage)
 
     # Convert gram histories to single dataframe
     return pd.concat(gram_usage)
 
@@ -483,27 +501,30 @@
     )
 
 
 def _compute_query_semantic_similarity_history(
     data: pd.DataFrame,
     query_vec: "Tensor",
     model: "SentenceTransformer",
+    tqdm_kws: Dict[str, Any] = {},
 ) -> pd.DataFrame:
     # Construct partial for threaded counter func
     process_func = partial(
         _compute_transcript_sim_stats,
         query_vec=query_vec,
         model=model,
     )
 
     # Compute min, max, and mean cos_sim using the sentences
     # of each transcript
     sim_stats_list: List[pd.DataFrame] = []
     for _, row in tqdm(
-        data.iterrows(), "Computing semantic similarity for each transcript"
+        data.iterrows(),
+        desc="Computing semantic similarity for each transcript",
+        **tqdm_kws,
     ):
         sim_stats_list.append(
             process_func(
                 _TranscriptProcessingParams(
                     session_id=row.id,
                     session_datetime=row.session_datetime,
                     transcript_path=row.transcript_path,
@@ -536,14 +557,16 @@
 def compute_query_semantic_similarity_history(
     query: Union[str, List[str]],
     infrastructure_slug: Union[str, List[str]],
     start_datetime: Optional[Union[str, datetime]] = None,
     end_datetime: Optional[Union[str, datetime]] = None,
     cache_dir: Optional[Union[str, Path]] = None,
     embedding_model: str = "msmarco-distilbert-base-v4",
+    raise_on_error: bool = True,
+    tqdm_kws: Dict[str, Any] = {},
 ) -> pd.DataFrame:
     """
     Compute the semantic similarity of a query against every sentence of every meeting.
     The max, min, and mean semantic similarity of each meeting will be returned.
 
     Parameters
     ----------
@@ -563,15 +586,21 @@
         Default: "./cdp-datasets"
     embedding_model: str
         The sentence transformers model to use for embedding the query and
         each sentence.
         Default: "msmarco-distilbert-base-v4"
         All embedding models are available here:
         https://www.sbert.net/docs/pretrained-models/msmarco-v3.html
-        Select any of the "Models tuned for cosine-similarity".
+        Select any of the "Models tuned for cosine-similarity".'
+    raise_on_error: bool
+        Should any failure to pull files result in an error or be ignored.
+        Default: True (raise on any failure)
+    tqdm_kws: Dict[str, Any]
+        A dictionary with extra keyword arguments to provide to tqdm progress
+        bars. Must not include the `desc` keyword argument.
 
     Returns
     -------
     pd.DataFrame
         The min, max, and mean semantic similarity for each event as compared
         to the query for the events within the datetime range.
 
@@ -599,37 +628,46 @@
     model = SentenceTransformer(embedding_model)
 
     # Create dataframe for all histories
     semantic_histories = []
 
     # Start collecting datasets for each infrastructure
     for infra_slug in tqdm(
-        infrastructure_slug, "Computing semantic similarity for each infrastructure"
+        infrastructure_slug,
+        desc="Computing semantic similarity for each infrastructure",
+        **tqdm_kws,
     ):
         # Get the dataset
         log.info(f"Getting session dataset for {infra_slug}")
         infra_ds = datasets.get_session_dataset(
             infrastructure_slug=infra_slug,
             start_datetime=start_datetime,
             end_datetime=end_datetime,
             store_transcript=True,
             cache_dir=cache_dir,
+            raise_on_error=raise_on_error,
+            tqdm_kws=tqdm_kws,
         )
 
-        for q in tqdm(query, "Computing semantic similarlity for each query"):
+        for q in tqdm(
+            query,
+            desc="Computing semantic similarlity for each query",
+            **tqdm_kws,
+        ):
             # Get query embedding
             query_vec = model.encode(q)
 
             # Compute semantic similarity for query
             log.info(f"Computing semantic similary history for {infra_slug}")
             infra_query_semantic_sim_history = (
                 _compute_query_semantic_similarity_history(
                     data=infra_ds,
                     query_vec=query_vec,
                     model=model,
+                    tqdm_kws=tqdm_kws,
                 )
             )
             infra_query_semantic_sim_history["infrastructure"] = infra_slug
             infra_query_semantic_sim_history["query"] = q
             semantic_histories.append(infra_query_semantic_sim_history)
 
     # Convert gram histories to single dataframe
```

### Comparing `cdp-data-0.0.8/cdp_data/plots.py` & `cdp-data-0.0.9/cdp_data/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,15 @@
 
 
 def plot_ngram_usage_histories(
     ngram: Union[str, List[str]],
     gram_usage: pd.DataFrame,
     strict: bool = False,
     lmplot_kws: Dict[str, Any] = {},
+    tqdm_kws: Dict[str, Any] = {},
 ) -> "sns.FacetGrid":
     """
     Select and plot specific ngram usage histories from the provided gram usage
     DataFrame.
 
     Parameters
     ----------
@@ -257,14 +258,17 @@
         of use as a percent of their use for the day over the sum of all other ngrams
         used that day.
     strict: bool
         Should all ngrams be stemmed or left unstemmed for a more strict usage history.
         Default: False (stem and clean all grams in the dataset)
     lmplot_kws: Dict[str, Any]
         Any extra kwargs to provide to sns.lmplot.
+    tqdm_kws: Dict[str, Any]
+        A dictionary with extra keyword arguments to provide to tqdm progress
+        bars. Must not include the `desc` keyword argument.
 
     Returns
     -------
     grid: sns.FacetGrid
         The small multiples FacetGrid of all ngrams and infrastructures found in the
         provided dataset.
 
@@ -283,15 +287,19 @@
     # TODO:
     # Add keyword grouping??
 
     # Store prepared subsets
     gram_histories = []
 
     # Process the grams for the infrastructure
-    for gram in tqdm(ngram, "Preparing plotting data for each ngram"):
+    for gram in tqdm(
+        ngram,
+        desc="Preparing plotting data for each ngram",
+        **tqdm_kws,
+    ):
         gram_history = _prepare_ngram_usage_history_plotting_data(
             gram,
             data=gram_usage,
             strict=strict,
         )
 
         # Attach this gram history to all
```

### Comparing `cdp-data-0.0.8/cdp_data/tests/conftest.py` & `cdp-data-0.0.9/cdp_data/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/cdp_data/tests/test_datasets.py` & `cdp-data-0.0.9/cdp_data/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/cdp_data/tests/test_keywords_and_plotting.py` & `cdp-data-0.0.9/cdp_data/tests/test_keywords_and_plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 ###############################################################################
 
 
 def test_ngrams() -> None:
     ngram_usage = keywords.compute_ngram_usage_history(
         CDPInstances.Seattle,
         start_datetime="2021-01-01",
-        end_datetime="2021-02-01",
+        end_datetime="2021-01-10",
     )
     grid = plots.plot_ngram_usage_histories(
-        ["police", "housing", "transportation"],
+        ["police", "housing"],
         ngram_usage,
     )
     grid.savefig("test-generated-ngram-usage-histories-plot.pdf")
 
     # Or with extra kwargs like order
     grid_third_order = plots.plot_ngram_usage_histories(
         ["police", "housing", "transportation"],
@@ -28,19 +28,18 @@
 
 
 def test_semantic_sim() -> None:
     semantic_hist = keywords.compute_query_semantic_similarity_history(
         [
             "defund the police",
             "missing middle housing",
-            "vision zero and traffic fatalities",
         ],
         CDPInstances.Seattle,
         start_datetime="2021-01-01",
-        end_datetime="2021-01-20",
+        end_datetime="2021-01-10",
     )
     grid = plots.plot_query_semantic_similarity_history(
         semantic_hist,
     )
     grid.savefig("test-generated-semantic-sim-histories-plot.pdf")
 
     # Or with extra kwargs like order
```

### Comparing `cdp-data-0.0.8/cdp_data/tests/utils/test_incremental_average.py` & `cdp-data-0.0.9/cdp_data/tests/utils/test_incremental_average.py`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/cdp_data/utils/db_utils.py` & `cdp-data-0.0.9/cdp_data/utils/db_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from dataclasses import dataclass
 from functools import lru_cache
-from typing import Dict, List
+from typing import Any, Dict, List
 
 import fireo
 import pandas as pd
 from dataclasses_json import dataclass_json
 from fireo.models import Model
 from google.auth.credentials import AnonymousCredentials
 from google.cloud.firestore import Client
@@ -113,14 +113,15 @@
 
 
 def load_model_from_pd_columns(
     data: pd.DataFrame,
     join_id_col: str,
     model_ref_col: str,
     drop_original_model_ref: bool = True,
+    tqdm_kws: Dict[str, Any] = {},
 ) -> pd.DataFrame:
     """
     Load a model reference and attach the loaded model back to the original DataFrame.
 
     Parameters
     ----------
     data: pd.DataFrame
@@ -131,14 +132,17 @@
         loaded models DataFrame.
     model_ref_col: str
         The column name which contains the model ReferenceDocLoader objects.
     drop_original_model_ref: bool
         After loading and joining all models to the DataFrame, should the original
         `model_ref_col` be dropped.
         Default: True (drop the original `model_ref_column`)
+    tqdm_kws: Dict[str, Any]
+        A dictionary with extra keyword arguments to provide to tqdm progress
+        bars. Must not include the `desc` keyword argument.
 
     Returns
     -------
     data: pd.DataFrame
         A DataFrame with all of the original data and all the models loaded from the
         original DataFrame's `model_ref_col` ReferenceDocLoader objects.
 
@@ -182,14 +186,15 @@
             _ModelRefJoiner(
                 join_id=row[join_id_col],
                 model_ref=row[model_ref_col],
             )
             for _, row in data.iterrows()
         ],
         desc=f"Fetching each model attached to {model_ref_col}",
+        **tqdm_kws,
     )
 
     # Convert to dataframe
     models_to_join = pd.DataFrame([j.to_dict() for j in loaded_models])
 
     # Rename column to collection name
     models_to_join = models_to_join.rename(
@@ -207,22 +212,24 @@
     return joined
 
 
 def expand_models_from_pd_column(
     data: pd.DataFrame,
     model_col: str,
     model_attr_rename_lut: Dict[str, str],
+    tqdm_kws: Dict[str, Any] = {},
 ) -> pd.DataFrame:
     # Store individual rows
     expanded_data: List[pd.Series] = []
 
     # Iter rows and unpack
     for _, row in tqdm(
         data.iterrows(),
         desc=f"Expanding {model_col} models",
+        **tqdm_kws,
     ):
         for model_attr_name, attr_replace_name in model_attr_rename_lut.items():
             row[attr_replace_name] = getattr(row[model_col], model_attr_name)
 
         expanded_data.append(row)
 
     # New dataframe with expanded data
```

### Comparing `cdp-data-0.0.8/cdp_data/utils/incremental_average.py` & `cdp-data-0.0.9/cdp_data/utils/incremental_average.py`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/cdp_data.egg-info/PKG-INFO` & `cdp-data-0.0.9/cdp_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdp-data
-Version: 0.0.8
+Version: 0.0.9
 Summary: Data Utilities and Processing Generalized for All CDP Instances
 Author-email: "Eva Maxfield Brown, Council Data Project Contributors" <evamaxfieldbrown@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/CouncilDataProject/cdp-data
 Project-URL: Bug Tracker, https://github.com/CouncilDataProject/cdp-data/issues
 Project-URL: Documentation, https://CouncilDataProject.github.io/cdp-data
 Project-URL: User Support, https://github.com/CouncilDataProject/cdp-data/issues
```

### Comparing `cdp-data-0.0.8/cdp_data.egg-info/SOURCES.txt` & `cdp-data-0.0.9/cdp_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/cdp_data.egg-info/requires.txt` & `cdp-data-0.0.9/cdp_data.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 docutils<0.19,>=0.18
 
 [lint]
 black>=22.3.0
 check-manifest>=0.48
 flake8>=3.8.3
 flake8-debugger>=3.2.1
-flake8-pyprojecttoml
+flake8-pyprojecttoml==0.0.1
 flake8-typing-imports>=1.9.0
 isort>=5.7.0
 mypy>=0.790
 pre-commit>=2.20.0
 
 [plot]
 matplotlib>=3
```

### Comparing `cdp-data-0.0.8/docs/_static/header-keywords-over-time.png` & `cdp-data-0.0.9/docs/_static/header-keywords-over-time.png`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/docs/_static/seattle-keywords-over-time.png` & `cdp-data-0.0.9/docs/_static/seattle-keywords-over-time.png`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/docs/conf.py` & `cdp-data-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/docs/installation.rst` & `cdp-data-0.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/notebooks/historical_vote_proportions.ipynb` & `cdp-data-0.0.9/notebooks/historical_vote_proportions.ipynb`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/notebooks/plot_keyword_history.ipynb` & `cdp-data-0.0.9/notebooks/plot_keyword_history.ipynb`

 * *Files identical despite different names*

### Comparing `cdp-data-0.0.8/pyproject.toml` & `cdp-data-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
   "ipywidgets>=7.7.0",
 ]
 lint = [
   "black>=22.3.0",
   "check-manifest>=0.48",
   "flake8>=3.8.3",
   "flake8-debugger>=3.2.1",
-  "flake8-pyprojecttoml",
+  "flake8-pyprojecttoml==0.0.1",
   "flake8-typing-imports>=1.9.0",
   "isort>=5.7.0",
   "mypy>=0.790",
   "pre-commit>=2.20.0",
 ]
 test = [
   "coverage>=5.1",
```

### Comparing `cdp-data-0.0.8/scripts/generate-readme-figs.py` & `cdp-data-0.0.9/scripts/generate-readme-figs.py`

 * *Files identical despite different names*

