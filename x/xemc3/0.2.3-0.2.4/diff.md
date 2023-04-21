# Comparing `tmp/xemc3-0.2.3.tar.gz` & `tmp/xemc3-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xemc3-0.2.3.tar", last modified: Tue Apr 18 07:17:53 2023, max compression
+gzip compressed data, was "xemc3-0.2.4.tar", last modified: Fri Apr 21 06:56:10 2023, max compression
```

## Comparing `xemc3-0.2.3.tar` & `xemc3-0.2.4.tar`

### file list

```diff
@@ -1,88 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-18 07:17:39.000000 xemc3-0.2.3/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.167501 xemc3-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/black-fix.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/zenodo.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 07:17:39.000000 xemc3-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 07:17:39.000000 xemc3-0.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-18 07:17:39.000000 xemc3-0.2.3/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 07:17:39.000000 xemc3-0.2.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-18 07:17:39.000000 xemc3-0.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-18 07:17:53.175501 xemc3-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-18 07:17:39.000000 xemc3-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/citing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/cli.rst.in.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/evaluate_at.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/heatflux.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/info.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/load1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/load2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/setup_plt.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/docs/exercises/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/exercises/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/exercises/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/xemc3.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 07:17:39.000000 xemc3-0.2.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-18 07:17:39.000000 xemc3-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-18 07:17:39.000000 xemc3-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-18 07:17:53.175501 xemc3-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 07:17:39.000000 xemc3-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/xemc3/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 07:17:52.000000 xemc3-0.2.3/xemc3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/xemc3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/append_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/to_archive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      887 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/to_netcdf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/xdivertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/core/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/depo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/evaluate_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/plot_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/load/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/gen_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_average.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_load_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_write_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/tools/run_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/write/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/write/fortran.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/write/nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/xemc3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.568656 xemc3-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 06:55:53.000000 xemc3-0.2.4/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.556656 xemc3-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/black-fix.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-21 06:55:53.000000 xemc3-0.2.4/.github/workflows/zenodo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-21 06:55:53.000000 xemc3-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 06:55:53.000000 xemc3-0.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-21 06:55:53.000000 xemc3-0.2.4/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 06:55:53.000000 xemc3-0.2.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-21 06:55:53.000000 xemc3-0.2.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 06:56:10.568656 xemc3-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-21 06:55:53.000000 xemc3-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/cli.rst.in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/evaluate_at.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/heatflux.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/info.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/load1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/load2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples/setup_plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/docs/exercises/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/exercises/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/exercises/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-21 06:55:53.000000 xemc3-0.2.4/docs/xemc3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-21 06:55:53.000000 xemc3-0.2.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 06:55:53.000000 xemc3-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-21 06:55:53.000000 xemc3-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-21 06:56:10.568656 xemc3-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-21 06:55:53.000000 xemc3-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.560656 xemc3-0.2.4/xemc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/append_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/to_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      887 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/to_netcdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/cli/xdivertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/depo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/evaluate_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66317 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/plot_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/plot_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/gen_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_load_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/test/test_write_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/tools/run_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.568656 xemc3-0.2.4/xemc3/write/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/write/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:55:53.000000 xemc3-0.2.4/xemc3/write/nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:56:10.564656 xemc3-0.2.4/xemc3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 06:56:10.000000 xemc3-0.2.4/xemc3.egg-info/top_level.txt
```

### Comparing `xemc3-0.2.3/.github/workflows/black-fix.yml` & `xemc3-0.2.4/.github/workflows/black-fix.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/.github/workflows/python_publish.yml` & `xemc3-0.2.4/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/.github/workflows/test-python-package.yml` & `xemc3-0.2.4/.github/workflows/test-python-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -33,16 +33,19 @@
 
   build:
     runs-on: ubuntu-latest
     needs: download
     timeout-minutes: 15
     strategy:
       matrix:
-        python-version: ['3.6', '3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
         extra-install: ["", "numba"]
+        exclude:
+          - python-version: '3.11'
+            extra-install: 'numba'
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v2
     - name: Get Remote SHA
       id: get-sha
       run: |
```

### Comparing `xemc3-0.2.3/COPYING` & `xemc3-0.2.4/COPYING`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/Makefile` & `xemc3-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/PKG-INFO` & `xemc3-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xemc3
-Version: 0.2.3
+Version: 0.2.4
 Summary: Collect data from EMC3 runs in python using xarray
 Home-page: https://github.com/dschwoerer/xemc3
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Tracker, https://github.com/dschwoerer/xemc3/issues
 Project-URL: Documentation, https://xemc3.rtfd.io
```

### Comparing `xemc3-0.2.3/README.md` & `xemc3-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/cli.rst.in.py` & `xemc3-0.2.4/docs/cli.rst.in.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/conf.py` & `xemc3-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/examples/evaluate_at.ipynb` & `xemc3-0.2.4/docs/examples/evaluate_at.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/examples/get_data.py` & `xemc3-0.2.4/docs/examples/get_data.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/examples/heatflux.ipynb` & `xemc3-0.2.4/docs/examples/heatflux.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/examples/info.ipynb` & `xemc3-0.2.4/docs/examples/info.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/examples/introduction.ipynb` & `xemc3-0.2.4/docs/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/examples/load1.ipynb` & `xemc3-0.2.4/docs/examples/load1.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/examples/load2.ipynb` & `xemc3-0.2.4/docs/examples/load2.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/exercises/get_data.py` & `xemc3-0.2.4/docs/exercises/get_data.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/exercises/introduction.ipynb` & `xemc3-0.2.4/docs/exercises/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/index.rst` & `xemc3-0.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/introduction.rst` & `xemc3-0.2.4/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/xarray.rst` & `xemc3-0.2.4/docs/xarray.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/docs/xemc3.rst` & `xemc3-0.2.4/docs/xemc3.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/requirements.txt` & `xemc3-0.2.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/setup.cfg` & `xemc3-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/__init__.py` & `xemc3-0.2.4/xemc3/__init__.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/cli/_common.py` & `xemc3-0.2.4/xemc3/cli/_common.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/cli/append_time.py` & `xemc3-0.2.4/xemc3/cli/append_time.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/cli/to_archive.py` & `xemc3-0.2.4/xemc3/cli/to_archive.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/cli/to_netcdf.py` & `xemc3-0.2.4/xemc3/cli/to_netcdf.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/cli/xdivertor.py` & `xemc3-0.2.4/xemc3/cli/xdivertor.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/core/dataset.py` & `xemc3-0.2.4/xemc3/core/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Any, Mapping, Union
+from typing import Any, Mapping, Union, Optional
 import sys
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -232,15 +232,18 @@
             }
             phid = ds[self._get_alt_name("phi", "_dims")].data
             xd = ds[self._get_alt_name("x", "_dims")].data
 
             for key in var_list:
                 ds[key] = var_list[key][i]
             if len(phid.shape) == 1:
-                assert phid.shape == xd.shape
+                assert phid.shape == xd.shape, (
+                    f"Expected phi.shape = {phid.shape} == x.shape = {xd.shape} to match."
+                    + utils.raise_issue
+                )
                 for j in range(ds.dims["plate_ind"]):
                     yield ds.isel(
                         plate_ind=j, **{k: slice(None, v[j]) for k, v in crop.items()}
                     )
             else:
                 for j in range(ds.dims["plate_ind"]):
                     yield ds.isel(plate_ind=j)
@@ -391,15 +394,14 @@
         da = self.data[key]
         if len(da.dims) < 3:
             return da.plot(*args, **kw)
         # For 3D:
         from . import plot_3d
 
         if "plate_ind" in self.data.dims:
-            # assert args == []
             return plot_3d.divertor(self.data, key, *args, **kw)
 
         init = {}
         for k in "updownsym", "periodicity":
             if k in kw:
                 init[k] = kw.pop(k)
         vol = plot_3d.volume(self.data, **init)
@@ -433,15 +435,15 @@
                 attrs = ds[k].attrs
                 ds[k] = ds[k].mean(dim="time")
                 ds[k].attrs = attrs
         return ds
 
     def isel(
         self,
-        indexers: Mapping[str, Any] = None,
+        indexers: Optional[Mapping[str, Any]] = None,
         drop: bool = False,
         missing_dims: Union[
             Literal["raise"], Literal["warn"], Literal["ignore"]
         ] = "raise",
         **indexers_kwargs: Any,
     ) -> xr.Dataset:
         ds = self.data
@@ -474,26 +476,28 @@
                     else:
                         ds_[co] = ds[co]
                 ds = ds_
         return ds
 
     def sel(
         self,
-        indexers: Mapping[str, Any] = None,
+        indexers: Optional[Mapping[str, Any]] = None,
         drop: bool = False,
         missing_dims: str = "raise",
         **indexers_kwargs: Any,
     ) -> xr.Dataset:
         ds = self.data
         indexers = utils.merge_indexers(indexers, indexers_kwargs)
         forisel = {}
         for k in indexers.keys():
             val = indexers[k]
             if "delta_" + k in ds.dims and k + "_bounds" in ds:
-                assert k in ds.dims
+                assert (
+                    k in ds.dims
+                ), f"Expected {k} in {ds.dims} - maybe you already selected in {k} dim?"
                 assert (
                     len(ds[k + "_bounds"].dims) == 2
                 ), "Only 1D bounds are currently supported. Maybe try isel."
                 dat = ds[k + "_bounds"]
                 if dat.dims == (k, "delta_" + k):
                     pass
                 elif dat.T.dims == (k, "delta_" + k):
@@ -509,15 +513,17 @@
                 else:
                     raise RuntimeError(f"Didn't find {val} in {k}_bounds")
                 fac = (val - dat[i, 0]) / (dat[i, 1] - dat[i, 0])
                 forisel[k] = i + fac
             else:
                 forisel[k] = val
         ds = ds.emc3.isel(forisel)
-        assert isinstance(ds, xr.Dataset)
+        assert isinstance(
+            ds, xr.Dataset
+        ), f"Expected to have an xr.Dataset, but instead got {type(ds)}"
         return ds
 
     def evaluate_at_xyz(self, x, y, z, *args, **kwargs):
         """
         See evaluate_at_rpz for options. Unlike evaluate_at_rpz the
         coordinates are given here in cartesian coordinates.
         """
@@ -529,15 +535,15 @@
         self,
         r,
         phi,
         z,
         key=None,
         periodicity: int = 5,
         updownsym: bool = True,
-        delta_phi: float = None,
+        delta_phi: Optional[float] = None,
         fill_value=None,
         lazy=False,
         progress=False,
     ):
         """
         Evaluate the field key in the dataset at the positions given by
         the array r, phi, z.  If key is None, return the indices to access
```

### Comparing `xemc3-0.2.3/xemc3/core/depo.py` & `xemc3-0.2.4/xemc3/core/depo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import xarray as xr
 import numpy as np
 import re
 import typing
 
-from .utils import rrange
+from .utils import rrange, raise_issue
 
 
 if 0:
     import sparse  # type: ignore
 else:
     sparse = None
 
@@ -82,15 +82,18 @@
     haszone = "zone" in ds.dims
     if haszone:
         shape = len(ds.zone), *shape
         dims = "zone", *dims
 
     with open(fn) as f:
         line = f.readline().split()
-        assert len(line) == 2
+        assert len(line) == 2, (
+            f"Unexpected: `{line}` at start of `{fn}` - expected 2 elements"
+            + raise_issue
+        )
         blockasize = int(line[0])
         # Lines look like this:
         # Index
         # 3
         # type of the surface
         # index of zone
         # index of surface in radial
@@ -106,29 +109,36 @@
 
         hasother = hasother2 = False
         last = None
         for i in range(blockasize):
             line = bad.sub(r"\1E\2", f.readline()).split()
             ints = [int(x) for x in line[:7]]
             floats = [float(x) for x in line[7:]]
-            assert (
-                ints[0] == i + 1
-            ), f"Expected first index to be contigous, thus expected {i+1} but got {ints[0]}"
-            assert ints[1] == 3, f"Expected 3 but got {ints[1]}"
+            assert ints[0] == i + 1, (
+                f"Expected first index to be contigous, thus expected {i+1} but got {ints[0]} while reading {fn}"
+                + raise_issue
+            )
+            assert ints[1] == 3, (
+                f"Expected 3 but got {ints[1]} while reading `{fn}`." + raise_issue
+            )
             # print(ints[3:])
             if haszone:
                 slc = tuple(ints[3:])
             else:
-                assert ints[3] == 0, f"Expected zoneid=0 but got {ints[3]}"
+                assert ints[3] == 0, (
+                    f"Expected zoneid=0 but got {ints[3]}" + raise_issue
+                )
                 slc = tuple(ints[4:])
 
             for name, val in zip(varnames, (ints[2] == 1, floats[0])):
                 out[name][slc] = val
             if last:
-                assert not out["surftype"][last]
+                assert not out["surftype"][last], (
+                    f"Unexpected input in `{fn}`." + raise_issue
+                )
             if ints[2] != 1:
                 last = slc
             # print("a", out["surftype"][slc], ints[2] == 1)
 
             if len(floats) > 1:
                 hasother = True
                 for j in range(4):
@@ -144,46 +154,46 @@
 
         while True:
             line = bad.sub(r"\1E\2", f.readline()).split()
             if line == []:
                 break
             ints = [int(x) for x in line[:7]]
             floats = [float(x) for x in line[7:]]
-            assert ints[1] == 3, f"Expected 3 but got {ints[1]}"
+            assert ints[1] == 3, f"Expected 3 but got {ints[1]}" + raise_issue
             if haszone:
                 slc = tuple(ints[3:])
             else:
-                assert ints[3] == 0
+                assert ints[3] == 0, f"Unexpected input in {fn} `line`." + raise_issue
                 slc = tuple(ints[4:])
             for name, val in zip(varnames, (ints[2] == 1, floats[0])):
                 out2[name][slc] = val
             # print("b", out["surftype"][slc], ints[2] == 1)
 
             if len(floats) > 1:
                 hasother2 = True
                 for j in range(4):
                     out2["other"][j][slc] = floats[j + 1]
 
     if sparse:
-        assert any([d.nnz for d in out["other"]]) == hasother
-        assert any([d.nnz for d in out2["other"]]) == hasother2
+        assert any([d.nnz for d in out["other"]]) == hasother, raise_issue
+        assert any([d.nnz for d in out2["other"]]) == hasother2, raise_issue
     # if not hasother:
     # out["other"] = []
-    assert not hasother2
+    assert not hasother2, raise_issue
     out2["other"] = []
 
     ret = [
         xr.DataArray(data=tocoo(d), dims=dims)
         for d in [out["surftype"], out["flux"], *out["other"]]
     ], [
         xr.DataArray(data=tocoo(d), dims=dims)
         for d in [out2["surftype"], out2["flux"], *out2["other"]]
     ]
-    assert len(ret[0]) == 6, f"{len(ret[0])}"
-    assert len(ret[1]) == 2
+    assert len(ret[0]) == 6, f"Expected 6 items but got {len(ret[0])}." + raise_issue
+    assert len(ret[1]) == 2, raise_issue
     return ret[0] + ret[1]
 
 
 def write_depo_raw_part(datas, f, i):
     surf = datas[0].data
     dats = [d.data for d in datas[1:]]
     zone = [] if "zone" in datas[0].dims else [0]
@@ -204,15 +214,17 @@
             )
             + "\n"
         )
     return i
 
 
 def write_depo_raw(datas, fn):
-    assert len(datas) == 8, f"Expected 8 data entries, but got { len(datas) }"
+    assert len(datas) == 8, (
+        f"Expected 8 data entries, but got { len(datas) }" + raise_issue
+    )
     datas = datas[:6], datas[6:]
     i = 0
     with open(fn, "w") as f:
         f.write(
             f"      {nnz(datas[0][1].data):6d} "
             + (
                 f"{nnz(datas[1][1].data):11d}\n"
```

### Comparing `xemc3-0.2.3/xemc3/core/evaluate_at.py` & `xemc3-0.2.4/xemc3/core/evaluate_at.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import xarray as xr
 from eudist import PolyMesh  # type: ignore
 
 from . import utils
 
 
 def _evaluate_get_keys(ds, r, phi, z, periodicity, updownsym, delta_phi, progress):
-
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", "invalid value encountered in remainder")
         phi = phi % (np.pi * 2 / periodicity)
     # Get raw data
     dims, shape, coords, (r, phi, z) = get_out_shape(r, phi, z)
     pln = xr.Dataset()
     pln = pln.assign_coords({k: ds[k] for k in ["z_bounds", "R_bounds", "phi_bounds"]})
```

### Comparing `xemc3-0.2.3/xemc3/core/load.py` & `xemc3-0.2.4/xemc3/core/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import typing
 import uuid
 
 import numpy as np
 import xarray as xr
 
-from .utils import from_interval, open, prod, rrange, timeit, to_interval
+from .utils import from_interval, open, prod, rrange, timeit, to_interval, raise_issue
 from .depo import read_depo_raw, write_depo_raw
 
 try:
     from numba import jit  # type: ignore
 except ImportError:
 
     def jit(x):
@@ -231,22 +231,25 @@
     with open(fn) as f:
         last = None
         for i, line in enumerate(f):
             lines = [int(x) for x in line.split()]
             if last:
                 lines = last + lines
             zone, r, theta, num = lines[:4]
-            assert zone == 0
-            assert num % 2 == 0
+            if zone != 0:
+                raise ValueError(
+                    "Multiple zones are currently not supported." + raise_issue
+                )
+            assert num % 2 == 0, f"Unexpected input in {fn}:{i} `line`" + raise_issue
             if num + 4 > len(lines):
                 last = lines
                 continue
             assert num + 4 == len(lines), (
                 f"failed to parse line {i+1}{' (continued from previous incomplete line)' if last else ''}"
-                f" from {fn}: {' '.join([str(x) for x in lines])}"
+                f" from {fn}: {' '.join([str(x) for x in lines])}" + raise_issue
             )
             last = None
             for t in range(num // 2):
                 a, b = lines[4 + 2 * t : 6 + 2 * t]
                 ret[r, theta, a : b + 1] = True
     return xr.DataArray(data=ret, dims=("r", "theta", "phi"))
 
@@ -360,15 +363,15 @@
 
 
 def write_raw(da: xr.DataArray, fn: str) -> None:
     with open(fn, "w") as f:
         f.write(str(da.data))
 
 
-def read_locations(path: str, ds: xr.Dataset = None) -> xr.Dataset:
+def read_locations(path: str, ds: typing.Optional[xr.Dataset] = None) -> xr.Dataset:
     """
     Read locations from folder path and add to dataset (if given).
 
     Parameters
     ----------
     path : str
         folder from which to read
@@ -446,15 +449,15 @@
 
     Raises
     ------
     AssertionError
         if the file is not at the end.
     """
     test = _fromfile(f, dtype=float, count=2, sep=" ")
-    assert len(test) == 0, f"Expected EOF, but found more data in {fn}"
+    assert len(test) == 0, f"Expected EOF, but found more data in {fn}" + raise_issue
 
 
 def read_plate(filename: str) -> typing.Tuple[np.ndarray, ...]:
     """
     Read Target structures from a file that is in the Kisslinger
     format as used by EMC3. It returns the coordinates as plain array
     in the order or R, z, phi.
@@ -473,17 +476,19 @@
     np.ndarray
         the phi coordinate of the corners in radian
     """
     with open(filename) as f:
         # first line is a comment ...
         _ = next(f)
         setup = next(f).split()
-        assert len(setup) == 5, f"Expected 5 values but got {setup}"
+        assert len(setup) == 5, f"Expected 5 values but got {setup}" + raise_issue
         for zero in setup[3:]:
-            assert float(zero) == 0.0
+            assert float(zero) == 0.0, (
+                "A shifted divertor is currently not supported in xemc3." + raise_issue
+            )
         nx, ny, nz = [int(i) for i in setup[:3]]
         r = np.empty((nx, ny))
         z = np.empty((nx, ny))
         phi = np.empty(nx)
         for x in range(nx):
             phi[x] = float(next(f)) / 180 * np.pi
             for y in range(ny):
@@ -541,20 +546,26 @@
         dir = ""
     files = []
     with open(filename) as f:
         num = int(scrape(f))
         for _ in range(num):
             line = scrape(f)
             lines = line.split()
-            assert len(lines) == 3, f"Unexpected content in {filename}: {line}"
-            assert [int(x) for x in lines] == [
-                0,
-                -4,
-                1,
-            ], f"Unexpected content in {filename}: {line}"
+            assert len(lines) == 3, (
+                f"Unexpected content in {filename}:{line}." + raise_issue
+            )
+            if int(lines[0]) != 0:
+                raise ValueError(
+                    f"Only Kisslinger files are currently supported, not triangulated meshes - while reading {filename}:{line}"
+                )
+            # assert [int(x) for x in lines] == [
+            #     0,
+            #     -4,
+            #     1,
+            # ], f"Unexpected content in {filename}: {line}"
             files.append(dir + scrape(f).strip())
     return read_plate_nice(files)
 
 
 plate_prefix = "plate_"
 
 
@@ -576,15 +587,17 @@
     """
     rzp = read_plate(filename)
     out = xr.Dataset()
     for name, dat in zip(("R", "z", "phi"), rzp):
         if len(dat.shape) == 2:
             dims = ["phi", "x"]
         else:
-            assert len(dat.shape) == 1
+            assert len(dat.shape) == 1, (
+                f"Unexpected number of dimensions {dat.shape}." + raise_issue
+            )
             dims = ["phi"]
         out = out.assign_coords(
             {f"{plate_prefix}{name}": ([f"{plate_prefix}{d}_plus1" for d in dims], dat)}
         )
     for var, attrs in files["ADD_SF_N0"]["vars"].items():
         out[var].attrs.update(attrs)
 
@@ -612,30 +625,34 @@
     """
     with open(cwd + fn) as f:
         s = scrape(f).split()
         _, num_plates = [int(i) for i in s]
         plates = []
         for plate in range(num_plates):
             s = scrape(f).split()
-            assert len(s) == 2, f"{plate} : {s}"
+            assert len(s) == 2, (
+                f"Unexpected string `{s}` while reading {plate}." + raise_issue
+            )
             _, geom = s
             r, z, phi = read_plate(cwd + geom)
             nx, ny = r.shape
             nx -= 1
             ny -= 1
             s = scrape(f).split()
             total = np.array([float(i) for i in s])
             s = scrape(f).split()
             if len(s) == 3:
                 items, yref, xref = [int(i) for i in s]
                 nxr = nx * xref
                 nyr = ny * yref
                 mode = 2
             else:
-                assert len(s) == 2, f"Unexpected string `{s}` while reading {cwd + fn}"
+                assert len(s) == 2, (
+                    f"Unexpected string `{s}` while reading {cwd + fn}" + raise_issue
+                )
                 nyr, nxr = [int(i) for i in s]
                 xref = nxr // nx
                 yref = nyr // ny
                 items = nx * ny
                 mode = 1
 
             assert items == nx * ny
@@ -920,31 +937,34 @@
         A dataset with the required information
 
     Raises
     ------
     FileNotFoundError
         If the required info could not be read
     """
+    error = f"""Reading {fn+ ' ' if fn is not None else ''}mapped requires mapping information, but the required
+information in '{dir}' could not be found.  Ensure all files are present
+in the folder or pass in a dataset that contains the mapping
+information. Failed to open `%s`."""
     if dir == "":
         dir = "."
     if mapping is None:
         try:
             mapping = read_locations(dir)
-            if need_mapping:
-                mapping = read_fort_file(mapping, f"{dir}/fort.70", **files["fort.70"])
-        except FileNotFoundError:
-            raise FileNotFoundError(
-                f"""Reading {fn+ ' ' if fn is not None else ''} mapped requires mapping information, but the required
-information in '{dir}' could not be found.  Ensure all files are present
-in the folder or pass in a dataset that contains the mapping
-information."""
-            )
-    else:
-        if isinstance(mapping, xr.DataArray):
-            mapping = xr.Dataset(dict(_plasma_map=mapping))
+        except FileNotFoundError as e:
+            raise FileNotFoundError(33, error % e.filename)
+    if isinstance(mapping, xr.DataArray):
+        if mapping.name == "_plasma_map":
+            return xr.Dataset(dict(_plasma_map=mapping))
+    assert isinstance(mapping, xr.Dataset)
+    if need_mapping:
+        try:
+            mapping = read_fort_file(mapping, f"{dir}/fort.70", **files["fort.70"])
+        except FileNotFoundError as e:
+            raise FileNotFoundError(33, error % e.filename)
     return mapping
 
 
 def read_var(
     dir: str, var: str, ds: typing.Union[None, xr.Dataset, xr.DataArray] = None
 ) -> xr.Dataset:
     """
@@ -973,26 +993,29 @@
             continue
         for v in fd["vars"]:
             if v == var or (
                 v.endswith("%d")
                 and var.startswith(v[:-2])
                 and var[len(v[:-2]) :].isdigit()
             ):
-                ds = ensure_mapping(dir, ds, fd.get("type", "mapped") == "mapped")
+                ds = ensure_mapping(
+                    dir, ds, fd.get("type", "mapped") == "mapped", fn=fn
+                )
                 assert isinstance(ds, xr.Dataset)
                 return read_fort_file(ds, f"{dir}/{fn}", **fd)
     raise ValueError(f"Don't know how to read {var}")
 
 
 def read_mapped(
     fn: str,
     mapping: typing.Union[xr.Dataset, xr.DataArray],
     skip_first: int = 0,
     ignore_broken: bool = False,
     kinetic: bool = False,
+    unmapped: bool = False,
     dtype: DTypeLike = float,
     squeeze: bool = True,
 ) -> typing.Sequence[xr.DataArray]:
     """
     Read a file with the EMC3 mapping. Note that this function does
     not add meta-data or does normalisation of the data, thus
     `xemc3.load.file` is generally preferred.
@@ -1007,14 +1030,17 @@
     skip_first : int (optional)
         Ignore the first n lines. Default 0
     ignore_broken: bool (optional)
         if incomplete datasets at the end should be ignored. Default: False
     kinetic : bool (optional)
         The file contains also data for cells that are only evolved by
         EIRENE, rather then EMC3. Default: False
+    unmapped : bool (optional)
+        The file contains unmapped data, i.e. on value for each cell.
+        Default: False
     dtype : datatype (optional)
         The type of the data, e.g. float or int. Is passed to
         numpy. Default: float
     squeeze : bool
         If True return a DataArray if only one field is read.
 
     Returns
@@ -1023,27 +1049,34 @@
         The data that has been read from the file. If squeeze is True
         and only one field is read only a single DataArray is
         returned.
 
     """
 
     if isinstance(mapping, xr.Dataset):
-        mapping = ensure_mapping(_dir_of(fn), mapping)
+        mapping = ensure_mapping(_dir_of(fn), mapping, fn=fn)
         mapping = mapping["_plasma_map"]
     if kinetic:
+        assert unmapped == False
         max = np.max(mapping.data) + 1
+    elif unmapped:
+        max = mapping.attrs["numcells"]
     else:
         max = mapping.attrs["plasmacells"]
     firsts = []
     with open(fn) as f:
         raws = []
         while True:
             if skip_first:
                 first = ""
-                for _ in range(skip_first):
+                if isinstance(skip_first, int):
+                    sf = skip_first
+                else:
+                    sf = skip_first[min(len(raws), len(skip_first) - 1)]
+                for _ in range(sf):
                     first += f.readline()
                 firsts.append(first)
             raw = _fromfile(f, dtype=dtype, count=max, sep=" ")
             if ignore_broken and len(raw) > max:
                 print(f"Ignoring data: {raw[max:]}")
                 raw = raw[:max]
             if len(raw) == max:
@@ -1055,33 +1088,39 @@
                     print(f"Ignoring {len(raw)} data points, {max} required")
                     break
                 print(raw)
                 raise RuntimeError(
                     f"Incomplete dataset found ({len(raw)} out of {max}) after reading {len(raws)} datasets of file {fn}"
                 )
 
-    def to_da(raw):
+    def to_da_mapped(raw):
         out = np.ones(mapping.shape) * np.nan
         mapdat = mapping.data
         for ijk in rrange(mapping.shape):
             mapid = mapdat[ijk]
             if mapid < max:
                 out[ijk] = raw[mapid]
         return xr.DataArray(data=out, dims=mapping.dims)
 
+    def to_da_unmapped(raw):
+        return xr.DataArray(data=raw.reshape(mapping.shape), dims=mapping.dims)
+
+    to_da = to_da_unmapped if unmapped else to_da_mapped
     das = [to_da(raw) for raw in raws]
     if skip_first:
         for first, da in zip(firsts, das):
             da.attrs["print_before"] = first
     if squeeze and len(das) == 1:
         das = das[0]
     return das
 
 
-def write_mapped_nice(ds: xr.Dataset, dir: str, fn: str = None, **args) -> None:
+def write_mapped_nice(
+    ds: xr.Dataset, dir: str, fn: typing.Optional[str] = None, **args
+) -> None:
     """
     Write a file for EMC3 using the mapped format.
 
     Parameters
     ----------
     ds : xr.Dataset
         A xemc3 dataset
@@ -1208,15 +1247,14 @@
 
 def to_mapped(
     data: xr.DataArray,
     mapping: xr.DataArray,
     kinetic: bool = False,
     dtype: typing.Union[DTypeLike, None] = None,
 ) -> np.ndarray:
-
     if kinetic:
         max = np.max(mapping.values) + 1
     else:
         max = np.max(mapping.attrs["plasmacells"])
     if dtype is None:
         dtype = data.values.dtype
 
@@ -1226,15 +1264,17 @@
     datdat = data.values
     if out.dtype != datdat.dtype:
         if out.dtype == np.int64 and datdat.dtype == np.float64:
             datdat = (datdat + 0.5).astype(dtype)
     count = np.zeros(max, dtype=int)
     args = datdat, mapdat, out, count
     for arg in args:
-        assert isinstance(arg, np.ndarray)
+        assert isinstance(
+            arg, np.ndarray
+        ), f"Expected to write np.ndarray, but got {type(arg)}."
     out, count = to_mapped_core(*args, max)
     if out.dtype in [np.dtype(x) for x in [int, np.int32, np.int64]]:
         out //= count
     else:
         out /= count
     assert isinstance(out, np.ndarray)
     return out
@@ -1243,14 +1283,15 @@
 def write_mapped(
     datas,
     mapping,
     fn,
     skip_first=0,
     ignore_broken=False,
     kinetic=False,
+    unmapped=False,
     dtype=None,
     fmt=None,
 ):
     """
     Write a some files using the EMC3 mapping.
 
     Parameters
@@ -1264,14 +1305,16 @@
     skip_first : None or int
         If not None, it needs to be the number of lines that are in
         the `print_before` attribute.
     ignore_broken : any
         ignored.
     kinetic : bool
         If true the data is defined also outside of the plasma region.
+    unmapped : bool
+        If true the data is not mapped
     dtype : any
         if not None, it needs to match the dtype of the data
     fmt : None or str
         The Format to be used for printing the data.
     """
     if skip_first is not None:
         for d in datas:
@@ -1282,15 +1325,19 @@
                 )
                 assert d.attrs["print_before"] != ""
             else:
                 if "print_before" in d.attrs:
                     assert d.attrs["print_before"] == ""
     if not isinstance(datas, (list, tuple)):
         datas = [datas]
-    out = [to_mapped(x, mapping, kinetic, dtype) for x in datas]
+    if unmapped:
+        assert kinetic == False
+        out = [np.ravel(x) for x in datas]
+    else:
+        out = [to_mapped(x, mapping, kinetic, dtype) for x in datas]
     with open(fn, "w") as f:
         for i, da in zip(out, datas):
             if "print_before" in da.attrs:
                 f.write(da.attrs["print_before"])
             if fmt is None:
                 tfmt = "%.4e" if dtype != int else "%d"
             else:
@@ -1422,14 +1469,20 @@
         vars={"DENSITY_E_I_%d": dict()},
     ),
     "DENSITY_E_M": dict(
         type="mapped",
         kinetic=True,
         vars={"DENSITY_E_M_%d": dict()},
     ),
+    "NEUTRAL_DENSITY": dict(
+        type="mapped",
+        skip_first=[3, 2],
+        unmapped=True,
+        vars={"NEUTRAL_DENSITY_%d": dict()},
+    ),
     "fort.1": dict(
         type="raw",
         vars={"fort.1": dict(long_name="Geometry input file")},
     ),
     "fort.2": dict(
         type="raw",
         vars={
@@ -1695,31 +1748,37 @@
     defaults = files[filename].copy()
     defaults.update(opts)
     type = defaults.get("type", "mapped")
     if type == "info":
         if not isinstance(ds, xr.Dataset):
             ds = xr.Dataset()
         return read_fort_file(ds, fn, **defaults)
-    ds = ensure_mapping("/".join(fn.split("/")[:-1]), ds, type == "mapped")
+    ds = ensure_mapping("/".join(fn.split("/")[:-1]), ds, type == "mapped", fn=fn)
     assert isinstance(ds, xr.Dataset)
     return read_fort_file(ds, fn, **defaults)
 
 
 def read_fort_file(ds: xr.Dataset, fn: str, type: str = "mapped", **opts) -> xr.Dataset:
     """
     Read an EMC3 simulation file and add to a dataset.
 
     """
     assert files == _files_bak
     datas = None
     vars = opts.pop("vars")
     if type == "mapping":
-        ds["_plasma_map"] = read_mappings(fn, ds.R_bounds.data.shape[:3])
+        ds["_plasma_map"] = read_mappings(
+            fn, tuple([len(ds[k]) for k in ("r", "theta", "phi")])
+        )
     elif type == "mapped":
-        ds = ensure_mapping(_dir_of(fn), ds)
+        # Ensure file is present before we try to read mapping
+        # This is because missing mapping is handled differently.
+        with open(fn):
+            pass
+        ds = ensure_mapping(_dir_of(fn), ds, fn=fn)
         datas = read_mapped(fn, ds["_plasma_map"], **opts, squeeze=False)
         opts = {}
     elif type == "full":
         datas = [read_magnetic_field(fn, ds)]
     elif type == "plates_mag":
         datas = [read_plates_mag(fn, ds)]
     elif type == "geom":
@@ -1871,18 +1930,17 @@
     arch.to_netcdf(
         fn,
         encoding={
             i: {"zlib": True, "complevel": 9} for i in list(arch) + list(arch.coords)
         },
     )
     print(f"done with {fn}")
-    pass
 
 
-def load_all(path: str, ignore_missing: bool = None) -> xr.Dataset:
+def load_all(path: str, ignore_missing: typing.Optional[bool] = None) -> xr.Dataset:
     """
     Load all data from a path and return as dataset
 
     Parameters
     ----------
     path : str
          Directory that contains files to be read
@@ -1902,15 +1960,17 @@
         present.
     """
     ds = read_locations(path)
     for fn, opts in files.items():
         opts = opts.copy()
         try:
             ds = read_fort_file(ds, f"{path}/{fn}", **opts)
-        except FileNotFoundError:
+        except FileNotFoundError as e:
+            if e.args[0] == 33:
+                raise
             if ignore_missing is None:
                 if not opts.get("ignore_missing", True):
                     raise
             elif not ignore_missing:
                 raise
     return ds
```

### Comparing `xemc3-0.2.3/xemc3/core/plot_2d.py` & `xemc3-0.2.4/xemc3/core/plot_2d.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import matplotlib.pyplot as plt  # type: ignore
+import matplotlib as mpl  # type: ignore
 import numpy as np
 import xarray as xr
 
 from . import utils
 from .load import plate_prefix
 
 
@@ -14,17 +15,18 @@
     Rmin=None,
     Rmax=None,
     zmin=None,
     zmax=None,
     aspect=True,
     figsize=None,
     target=False,
+    log=False,
+    robust=False,
     **kwargs,
 ):
-
     phis = ds["phi_bounds"]
     if phi < np.min(phis.data) or phi > np.max(phis.data):
         raise RuntimeError(
             f"{phi} outside of bounds in dataset {np.min(phis)}:{np.max(phis)}"
         )
     for phi_i, phib in enumerate(phis):
         if phib[0] <= phi <= phib[1]:
@@ -37,32 +39,51 @@
     das = [ds[k] for k in ["R_bounds", "z_bounds"]]
     if key:
         das.append(ds[key])
     pp = xr.DataArray(data=[(1 - p), p], dims="delta_phi")
     das = [
         (da * pp).sum(dim="delta_phi") if "delta_phi" in da.dims else da for da in das
     ]
+    norm = None
     if key:
         data = das[2].data
-        if "time" in ds[key].dims:
+        if "time" in das[2].dims:
             raise ValueError(
                 "Unexpected dimension `time` - animation is not yet supported!"
             )
-        if len(ds[key].dims) != 2:
-            raise ValueError(
-                f"Expected 2 dimensions for R-z plot, but found {len(ds[key].dims)}: {ds[key].dims}!"
-            )
+        if len(das[2].dims) != 2:
+            if das[2].dims == das[0].dims:
+                data = utils.from_interval(das[2])
+                if "shading" not in kwargs:
+                    kwargs["shading"] = "gouraud"
+            else:
+                raise ValueError(
+                    f"Expected 2 dimensions for R-z plot, but found {len(das[2].dims)}: {das[2].dims}!"
+                )
+        if robust:
+            vmin, vmax = np.nanpercentile(data, [1, 99])
+        else:
+            vmin = np.nanmin(data)
+            vmax = np.nanmax(data)
+        vmin = kwargs.pop("vmin", vmin)
+        vmax = kwargs.pop("vmax", vmax)
+        if log and vmin <= 0:
+            raise ValueError(f"vmin ({vmin}) is not positive but log plot requested!")
+        assert vmin < vmax, f"vmin ({vmin}) is not smaller than vmax ({vmax})"
+        norm = (mpl.colors.LogNorm if log else mpl.colors.Normalize)(
+            vmin=vmin, vmax=vmax
+        )
     else:
         data = np.zeros(das[0].shape[:2]) * np.nan
         if "edgecolors" not in kwargs:
             kwargs["edgecolors"] = "k"
     r = utils.from_interval(das[0])
     z = utils.from_interval(das[1])
     ax = _get_ax(figsize, ax)
-    p = ax.pcolormesh(r, z, data, **kwargs)
+    p = ax.pcolormesh(r, z, data, norm=norm, **kwargs)
     # plt.xlabel(xr.plot.utils.label_from_attrs(r))
     if aspect:
         ax.set_aspect(1)
     ax.set_xlabel("R [m]")
     ax.set_ylabel("z [m]")
     plt.colorbar(p, ax=ax)
     if Rmin is not None or Rmax is not None:
```

### Comparing `xemc3-0.2.3/xemc3/core/plot_3d.py` & `xemc3-0.2.4/xemc3/core/plot_3d.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/core/utils.py` & `xemc3-0.2.4/xemc3/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 def prod(args):
     ret = 1
     for arg in args:
         ret *= arg
     return ret
 
 
+raise_issue = " If you think the input is valid, please open a bug at https://github.com/dschwoerer/xemc3/issues"
+
+
 def to_interval(dims, data=None) -> xr.DataArray:
     """Transforms a N-D i_1+1 x ... x i_N+1 mesh to an
     i_1 x ... x i_N x 2 x ... x 2 mesh of quads
     """
     if isinstance(dims, tuple) and data is None:
         dims, data = dims
```

### Comparing `xemc3-0.2.3/xemc3/load/__init__.py` & `xemc3-0.2.4/xemc3/load/__init__.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/test/gen_ds.py` & `xemc3-0.2.4/xemc3/test/gen_ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,27 +151,34 @@
             }[load.files[f].get("type", "mapped")]
             if load.files[f].get("kinetic", False):
                 assert genf == gen_mapped
                 genf = gen_kinetic
             pre = load.files[f].get("skip_first", 0)
             dtype = load.files[f].get("dtype", float)
 
+            def add_pre(ds, k, pre, i):
+                if pre:
+                    if isinstance(pre, int):
+                        pret = pre
+                    else:
+                        pret = pre[min(len(pre) - 1, i)]
+                    ds[k].attrs["print_before"] = ("   %d\n" % i) * pret
+                return ds
+
             if "%" in v:
                 for i in range(i, i + ids):
                     ds[v % i] = genf(ds, index=i)
                     if dtype != float and genf != gen_depo:
                         ds[v % i] = genf(ds)[0], np.round(genf(ds)[1] * 20)
                     ds[v % i].attrs.update(get_attrs(vs[v]))
-                    if pre:
-                        ds[v % i].attrs["print_before"] = "   %d\n" % i
+                    ds = add_pre(ds, v % i, pre, i)
             else:
                 ds[v] = genf(ds, index=i)
                 ds[v].attrs.update(get_attrs(vs[v]))
-                if pre:
-                    ds[v].attrs["print_before"] = "   %d\n" % i
+                ds = add_pre(ds, v, pre, i)
                 if genf == gen_depo and i == 0:
                     ds[v].attrs["description"] = "True means +1, False means -1"
 
             i += 1
     return ds
```

### Comparing `xemc3-0.2.3/xemc3/test/test_average.py` & `xemc3-0.2.4/xemc3/test/test_average.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/test/test_cli.py` & `xemc3-0.2.4/xemc3/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/test/test_dataset.py` & `xemc3-0.2.4/xemc3/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/test/test_load_real.py` & `xemc3-0.2.4/xemc3/test/test_load_real.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import numpy as np
 import pytest
 import xarray as xr
 from xarray.testing import assert_identical
 
 import xemc3
 
+
 # simple regression test
 def test_load_all():
     bd = get_data()
     result = xemc3.load.all(bd)
     expected = xr.open_dataset(bd + ".nc")
 
     # Remove changing attributes
```

### Comparing `xemc3-0.2.3/xemc3/test/test_utils.py` & `xemc3-0.2.4/xemc3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/test/test_write_load.py` & `xemc3-0.2.4/xemc3/test/test_write_load.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/tools/run_wrapper.py` & `xemc3-0.2.4/xemc3/tools/run_wrapper.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3/write/fortran.py` & `xemc3-0.2.4/xemc3/write/fortran.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.3/xemc3.egg-info/PKG-INFO` & `xemc3-0.2.4/xemc3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xemc3
-Version: 0.2.3
+Version: 0.2.4
 Summary: Collect data from EMC3 runs in python using xarray
 Home-page: https://github.com/dschwoerer/xemc3
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Tracker, https://github.com/dschwoerer/xemc3/issues
 Project-URL: Documentation, https://xemc3.rtfd.io
```

### Comparing `xemc3-0.2.3/xemc3.egg-info/SOURCES.txt` & `xemc3-0.2.4/xemc3.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 mypy.ini
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/black-fix.yml
 .github/workflows/build.yml
-.github/workflows/coverage.yml
 .github/workflows/python_publish.yml
 .github/workflows/test-python-package.yml
 .github/workflows/zenodo.yml
 docs/citing.rst
 docs/cli.rst
 docs/cli.rst.in.py
 docs/conf.py
```

