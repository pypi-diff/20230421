# Comparing `tmp/xarray-2023.4.1.tar.gz` & `tmp/xarray-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-2023.4.1.tar", last modified: Tue Apr 18 15:33:19 2023, max compression
+gzip compressed data, was "xarray-2023.4.2.tar", last modified: Thu Apr 20 18:28:08 2023, max compression
```

## Comparing `xarray-2023.4.1.tar` & `xarray-2023.4.2.tar`

### file list

```diff
@@ -1,368 +1,369 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.578976 xarray-2023.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.538976 xarray-2023.4.1/.binder/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-18 15:33:02.000000 xarray-2023.4.1/.binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-18 15:33:02.000000 xarray-2023.4.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-18 15:33:02.000000 xarray-2023.4.1/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-18 15:33:02.000000 xarray-2023.4.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 15:33:02.000000 xarray-2023.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.538976 xarray-2023.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.538976 xarray-2023.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/ISSUE_TEMPLATE/misc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.538976 xarray-2023.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/ci-additional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/configure-testpypi-version.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/label-all.yml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/label-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/publish-test-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/pypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-18 15:33:02.000000 xarray-2023.4.1/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-18 15:33:02.000000 xarray-2023.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 15:33:02.000000 xarray-2023.4.1/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-18 15:33:02.000000 xarray-2023.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-18 15:33:02.000000 xarray-2023.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-18 15:33:02.000000 xarray-2023.4.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-18 15:33:02.000000 xarray-2023.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 15:33:02.000000 xarray-2023.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-18 15:33:02.000000 xarray-2023.4.1/HOW_TO_RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-18 15:33:02.000000 xarray-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-18 15:33:19.582976 xarray-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-04-18 15:33:02.000000 xarray-2023.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.538976 xarray-2023.4.1/asv_bench/
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.542976 xarray-2023.4.1/asv_bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/README_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/dataarray_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/dataset_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/polyfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/reindexing.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/renaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/rolling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-18 15:33:02.000000 xarray-2023.4.1/asv_bench/benchmarks/unstacking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.542976 xarray-2023.4.1/ci/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/install-upstream-wheels.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     6565 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/min_deps_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.542976 xarray-2023.4.1/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/requirements/all-but-dask.yml
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/requirements/bare-minimum.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/requirements/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/requirements/environment-py311.yml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/requirements/environment-windows-py311.yml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/requirements/environment-windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 15:33:02.000000 xarray-2023.4.1/ci/requirements/min-all-deps.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-18 15:33:02.000000 xarray-2023.4.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.542976 xarray-2023.4.1/design_notes/
--rw-r--r--   0 runner    (1001) docker     (123)    28105 2023-04-18 15:33:02.000000 xarray-2023.4.1/design_notes/flexible_indexes_notes.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.542976 xarray-2023.4.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.546976 xarray-2023.4.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    31185 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/advanced_selection_interpolation.svg
--rw-r--r--   0 runner    (1001) docker     (123)   114027 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/ci.png
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dask_array.png
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram-build.sh
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram-logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   117124 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    66565 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram-logo.tex
--rw-r--r--   0 runner    (1001) docker     (123)   183796 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram-square-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram-square-logo.tex
--rw-r--r--   0 runner    (1001) docker     (123)    45348 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/dataset-diagram.tex
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/index_api.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/index_contribute.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/index_getting_started.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/index_user_guide.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/numfocus_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   104979 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/opendap-prism-tmax.png
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.550976 xarray-2023.4.1/doc/_static/thumbnails/
--rw-r--r--   0 runner    (1001) docker     (123)    32739 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/thumbnails/ERA5-GRIB-example.png
--rw-r--r--   0 runner    (1001) docker     (123)    77903 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/thumbnails/ROMS_ocean_model.png
--rw-r--r--   0 runner    (1001) docker     (123)    26018 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/thumbnails/area_weighted_temperature.png
--rw-r--r--   0 runner    (1001) docker     (123)   454794 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/thumbnails/monthly-means.png
--rw-r--r--   0 runner    (1001) docker     (123)    57609 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/thumbnails/multidimensional-coords.png
--rw-r--r--   0 runner    (1001) docker     (123)    37844 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/thumbnails/toy-weather-data.png
--rw-r--r--   0 runner    (1001) docker     (123)    43053 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/thumbnails/visualization_gallery.png
--rw-r--r--   0 runner    (1001) docker     (123)   664021 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_static/view-docs.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.534976 xarray-2023.4.1/doc/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.550976 xarray-2023.4.1/doc/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_templates/autosummary/accessor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/_templates/autosummary/accessor_method.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19245 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/api-hidden.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    42873 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/developers-meeting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/ecosystem.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.550976 xarray-2023.4.1/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/ERA5-GRIB-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/ROMS_ocean_model.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.550976 xarray-2023.4.1/doc/examples/_code/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/_code/accessor_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    28228 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/apply_ufunc_vectorize_1d.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/area_weighted_temperature.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/blank_template.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/monthly-means.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   445711 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/monthly_means_output.png
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/multidimensional-coords.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/visualization_gallery.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/examples/weather-data.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.550976 xarray-2023.4.1/doc/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/gallery/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/gallery/plot_cartopy_facetgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/gallery/plot_colorbar_center.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/gallery/plot_control_colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/gallery/plot_lines_from_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/gallery.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/gallery.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.550976 xarray-2023.4.1/doc/getting-started-guide/
--rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/getting-started-guide/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/getting-started-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/getting-started-guide/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/getting-started-guide/quick-overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/getting-started-guide/why-xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/howdoi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.554976 xarray-2023.4.1/doc/internals/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/internals/duck-arrays-integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/internals/extending-xarray.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/internals/how-to-add-new-backend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/internals/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/internals/variable-objects.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/internals/zarr-encoding-spec.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/tutorials-and-videos.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.554976 xarray-2023.4.1/doc/user-guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/combining.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29078 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/computation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/dask.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/data-structures.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/duckarrays.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/groupby.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    27433 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/indexing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    47085 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/io.rst
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/options.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/pandas.rst
--rw-r--r--   0 runner    (1001) docker     (123)    31542 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/plotting.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/reshaping.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/terminology.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/time-series.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/user-guide/weather-climate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/videos.yml
--rw-r--r--   0 runner    (1001) docker     (123)   317725 2023-04-18 15:33:02.000000 xarray-2023.4.1/doc/whats-new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.554976 xarray-2023.4.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 15:33:02.000000 xarray-2023.4.1/licenses/DASK_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-04-18 15:33:02.000000 xarray-2023.4.1/licenses/ICOMOON_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-18 15:33:02.000000 xarray-2023.4.1/licenses/NUMPY_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-18 15:33:02.000000 xarray-2023.4.1/licenses/PANDAS_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-18 15:33:02.000000 xarray-2023.4.1/licenses/PYTHON_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-18 15:33:02.000000 xarray-2023.4.1/licenses/SCIKIT_LEARN_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-18 15:33:02.000000 xarray-2023.4.1/licenses/SEABORN_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.554976 xarray-2023.4.1/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-18 15:33:02.000000 xarray-2023.4.1/properties/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 15:33:02.000000 xarray-2023.4.1/properties/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 15:33:02.000000 xarray-2023.4.1/properties/test_encode_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-18 15:33:02.000000 xarray-2023.4.1/properties/test_pandas_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-18 15:33:02.000000 xarray-2023.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-18 15:33:02.000000 xarray-2023.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-18 15:33:19.582976 xarray-2023.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-04-18 15:33:02.000000 xarray-2023.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.558976 xarray-2023.4.1/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.558976 xarray-2023.4.1/xarray/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64180 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/h5netcdf_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/netCDF4_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/netcdf3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/pseudonetcdf_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/pydap_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/pynio_.py
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/scipy_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/backends/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.562976 xarray-2023.4.1/xarray/coding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/coding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/coding/calendar_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    47274 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/coding/cftime_offsets.py
--rw-r--r--   0 runner    (1001) docker     (123)    29864 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/coding/cftimeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/coding/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/coding/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/coding/times.py
--rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/coding/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    29000 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.566976 xarray-2023.4.1/xarray/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   293555 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26253 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/_typed_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    30052 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/_typed_ops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/accessor_dt.py
--rw-r--r--   0 runner    (1001) docker     (123)    86739 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/accessor_str.py
--rw-r--r--   0 runner    (1001) docker     (123)    37538 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    37528 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)    61997 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    75080 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    28139 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/dask_array_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)   254214 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/dataarray.py
--rw-r--r--   0 runner    (1001) docker     (123)   354135 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22628 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/duck_array_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27908 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/formatting_html.py
--rw-r--r--   0 runner    (1001) docker     (123)    52185 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)    54154 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    57705 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39490 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/nanops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/npcompat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/nputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/pdcompat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/pycompat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/resample_cftime.py
--rw-r--r--   0 runner    (1001) docker     (123)    40143 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/rolling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/rolling_exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    35253 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/core/weighted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.566976 xarray-2023.4.1/xarray/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/indexes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.566976 xarray-2023.4.1/xarray/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41974 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/plot/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    85980 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/plot/dataarray_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    30818 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/plot/dataset_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/plot/facetgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    59520 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.566976 xarray-2023.4.1/xarray/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.566976 xarray-2023.4.1/xarray/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/static/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.570976 xarray-2023.4.1/xarray/static/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/static/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/static/html/icons-svg-inline.html
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.578976 xarray-2023.4.1/xarray/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.578976 xarray-2023.4.1/xarray/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/data/bears.nc
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/data/example.grib
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/data/example.ict
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/data/example.uamiv
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/data/example_1.nc
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/data/example_1.nc.gz
--rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_accessor_dt.py
--rw-r--r--   0 runner    (1001) docker     (123)   121928 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_accessor_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_array_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   205405 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_backends_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_backends_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_backends_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_backends_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_backends_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_calendar_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    44969 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_cftime_offsets.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_cftimeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_cftimeindex_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_coarsen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_coding_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    43161 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_coding_times.py
--rw-r--r--   0 runner    (1001) docker     (123)    44271 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)    77115 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    46051 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)    59984 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)   246009 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_dataarray.py
--rw-r--r--   0 runner    (1001) docker     (123)   259858 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_deprecation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_duck_array_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24804 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_formatting_html.py
--rw-r--r--   0 runner    (1001) docker     (123)    79675 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)    25785 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    31184 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    29970 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    18119 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_nputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)   119180 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31207 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_rolling.py
--rw-r--r--   0 runner    (1001) docker     (123)    28760 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_ufuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)   188860 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   110147 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    24189 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tests/test_weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.578976 xarray-2023.4.1/xarray/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/util/deprecation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/util/generate_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/util/generate_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5219 2023-04-18 15:33:02.000000 xarray-2023.4.1/xarray/util/print_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:33:19.558976 xarray-2023.4.1/xarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-18 15:33:19.000000 xarray-2023.4.1/xarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-04-18 15:33:19.000000 xarray-2023.4.1/xarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:33:19.000000 xarray-2023.4.1/xarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:33:19.000000 xarray-2023.4.1/xarray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-18 15:33:19.000000 xarray-2023.4.1/xarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 15:33:19.000000 xarray-2023.4.1/xarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.168488 xarray-2023.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.068488 xarray-2023.4.2/.binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-20 18:27:47.000000 xarray-2023.4.2/.binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 18:27:47.000000 xarray-2023.4.2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 18:27:47.000000 xarray-2023.4.2/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 18:27:47.000000 xarray-2023.4.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 18:27:47.000000 xarray-2023.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.068488 xarray-2023.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.072487 xarray-2023.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/ISSUE_TEMPLATE/misc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.072487 xarray-2023.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/benchmarks-last-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/ci-additional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/configure-testpypi-version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/label-all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/label-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/publish-test-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-20 18:27:47.000000 xarray-2023.4.2/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-20 18:27:47.000000 xarray-2023.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-20 18:27:47.000000 xarray-2023.4.2/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-20 18:27:47.000000 xarray-2023.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-20 18:27:47.000000 xarray-2023.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-20 18:27:47.000000 xarray-2023.4.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-20 18:27:47.000000 xarray-2023.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 18:27:47.000000 xarray-2023.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-20 18:27:47.000000 xarray-2023.4.2/HOW_TO_RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-20 18:27:47.000000 xarray-2023.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-20 18:28:08.168488 xarray-2023.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-04-20 18:27:47.000000 xarray-2023.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.072487 xarray-2023.4.2/asv_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.076487 xarray-2023.4.2/asv_bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/README_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/dataarray_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/dataset_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/polyfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/reindexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/renaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/rolling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-20 18:27:47.000000 xarray-2023.4.2/asv_bench/benchmarks/unstacking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.076487 xarray-2023.4.2/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/install-upstream-wheels.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6565 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/min_deps_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.080487 xarray-2023.4.2/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/requirements/all-but-dask.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/requirements/bare-minimum.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/requirements/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/requirements/environment-py311.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/requirements/environment-windows-py311.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/requirements/environment-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-20 18:27:47.000000 xarray-2023.4.2/ci/requirements/min-all-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-20 18:27:47.000000 xarray-2023.4.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.080487 xarray-2023.4.2/design_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)    28105 2023-04-20 18:27:47.000000 xarray-2023.4.2/design_notes/flexible_indexes_notes.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.084488 xarray-2023.4.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.092487 xarray-2023.4.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    31185 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/advanced_selection_interpolation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   114027 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/ci.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dask_array.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram-build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram-logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   117124 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66565 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram-logo.tex
+-rw-r--r--   0 runner    (1001) docker     (123)   183796 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram-square-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram-square-logo.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    45348 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/dataset-diagram.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/index_api.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/index_contribute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/index_getting_started.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/index_user_guide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/numfocus_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   104979 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/opendap-prism-tmax.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.096488 xarray-2023.4.2/doc/_static/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)    32739 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/thumbnails/ERA5-GRIB-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    77903 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/thumbnails/ROMS_ocean_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26018 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/thumbnails/area_weighted_temperature.png
+-rw-r--r--   0 runner    (1001) docker     (123)   454794 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/thumbnails/monthly-means.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57609 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/thumbnails/multidimensional-coords.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37844 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/thumbnails/toy-weather-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43053 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/thumbnails/visualization_gallery.png
+-rw-r--r--   0 runner    (1001) docker     (123)   664021 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_static/view-docs.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.064487 xarray-2023.4.2/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.096488 xarray-2023.4.2/doc/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_templates/autosummary/accessor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19245 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/api-hidden.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42873 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/developers-meeting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/ecosystem.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.100488 xarray-2023.4.2/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/ERA5-GRIB-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/ROMS_ocean_model.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.100488 xarray-2023.4.2/doc/examples/_code/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/_code/accessor_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28228 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/apply_ufunc_vectorize_1d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/area_weighted_temperature.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/blank_template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/monthly-means.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   445711 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/monthly_means_output.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/multidimensional-coords.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/visualization_gallery.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/examples/weather-data.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.104488 xarray-2023.4.2/doc/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/gallery/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/gallery/plot_cartopy_facetgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/gallery/plot_colorbar_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/gallery/plot_control_colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/gallery/plot_lines_from_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/gallery.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.104488 xarray-2023.4.2/doc/getting-started-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/getting-started-guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/getting-started-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/getting-started-guide/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/getting-started-guide/quick-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/getting-started-guide/why-xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/howdoi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.108487 xarray-2023.4.2/doc/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/internals/duck-arrays-integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/internals/extending-xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/internals/how-to-add-new-backend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/internals/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/internals/variable-objects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/internals/zarr-encoding-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/tutorials-and-videos.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.112488 xarray-2023.4.2/doc/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/combining.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29078 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/computation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/dask.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/data-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/duckarrays.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/groupby.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    27433 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    47085 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/io.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/pandas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    31542 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/reshaping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/terminology.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/time-series.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/user-guide/weather-climate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/videos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   318211 2023-04-20 18:27:47.000000 xarray-2023.4.2/doc/whats-new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.116488 xarray-2023.4.2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-20 18:27:47.000000 xarray-2023.4.2/licenses/DASK_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-04-20 18:27:47.000000 xarray-2023.4.2/licenses/ICOMOON_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-20 18:27:47.000000 xarray-2023.4.2/licenses/NUMPY_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-20 18:27:47.000000 xarray-2023.4.2/licenses/PANDAS_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-04-20 18:27:47.000000 xarray-2023.4.2/licenses/PYTHON_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-20 18:27:47.000000 xarray-2023.4.2/licenses/SCIKIT_LEARN_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-20 18:27:47.000000 xarray-2023.4.2/licenses/SEABORN_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.116488 xarray-2023.4.2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-20 18:27:47.000000 xarray-2023.4.2/properties/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-20 18:27:47.000000 xarray-2023.4.2/properties/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-20 18:27:47.000000 xarray-2023.4.2/properties/test_encode_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-20 18:27:47.000000 xarray-2023.4.2/properties/test_pandas_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-20 18:27:47.000000 xarray-2023.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-20 18:27:47.000000 xarray-2023.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-20 18:28:08.168488 xarray-2023.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-04-20 18:27:47.000000 xarray-2023.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.120488 xarray-2023.4.2/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.128488 xarray-2023.4.2/xarray/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64180 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/h5netcdf_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/netCDF4_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/netcdf3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/pseudonetcdf_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/pydap_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/pynio_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/scipy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/backends/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.128488 xarray-2023.4.2/xarray/coding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/coding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/coding/calendar_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47274 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/coding/cftime_offsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29864 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/coding/cftimeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/coding/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/coding/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/coding/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/coding/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29000 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.144488 xarray-2023.4.2/xarray/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   293555 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26253 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/_typed_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30052 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/_typed_ops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/accessor_dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98648 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/accessor_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37538 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37528 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61997 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75080 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28139 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/dask_array_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)   254214 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)   354135 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22628 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/duck_array_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27908 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/formatting_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52226 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54154 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57705 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39490 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/nanops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/npcompat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/nputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/pdcompat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/pycompat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/resample_cftime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40143 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/rolling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/rolling_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35253 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/core/weighted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.144488 xarray-2023.4.2/xarray/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/indexes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.148488 xarray-2023.4.2/xarray/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41974 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/plot/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85980 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/plot/dataarray_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30818 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/plot/dataset_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/plot/facetgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59520 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.148488 xarray-2023.4.2/xarray/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.148488 xarray-2023.4.2/xarray/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/static/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.148488 xarray-2023.4.2/xarray/static/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/static/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/static/html/icons-svg-inline.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.164488 xarray-2023.4.2/xarray/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.168488 xarray-2023.4.2/xarray/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/data/bears.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/data/example.grib
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/data/example.ict
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/data/example.uamiv
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/data/example_1.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/data/example_1.nc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_accessor_dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121928 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_accessor_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_array_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   205405 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_backends_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_backends_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_backends_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_backends_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_backends_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_calendar_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44969 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_cftime_offsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_cftimeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_cftimeindex_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_coarsen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_coding_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43161 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_coding_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44271 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77115 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46051 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59984 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246009 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)   259858 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_deprecation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_duck_array_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24804 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_formatting_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25785 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31184 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29970 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18119 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_nputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119180 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31207 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_rolling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28760 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_ufuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188860 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110147 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24189 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tests/test_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.168488 xarray-2023.4.2/xarray/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/util/deprecation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/util/generate_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/util/generate_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5219 2023-04-20 18:27:47.000000 xarray-2023.4.2/xarray/util/print_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:28:08.120488 xarray-2023.4.2/xarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-20 18:28:07.000000 xarray-2023.4.2/xarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-04-20 18:28:08.000000 xarray-2023.4.2/xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:28:07.000000 xarray-2023.4.2/xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:28:07.000000 xarray-2023.4.2/xarray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-20 18:28:07.000000 xarray-2023.4.2/xarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:28:07.000000 xarray-2023.4.2/xarray.egg-info/top_level.txt
```

### Comparing `xarray-2023.4.1/.binder/environment.yml` & `xarray-2023.4.2/.binder/environment.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/ISSUE_TEMPLATE/bugreport.yml` & `xarray-2023.4.2/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/ISSUE_TEMPLATE/config.yml` & `xarray-2023.4.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/ISSUE_TEMPLATE/newfeature.yml` & `xarray-2023.4.2/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/config.yml` & `xarray-2023.4.2/.github/config.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/labeler.yml` & `xarray-2023.4.2/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/stale.yml` & `xarray-2023.4.2/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/benchmarks.yml` & `xarray-2023.4.2/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/ci-additional.yaml` & `xarray-2023.4.2/.github/workflows/ci-additional.yaml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/ci.yaml` & `xarray-2023.4.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/configure-testpypi-version.py` & `xarray-2023.4.2/.github/workflows/configure-testpypi-version.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/parse_logs.py` & `xarray-2023.4.2/.github/workflows/parse_logs.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/publish-test-results.yaml` & `xarray-2023.4.2/.github/workflows/publish-test-results.yaml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/pypi-release.yaml` & `xarray-2023.4.2/.github/workflows/pypi-release.yaml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/testpypi-release.yaml` & `xarray-2023.4.2/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.github/workflows/upstream-dev-ci.yaml` & `xarray-2023.4.2/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.gitignore` & `xarray-2023.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/.pre-commit-config.yaml` & `xarray-2023.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/CITATION.cff` & `xarray-2023.4.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/CODE_OF_CONDUCT.md` & `xarray-2023.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/HOW_TO_RELEASE.md` & `xarray-2023.4.2/HOW_TO_RELEASE.md`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/LICENSE` & `xarray-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/PKG-INFO` & `xarray-2023.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: N-D labeled arrays and datasets in Python
 Home-page: https://github.com/pydata/xarray
 Author: xarray Developers
 Author-email: xarray@googlegroups.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `xarray-2023.4.1/README.md` & `xarray-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/asv.conf.json` & `xarray-2023.4.2/asv_bench/asv.conf.json`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/README_CI.md` & `xarray-2023.4.2/asv_bench/benchmarks/README_CI.md`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/__init__.py` & `xarray-2023.4.2/asv_bench/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/alignment.py` & `xarray-2023.4.2/asv_bench/benchmarks/alignment.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/combine.py` & `xarray-2023.4.2/asv_bench/benchmarks/combine.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/dataarray_missing.py` & `xarray-2023.4.2/asv_bench/benchmarks/dataarray_missing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/dataset_io.py` & `xarray-2023.4.2/asv_bench/benchmarks/dataset_io.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/groupby.py` & `xarray-2023.4.2/asv_bench/benchmarks/groupby.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/indexing.py` & `xarray-2023.4.2/asv_bench/benchmarks/indexing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/interp.py` & `xarray-2023.4.2/asv_bench/benchmarks/interp.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/merge.py` & `xarray-2023.4.2/asv_bench/benchmarks/merge.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/pandas.py` & `xarray-2023.4.2/asv_bench/benchmarks/pandas.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/polyfit.py` & `xarray-2023.4.2/asv_bench/benchmarks/polyfit.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/reindexing.py` & `xarray-2023.4.2/asv_bench/benchmarks/reindexing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/renaming.py` & `xarray-2023.4.2/asv_bench/benchmarks/renaming.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/repr.py` & `xarray-2023.4.2/asv_bench/benchmarks/repr.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/rolling.py` & `xarray-2023.4.2/asv_bench/benchmarks/rolling.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/asv_bench/benchmarks/unstacking.py` & `xarray-2023.4.2/asv_bench/benchmarks/unstacking.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/install-upstream-wheels.sh` & `xarray-2023.4.2/ci/install-upstream-wheels.sh`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/min_deps_check.py` & `xarray-2023.4.2/ci/min_deps_check.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/requirements/all-but-dask.yml` & `xarray-2023.4.2/ci/requirements/all-but-dask.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/requirements/doc.yml` & `xarray-2023.4.2/ci/requirements/doc.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/requirements/environment-py311.yml` & `xarray-2023.4.2/ci/requirements/environment-py311.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/requirements/environment-windows-py311.yml` & `xarray-2023.4.2/ci/requirements/environment-windows-py311.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/requirements/environment-windows.yml` & `xarray-2023.4.2/ci/requirements/environment-windows.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/requirements/environment.yml` & `xarray-2023.4.2/ci/requirements/environment.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/ci/requirements/min-all-deps.yml` & `xarray-2023.4.2/ci/requirements/min-all-deps.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/conftest.py` & `xarray-2023.4.2/conftest.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/design_notes/flexible_indexes_notes.md` & `xarray-2023.4.2/design_notes/flexible_indexes_notes.md`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/Makefile` & `xarray-2023.4.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/advanced_selection_interpolation.svg` & `xarray-2023.4.2/doc/_static/advanced_selection_interpolation.svg`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/ci.png` & `xarray-2023.4.2/doc/_static/ci.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dask_array.png` & `xarray-2023.4.2/doc/_static/dask_array.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dataset-diagram-logo.pdf` & `xarray-2023.4.2/doc/_static/dataset-diagram-logo.pdf`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dataset-diagram-logo.png` & `xarray-2023.4.2/doc/_static/dataset-diagram-logo.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dataset-diagram-logo.svg` & `xarray-2023.4.2/doc/_static/dataset-diagram-logo.svg`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dataset-diagram-logo.tex` & `xarray-2023.4.2/doc/_static/dataset-diagram-logo.tex`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dataset-diagram-square-logo.png` & `xarray-2023.4.2/doc/_static/dataset-diagram-square-logo.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dataset-diagram-square-logo.tex` & `xarray-2023.4.2/doc/_static/dataset-diagram-square-logo.tex`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dataset-diagram.png` & `xarray-2023.4.2/doc/_static/dataset-diagram.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/dataset-diagram.tex` & `xarray-2023.4.2/doc/_static/dataset-diagram.tex`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/favicon.ico` & `xarray-2023.4.2/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/index_api.svg` & `xarray-2023.4.2/doc/_static/index_api.svg`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/index_contribute.svg` & `xarray-2023.4.2/doc/_static/index_contribute.svg`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/index_getting_started.svg` & `xarray-2023.4.2/doc/_static/index_getting_started.svg`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/index_user_guide.svg` & `xarray-2023.4.2/doc/_static/index_user_guide.svg`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/numfocus_logo.png` & `xarray-2023.4.2/doc/_static/numfocus_logo.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/opendap-prism-tmax.png` & `xarray-2023.4.2/doc/_static/opendap-prism-tmax.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/style.css` & `xarray-2023.4.2/doc/_static/style.css`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/thumbnails/ERA5-GRIB-example.png` & `xarray-2023.4.2/doc/_static/thumbnails/ERA5-GRIB-example.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/thumbnails/ROMS_ocean_model.png` & `xarray-2023.4.2/doc/_static/thumbnails/ROMS_ocean_model.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/thumbnails/area_weighted_temperature.png` & `xarray-2023.4.2/doc/_static/thumbnails/area_weighted_temperature.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/thumbnails/monthly-means.png` & `xarray-2023.4.2/doc/_static/thumbnails/monthly-means.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/thumbnails/multidimensional-coords.png` & `xarray-2023.4.2/doc/_static/thumbnails/multidimensional-coords.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/thumbnails/toy-weather-data.png` & `xarray-2023.4.2/doc/_static/thumbnails/toy-weather-data.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/thumbnails/visualization_gallery.png` & `xarray-2023.4.2/doc/_static/thumbnails/visualization_gallery.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/_static/view-docs.png` & `xarray-2023.4.2/doc/_static/view-docs.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/api-hidden.rst` & `xarray-2023.4.2/doc/api-hidden.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/api.rst` & `xarray-2023.4.2/doc/api.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/conf.py` & `xarray-2023.4.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/contributing.rst` & `xarray-2023.4.2/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/developers-meeting.rst` & `xarray-2023.4.2/doc/developers-meeting.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/ecosystem.rst` & `xarray-2023.4.2/doc/ecosystem.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/ERA5-GRIB-example.ipynb` & `xarray-2023.4.2/doc/examples/ERA5-GRIB-example.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/ROMS_ocean_model.ipynb` & `xarray-2023.4.2/doc/examples/ROMS_ocean_model.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/_code/accessor_example.py` & `xarray-2023.4.2/doc/examples/_code/accessor_example.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/apply_ufunc_vectorize_1d.ipynb` & `xarray-2023.4.2/doc/examples/apply_ufunc_vectorize_1d.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/area_weighted_temperature.ipynb` & `xarray-2023.4.2/doc/examples/area_weighted_temperature.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/blank_template.ipynb` & `xarray-2023.4.2/doc/examples/blank_template.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/monthly-means.ipynb` & `xarray-2023.4.2/doc/examples/monthly-means.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/monthly_means_output.png` & `xarray-2023.4.2/doc/examples/monthly_means_output.png`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/multidimensional-coords.ipynb` & `xarray-2023.4.2/doc/examples/multidimensional-coords.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/visualization_gallery.ipynb` & `xarray-2023.4.2/doc/examples/visualization_gallery.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/examples/weather-data.ipynb` & `xarray-2023.4.2/doc/examples/weather-data.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/gallery/plot_cartopy_facetgrid.py` & `xarray-2023.4.2/doc/gallery/plot_cartopy_facetgrid.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/gallery/plot_colorbar_center.py` & `xarray-2023.4.2/doc/gallery/plot_colorbar_center.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/gallery/plot_control_colorbar.py` & `xarray-2023.4.2/doc/gallery/plot_control_colorbar.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/gallery/plot_lines_from_2d.py` & `xarray-2023.4.2/doc/gallery/plot_lines_from_2d.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/gallery.rst` & `xarray-2023.4.2/doc/gallery.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/gallery.yml` & `xarray-2023.4.2/doc/gallery.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/getting-started-guide/faq.rst` & `xarray-2023.4.2/doc/getting-started-guide/faq.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/getting-started-guide/installing.rst` & `xarray-2023.4.2/doc/getting-started-guide/installing.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/getting-started-guide/quick-overview.rst` & `xarray-2023.4.2/doc/getting-started-guide/quick-overview.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/getting-started-guide/why-xarray.rst` & `xarray-2023.4.2/doc/getting-started-guide/why-xarray.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/howdoi.rst` & `xarray-2023.4.2/doc/howdoi.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/index.rst` & `xarray-2023.4.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/internals/duck-arrays-integration.rst` & `xarray-2023.4.2/doc/internals/duck-arrays-integration.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/internals/extending-xarray.rst` & `xarray-2023.4.2/doc/internals/extending-xarray.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/internals/how-to-add-new-backend.rst` & `xarray-2023.4.2/doc/internals/how-to-add-new-backend.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/internals/variable-objects.rst` & `xarray-2023.4.2/doc/internals/variable-objects.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/internals/zarr-encoding-spec.rst` & `xarray-2023.4.2/doc/internals/zarr-encoding-spec.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/roadmap.rst` & `xarray-2023.4.2/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/tutorials-and-videos.rst` & `xarray-2023.4.2/doc/tutorials-and-videos.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/combining.rst` & `xarray-2023.4.2/doc/user-guide/combining.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/computation.rst` & `xarray-2023.4.2/doc/user-guide/computation.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/dask.rst` & `xarray-2023.4.2/doc/user-guide/dask.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/data-structures.rst` & `xarray-2023.4.2/doc/user-guide/data-structures.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/duckarrays.rst` & `xarray-2023.4.2/doc/user-guide/duckarrays.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/groupby.rst` & `xarray-2023.4.2/doc/user-guide/groupby.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/indexing.rst` & `xarray-2023.4.2/doc/user-guide/indexing.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/interpolation.rst` & `xarray-2023.4.2/doc/user-guide/interpolation.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/io.rst` & `xarray-2023.4.2/doc/user-guide/io.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/options.rst` & `xarray-2023.4.2/doc/user-guide/options.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/pandas.rst` & `xarray-2023.4.2/doc/user-guide/pandas.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/plotting.rst` & `xarray-2023.4.2/doc/user-guide/plotting.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/reshaping.rst` & `xarray-2023.4.2/doc/user-guide/reshaping.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/terminology.rst` & `xarray-2023.4.2/doc/user-guide/terminology.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/time-series.rst` & `xarray-2023.4.2/doc/user-guide/time-series.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/user-guide/weather-climate.rst` & `xarray-2023.4.2/doc/user-guide/weather-climate.rst`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/videos.yml` & `xarray-2023.4.2/doc/videos.yml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/doc/whats-new.rst` & `xarray-2023.4.2/doc/whats-new.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,34 @@
     import xarray as xray
     import xarray
     import xarray as xr
 
     np.random.seed(123456)
 
 
+.. _whats-new.2023.04.2:
+
+v2023.04.2 (April 20, 2023)
+---------------------------
+
+This is a patch release to fix a bug with binning (:issue:`7766`)
+
+Bug fixes
+~~~~~~~~~
+
+- Fix binning when ``labels`` is specified. (:issue:`7766`).
+  By `Deepak Cherian <https://github.com/dcherian>`_.
+
+
+Documentation
+~~~~~~~~~~~~~
+- Added examples to docstrings for :py:meth:`xarray.core.accessor_str.StringAccessor` methods.
+  (:pull:`7669`) .
+  By `Mary Gathoni <https://github.com/remigathoni>`_.
+
 
 .. _whats-new.2023.04.1:
 
 v2023.04.1 (April 18, 2023)
 ---------------------------
 
 This is a patch release to fix a bug with binning (:issue:`7759`)
```

### Comparing `xarray-2023.4.1/licenses/DASK_LICENSE` & `xarray-2023.4.2/licenses/DASK_LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/licenses/ICOMOON_LICENSE` & `xarray-2023.4.2/licenses/ICOMOON_LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/licenses/NUMPY_LICENSE` & `xarray-2023.4.2/licenses/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/licenses/PANDAS_LICENSE` & `xarray-2023.4.2/licenses/PANDAS_LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/licenses/PYTHON_LICENSE` & `xarray-2023.4.2/licenses/PYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/licenses/SCIKIT_LEARN_LICENSE` & `xarray-2023.4.2/licenses/SCIKIT_LEARN_LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/licenses/SEABORN_LICENSE` & `xarray-2023.4.2/licenses/SEABORN_LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/properties/README.md` & `xarray-2023.4.2/properties/README.md`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/properties/test_encode_decode.py` & `xarray-2023.4.2/properties/test_encode_decode.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/properties/test_pandas_roundtrip.py` & `xarray-2023.4.2/properties/test_pandas_roundtrip.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/pyproject.toml` & `xarray-2023.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/setup.cfg` & `xarray-2023.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/__init__.py` & `xarray-2023.4.2/xarray/__init__.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/__init__.py` & `xarray-2023.4.2/xarray/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/api.py` & `xarray-2023.4.2/xarray/backends/api.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/common.py` & `xarray-2023.4.2/xarray/backends/common.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/file_manager.py` & `xarray-2023.4.2/xarray/backends/file_manager.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/h5netcdf_.py` & `xarray-2023.4.2/xarray/backends/h5netcdf_.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/locks.py` & `xarray-2023.4.2/xarray/backends/locks.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/lru_cache.py` & `xarray-2023.4.2/xarray/backends/lru_cache.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/memory.py` & `xarray-2023.4.2/xarray/backends/memory.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/netCDF4_.py` & `xarray-2023.4.2/xarray/backends/netCDF4_.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/netcdf3.py` & `xarray-2023.4.2/xarray/backends/netcdf3.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/plugins.py` & `xarray-2023.4.2/xarray/backends/plugins.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/pseudonetcdf_.py` & `xarray-2023.4.2/xarray/backends/pseudonetcdf_.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/pydap_.py` & `xarray-2023.4.2/xarray/backends/pydap_.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/pynio_.py` & `xarray-2023.4.2/xarray/backends/pynio_.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/scipy_.py` & `xarray-2023.4.2/xarray/backends/scipy_.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/store.py` & `xarray-2023.4.2/xarray/backends/store.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/backends/zarr.py` & `xarray-2023.4.2/xarray/backends/zarr.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/coding/calendar_ops.py` & `xarray-2023.4.2/xarray/coding/calendar_ops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/coding/cftime_offsets.py` & `xarray-2023.4.2/xarray/coding/cftime_offsets.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/coding/cftimeindex.py` & `xarray-2023.4.2/xarray/coding/cftimeindex.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/coding/frequencies.py` & `xarray-2023.4.2/xarray/coding/frequencies.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/coding/strings.py` & `xarray-2023.4.2/xarray/coding/strings.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/coding/times.py` & `xarray-2023.4.2/xarray/coding/times.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/coding/variables.py` & `xarray-2023.4.2/xarray/coding/variables.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/conventions.py` & `xarray-2023.4.2/xarray/conventions.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/convert.py` & `xarray-2023.4.2/xarray/convert.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/_aggregations.py` & `xarray-2023.4.2/xarray/core/_aggregations.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/_typed_ops.py` & `xarray-2023.4.2/xarray/core/_typed_ops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/_typed_ops.pyi` & `xarray-2023.4.2/xarray/core/_typed_ops.pyi`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/accessor_dt.py` & `xarray-2023.4.2/xarray/core/accessor_dt.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/accessor_str.py` & `xarray-2023.4.2/xarray/core/accessor_str.py`

 * *Files 23% similar despite different names*

```diff
@@ -668,69 +668,165 @@
     def capitalize(self) -> T_DataArray:
         """
         Convert strings in the array to be capitalized.
 
         Returns
         -------
         capitalized : same type as values
+
+        Examples
+        --------
+        >>> da = xr.DataArray(
+        ...     ["temperature", "PRESSURE", "PreCipiTation", "daily rainfall"], dims="x"
+        ... )
+        >>> da
+        <xarray.DataArray (x: 4)>
+        array(['temperature', 'PRESSURE', 'PreCipiTation', 'daily rainfall'],
+              dtype='<U14')
+        Dimensions without coordinates: x
+        >>> capitalized = da.str.capitalize()
+        >>> capitalized
+        <xarray.DataArray (x: 4)>
+        array(['Temperature', 'Pressure', 'Precipitation', 'Daily rainfall'],
+              dtype='<U14')
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.capitalize())
 
     def lower(self) -> T_DataArray:
         """
         Convert strings in the array to lowercase.
 
         Returns
         -------
-        lowerd : same type as values
+        lowered : same type as values
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["Temperature", "PRESSURE"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 2)>
+        array(['Temperature', 'PRESSURE'], dtype='<U11')
+        Dimensions without coordinates: x
+        >>> lowered = da.str.lower()
+        >>> lowered
+        <xarray.DataArray (x: 2)>
+        array(['temperature', 'pressure'], dtype='<U11')
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.lower())
 
     def swapcase(self) -> T_DataArray:
         """
         Convert strings in the array to be swapcased.
 
         Returns
         -------
         swapcased : same type as values
+
+        Examples
+        --------
+        >>> import xarray as xr
+        >>> da = xr.DataArray(["temperature", "PRESSURE", "HuMiDiTy"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['temperature', 'PRESSURE', 'HuMiDiTy'], dtype='<U11')
+        Dimensions without coordinates: x
+        >>> swapcased = da.str.swapcase()
+        >>> swapcased
+        <xarray.DataArray (x: 3)>
+        array(['TEMPERATURE', 'pressure', 'hUmIdItY'], dtype='<U11')
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.swapcase())
 
     def title(self) -> T_DataArray:
         """
         Convert strings in the array to titlecase.
 
         Returns
         -------
         titled : same type as values
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["temperature", "PRESSURE", "HuMiDiTy"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['temperature', 'PRESSURE', 'HuMiDiTy'], dtype='<U11')
+        Dimensions without coordinates: x
+        >>> titled = da.str.title()
+        >>> titled
+        <xarray.DataArray (x: 3)>
+        array(['Temperature', 'Pressure', 'Humidity'], dtype='<U11')
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.title())
 
     def upper(self) -> T_DataArray:
         """
         Convert strings in the array to uppercase.
 
         Returns
         -------
         uppered : same type as values
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["temperature", "HuMiDiTy"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 2)>
+        array(['temperature', 'HuMiDiTy'], dtype='<U11')
+        Dimensions without coordinates: x
+        >>> uppered = da.str.upper()
+        >>> uppered
+        <xarray.DataArray (x: 2)>
+        array(['TEMPERATURE', 'HUMIDITY'], dtype='<U11')
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.upper())
 
     def casefold(self) -> T_DataArray:
         """
         Convert strings in the array to be casefolded.
 
         Casefolding is similar to converting to lowercase,
         but removes all case distinctions.
         This is important in some languages that have more complicated
-        cases and case conversions.
+        cases and case conversions. For example,
+        the 'ß' character in German is case-folded to 'ss', whereas it is lowercased
+        to 'ß'.
 
         Returns
         -------
         casefolded : same type as values
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["TEMPERATURE", "HuMiDiTy"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 2)>
+        array(['TEMPERATURE', 'HuMiDiTy'], dtype='<U11')
+        Dimensions without coordinates: x
+        >>> casefolded = da.str.casefold()
+        >>> casefolded
+        <xarray.DataArray (x: 2)>
+        array(['temperature', 'humidity'], dtype='<U11')
+        Dimensions without coordinates: x
+
+        >>> da = xr.DataArray(["ß", "İ"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 2)>
+        array(['ß', 'İ'], dtype='<U1')
+        Dimensions without coordinates: x
+        >>> casefolded = da.str.casefold()
+        >>> casefolded
+        <xarray.DataArray (x: 2)>
+        array(['ss', 'i̇'], dtype='<U2')
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.casefold())
 
     def normalize(
         self,
         form: str,
     ) -> T_DataArray:
@@ -756,102 +852,228 @@
         """
         Check whether all characters in each string are alphanumeric.
 
         Returns
         -------
         isalnum : array of bool
             Array of boolean values with the same shape as the original array.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["H2O", "NaCl-"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 2)>
+        array(['H2O', 'NaCl-'], dtype='<U5')
+        Dimensions without coordinates: x
+        >>> isalnum = da.str.isalnum()
+        >>> isalnum
+        <xarray.DataArray (x: 2)>
+        array([ True, False])
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.isalnum(), dtype=bool)
 
     def isalpha(self) -> T_DataArray:
         """
         Check whether all characters in each string are alphabetic.
 
         Returns
         -------
         isalpha : array of bool
             Array of boolean values with the same shape as the original array.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["Mn", "H2O", "NaCl-"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['Mn', 'H2O', 'NaCl-'], dtype='<U5')
+        Dimensions without coordinates: x
+        >>> isalpha = da.str.isalpha()
+        >>> isalpha
+        <xarray.DataArray (x: 3)>
+        array([ True, False, False])
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.isalpha(), dtype=bool)
 
     def isdecimal(self) -> T_DataArray:
         """
         Check whether all characters in each string are decimal.
 
         Returns
         -------
         isdecimal : array of bool
             Array of boolean values with the same shape as the original array.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["2.3", "123", "0"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['2.3', '123', '0'], dtype='<U3')
+        Dimensions without coordinates: x
+        >>> isdecimal = da.str.isdecimal()
+        >>> isdecimal
+        <xarray.DataArray (x: 3)>
+        array([False,  True,  True])
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.isdecimal(), dtype=bool)
 
     def isdigit(self) -> T_DataArray:
         """
         Check whether all characters in each string are digits.
 
         Returns
         -------
         isdigit : array of bool
             Array of boolean values with the same shape as the original array.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["123", "1.2", "0", "CO2", "NaCl"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 5)>
+        array(['123', '1.2', '0', 'CO2', 'NaCl'], dtype='<U4')
+        Dimensions without coordinates: x
+        >>> isdigit = da.str.isdigit()
+        >>> isdigit
+        <xarray.DataArray (x: 5)>
+        array([ True, False,  True, False, False])
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.isdigit(), dtype=bool)
 
     def islower(self) -> T_DataArray:
         """
         Check whether all characters in each string are lowercase.
 
         Returns
         -------
         islower : array of bool
-            Array of boolean values with the same shape as the original array.
+            Array of boolean values with the same shape as the original array indicating whether all characters of each
+            element of the string array are lowercase (True) or not (False).
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["temperature", "HUMIDITY", "pREciPiTaTioN"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['temperature', 'HUMIDITY', 'pREciPiTaTioN'], dtype='<U13')
+        Dimensions without coordinates: x
+        >>> islower = da.str.islower()
+        >>> islower
+        <xarray.DataArray (x: 3)>
+        array([ True, False, False])
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.islower(), dtype=bool)
 
     def isnumeric(self) -> T_DataArray:
         """
         Check whether all characters in each string are numeric.
 
         Returns
         -------
         isnumeric : array of bool
             Array of boolean values with the same shape as the original array.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["123", "2.3", "H2O", "NaCl-", "Mn"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 5)>
+        array(['123', '2.3', 'H2O', 'NaCl-', 'Mn'], dtype='<U5')
+        Dimensions without coordinates: x
+        >>> isnumeric = da.str.isnumeric()
+        >>> isnumeric
+        <xarray.DataArray (x: 5)>
+        array([ True, False, False, False, False])
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.isnumeric(), dtype=bool)
 
     def isspace(self) -> T_DataArray:
         """
         Check whether all characters in each string are spaces.
 
         Returns
         -------
         isspace : array of bool
             Array of boolean values with the same shape as the original array.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["", " ", "\\t", "\\n"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 4)>
+        array(['', ' ', '\\t', '\\n'], dtype='<U1')
+        Dimensions without coordinates: x
+        >>> isspace = da.str.isspace()
+        >>> isspace
+        <xarray.DataArray (x: 4)>
+        array([False,  True,  True,  True])
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.isspace(), dtype=bool)
 
     def istitle(self) -> T_DataArray:
         """
         Check whether all characters in each string are titlecase.
 
         Returns
         -------
         istitle : array of bool
             Array of boolean values with the same shape as the original array.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(
+        ...     [
+        ...         "The Evolution Of Species",
+        ...         "The Theory of relativity",
+        ...         "the quantum mechanics of atoms",
+        ...     ],
+        ...     dims="title",
+        ... )
+        >>> da
+        <xarray.DataArray (title: 3)>
+        array(['The Evolution Of Species', 'The Theory of relativity',
+               'the quantum mechanics of atoms'], dtype='<U30')
+        Dimensions without coordinates: title
+        >>> istitle = da.str.istitle()
+        >>> istitle
+        <xarray.DataArray (title: 3)>
+        array([ True, False, False])
+        Dimensions without coordinates: title
         """
         return self._apply(func=lambda x: x.istitle(), dtype=bool)
 
     def isupper(self) -> T_DataArray:
         """
         Check whether all characters in each string are uppercase.
 
         Returns
         -------
         isupper : array of bool
             Array of boolean values with the same shape as the original array.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["TEMPERATURE", "humidity", "PreCIpiTAtioN"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['TEMPERATURE', 'humidity', 'PreCIpiTAtioN'], dtype='<U13')
+        Dimensions without coordinates: x
+        >>> isupper = da.str.isupper()
+        >>> isupper
+        <xarray.DataArray (x: 3)>
+        array([ True, False, False])
+        Dimensions without coordinates: x
         """
         return self._apply(func=lambda x: x.isupper(), dtype=bool)
 
     def count(
         self, pat: str | bytes | Pattern | Any, flags: int = 0, case: bool | None = None
     ) -> T_DataArray:
         """
@@ -879,14 +1101,54 @@
             If True, case sensitive.
             Cannot be set if `pat` is a compiled regex.
             Equivalent to setting the `re.IGNORECASE` flag.
 
         Returns
         -------
         counts : array of int
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["jjklmn", "opjjqrs", "t-JJ99vwx"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['jjklmn', 'opjjqrs', 't-JJ99vwx'], dtype='<U9')
+        Dimensions without coordinates: x
+
+        Using a string:
+        >>> da.str.count("jj")
+        <xarray.DataArray (x: 3)>
+        array([1, 1, 0])
+        Dimensions without coordinates: x
+
+        Enable case-insensitive matching by setting case to false:
+        >>> counts = da.str.count("jj", case=False)
+        >>> counts
+        <xarray.DataArray (x: 3)>
+        array([1, 1, 1])
+        Dimensions without coordinates: x
+
+        Using regex:
+        >>> pat = "JJ[0-9]{2}[a-z]{3}"
+        >>> counts = da.str.count(pat)
+        >>> counts
+        <xarray.DataArray (x: 3)>
+        array([0, 0, 1])
+        Dimensions without coordinates: x
+
+        Using an array of strings (the pattern will be broadcast against the array):
+
+        >>> pat = xr.DataArray(["jj", "JJ"], dims="y")
+        >>> counts = da.str.count(pat)
+        >>> counts
+        <xarray.DataArray (x: 3, y: 2)>
+        array([[1, 0],
+               [1, 0],
+               [0, 1]])
+        Dimensions without coordinates: x, y
         """
         pat = self._re_compile(pat=pat, flags=flags, case=case)
 
         func = lambda x, ipat: len(ipat.findall(x))
         return self._apply(func=func, func_args=(pat,), dtype=int)
 
     def startswith(self, pat: str | bytes | Any) -> T_DataArray:
@@ -903,14 +1165,27 @@
             If array-like, it is broadcast.
 
         Returns
         -------
         startswith : array of bool
             An array of booleans indicating whether the given pattern matches
             the start of each string element.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["$100", "£23", "100"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['$100', '£23', '100'], dtype='<U4')
+        Dimensions without coordinates: x
+        >>> startswith = da.str.startswith("$")
+        >>> startswith
+        <xarray.DataArray (x: 3)>
+        array([ True, False, False])
+        Dimensions without coordinates: x
         """
         pat = self._stringify(pat)
         func = lambda x, y: x.startswith(y)
         return self._apply(func=func, func_args=(pat,), dtype=bool)
 
     def endswith(self, pat: str | bytes | Any) -> T_DataArray:
         """
@@ -926,14 +1201,27 @@
             If array-like, it is broadcast.
 
         Returns
         -------
         endswith : array of bool
             A Series of booleans indicating whether the given pattern matches
             the end of each string element.
+
+        Examples
+        --------
+        >>> da = xr.DataArray(["10C", "10c", "100F"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 3)>
+        array(['10C', '10c', '100F'], dtype='<U4')
+        Dimensions without coordinates: x
+        >>> endswith = da.str.endswith("C")
+        >>> endswith
+        <xarray.DataArray (x: 3)>
+        array([ True, False, False])
+        Dimensions without coordinates: x
         """
         pat = self._stringify(pat)
         func = lambda x, y: x.endswith(y)
         return self._apply(func=func, func_args=(pat,), dtype=bool)
 
     def pad(
         self,
@@ -959,14 +1247,74 @@
             Additional character for filling, default is a space.
             If array-like, it is broadcast.
 
         Returns
         -------
         filled : same type as values
             Array with a minimum number of char in each element.
+
+        Examples
+        --------
+        Pad strings in the array with a single string on the left side.
+
+        Define the string in the array.
+
+        >>> da = xr.DataArray(["PAR184", "TKO65", "NBO9139", "NZ39"], dims="x")
+        >>> da
+        <xarray.DataArray (x: 4)>
+        array(['PAR184', 'TKO65', 'NBO9139', 'NZ39'], dtype='<U7')
+        Dimensions without coordinates: x
+
+        Pad the strings
+
+        >>> filled = da.str.pad(8, side="left", fillchar="0")
+        >>> filled
+        <xarray.DataArray (x: 4)>
+        array(['00PAR184', '000TKO65', '0NBO9139', '0000NZ39'], dtype='<U8')
+        Dimensions without coordinates: x
+
+        Pad strings on the right side
+
+        >>> filled = da.str.pad(8, side="right", fillchar="0")
+        >>> filled
+        <xarray.DataArray (x: 4)>
+        array(['PAR18400', 'TKO65000', 'NBO91390', 'NZ390000'], dtype='<U8')
+        Dimensions without coordinates: x
+
+        Pad strings on both sides
+
+        >>> filled = da.str.pad(8, side="both", fillchar="0")
+        >>> filled
+        <xarray.DataArray (x: 4)>
+        array(['0PAR1840', '0TKO6500', 'NBO91390', '00NZ3900'], dtype='<U8')
+        Dimensions without coordinates: x
+
+        Using an array-like width
+
+        >>> width = xr.DataArray([8, 10], dims="y")
+        >>> filled = da.str.pad(width, side="left", fillchar="0")
+        >>> filled
+        <xarray.DataArray (x: 4, y: 2)>
+        array([['00PAR184', '0000PAR184'],
+               ['000TKO65', '00000TKO65'],
+               ['0NBO9139', '000NBO9139'],
+               ['0000NZ39', '000000NZ39']], dtype='<U10')
+        Dimensions without coordinates: x, y
+
+        Using an array-like value for fillchar
+
+        >>> fillchar = xr.DataArray(["0", "-"], dims="y")
+        >>> filled = da.str.pad(8, side="left", fillchar=fillchar)
+        >>> filled
+        <xarray.DataArray (x: 4, y: 2)>
+        array([['00PAR184', '--PAR184'],
+               ['000TKO65', '---TKO65'],
+               ['0NBO9139', '-NBO9139'],
+               ['0000NZ39', '----NZ39']], dtype='<U8')
+        Dimensions without coordinates: x, y
         """
         if side == "left":
             func = self.rjust
         elif side == "right":
             func = self.ljust
         elif side == "both":
             func = self.center
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xarray-2023.4.1/xarray/core/alignment.py` & `xarray-2023.4.2/xarray/core/alignment.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/arithmetic.py` & `xarray-2023.4.2/xarray/core/arithmetic.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/combine.py` & `xarray-2023.4.2/xarray/core/combine.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/common.py` & `xarray-2023.4.2/xarray/core/common.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/computation.py` & `xarray-2023.4.2/xarray/core/computation.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/concat.py` & `xarray-2023.4.2/xarray/core/concat.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/coordinates.py` & `xarray-2023.4.2/xarray/core/coordinates.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/dask_array_ops.py` & `xarray-2023.4.2/xarray/core/dask_array_ops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/dataarray.py` & `xarray-2023.4.2/xarray/core/dataarray.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/dataset.py` & `xarray-2023.4.2/xarray/core/dataset.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/dtypes.py` & `xarray-2023.4.2/xarray/core/dtypes.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/duck_array_ops.py` & `xarray-2023.4.2/xarray/core/duck_array_ops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/extensions.py` & `xarray-2023.4.2/xarray/core/extensions.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/formatting.py` & `xarray-2023.4.2/xarray/core/formatting.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/formatting_html.py` & `xarray-2023.4.2/xarray/core/formatting_html.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/groupby.py` & `xarray-2023.4.2/xarray/core/groupby.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,16 @@
     if duck_array_ops.isnull(bins).all():
         raise ValueError("All bin edges are NaN.")
     binned, bins = pd.cut(group.values, bins, **cut_kwargs, retbins=True)
     codes = binned.codes
     if (codes == -1).all():
         raise ValueError(f"None of the data falls within bins with edges {bins!r}")
     full_index = binned.categories
-    unique_values = np.sort(binned.unique().dropna())
+    uniques = np.sort(pd.unique(codes))
+    unique_values = full_index[uniques[uniques != -1]]
     group_indices = [g for g in _codes_to_groups(codes, len(full_index)) if g]
 
     if len(group_indices) == 0:
         raise ValueError(f"None of the data falls within bins with edges {bins!r}")
 
     new_dim_name = str(group.name) + "_bins"
     group_ = DataArray(binned, getattr(group, "coords", None), name=new_dim_name)
```

### Comparing `xarray-2023.4.1/xarray/core/indexes.py` & `xarray-2023.4.2/xarray/core/indexes.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/indexing.py` & `xarray-2023.4.2/xarray/core/indexing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/merge.py` & `xarray-2023.4.2/xarray/core/merge.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/missing.py` & `xarray-2023.4.2/xarray/core/missing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/nanops.py` & `xarray-2023.4.2/xarray/core/nanops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/npcompat.py` & `xarray-2023.4.2/xarray/core/npcompat.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/nputils.py` & `xarray-2023.4.2/xarray/core/nputils.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/ops.py` & `xarray-2023.4.2/xarray/core/ops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/options.py` & `xarray-2023.4.2/xarray/core/options.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/parallel.py` & `xarray-2023.4.2/xarray/core/parallel.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/pdcompat.py` & `xarray-2023.4.2/xarray/core/pdcompat.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/pycompat.py` & `xarray-2023.4.2/xarray/core/pycompat.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/resample.py` & `xarray-2023.4.2/xarray/core/resample.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/resample_cftime.py` & `xarray-2023.4.2/xarray/core/resample_cftime.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/rolling.py` & `xarray-2023.4.2/xarray/core/rolling.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/rolling_exp.py` & `xarray-2023.4.2/xarray/core/rolling_exp.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/types.py` & `xarray-2023.4.2/xarray/core/types.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/utils.py` & `xarray-2023.4.2/xarray/core/utils.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/variable.py` & `xarray-2023.4.2/xarray/core/variable.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/core/weighted.py` & `xarray-2023.4.2/xarray/core/weighted.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/plot/__init__.py` & `xarray-2023.4.2/xarray/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/plot/accessor.py` & `xarray-2023.4.2/xarray/plot/accessor.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/plot/dataarray_plot.py` & `xarray-2023.4.2/xarray/plot/dataarray_plot.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/plot/dataset_plot.py` & `xarray-2023.4.2/xarray/plot/dataset_plot.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/plot/facetgrid.py` & `xarray-2023.4.2/xarray/plot/facetgrid.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/plot/utils.py` & `xarray-2023.4.2/xarray/plot/utils.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/static/css/style.css` & `xarray-2023.4.2/xarray/static/css/style.css`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/static/html/icons-svg-inline.html` & `xarray-2023.4.2/xarray/static/html/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/testing.py` & `xarray-2023.4.2/xarray/testing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/__init__.py` & `xarray-2023.4.2/xarray/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/conftest.py` & `xarray-2023.4.2/xarray/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/data/bears.nc` & `xarray-2023.4.2/xarray/tests/data/bears.nc`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/data/example.grib` & `xarray-2023.4.2/xarray/tests/data/example.grib`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/data/example.ict` & `xarray-2023.4.2/xarray/tests/data/example.ict`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/data/example.uamiv` & `xarray-2023.4.2/xarray/tests/data/example.uamiv`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/data/example_1.nc` & `xarray-2023.4.2/xarray/tests/data/example_1.nc`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_accessor_dt.py` & `xarray-2023.4.2/xarray/tests/test_accessor_dt.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_accessor_str.py` & `xarray-2023.4.2/xarray/tests/test_accessor_str.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_array_api.py` & `xarray-2023.4.2/xarray/tests/test_array_api.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_backends.py` & `xarray-2023.4.2/xarray/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_backends_api.py` & `xarray-2023.4.2/xarray/tests/test_backends_api.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_backends_common.py` & `xarray-2023.4.2/xarray/tests/test_backends_common.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_backends_file_manager.py` & `xarray-2023.4.2/xarray/tests/test_backends_file_manager.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_backends_lru_cache.py` & `xarray-2023.4.2/xarray/tests/test_backends_lru_cache.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_calendar_ops.py` & `xarray-2023.4.2/xarray/tests/test_calendar_ops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_cftime_offsets.py` & `xarray-2023.4.2/xarray/tests/test_cftime_offsets.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_cftimeindex.py` & `xarray-2023.4.2/xarray/tests/test_cftimeindex.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_cftimeindex_resample.py` & `xarray-2023.4.2/xarray/tests/test_cftimeindex_resample.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_coarsen.py` & `xarray-2023.4.2/xarray/tests/test_coarsen.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_coding.py` & `xarray-2023.4.2/xarray/tests/test_coding.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_coding_strings.py` & `xarray-2023.4.2/xarray/tests/test_coding_strings.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_coding_times.py` & `xarray-2023.4.2/xarray/tests/test_coding_times.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_combine.py` & `xarray-2023.4.2/xarray/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_computation.py` & `xarray-2023.4.2/xarray/tests/test_computation.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_concat.py` & `xarray-2023.4.2/xarray/tests/test_concat.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_conventions.py` & `xarray-2023.4.2/xarray/tests/test_conventions.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_cupy.py` & `xarray-2023.4.2/xarray/tests/test_cupy.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_dask.py` & `xarray-2023.4.2/xarray/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_dataarray.py` & `xarray-2023.4.2/xarray/tests/test_dataarray.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_dataset.py` & `xarray-2023.4.2/xarray/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_deprecation_helpers.py` & `xarray-2023.4.2/xarray/tests/test_deprecation_helpers.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_distributed.py` & `xarray-2023.4.2/xarray/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_dtypes.py` & `xarray-2023.4.2/xarray/tests/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_duck_array_ops.py` & `xarray-2023.4.2/xarray/tests/test_duck_array_ops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_extensions.py` & `xarray-2023.4.2/xarray/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_formatting.py` & `xarray-2023.4.2/xarray/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_formatting_html.py` & `xarray-2023.4.2/xarray/tests/test_formatting_html.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_groupby.py` & `xarray-2023.4.2/xarray/tests/test_groupby.py`

 * *Files 2% similar despite different names*

```diff
@@ -1369,57 +1369,101 @@
             coords=array.coords,
             dims=array.dims,
         )
         assert_identical(expected, actual)
 
     @pytest.mark.parametrize("use_flox", [True, False])
     @pytest.mark.parametrize("coords", [np.arange(4), np.arange(4)[::-1], [2, 0, 3, 1]])
-    def test_groupby_bins(self, coords: np.typing.ArrayLike, use_flox: bool) -> None:
+    @pytest.mark.parametrize(
+        "cut_kwargs",
+        (
+            {"labels": None, "include_lowest": True},
+            {"labels": None, "include_lowest": False},
+            {"labels": ["a", "b"]},
+            {"labels": [1.2, 3.5]},
+            {"labels": ["b", "a"]},
+        ),
+    )
+    def test_groupby_bins(
+        self,
+        coords: np.typing.ArrayLike,
+        use_flox: bool,
+        cut_kwargs: dict,
+    ) -> None:
         array = DataArray(
             np.arange(4), dims="dim_0", coords={"dim_0": coords}, name="a"
         )
         # the first value should not be part of any group ("right" binning)
         array[0] = 99
         # bins follow conventions for pandas.cut
         # http://pandas.pydata.org/pandas-docs/stable/generated/pandas.cut.html
         bins = [0, 1.5, 5]
 
         df = array.to_dataframe()
-        df["dim_0_bins"] = pd.cut(array["dim_0"], bins)
+        df["dim_0_bins"] = pd.cut(array["dim_0"], bins, **cut_kwargs)
 
         expected_df = df.groupby("dim_0_bins").sum()
         # TODO: can't convert df with IntervalIndex to Xarray
-
         expected = (
             expected_df.reset_index(drop=True)
             .to_xarray()
             .assign_coords(index=np.array(expected_df.index))
             .rename({"index": "dim_0_bins"})["a"]
         )
 
         with xr.set_options(use_flox=use_flox):
-            actual = array.groupby_bins("dim_0", bins=bins).sum()
+            actual = array.groupby_bins("dim_0", bins=bins, **cut_kwargs).sum()
             assert_identical(expected, actual)
 
-            actual = array.groupby_bins("dim_0", bins=bins, labels=[1.2, 3.5]).sum()
-            assert_identical(expected.assign_coords(dim_0_bins=[1.2, 3.5]), actual)
-
-            actual = array.groupby_bins("dim_0", bins=bins).map(lambda x: x.sum())
+            actual = array.groupby_bins("dim_0", bins=bins, **cut_kwargs).map(
+                lambda x: x.sum()
+            )
             assert_identical(expected, actual)
 
             # make sure original array dims are unchanged
             assert len(array.dim_0) == 4
 
-            da = xr.DataArray(np.ones((2, 3, 4)))
-            bins = [-1, 0, 1, 2]
-            with xr.set_options(use_flox=False):
-                actual = da.groupby_bins("dim_0", bins).mean(...)
-            with xr.set_options(use_flox=True):
-                expected = da.groupby_bins("dim_0", bins).mean(...)
-            assert_allclose(actual, expected)
+    def test_groupby_bins_ellipsis(self):
+        da = xr.DataArray(np.ones((2, 3, 4)))
+        bins = [-1, 0, 1, 2]
+        with xr.set_options(use_flox=False):
+            actual = da.groupby_bins("dim_0", bins).mean(...)
+        with xr.set_options(use_flox=True):
+            expected = da.groupby_bins("dim_0", bins).mean(...)
+        assert_allclose(actual, expected)
+
+    @pytest.mark.parametrize("use_flox", [True, False])
+    def test_groupby_bins_gives_correct_subset(self, use_flox: bool) -> None:
+        # GH7766
+        rng = np.random.default_rng(42)
+        coords = rng.normal(5, 5, 1000)
+        bins = np.logspace(-4, 1, 10)
+        labels = [
+            "one",
+            "two",
+            "three",
+            "four",
+            "five",
+            "six",
+            "seven",
+            "eight",
+            "nine",
+        ]
+        # xArray
+        # Make a mock dataarray
+        darr = xr.DataArray(coords, coords=[coords], dims=["coords"])
+        expected = xr.DataArray(
+            [np.nan, np.nan, 1, 1, 1, 8, 31, 104, 542],
+            dims="coords_bins",
+            coords={"coords_bins": labels},
+        )
+        gb = darr.groupby_bins("coords", bins, labels=labels)
+        with xr.set_options(use_flox=use_flox):
+            actual = gb.count()
+        assert_identical(actual, expected)
 
     def test_groupby_bins_empty(self):
         array = DataArray(np.arange(4), [("x", range(4))])
         # one of these bins will be empty
         bins = [0, 4, 5]
         bin_coords = pd.cut(array["x"], bins).categories
         actual = array.groupby_bins("x", bins).sum()
```

### Comparing `xarray-2023.4.1/xarray/tests/test_indexes.py` & `xarray-2023.4.2/xarray/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_indexing.py` & `xarray-2023.4.2/xarray/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_interp.py` & `xarray-2023.4.2/xarray/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_merge.py` & `xarray-2023.4.2/xarray/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_missing.py` & `xarray-2023.4.2/xarray/tests/test_missing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_nputils.py` & `xarray-2023.4.2/xarray/tests/test_nputils.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_options.py` & `xarray-2023.4.2/xarray/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_plot.py` & `xarray-2023.4.2/xarray/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_plugins.py` & `xarray-2023.4.2/xarray/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_rolling.py` & `xarray-2023.4.2/xarray/tests/test_rolling.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_sparse.py` & `xarray-2023.4.2/xarray/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_testing.py` & `xarray-2023.4.2/xarray/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_tutorial.py` & `xarray-2023.4.2/xarray/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_ufuncs.py` & `xarray-2023.4.2/xarray/tests/test_ufuncs.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_units.py` & `xarray-2023.4.2/xarray/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_utils.py` & `xarray-2023.4.2/xarray/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_variable.py` & `xarray-2023.4.2/xarray/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tests/test_weighted.py` & `xarray-2023.4.2/xarray/tests/test_weighted.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/tutorial.py` & `xarray-2023.4.2/xarray/tutorial.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/util/deprecation_helpers.py` & `xarray-2023.4.2/xarray/util/deprecation_helpers.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/util/generate_aggregations.py` & `xarray-2023.4.2/xarray/util/generate_aggregations.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/util/generate_ops.py` & `xarray-2023.4.2/xarray/util/generate_ops.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray/util/print_versions.py` & `xarray-2023.4.2/xarray/util/print_versions.py`

 * *Files identical despite different names*

### Comparing `xarray-2023.4.1/xarray.egg-info/PKG-INFO` & `xarray-2023.4.2/xarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: N-D labeled arrays and datasets in Python
 Home-page: https://github.com/pydata/xarray
 Author: xarray Developers
 Author-email: xarray@googlegroups.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `xarray-2023.4.1/xarray.egg-info/SOURCES.txt` & `xarray-2023.4.2/xarray.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 .github/dependabot.yml
 .github/labeler.yml
 .github/stale.yml
 .github/ISSUE_TEMPLATE/bugreport.yml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/misc.yml
 .github/ISSUE_TEMPLATE/newfeature.yml
+.github/workflows/benchmarks-last-release.yml
 .github/workflows/benchmarks.yml
 .github/workflows/ci-additional.yaml
 .github/workflows/ci.yaml
 .github/workflows/configure-testpypi-version.py
 .github/workflows/label-all.yml
 .github/workflows/label-prs.yml
 .github/workflows/parse_logs.py
```

### Comparing `xarray-2023.4.1/xarray.egg-info/requires.txt` & `xarray-2023.4.2/xarray.egg-info/requires.txt`

 * *Files identical despite different names*

