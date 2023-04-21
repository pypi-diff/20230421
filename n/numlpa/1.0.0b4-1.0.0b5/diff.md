# Comparing `tmp/numlpa-1.0.0b4.tar.gz` & `tmp/numlpa-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numlpa-1.0.0b4.tar", last modified: Mon Apr  3 21:08:50 2023, max compression
+gzip compressed data, was "numlpa-1.0.0b5.tar", last modified: Fri Apr 21 19:36:21 2023, max compression
```

## Comparing `numlpa-1.0.0b4.tar` & `numlpa-1.0.0b5.tar`

### file list

```diff
@@ -1,120 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.772823 numlpa-1.0.0b4/
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3191 2023-04-03 21:08:50.772823 numlpa-1.0.0b4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2638 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.740820 numlpa-1.0.0b4/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.742820 numlpa-1.0.0b4/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.730819 numlpa-1.0.0b4/docs/source/figures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.742820 numlpa-1.0.0b4/docs/source/figures/distributions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.742820 numlpa-1.0.0b4/docs/source/figures/distributions/dipoles/
--rw-rw-rw-   0 root         (0) root         (0)    76220 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/figures/distributions/dipoles/0.svg
--rwxrwxrwx   0 root         (0) root         (0)      369 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/figures/distributions/generate.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.743820 numlpa-1.0.0b4/docs/source/figures/distributions/images/
--rw-rw-rw-   0 root         (0) root         (0)   127041 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/figures/distributions/images/0.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.743820 numlpa-1.0.0b4/docs/source/figures/distributions/wilkens/
--rw-rw-rw-   0 root         (0) root         (0)    53578 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/figures/distributions/wilkens/0.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.745821 numlpa-1.0.0b4/docs/source/figures/restrictions/
--rw-rw-rw-   0 root         (0) root         (0)    39360 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/figures/restrictions/affine.svg
--rwxrwxrwx   0 root         (0) root         (0)     2201 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/figures/restrictions/generate.py
--rw-rw-rw-   0 root         (0) root         (0)    34233 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/figures/restrictions/none.svg
--rw-rw-rw-   0 root         (0) root         (0)    33981 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/figures/restrictions/positive.svg
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    13421 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.745821 numlpa-1.0.0b4/docs/source/practice/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.747821 numlpa-1.0.0b4/docs/source/practice/examples/
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/examples/configuration.rst
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/examples/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1379 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/examples/vanilla.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.748821 numlpa-1.0.0b4/docs/source/practice/formats/
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/formats/dislocation-sample.rst
--rw-rw-rw-   0 root         (0) root         (0)     3850 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/formats/fourier-transform.rst
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/formats/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3644 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/formats/model-adjustment.rst
--rw-rw-rw-   0 root         (0) root         (0)     3407 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/formats/spatial-analysis.rst
--rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.750821 numlpa-1.0.0b4/docs/source/practice/installation/
--rw-rw-rw-   0 root         (0) root         (0)     1457 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/installation/editable.rst
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/installation/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/installation/regular.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/docs/source/practice/installation/venv.rst
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 21:08:50.772823 numlpa-1.0.0b4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      414 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/setup.py
--rwxrwxrwx   0 root         (0) root         (0)     3022 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/setup.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.732819 numlpa-1.0.0b4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.751821 numlpa-1.0.0b4/src/numlpa/
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/__main__.py
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-03 21:08:50.000000 numlpa-1.0.0b4/src/numlpa/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.755821 numlpa-1.0.0b4/src/numlpa/core/
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/core/parallelism.py
--rw-rw-rw-   0 root         (0) root         (0)     9084 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/core/storage.py
--rw-rw-rw-   0 root         (0) root         (0)     1563 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/default.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.755821 numlpa-1.0.0b4/src/numlpa/kits/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.755821 numlpa-1.0.0b4/src/numlpa/kits/analyzers/
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/analyzers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.757822 numlpa-1.0.0b4/src/numlpa/kits/analyzers/cpu/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/analyzers/cpu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10029 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/analyzers/cpu/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3579 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/analyzers/cpu/interactionmodule.c
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/analyzers/cpu/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.757822 numlpa-1.0.0b4/src/numlpa/kits/diffractometers/
--rw-rw-rw-   0 root         (0) root         (0)     2130 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/diffractometers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.759822 numlpa-1.0.0b4/src/numlpa/kits/diffractometers/cpu/
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/diffractometers/cpu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17138 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/diffractometers/cpu/diffraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/diffractometers/cpu/displacementmodule.c
--rw-rw-rw-   0 root         (0) root         (0)     2523 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/diffractometers/cpu/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.760822 numlpa-1.0.0b4/src/numlpa/kits/distributions/
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/distributions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4160 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/distributions/dipoles.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/distributions/images.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/distributions/wilkens.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.761822 numlpa-1.0.0b4/src/numlpa/kits/fonts/
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   847840 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/fonts/latinmodern-math.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.764822 numlpa-1.0.0b4/src/numlpa/kits/models/
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/models/guw.py
--rw-rw-rw-   0 root         (0) root         (0)     3554 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/models/kr.py
--rw-rw-rw-   0 root         (0) root         (0)     4453 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/models/wilkens.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.765822 numlpa-1.0.0b4/src/numlpa/kits/optimizers/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/optimizers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3918 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/optimizers/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.766822 numlpa-1.0.0b4/src/numlpa/kits/representations/
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/representations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6484 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/representations/affine.py
--rw-rw-rw-   0 root         (0) root         (0)    10640 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/representations/basic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.767823 numlpa-1.0.0b4/src/numlpa/kits/restrictions/
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/restrictions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/restrictions/affine.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/restrictions/none.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/kits/restrictions/positive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.770823 numlpa-1.0.0b4/src/numlpa/main/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/main/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/main/analyze.py
--rw-rw-rw-   0 root         (0) root         (0)     4920 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/main/diffract.py
--rw-rw-rw-   0 root         (0) root         (0)     4581 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/main/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     7552 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/main/export.py
--rw-rw-rw-   0 root         (0) root         (0)     6866 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/main/extract.py
--rw-rw-rw-   0 root         (0) root         (0)     9748 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/main/fit.py
--rw-rw-rw-   0 root         (0) root         (0)     5169 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/src/numlpa/main/merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.754821 numlpa-1.0.0b4/src/numlpa.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3191 2023-04-03 21:08:50.000000 numlpa-1.0.0b4/src/numlpa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2984 2023-04-03 21:08:50.000000 numlpa-1.0.0b4/src/numlpa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 21:08:50.000000 numlpa-1.0.0b4/src/numlpa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-03 21:08:50.000000 numlpa-1.0.0b4/src/numlpa.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-03 21:08:50.000000 numlpa-1.0.0b4/src/numlpa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-03 21:08:50.000000 numlpa-1.0.0b4/src/numlpa.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.771823 numlpa-1.0.0b4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 21:08:50.771823 numlpa-1.0.0b4/tests/material/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/tests/material/.gitignore
--rwxrwxrwx   0 root         (0) root         (0)    30553 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/tests/references.json
--rwxrwxrwx   0 root         (0) root         (0)     5729 2023-04-03 21:07:53.000000 numlpa-1.0.0b4/tests/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.788021 numlpa-1.0.0b5/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3360 2023-04-21 19:36:21.788021 numlpa-1.0.0b5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.754018 numlpa-1.0.0b5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.755018 numlpa-1.0.0b5/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.744018 numlpa-1.0.0b5/docs/source/figures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.756018 numlpa-1.0.0b5/docs/source/figures/distributions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.756018 numlpa-1.0.0b5/docs/source/figures/distributions/dipoles/
+-rw-rw-rw-   0 root         (0) root         (0)    76220 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/figures/distributions/dipoles/0.svg
+-rwxrwxrwx   0 root         (0) root         (0)      369 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/figures/distributions/generate.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.757019 numlpa-1.0.0b5/docs/source/figures/distributions/images/
+-rw-rw-rw-   0 root         (0) root         (0)   127041 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/figures/distributions/images/0.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.757019 numlpa-1.0.0b5/docs/source/figures/distributions/wilkens/
+-rw-rw-rw-   0 root         (0) root         (0)    53578 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/figures/distributions/wilkens/0.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.759019 numlpa-1.0.0b5/docs/source/figures/restrictions/
+-rw-rw-rw-   0 root         (0) root         (0)    39360 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/figures/restrictions/affine.svg
+-rwxrwxrwx   0 root         (0) root         (0)     2201 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/figures/restrictions/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)    34233 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/figures/restrictions/none.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33981 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/figures/restrictions/positive.svg
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    13421 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.759019 numlpa-1.0.0b5/docs/source/practice/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.761019 numlpa-1.0.0b5/docs/source/practice/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/examples/configuration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/examples/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/examples/vanilla.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.763019 numlpa-1.0.0b5/docs/source/practice/formats/
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/formats/dislocation-sample.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/formats/energy-evaluation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/formats/fourier-transform.rst
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/formats/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3643 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/formats/model-adjustment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3406 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/formats/spatial-analysis.rst
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.764019 numlpa-1.0.0b5/docs/source/practice/installation/
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/installation/editable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/installation/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/installation/regular.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/docs/source/practice/installation/venv.rst
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 19:36:21.788021 numlpa-1.0.0b5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      569 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/setup.py
+-rwxrwxrwx   0 root         (0) root         (0)     3022 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.746018 numlpa-1.0.0b5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.765019 numlpa-1.0.0b5/src/numlpa/
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2677 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      162 2023-04-21 19:36:21.000000 numlpa-1.0.0b5/src/numlpa/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.769019 numlpa-1.0.0b5/src/numlpa/core/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/core/parallelism.py
+-rw-rw-rw-   0 root         (0) root         (0)     9084 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/core/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/default.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.769019 numlpa-1.0.0b5/src/numlpa/kits/
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.769019 numlpa-1.0.0b5/src/numlpa/kits/analyzers/
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/analyzers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.771020 numlpa-1.0.0b5/src/numlpa/kits/analyzers/cpu/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/analyzers/cpu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10029 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/analyzers/cpu/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/analyzers/cpu/interactionmodule.c
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/analyzers/cpu/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.772020 numlpa-1.0.0b5/src/numlpa/kits/diffractometers/
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/diffractometers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.773020 numlpa-1.0.0b5/src/numlpa/kits/diffractometers/cpu/
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/diffractometers/cpu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/diffractometers/cpu/diffraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/diffractometers/cpu/displacementmodule.c
+-rw-rw-rw-   0 root         (0) root         (0)     2501 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/diffractometers/cpu/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.775020 numlpa-1.0.0b5/src/numlpa/kits/distributions/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/distributions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4160 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/distributions/dipoles.py
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/distributions/images.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/distributions/wilkens.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.775020 numlpa-1.0.0b5/src/numlpa/kits/evaluators/
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/evaluators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.777020 numlpa-1.0.0b5/src/numlpa/kits/evaluators/cpu/
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/evaluators/cpu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5693 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/evaluators/cpu/energymodule.c
+-rw-rw-rw-   0 root         (0) root         (0)    12124 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/evaluators/cpu/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/evaluators/cpu/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.777020 numlpa-1.0.0b5/src/numlpa/kits/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   847840 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/fonts/latinmodern-math.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.780020 numlpa-1.0.0b5/src/numlpa/kits/models/
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/models/guw.py
+-rw-rw-rw-   0 root         (0) root         (0)     3554 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/models/kr.py
+-rw-rw-rw-   0 root         (0) root         (0)     4453 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/models/wilkens.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.781020 numlpa-1.0.0b5/src/numlpa/kits/optimizers/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/optimizers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/optimizers/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.782020 numlpa-1.0.0b5/src/numlpa/kits/representations/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/representations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6484 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/representations/affine.py
+-rw-rw-rw-   0 root         (0) root         (0)    10640 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/representations/basic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.783021 numlpa-1.0.0b5/src/numlpa/kits/restrictions/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/restrictions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/restrictions/affine.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/restrictions/none.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/kits/restrictions/positive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.786021 numlpa-1.0.0b5/src/numlpa/main/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/analyze.py
+-rw-rw-rw-   0 root         (0) root         (0)     4920 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/diffract.py
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     4878 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/evaluate.py
+-rw-rw-rw-   0 root         (0) root         (0)     7552 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     6866 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     9748 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/fit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7077 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/src/numlpa/main/merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.767019 numlpa-1.0.0b5/src/numlpa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3360 2023-04-21 19:36:21.000000 numlpa-1.0.0b5/src/numlpa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3277 2023-04-21 19:36:21.000000 numlpa-1.0.0b5/src/numlpa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:36:21.000000 numlpa-1.0.0b5/src/numlpa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-21 19:36:21.000000 numlpa-1.0.0b5/src/numlpa.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-21 19:36:21.000000 numlpa-1.0.0b5/src/numlpa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-21 19:36:21.000000 numlpa-1.0.0b5/src/numlpa.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.787021 numlpa-1.0.0b5/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:36:21.788021 numlpa-1.0.0b5/tests/material/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/tests/material/.gitignore
+-rwxrwxrwx   0 root         (0) root         (0)    36434 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/tests/references.json
+-rwxrwxrwx   0 root         (0) root         (0)     6593 2023-04-21 19:35:24.000000 numlpa-1.0.0b5/tests/run.py
```

### Comparing `numlpa-1.0.0b4/LICENSE.txt` & `numlpa-1.0.0b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/PKG-INFO` & `numlpa-1.0.0b5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numlpa
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: Numerical Line Profile Analysis package.
 Author-email: Dunstan Becht <dunstan.becht@orange.fr>
 Project-URL: Homepage, https://gitlab.com/x-rays/numlpa
 Project-URL: Bug Tracker, https://gitlab.com/x-rays/numlpa/issues
 Project-URL: Documentation, https://x-rays.gitlab.io/numlpa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -35,26 +35,27 @@
 ## Features
 
 NumLPA Has been developed to meet the need to analyze the accuracy of LPA models.
 The main features of the package are presented bellow:
 
 * `draw`: Generate samples of dislocations by random drawing from different probability distribution models.
 * `diffract`: Simulate X-ray diffraction on crystals containing the previously generated dislocations and compute the Fourier transform of the diffracted intensity.
-* `merge`: Average the Fourier transform coefficients from multiples samples drawn from a same distribution.
+* `merge`: Average the Fourier transform coefficients or the strain energy evaluations from multiple samples drawn from a same distribution.
 * `fit`: Fit LPA models on the simulated diffraction profiles to obtain their predictions and compare them to the real parameters of the distribution.
+* `evaluate`: Compute the strain energy density and the outer cut-off radius for a sample of dislocations.
 * `analyze`: Perform a spatial statistical analysis and calculate the strain energy contained in a sample of dislocations.
 * `export`: Export figures illustrating the previously generated data according to different representations.
 
 ## Installation
 
-You can find how to install the package in the [installation section](https://x-rays.gitlab.io/numlpa/installation.html) of the documentation.
+You can find how to install the package in the [installation section](https://x-rays.gitlab.io/numlpa/practice/installation/index.html) of the documentation.
 
 ## Usage
 
-You can find how to use the package in the [examples section](https://x-rays.gitlab.io/numlpa/examples.html) of the documentation.
+You can find how to use the package in the [examples section](https://x-rays.gitlab.io/numlpa/practice/examples/index.html) of the documentation.
 
 ## Credits
 
 * Dunstan Becht
 * Asdin Aoufi
 * András Borbély
```

### Comparing `numlpa-1.0.0b4/README.md` & `numlpa-1.0.0b5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 ## Features
 
 NumLPA Has been developed to meet the need to analyze the accuracy of LPA models.
 The main features of the package are presented bellow:
 
 * `draw`: Generate samples of dislocations by random drawing from different probability distribution models.
 * `diffract`: Simulate X-ray diffraction on crystals containing the previously generated dislocations and compute the Fourier transform of the diffracted intensity.
-* `merge`: Average the Fourier transform coefficients from multiples samples drawn from a same distribution.
+* `merge`: Average the Fourier transform coefficients or the strain energy evaluations from multiple samples drawn from a same distribution.
 * `fit`: Fit LPA models on the simulated diffraction profiles to obtain their predictions and compare them to the real parameters of the distribution.
+* `evaluate`: Compute the strain energy density and the outer cut-off radius for a sample of dislocations.
 * `analyze`: Perform a spatial statistical analysis and calculate the strain energy contained in a sample of dislocations.
 * `export`: Export figures illustrating the previously generated data according to different representations.
 
 ## Installation
 
-You can find how to install the package in the [installation section](https://x-rays.gitlab.io/numlpa/installation.html) of the documentation.
+You can find how to install the package in the [installation section](https://x-rays.gitlab.io/numlpa/practice/installation/index.html) of the documentation.
 
 ## Usage
 
-You can find how to use the package in the [examples section](https://x-rays.gitlab.io/numlpa/examples.html) of the documentation.
+You can find how to use the package in the [examples section](https://x-rays.gitlab.io/numlpa/practice/examples/index.html) of the documentation.
 
 ## Credits
 
 * Dunstan Becht
 * Asdin Aoufi
 * András Borbély
```

### Comparing `numlpa-1.0.0b4/docs/Makefile` & `numlpa-1.0.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/conf.py` & `numlpa-1.0.0b5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/figures/distributions/dipoles/0.svg` & `numlpa-1.0.0b5/docs/source/figures/distributions/dipoles/0.svg`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/figures/distributions/images/0.svg` & `numlpa-1.0.0b5/docs/source/figures/distributions/images/0.svg`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/figures/distributions/wilkens/0.svg` & `numlpa-1.0.0b5/docs/source/figures/distributions/wilkens/0.svg`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/figures/restrictions/affine.svg` & `numlpa-1.0.0b5/docs/source/figures/restrictions/affine.svg`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/figures/restrictions/generate.py` & `numlpa-1.0.0b5/docs/source/figures/restrictions/generate.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/figures/restrictions/none.svg` & `numlpa-1.0.0b5/docs/source/figures/restrictions/none.svg`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/figures/restrictions/positive.svg` & `numlpa-1.0.0b5/docs/source/figures/restrictions/positive.svg`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/index.rst` & `numlpa-1.0.0b5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/logo.svg` & `numlpa-1.0.0b5/docs/source/logo.svg`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/practice/examples/configuration.rst` & `numlpa-1.0.0b5/docs/source/practice/examples/configuration.rst`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/practice/examples/vanilla.rst` & `numlpa-1.0.0b5/docs/source/practice/examples/vanilla.rst`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 Go to a blank working directory and run the following commands in a terminal:
 
 .. code-block:: bash
 
    # generate dislocation samples
    numlpa draw samples.tar
 
+   # evaluate strain energy
+   numlpa evaluate samples.tar evaluations.tar
+
+   # merge energy evaluations
+   numlpa merge evaluations.tar evaluation.tar
+
    # compute Fourier transforms
    numlpa diffract samples.tar transforms.tar
 
    # merge Fourier transforms
    numlpa merge transforms.tar transform.tar
 
    # fit a model
```

### Comparing `numlpa-1.0.0b4/docs/source/practice/formats/dislocation-sample.rst` & `numlpa-1.0.0b5/docs/source/practice/formats/dislocation-sample.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Dislocation sample data format
 ==============================
 
 A dislocation sample is an outcome of a random draw from a probability distribution in a given region of space.
-The data related to a dislocation sample is contained in a dictionnary whose structure is given below.
+The data related to a dislocation sample is contained in a dictionary whose structure is given below.
 
 .. code-block:: python
 
    {
        'metadata': {
            'type': 'dislocation-sample',
            'date': 'YYYY-MM-DDTHH:MM:SS+00:00',
```

### Comparing `numlpa-1.0.0b4/docs/source/practice/formats/fourier-transform.rst` & `numlpa-1.0.0b5/docs/source/practice/formats/fourier-transform.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Fourier transform data format
 =============================
 
 A Fourier transform is the result of the Fourier analysis after diffraction.
-The data related to a Fourier transform is contained in a dictionnary whose structure is given below.
+The data related to a Fourier transform is contained in a dictionary whose structure is given below.
 
 .. code-block:: python
 
    {
        'metadata': {
            'type': 'fourier-transform',
            'date': 'YYYY-MM-DDTHH:MM:SS+00:00',
```

### Comparing `numlpa-1.0.0b4/docs/source/practice/formats/index.rst` & `numlpa-1.0.0b5/docs/source/practice/formats/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,9 @@
    :maxdepth: 2
    :caption: Contents:
    :glob:
 
    dislocation-sample
    fourier-transform
    model-adjustment
+   energy-evaluation
    spatial-analysis
```

### Comparing `numlpa-1.0.0b4/docs/source/practice/formats/model-adjustment.rst` & `numlpa-1.0.0b5/docs/source/practice/formats/model-adjustment.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Model adjustment data format
 ============================
 
 A model adjustment is the result of an optimization process aimed at determining the value of the model parameters that minimizes the deviation of its prediction from the true diffraction profile.
-The data related to a model adjustment is contained in a dictionnary whose structure is given below.
+The data related to a model adjustment is contained in a dictionary whose structure is given below.
 
 .. code-block:: python
 
    {
        'metadata': {
            'type': 'model-adjustment',
            'date': 'YYYY-MM-DDTHH:MM:SS+00:00',
```

### Comparing `numlpa-1.0.0b4/docs/source/practice/formats/spatial-analysis.rst` & `numlpa-1.0.0b5/docs/source/practice/formats/spatial-analysis.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Spatial analysis data format
 =============================
 
 A spatial analysis is the result of a calculation carried out on each pair of dislocations to determine the interaction term and the distribution of dislocations around a dislocation.
-The data related to a spatial analysis is contained in a dictionnary whose structure is given below.
+The data related to a spatial analysis is contained in a dictionary whose structure is given below.
 
 .. code-block:: python
 
    {
        'metadata': {
            'type': 'spatial-analysis',
            'date': 'YYYY-MM-DDTHH:MM:SS+00:00',
```

### Comparing `numlpa-1.0.0b4/docs/source/practice/installation/editable.rst` & `numlpa-1.0.0b5/docs/source/practice/installation/editable.rst`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/practice/installation/regular.rst` & `numlpa-1.0.0b5/docs/source/practice/installation/regular.rst`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/docs/source/practice/installation/venv.rst` & `numlpa-1.0.0b5/docs/source/practice/installation/venv.rst`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/pyproject.toml` & `numlpa-1.0.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/setup.sh` & `numlpa-1.0.0b5/setup.sh`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/__main__.py` & `numlpa-1.0.0b5/src/numlpa/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,22 @@
 
 from argparse import ArgumentParser
 from logging import getLogger
 from sys import exit as sys_exit
 
 from numlpa import config
 from numlpa._version import version
-from numlpa.main import analyze, diffract, draw, export, extract, fit, merge
-
+from numlpa.main import analyze
+from numlpa.main import diffract
+from numlpa.main import draw
+from numlpa.main import evaluate
+from numlpa.main import export
+from numlpa.main import extract
+from numlpa.main import fit
+from numlpa.main import merge
 
 logger = getLogger(__name__)
 
 
 def main():
     """Run the command-line interpreter.
 
@@ -48,15 +54,24 @@
     )
 
     logger.debug("defining subparsers")
     subparsers = parser.add_subparsers(
         required=True,
         help="name of the command to run",
     )
-    for module in (draw, diffract, merge, fit, analyze, export, extract):
+    for module in (
+        draw,
+        diffract,
+        merge,
+        fit,
+        evaluate,
+        analyze,
+        export,
+        extract,
+    ):
         subparser = subparsers.add_parser(
             name=module.__name__.rsplit('.', maxsplit=1)[-1],
             help=f"run {module.__name__} module",
         )
         module.setup(subparser)
 
     logger.debug("parsing command-line arguments")
```

### Comparing `numlpa-1.0.0b4/src/numlpa/core/parallelism.py` & `numlpa-1.0.0b5/src/numlpa/core/parallelism.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/core/storage.py` & `numlpa-1.0.0b5/src/numlpa/core/storage.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/default.conf` & `numlpa-1.0.0b5/src/numlpa/default.conf`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,27 @@
 radius = 1000e-9
 
 [numlpa.kits.distributions.wilkens]
 nsub = 5
 pairs = 4
 side = 2000e-9
 
+[numlpa.kits.evaluators.cpu]
+type = screw
+b_uvw = [ 1, 1, 0]
+cell = 0.4046e-9
+poisson = 0.345
+shear = 26e9
+core = 2.6
+absolute = False
+replicate = 2
+points = 1000
+processes = 0
+check = False
+
 [numlpa.kits.optimizers.default]
 maxiter = 1000
 method = Nelder-Mead
 points = 100
 seed = 0
 processes = 0
 
@@ -79,16 +92,17 @@
 
 [numlpa.main.draw]
 size = 10
 seed = 0
 format = json
 distribution = dipoles
 
-[numlpa.main.energy]
+[numlpa.main.evaluate]
 format = json
+evaluator = cpu
 
 [numlpa.main.export]
 format = svg
 font = latinmodern-math.ttf
 math = cm
 size = 10
 dpi = 600
```

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/__init__.py` & `numlpa-1.0.0b5/src/numlpa/kits/__init__.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/analyzers/__init__.py` & `numlpa-1.0.0b5/src/numlpa/kits/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/analyzers/cpu/analysis.py` & `numlpa-1.0.0b5/src/numlpa/kits/analyzers/cpu/analysis.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/analyzers/cpu/interactionmodule.c` & `numlpa-1.0.0b5/src/numlpa/kits/analyzers/cpu/interactionmodule.c`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/analyzers/cpu/parser.py` & `numlpa-1.0.0b5/src/numlpa/kits/analyzers/cpu/parser.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/diffractometers/__init__.py` & `numlpa-1.0.0b5/src/numlpa/kits/diffractometers/__init__.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/diffractometers/cpu/diffraction.py` & `numlpa-1.0.0b5/src/numlpa/kits/diffractometers/cpu/diffraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     absolute : bool
         If true, the range parameter becomes an absolute value.
     poisson : float
         Poisson number.
     harmonics : list of int
         List of harmonics to be calculated.
     replicate : int
-        Number of replication of the region of interest.
+        Number of replications of the region of interest.
     points : int
         Number of random points.
     processes : int
         Number of parallel processes.
     check : bool
         Display random points and replicated dislocations.
```

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/diffractometers/cpu/displacementmodule.c` & `numlpa-1.0.0b5/src/numlpa/kits/diffractometers/cpu/displacementmodule.c`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/diffractometers/cpu/parser.py` & `numlpa-1.0.0b5/src/numlpa/kits/diffractometers/cpu/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         type=float,
         metavar='float',
     )
     parser.add_argument(
         '--absolute',
         action='store_true',
         help="if true, the range parameter becomes an absolute value",
-        default=False,
     )
     parser.add_argument(
         '--poisson',
         help="Poisson number",
         type=float,
         metavar='float',
     )
@@ -83,15 +82,15 @@
         help="list of harmonics to be calculated",
         type=int,
         nargs='+',
         metavar='int',
     )
     parser.add_argument(
         '--replicate',
-        help="number of replication of the region of interest",
+        help="number of replications of the region of interest",
         type=int,
         metavar='int',
     )
     parser.add_argument(
         '--points',
         help="number of random points",
         type=int,
```

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/distributions/dipoles.py` & `numlpa-1.0.0b5/src/numlpa/kits/distributions/dipoles.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/distributions/images.py` & `numlpa-1.0.0b5/src/numlpa/kits/distributions/images.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/distributions/wilkens.py` & `numlpa-1.0.0b5/src/numlpa/kits/distributions/wilkens.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/fonts/__init__.py` & `numlpa-1.0.0b5/src/numlpa/kits/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/fonts/latinmodern-math.ttf` & `numlpa-1.0.0b5/src/numlpa/kits/fonts/latinmodern-math.ttf`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/models/guw.py` & `numlpa-1.0.0b5/src/numlpa/kits/models/guw.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/models/kr.py` & `numlpa-1.0.0b5/src/numlpa/kits/models/kr.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/models/wilkens.py` & `numlpa-1.0.0b5/src/numlpa/kits/models/wilkens.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/optimizers/default.py` & `numlpa-1.0.0b5/src/numlpa/kits/optimizers/default.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/representations/affine.py` & `numlpa-1.0.0b5/src/numlpa/kits/representations/affine.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/representations/basic.py` & `numlpa-1.0.0b5/src/numlpa/kits/representations/basic.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/restrictions/affine.py` & `numlpa-1.0.0b5/src/numlpa/kits/restrictions/affine.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/restrictions/none.py` & `numlpa-1.0.0b5/src/numlpa/kits/restrictions/none.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/kits/restrictions/positive.py` & `numlpa-1.0.0b5/src/numlpa/kits/restrictions/positive.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/main/analyze.py` & `numlpa-1.0.0b5/src/numlpa/main/analyze.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/main/diffract.py` & `numlpa-1.0.0b5/src/numlpa/main/diffract.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/main/draw.py` & `numlpa-1.0.0b5/src/numlpa/main/draw.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/main/export.py` & `numlpa-1.0.0b5/src/numlpa/main/export.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/main/extract.py` & `numlpa-1.0.0b5/src/numlpa/main/extract.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/main/fit.py` & `numlpa-1.0.0b5/src/numlpa/main/fit.py`

 * *Files identical despite different names*

### Comparing `numlpa-1.0.0b4/src/numlpa/main/merge.py` & `numlpa-1.0.0b5/src/numlpa/main/merge.py`

 * *Files 19% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     logger.debug("checking files")
     try:
         data['type'] = data['input'][0]['metadata']['type']
     except (KeyError, TypeError) as exc:
         raise RuntimeError("can not parse data from container") from exc
     if data['type'] == 'fourier-transform':
         process_transforms(containers, files, data)
+    elif data['type'] == 'energy-evaluation':
+        process_evaluations(containers, files, data)
     elif data['type'] == 'spatial-analysis':
         raise NotImplementedError()
     else:
         raise TypeError(f"can not merge data of type {data['type']}")
 
 
 def process_transforms(containers, files, data):
@@ -160,7 +162,56 @@
         'date': datetime.now(timezone.utc).isoformat(timespec="seconds"),
         'version': version_tuple,
     }
 
     logger.debug("saving %s", files['output'])
     series['output'] = serialize(data['output'], files['output'])
     containers['output'].add(series['output'], files['output'])
+
+
+def process_evaluations(containers, files, data):
+    """Merge the energy evaluations.
+
+    Parameters
+    ----------
+    containers : dict of Container
+        Input and output containers.
+    files : dict of list
+        Input and output files names.
+    data : dict
+        Input and output files data.
+
+    """
+    series = {}
+
+    logger.debug("gathering evaluations")
+    data['output'] = dict(data['input'][0])
+    data['energies'] = []
+    for i in range(len(data['input'])):
+        if data['input'][i]['metadata']['type'] != 'energy-evaluation':
+            raise TypeError(f"{files['input'][i]} is not an energy eval")
+        data['energies'].append(data['input'][i]['evaluation']['energy_mean'])
+
+    logger.debug("conputing mean and deviation")
+    data['energy_mean'] = np.average(data['energies'])
+    data['coefficient'] = 1/np.sqrt(len(files['input']))
+    data['energy_deviation'] = np.std(data['energies']) * data['coefficient']
+
+    logger.info("generating %s", files['target'])
+    data['output']['evaluation']['samples'] = len(files['input'])
+    data['output']['evaluation']['energy_mean'] = data['energy_mean']
+    data['output']['evaluation']['energy_deviation'] = data['energy_deviation']
+    data['output']['evaluation']['cutoff'] = (
+        data['output']['evaluation']['core'] * np.exp(
+            data['output']['evaluation']['factor'] *
+            data['output']['evaluation']['energy_mean']
+        )
+    )
+    data['output']['metadata'] = {
+        'type': 'energy-evaluation',
+        'date': datetime.now(timezone.utc).isoformat(timespec="seconds"),
+        'version': version_tuple,
+    }
+
+    logger.debug("saving %s", files['output'])
+    series['output'] = serialize(data['output'], files['output'])
+    containers['output'].add(series['output'], files['output'])
```

### Comparing `numlpa-1.0.0b4/src/numlpa.egg-info/PKG-INFO` & `numlpa-1.0.0b5/src/numlpa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numlpa
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: Numerical Line Profile Analysis package.
 Author-email: Dunstan Becht <dunstan.becht@orange.fr>
 Project-URL: Homepage, https://gitlab.com/x-rays/numlpa
 Project-URL: Bug Tracker, https://gitlab.com/x-rays/numlpa/issues
 Project-URL: Documentation, https://x-rays.gitlab.io/numlpa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -35,26 +35,27 @@
 ## Features
 
 NumLPA Has been developed to meet the need to analyze the accuracy of LPA models.
 The main features of the package are presented bellow:
 
 * `draw`: Generate samples of dislocations by random drawing from different probability distribution models.
 * `diffract`: Simulate X-ray diffraction on crystals containing the previously generated dislocations and compute the Fourier transform of the diffracted intensity.
-* `merge`: Average the Fourier transform coefficients from multiples samples drawn from a same distribution.
+* `merge`: Average the Fourier transform coefficients or the strain energy evaluations from multiple samples drawn from a same distribution.
 * `fit`: Fit LPA models on the simulated diffraction profiles to obtain their predictions and compare them to the real parameters of the distribution.
+* `evaluate`: Compute the strain energy density and the outer cut-off radius for a sample of dislocations.
 * `analyze`: Perform a spatial statistical analysis and calculate the strain energy contained in a sample of dislocations.
 * `export`: Export figures illustrating the previously generated data according to different representations.
 
 ## Installation
 
-You can find how to install the package in the [installation section](https://x-rays.gitlab.io/numlpa/installation.html) of the documentation.
+You can find how to install the package in the [installation section](https://x-rays.gitlab.io/numlpa/practice/installation/index.html) of the documentation.
 
 ## Usage
 
-You can find how to use the package in the [examples section](https://x-rays.gitlab.io/numlpa/examples.html) of the documentation.
+You can find how to use the package in the [examples section](https://x-rays.gitlab.io/numlpa/practice/examples/index.html) of the documentation.
 
 ## Credits
 
 * Dunstan Becht
 * Asdin Aoufi
 * András Borbély
```

### Comparing `numlpa-1.0.0b4/src/numlpa.egg-info/SOURCES.txt` & `numlpa-1.0.0b5/src/numlpa.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/source/figures/restrictions/none.svg
 docs/source/figures/restrictions/positive.svg
 docs/source/practice/index.rst
 docs/source/practice/examples/configuration.rst
 docs/source/practice/examples/index.rst
 docs/source/practice/examples/vanilla.rst
 docs/source/practice/formats/dislocation-sample.rst
+docs/source/practice/formats/energy-evaluation.rst
 docs/source/practice/formats/fourier-transform.rst
 docs/source/practice/formats/index.rst
 docs/source/practice/formats/model-adjustment.rst
 docs/source/practice/formats/spatial-analysis.rst
 docs/source/practice/installation/editable.rst
 docs/source/practice/installation/index.rst
 docs/source/practice/installation/regular.rst
@@ -55,14 +56,19 @@
 src/numlpa/kits/diffractometers/cpu/diffraction.py
 src/numlpa/kits/diffractometers/cpu/displacementmodule.c
 src/numlpa/kits/diffractometers/cpu/parser.py
 src/numlpa/kits/distributions/__init__.py
 src/numlpa/kits/distributions/dipoles.py
 src/numlpa/kits/distributions/images.py
 src/numlpa/kits/distributions/wilkens.py
+src/numlpa/kits/evaluators/__init__.py
+src/numlpa/kits/evaluators/cpu/__init__.py
+src/numlpa/kits/evaluators/cpu/energymodule.c
+src/numlpa/kits/evaluators/cpu/evaluation.py
+src/numlpa/kits/evaluators/cpu/parser.py
 src/numlpa/kits/fonts/__init__.py
 src/numlpa/kits/fonts/latinmodern-math.ttf
 src/numlpa/kits/models/__init__.py
 src/numlpa/kits/models/guw.py
 src/numlpa/kits/models/kr.py
 src/numlpa/kits/models/wilkens.py
 src/numlpa/kits/optimizers/__init__.py
@@ -74,14 +80,15 @@
 src/numlpa/kits/restrictions/affine.py
 src/numlpa/kits/restrictions/none.py
 src/numlpa/kits/restrictions/positive.py
 src/numlpa/main/__init__.py
 src/numlpa/main/analyze.py
 src/numlpa/main/diffract.py
 src/numlpa/main/draw.py
+src/numlpa/main/evaluate.py
 src/numlpa/main/export.py
 src/numlpa/main/extract.py
 src/numlpa/main/fit.py
 src/numlpa/main/merge.py
 tests/references.json
 tests/run.py
 tests/material/.gitignore
```

### Comparing `numlpa-1.0.0b4/tests/references.json` & `numlpa-1.0.0b5/tests/references.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'evaluators'": "OrderedDict([('cpu', OrderedDict([('parameters-screw', OrderedDict([('sample', "*

 * *                 "OrderedDict([('distribution', OrderedDict([('module', "*

 * *                 "'numlpa.kits.distributions.wilkens'), ('seed', 0), ('density', 8.0), ('nsub', "*

 * *                 "2), ('pairs', 1), ('side', 1)])), ('region', OrderedDict([('type', 'square'), "*

 * *                 "('side', 1)])), ('dislocations', OrderedDict([('senses', [-1, 1, -1, 1, -1, 1, "*

 * *                 "-1, 1]), ('positions', [[0 […]*

```diff
@@ -502,14 +502,190 @@
                     1,
                     -1,
                     1
                 ]
             }
         }
     },
+    "evaluators": {
+        "cpu": {
+            "parameters-edge": {
+                "absolute": true,
+                "b_uvw": [
+                    1,
+                    1,
+                    0
+                ],
+                "cell": 10,
+                "core": 0.1,
+                "points": 10,
+                "poisson": 0.345,
+                "processes": 0,
+                "replicate": 3,
+                "sample": {
+                    "dislocations": {
+                        "positions": [
+                            [
+                                0.42221092576252406,
+                                0.2102857904154225,
+                                0.25563736068430426,
+                                0.3918992945173863,
+                                0.7382984770761779,
+                                0.9540564425976676,
+                                0.6409189221998519,
+                                0.8091844983376658
+                            ],
+                            [
+                                0.37897720147015124,
+                                0.12945837514648167,
+                                0.7024670687252071,
+                                0.6516563630394637,
+                                0.2916910197275156,
+                                0.25234342790869513,
+                                0.877902102078612,
+                                0.6252531706812203
+                            ]
+                        ],
+                        "senses": [
+                            -1,
+                            1,
+                            -1,
+                            1,
+                            -1,
+                            1,
+                            -1,
+                            1
+                        ]
+                    },
+                    "distribution": {
+                        "density": 8.0,
+                        "module": "numlpa.kits.distributions.wilkens",
+                        "nsub": 2,
+                        "pairs": 1,
+                        "seed": 0,
+                        "side": 1
+                    },
+                    "region": {
+                        "side": 1,
+                        "type": "square"
+                    }
+                },
+                "shear": 9.9,
+                "type": "edge"
+            },
+            "parameters-screw": {
+                "absolute": true,
+                "b_uvw": [
+                    1,
+                    1,
+                    0
+                ],
+                "cell": 10,
+                "core": 0.1,
+                "points": 10,
+                "poisson": 0.345,
+                "processes": 0,
+                "replicate": 3,
+                "sample": {
+                    "dislocations": {
+                        "positions": [
+                            [
+                                0.42221092576252406,
+                                0.2102857904154225,
+                                0.25563736068430426,
+                                0.3918992945173863,
+                                0.7382984770761779,
+                                0.9540564425976676,
+                                0.6409189221998519,
+                                0.8091844983376658
+                            ],
+                            [
+                                0.37897720147015124,
+                                0.12945837514648167,
+                                0.7024670687252071,
+                                0.6516563630394637,
+                                0.2916910197275156,
+                                0.25234342790869513,
+                                0.877902102078612,
+                                0.6252531706812203
+                            ]
+                        ],
+                        "senses": [
+                            -1,
+                            1,
+                            -1,
+                            1,
+                            -1,
+                            1,
+                            -1,
+                            1
+                        ]
+                    },
+                    "distribution": {
+                        "density": 8.0,
+                        "module": "numlpa.kits.distributions.wilkens",
+                        "nsub": 2,
+                        "pairs": 1,
+                        "seed": 0,
+                        "side": 1
+                    },
+                    "region": {
+                        "side": 1,
+                        "type": "square"
+                    }
+                },
+                "shear": 9.9,
+                "type": "screw"
+            },
+            "returns-edge": {
+                "b_len": 7.0710678,
+                "b_uvw": [
+                    1,
+                    1,
+                    0
+                ],
+                "cell": 10,
+                "core": 0.1,
+                "cutoff": 0.36633606,
+                "energy_deviation": 406.06265,
+                "energy_mean": 624.66352,
+                "factor": 0.0020785285,
+                "hidden": 1,
+                "module": "numlpa.kits.evaluators.cpu",
+                "points": 10,
+                "poisson": 0.345,
+                "replicate": 3,
+                "samples": 1,
+                "shear": 9.9,
+                "type": "edge"
+            },
+            "returns-screw": {
+                "b_len": 7.0710678,
+                "b_uvw": [
+                    1,
+                    1,
+                    0
+                ],
+                "cell": 10,
+                "core": 0.1,
+                "cutoff": 0.27328747,
+                "energy_deviation": 132.00463,
+                "energy_mean": 316.81399,
+                "factor": 0.0031733259,
+                "hidden": 1,
+                "module": "numlpa.kits.evaluators.cpu",
+                "points": 10,
+                "poisson": 0.345,
+                "replicate": 3,
+                "samples": 1,
+                "shear": 9.9,
+                "type": "screw"
+            }
+        }
+    },
     "models": {
         "guw": {
             "parameters": {
                 "harmonic": 1,
                 "parameters": [
                     50000000000000.0,
                     1e-07,
```

### Comparing `numlpa-1.0.0b4/tests/run.py` & `numlpa-1.0.0b5/tests/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -163,14 +163,33 @@
             model = kits.get('models', name)
             dat = model.model(transform, harmonic)(*parameters)
             self.assertEqual(
                 ref['models'][name]['returns'],
                 rounded(list(dat)),
             )
 
+    def test_evaluators(self):
+        """Test strain energy evaluators."""
+        self.__dict__['maxDiff'] = None
+        tested = kits.names('evaluators')
+        for name in tested:
+            for kind in ('screw', 'edge',):
+                with self.subTest(name=name, kind=kind):
+                    params_key = f'parameters-{kind}'
+                    return_key = f'returns-{kind}'
+                    evaluator = kits.get('evaluators', name)
+                    parameters = ref['evaluators'][name][params_key]
+                    dat = evaluator.evaluate(**parameters)
+                    dat['evaluation'].pop('duration')
+                    dat['evaluation'].pop('processes')
+                    self.assertEqual(
+                        ref['evaluators'][name][return_key],
+                        rounded(dat['evaluation']),
+                    )
+
 
 class TestCommandLineInterface(TestCase):
     """Class for testing the command-line interface."""
 
     def test_draw(self):
         """Test draw command."""
         for distribution in kits.names('distributions'):
```

