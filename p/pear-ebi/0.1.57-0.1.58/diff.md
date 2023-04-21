# Comparing `tmp/pear_ebi-0.1.57.tar.gz` & `tmp/pear_ebi-0.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pear_ebi-0.1.57.tar", last modified: Wed Apr 19 09:54:21 2023, max compression
+gzip compressed data, was "pear_ebi-0.1.58.tar", last modified: Fri Apr 21 09:56:10 2023, max compression
```

## Comparing `pear_ebi-0.1.57.tar` & `pear_ebi-0.1.58.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1120 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/LICENSE.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)       93 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/MANIFEST.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5309 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/PKG-INFO
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5052 2023-03-22 14:38:42.000000 pear_ebi-0.1.57/README.md
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.497666 pear_ebi-0.1.57/pear_ebi/
--rw-r--r--   0 andrear   (1000) andrear   (1000)      349 2023-04-19 09:51:28.000000 pear_ebi-0.1.57/pear_ebi/__init__.py
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)    18447 2023-04-05 18:11:56.000000 pear_ebi-0.1.57/pear_ebi/__main__.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.497666 pear_ebi-0.1.57/pear_ebi/calculate_distances/
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/
--rw-r--r--   0 andrear   (1000) andrear   (1000)       36 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/AUTHORS
--rw-r--r--   0 andrear   (1000) andrear   (1000)    18337 2023-02-20 10:02:47.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/ChangeLog
--rw-r--r--   0 andrear   (1000) andrear   (1000)     9732 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/INSTALL
--rw-r--r--   0 andrear   (1000) andrear   (1000)    20283 2023-02-20 10:02:47.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)      490 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Makefile.am
--rw-r--r--   0 andrear   (1000) andrear   (1000)    20957 2023-02-20 10:02:47.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Makefile.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/NEWS
--rw-r--r--   0 andrear   (1000) andrear   (1000)      157 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/README
--rw-r--r--   0 andrear   (1000) andrear   (1000)    50999 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Random.cpp
--rw-r--r--   0 andrear   (1000) andrear   (1000)  3230664 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Random.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)    33526 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/aclocal.m4
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2366 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.h
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2148 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.h.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2271 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2073 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.hh.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)    16107 2023-02-20 10:02:47.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.log
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)    31318 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.status
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)   188210 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/configure
--rw-r--r--   0 andrear   (1000) andrear   (1000)      485 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/configure.ac
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)   186547 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/configure.lineno
--rw-r--r--   0 andrear   (1000) andrear   (1000)    16466 2023-02-14 10:37:26.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/depcomp
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2243 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hash.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1915 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hash.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   595768 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hash.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2968 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashfunc.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2166 2023-02-20 10:02:48.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashfunc.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   331744 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashfunc.o
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)  4547960 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashrf
--rw-r--r--   0 andrear   (1000) andrear   (1000)    28716 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashrf.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)  6651416 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashrf.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)     9556 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/install-sh
--rw-r--r--   0 andrear   (1000) andrear   (1000)      795 2023-02-20 10:02:47.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/label-map.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1026 2023-02-20 10:02:47.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/label-map.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   540936 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/label-map.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)    11374 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/missing
--rw-r--r--   0 andrear   (1000) andrear   (1000)    12315 2023-02-20 10:02:47.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/newick.c
--rw-r--r--   0 andrear   (1000) andrear   (1000)      723 2023-02-20 10:02:47.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/newick.h
--rw-r--r--   0 andrear   (1000) andrear   (1000)    38568 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/newick.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)       24 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/stamp-h1
--rw-r--r--   0 andrear   (1000) andrear   (1000)      660 2023-02-22 10:35:23.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/RF_pypy.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4810 2023-04-03 16:09:45.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/hashrf.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    24634 2023-04-03 16:09:45.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/maple_RF.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._CMakeFiles
--rw-r--r--   0 andrear   (1000) andrear   (1000)      269 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._CMakeLists.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._COPYING.LESSER
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._CPackConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._CPackSourceConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._CTestTestfile.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._README
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._bin
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._cmake_install.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._icon.ico
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._icon.jpg
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._tqDist
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/._trees
--rw-r--r--   0 andrear   (1000) andrear   (1000)    15581 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CMakeCache.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2436 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CMakeLists.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)    35820 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)     7815 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/COPYING.LESSER
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4094 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4880 2023-02-14 10:37:27.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      275 2023-02-20 10:02:48.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CTestTestfile.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)    12995 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3071 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/README
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1828 2023-02-14 10:37:28.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/cmake_install.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)    32038 2023-02-14 10:37:28.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/icon.ico
--rw-r--r--   0 andrear   (1000) andrear   (1000)     7953 2023-02-14 10:37:28.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/icon.jpg
--rw-r--r--   0 andrear   (1000) andrear   (1000)      205 2023-02-20 10:02:50.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/install_manifest.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5429 2023-04-03 16:09:45.000000 pear_ebi-0.1.57/pear_ebi/calculate_distances/tqdist.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/pear_ebi/embeddings/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1790 2023-04-05 18:11:55.000000 pear_ebi-0.1.57/pear_ebi/embeddings/Isomap_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1838 2023-04-05 18:11:55.000000 pear_ebi-0.1.57/pear_ebi/embeddings/LLE_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1936 2023-04-05 18:11:55.000000 pear_ebi-0.1.57/pear_ebi/embeddings/PCA_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.57/pear_ebi/embeddings/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1473 2023-03-22 16:31:08.000000 pear_ebi-0.1.57/pear_ebi/embeddings/emb_quality.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/pear_ebi/embeddings/graph/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.57/pear_ebi/embeddings/graph/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    37131 2023-03-20 22:03:04.000000 pear_ebi-0.1.57/pear_ebi/embeddings/graph/graph.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2208 2023-04-05 18:11:55.000000 pear_ebi-0.1.57/pear_ebi/embeddings/tSNE_e.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/pear_ebi/interactive_mode/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.57/pear_ebi/interactive_mode/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5859 2023-02-22 10:35:24.000000 pear_ebi-0.1.57/pear_ebi/interactive_mode/interactive.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/pear_ebi/subsample/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.57/pear_ebi/subsample/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3855 2023-02-20 16:46:41.000000 pear_ebi-0.1.57/pear_ebi/subsample/subsample.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5050 2023-02-20 16:46:42.000000 pear_ebi-0.1.57/pear_ebi/subsample/subsample_multiprocess.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3681 2023-04-19 09:41:07.000000 pear_ebi-0.1.57/pear_ebi/tree_emb_parser.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    33226 2023-04-05 18:20:31.000000 pear_ebi-0.1.57/pear_ebi/tree_set.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.497666 pear_ebi-0.1.57/pear_ebi.egg-info/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5309 2023-04-19 09:54:21.000000 pear_ebi-0.1.57/pear_ebi.egg-info/PKG-INFO
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4297 2023-04-19 09:54:21.000000 pear_ebi-0.1.57/pear_ebi.egg-info/SOURCES.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)        1 2023-04-19 09:54:21.000000 pear_ebi-0.1.57/pear_ebi.egg-info/dependency_links.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)       52 2023-04-19 09:54:21.000000 pear_ebi-0.1.57/pear_ebi.egg-info/entry_points.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pear_ebi.egg-info/not-zip-safe
--rw-r--r--   0 andrear   (1000) andrear   (1000)       94 2023-04-19 09:54:21.000000 pear_ebi-0.1.57/pear_ebi.egg-info/requires.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)        9 2023-04-19 09:54:21.000000 pear_ebi-0.1.57/pear_ebi.egg-info/top_level.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)      228 2023-02-20 16:30:29.000000 pear_ebi-0.1.57/pyproject.toml
--rw-r--r--   0 andrear   (1000) andrear   (1000)      107 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/setup.cfg
--rw-r--r--   0 andrear   (1000) andrear   (1000)      946 2023-04-19 09:51:26.000000 pear_ebi-0.1.57/setup.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-19 09:54:21.547663 pear_ebi-0.1.57/test/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1191 2023-04-03 16:09:45.000000 pear_ebi-0.1.57/test/test.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:10.238526 pear_ebi-0.1.58/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1120 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/LICENSE.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       93 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/MANIFEST.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5309 2023-04-21 09:56:10.238526 pear_ebi-0.1.58/PKG-INFO
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5052 2023-03-22 14:38:42.000000 pear_ebi-0.1.58/README.md
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:09.928526 pear_ebi-0.1.58/pear_ebi/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      349 2023-04-21 09:55:58.000000 pear_ebi-0.1.58/pear_ebi/__init__.py
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)    18447 2023-04-05 18:11:56.000000 pear_ebi-0.1.58/pear_ebi/__main__.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:09.928526 pear_ebi-0.1.58/pear_ebi/calculate_distances/
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:10.218526 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       36 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/AUTHORS
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    18337 2023-02-20 10:02:47.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/ChangeLog
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     9732 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/INSTALL
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    20283 2023-02-20 10:02:47.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      490 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Makefile.am
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    20957 2023-02-20 10:02:47.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Makefile.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/NEWS
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      157 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/README
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    50999 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Random.cpp
+-rw-r--r--   0 andrear   (1000) andrear   (1000)  3230664 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Random.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    33526 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/aclocal.m4
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2366 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.h
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2148 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.h.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2271 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2073 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.hh.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    16107 2023-02-20 10:02:47.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.log
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)    31318 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.status
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)   188210 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/configure
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      485 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/configure.ac
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)   186547 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/configure.lineno
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    16466 2023-02-14 10:37:26.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/depcomp
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2243 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hash.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1915 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hash.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   595768 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hash.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2968 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashfunc.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2166 2023-02-20 10:02:48.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashfunc.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   331744 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashfunc.o
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)  4547960 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashrf
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    28716 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashrf.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)  6651416 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashrf.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     9556 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/install-sh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      795 2023-02-20 10:02:47.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/label-map.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1026 2023-02-20 10:02:47.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/label-map.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   540936 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/label-map.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    11374 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/missing
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    12315 2023-02-20 10:02:47.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/newick.c
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      723 2023-02-20 10:02:47.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/newick.h
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    38568 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/newick.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       24 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/stamp-h1
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      660 2023-02-22 10:35:23.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/RF_pypy.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4810 2023-04-03 16:09:45.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/hashrf.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    24634 2023-04-03 16:09:45.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/maple_RF.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:10.228526 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._CMakeFiles
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      269 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._CMakeLists.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._COPYING.LESSER
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._CPackConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._CPackSourceConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._CTestTestfile.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._README
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._bin
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._cmake_install.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._icon.ico
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._icon.jpg
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._tqDist
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/._trees
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    15581 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CMakeCache.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2436 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CMakeLists.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    35820 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     7815 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/COPYING.LESSER
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4094 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4880 2023-02-14 10:37:27.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      275 2023-02-20 10:02:48.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CTestTestfile.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    12995 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3071 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/README
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1828 2023-02-14 10:37:28.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/cmake_install.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    32038 2023-02-14 10:37:28.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/icon.ico
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     7953 2023-02-14 10:37:28.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/icon.jpg
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      205 2023-02-20 10:02:50.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/install_manifest.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5429 2023-04-03 16:09:45.000000 pear_ebi-0.1.58/pear_ebi/calculate_distances/tqdist.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:10.228526 pear_ebi-0.1.58/pear_ebi/embeddings/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1790 2023-04-05 18:11:55.000000 pear_ebi-0.1.58/pear_ebi/embeddings/Isomap_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1838 2023-04-05 18:11:55.000000 pear_ebi-0.1.58/pear_ebi/embeddings/LLE_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1936 2023-04-05 18:11:55.000000 pear_ebi-0.1.58/pear_ebi/embeddings/PCA_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.58/pear_ebi/embeddings/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1473 2023-03-22 16:31:08.000000 pear_ebi-0.1.58/pear_ebi/embeddings/emb_quality.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:10.238526 pear_ebi-0.1.58/pear_ebi/embeddings/graph/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.58/pear_ebi/embeddings/graph/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    38664 2023-04-21 09:50:56.000000 pear_ebi-0.1.58/pear_ebi/embeddings/graph/graph.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2208 2023-04-05 18:11:55.000000 pear_ebi-0.1.58/pear_ebi/embeddings/tSNE_e.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:10.238526 pear_ebi-0.1.58/pear_ebi/interactive_mode/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.58/pear_ebi/interactive_mode/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5859 2023-02-22 10:35:24.000000 pear_ebi-0.1.58/pear_ebi/interactive_mode/interactive.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:10.238526 pear_ebi-0.1.58/pear_ebi/subsample/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.58/pear_ebi/subsample/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3855 2023-02-20 16:46:41.000000 pear_ebi-0.1.58/pear_ebi/subsample/subsample.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5050 2023-02-20 16:46:42.000000 pear_ebi-0.1.58/pear_ebi/subsample/subsample_multiprocess.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3681 2023-04-19 10:09:29.000000 pear_ebi-0.1.58/pear_ebi/tree_emb_parser.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    33266 2023-04-20 15:17:02.000000 pear_ebi-0.1.58/pear_ebi/tree_set.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:09.928526 pear_ebi-0.1.58/pear_ebi.egg-info/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5309 2023-04-21 09:56:09.000000 pear_ebi-0.1.58/pear_ebi.egg-info/PKG-INFO
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4297 2023-04-21 09:56:09.000000 pear_ebi-0.1.58/pear_ebi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        1 2023-04-21 09:56:09.000000 pear_ebi-0.1.58/pear_ebi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       52 2023-04-21 09:56:09.000000 pear_ebi-0.1.58/pear_ebi.egg-info/entry_points.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pear_ebi.egg-info/not-zip-safe
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       94 2023-04-21 09:56:09.000000 pear_ebi-0.1.58/pear_ebi.egg-info/requires.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        9 2023-04-21 09:56:09.000000 pear_ebi-0.1.58/pear_ebi.egg-info/top_level.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      228 2023-02-20 16:30:29.000000 pear_ebi-0.1.58/pyproject.toml
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      107 2023-04-21 09:56:10.238526 pear_ebi-0.1.58/setup.cfg
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      946 2023-04-21 09:56:02.000000 pear_ebi-0.1.58/setup.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-04-21 09:56:10.238526 pear_ebi-0.1.58/test/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1191 2023-04-03 16:09:45.000000 pear_ebi-0.1.58/test/test.py
```

### Comparing `pear_ebi-0.1.57/LICENSE.txt` & `pear_ebi-0.1.58/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/PKG-INFO` & `pear_ebi-0.1.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pear_ebi
-Version: 0.1.57
+Version: 0.1.58
 Summary: Embeds phylogenetic tree distances and produce representations
 Home-page: https://github.com/AndreaRubbi/TreeEmbedding
 Author: Andrea Rubbi
 Author-email: andrea.rubbi.98@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pear_ebi Version: 0.1.57 Summary: Embeds
+Metadata-Version: 2.1 Name: pear_ebi Version: 0.1.58 Summary: Embeds
 phylogenetic tree distances and produce representations Home-page: https://
 github.com/AndreaRubbi/TreeEmbedding Author: Andrea Rubbi Author-email:
 andrea.rubbi.98@gmail.com License: MIT License Description-Content-Type: text/
 markdown License-File: LICENSE.txt
 ****** Phylogeny Embedding &
 Approximate Representation ******
 [logos/LOGO_PEAR.png] ## Goldman Group - European Bioinformatics Institute
```

### Comparing `pear_ebi-0.1.57/README.md` & `pear_ebi-0.1.58/README.md`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/__main__.py` & `pear_ebi-0.1.58/pear_ebi/__main__.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/COPYING` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/COPYING`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/INSTALL` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/INSTALL`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Makefile` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Makefile`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Makefile.in` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Makefile.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Random.cpp` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Random.cpp`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/Random.o` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/Random.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/aclocal.m4` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/aclocal.m4`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.h` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.h`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.h.in` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.h.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.hh` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.hh.in` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.hh.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.log` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.log`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/config.status` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/config.status`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/configure` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/configure`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/configure.lineno` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/configure.lineno`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/depcomp` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/depcomp`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hash.cc` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hash.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hash.hh` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hash.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hash.o` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hash.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashfunc.cc` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashfunc.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashfunc.hh` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashfunc.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashfunc.o` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashfunc.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashrf` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashrf`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashrf.cc` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashrf.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/hashrf.o` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/hashrf.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/install-sh` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/install-sh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/label-map.cc` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/label-map.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/label-map.hh` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/label-map.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/label-map.o` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/label-map.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/missing` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/missing`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/newick.c` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/newick.c`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/newick.h` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/newick.h`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/HashRF/newick.o` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/HashRF/newick.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/RF_pypy.py` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/RF_pypy.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/hashrf.py` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/hashrf.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/maple_RF.py` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/maple_RF.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CMakeCache.txt` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CMakeLists.txt` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/COPYING` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/COPYING`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/COPYING.LESSER` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/Makefile` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/Makefile`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/README` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/README`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/cmake_install.cmake` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/icon.ico` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/icon.ico`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqDist/icon.jpg` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqDist/icon.jpg`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/calculate_distances/tqdist.py` & `pear_ebi-0.1.58/pear_ebi/calculate_distances/tqdist.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/embeddings/Isomap_e.py` & `pear_ebi-0.1.58/pear_ebi/embeddings/Isomap_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/embeddings/LLE_e.py` & `pear_ebi-0.1.58/pear_ebi/embeddings/LLE_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/embeddings/PCA_e.py` & `pear_ebi-0.1.58/pear_ebi/embeddings/PCA_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/embeddings/emb_quality.py` & `pear_ebi-0.1.58/pear_ebi/embeddings/emb_quality.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/embeddings/graph/graph.py` & `pear_ebi-0.1.58/pear_ebi/embeddings/graph/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from ipywidgets import widgets
 from pylab import cm
 
+random.seed(123)
+np.random.seed(123)
+
 
 def plot_embedding(
     data,
     metadata,
     dimensions,
     save=False,
     name_plot="Tree_embedding",
@@ -250,35 +253,44 @@
             "viridis",
             "ylgn",
             "ylgnbu",
             "ylorbr",
             "ylorrd",
         ]
 
-        # single colors for interpretability
+        # single colors (colorscales) for interpretability
         colorscales_GO = [
             "blues",
             "darkmint",
-            "gray",
-            "greens",
             "greys",
-            "hot",
-            "ice",
             "magenta",
             "mint",
             "oranges",
             "peach",
             "purples",
             "reds",
+            "greens",
         ]
 
+        colors_nick_goldman = [
+            "#a6cee3",
+            "#1f78b4",
+            "#b2df8a",
+            "#33a02c",
+            "#fb9a99",
+            "#e31a1c",
+            "#fdbf6f",
+            "#ff7f00",
+            "#cab2d6",
+            "#6a3d9a",
+        ]
         colorscale_cont = random.sample(colorscales, 1)[0]
         cmap = cm.get_cmap(colorscale_cont, max(20, len(elements)))
-        # here we generate a color map --> if there are more than 1000 unique elements,
-        # we assume that the variable is some sort of common parameter. e.g. likelihood, step, parsimony...
+        # here we generate a color map --> if there are more than 10 unique elements,
+        # we assume that the variable is some sort of continuous parameter. e.g. likelihood, step, parsimony...
         cont_colorsc = False
         if len(elements) > 10:
             cont_colorsc = True
         # else, we presume this is some kind of difference between sets - e.g. different tree_set
         # we generate random colors to maximize the visual division
         else:
             col_list = [mcolors.rgb2hex(cmap(i)[:3]) for i in range(cmap.N)]
@@ -294,21 +306,27 @@
 
         Sets = np.unique(metadata["SET-ID"])
         for i, SetID in enumerate(Sets):
             idx = metadata["SET-ID"] == SetID
             color_plot_set = color_plot[idx]
             if cont_colorsc:
                 col_list = (
-                    random.sample(colorscales_GO, 1)[0] if not same_scale else "jet"
+                    colorscales_GO[i % len(colorscales_GO)] if not same_scale else "jet"
                 )
             color = col_list
             if len(np.unique(color_plot_set)) == 1:
-                color = random.sample(
-                    [mcolors.rgb2hex(cmap(i)[:3]) for i in range(cmap.N)], 10
-                )
+                if i > len(Sets):
+                    color = random.sample(
+                        [mcolors.rgb2hex(cmap(i)[:3]) for i in range(cmap.N)], 10
+                    )
+                else:
+                    color = [
+                        colors_nick_goldman[i % len(colors_nick_goldman)]
+                        for j in range(3)
+                    ]  # for some reason plotly wants a list of colors to sample from
             metadata_colors[f"{meta}_color_plot"].append(color_plot_set.tolist())
             metadata_colors[f"{meta}_color_map"].append(color)
 
     # initialize go.Figure()
     fig = go.Figure()
 
     # widget for the modification of metadata coloring
@@ -334,14 +352,18 @@
             for i in range(nUnique):
                 fig.data[i + traces_start_at].marker["color"] = metadata_colors[
                     f"{meta_widget.value}_color_plot"
                 ][i]
                 fig.data[i + traces_start_at].marker["colorscale"] = metadata_colors[
                     f"{meta_widget.value}_color_map"
                 ][i]
+                cmin = min(metadata[meta_widget.value]) if type(metadata[meta_widget.value][0]) in ('float', 'int') else 0
+                cmax = max(metadata[meta_widget.value]) if type(metadata[meta_widget.value][0]) in ('float', 'int') else 1
+                fig.data[i + traces_start_at].marker["cmin"]=cmin
+                fig.data[i + traces_start_at].marker["cmax"]=cmax
 
     # bind widget to function response_metadata
     meta_widget.observe(response_meta, names="value")
 
     # define save_pdf_funct to save pdf
     def save_pdf_func(b):
         fig.write_image(name_plot + ".pdf")
@@ -365,14 +387,16 @@
             shapes = np.array(["circle" for _ in range(metadata.shape[0])])
 
         # add a scatter3d trace for each tree_set - i.e. SET-ID unique value
         Sets, nSetID = np.unique(metadata["SET-ID"], return_counts=True)
         # number of sets
         nUnique = len(Sets)
         for i, SetID in enumerate(Sets):
+            cmin = min(metadata[plot_meta]) if type(metadata[plot_meta][0]) in ('float', 'int') else 0
+            cmax = max(metadata[plot_meta]) if type(metadata[plot_meta][0]) in ('float', 'int') else 1
             idx = metadata["SET-ID"] == SetID
             fig.add_trace(
                 go.Scatter3d(
                     name=SetID,
                     x=data[idx, 0],
                     y=data[idx, 1],
                     z=data[idx, 2],
@@ -388,14 +412,16 @@
                     marker_symbol=shapes[idx],
                     marker_color=metadata_colors[f"{plot_meta}_color_plot"][i],
                     text=metadata["SET-ID"].values[idx],
                     opacity=0.7,
                     marker=dict(
                         colorscale=metadata_colors[f"{plot_meta}_color_map"][i],
                         size=size[idx],
+                        cmin=cmin,
+                        cmax=cmax,
                         line=dict(
                             # color='MediumPurple',
                             width=10,
                             color="rgba( 30, 30, 30, 0.3)",
                         ),
                     ),
                 )
@@ -451,15 +477,15 @@
                             - 0.06 * (i - nUnique // 2 * int(round((i + 1) / (nUnique)))),
                             # y=1.5 - 0.06*(i - nUnique//2 * int(round((i+1)/(nUnique)))),
                             yanchor="top",
                         ),
                     )
 
         # buttons_meta define the metadata variable used to color the traces
-        # TODO : this is currently not working for some reson - coming back to it asap
+        # TODO : this is currently not working for some reason - coming back to it asap
         buttons_meta = [
             dict(
                 args=[
                     {
                         "marker": {
                             "color": f"metadata_colors['{plot_meta}_color_plot']",
                             # "colorscale" : f"metadata_colors['{plot_meta}_color_map']"
@@ -598,14 +624,16 @@
             shapes = np.array(["circle" for _ in range(metadata.shape[0])])
 
         # for each tree_set add a scatter trace to the figure
         Sets, nSetID = np.unique(metadata["SET-ID"], return_counts=True)
         # number of unique tree_sets
         nUnique = len(Sets)
         for i, SetID in enumerate(Sets):
+            cmin = min(metadata[plot_meta]) if type(metadata[plot_meta][0]) in ('float', 'int') else 0
+            cmax = max(metadata[plot_meta]) if type(metadata[plot_meta][0]) in ('float', 'int') else 1
             idx = metadata["SET-ID"] == SetID
             fig.add_trace(
                 go.Scatter(
                     name=SetID,
                     x=data[idx, 0],
                     y=data[idx, 1],
                     mode="markers",
@@ -619,14 +647,16 @@
                     marker_symbol=shapes[idx],
                     marker_color=metadata_colors[f"{plot_meta}_color_plot"][i],
                     text=metadata["SET-ID"].values[idx],
                     opacity=0.7,
                     marker=dict(
                         colorscale=metadata_colors[f"{plot_meta}_color_map"][i],
                         size=size[idx],
+                        cmin=cmin,
+                        cmax=cmax,
                         line=dict(
                             # color='MediumPurple',
                             width=2,
                         ),
                     ),
                 )
             )
```

### Comparing `pear_ebi-0.1.57/pear_ebi/embeddings/tSNE_e.py` & `pear_ebi-0.1.58/pear_ebi/embeddings/tSNE_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/interactive_mode/interactive.py` & `pear_ebi-0.1.58/pear_ebi/interactive_mode/interactive.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/subsample/subsample.py` & `pear_ebi-0.1.58/pear_ebi/subsample/subsample.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/subsample/subsample_multiprocess.py` & `pear_ebi-0.1.58/pear_ebi/subsample/subsample_multiprocess.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/tree_emb_parser.py` & `pear_ebi-0.1.58/pear_ebi/tree_emb_parser.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/pear_ebi/tree_set.py` & `pear_ebi-0.1.58/pear_ebi/tree_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             "tsne": tSNE_e.tsne,
             "isomap": Isomap_e.isomap,
             "lle": LLE_e.lle,
             "None": None,
         }
 
         if type(self.distance_matrix) == type(None):
-            self.calculate_distances("hashrf")
+            self.calculate_distances("hashrf_RF")
 
         dim = dimensions if dimensions > 2 else 3
 
         with self.console.status("[bold green]Embedding distances...") as status:
             embedding = methods[method](
                 self.distance_matrix,
                 dim,
@@ -667,36 +667,36 @@
     def calculate_distances(self, method):
         """Computes tree_set distance matrix with method of choice
 
         Args:
             method (str): method/algorithm used to compute distance matrix
         """
         methods = {
-            "hashrf": hashrf.hashrf,
-            "hashrf_weighted": hashrf.hashrf_weighted,
-            "days_RF": maple_RF.calculate_distance_matrix,
-            "quartet": tqdist.quartet,
-            "triplet": tqdist.triplet,
+            "hashrf_RF": hashrf.hashrf,
+            "hashrf_wRF": hashrf.hashrf_weighted,
+            "smart_RF": maple_RF.calculate_distance_matrix,
+            "tqdist_quartet": tqdist.quartet,
+            "tqdist_triplet": tqdist.triplet,
             "None": None,
         }
 
-        if method in ("hashrf", "hashrf_weighted", "quartet", "triplet"):
+        if method in ("hashrf_RF", "hashrf_wRF", "tqdist_quartet", "tqdist_triplet"):
             with open(self.file, "w") as trees:
                 for set in self.collection:
                     with open(set.file, "r") as file:
                         trees.write(file.read())
                         file.close()
                 trees.close()
 
         with self.console.status("[bold green]Calculating distances...") as status:
             self.distance_matrix = methods[method](
                 self.file, self.n_trees, self.output_file
             )
 
-        if method in ("hashrf", "hashrf_weighted", "quartet", "triplet"):
+        if method in ("hashrf_RF", "hashrf_wRF", "tqdist_quartet", "tqdist_triplet"):
             hashrf.bash_command(f"rm {self.file}")
 
         print(f"[bold blue]{method} | Done!")
 
     # the result of addition between two collections
     # is the concatenation of the two collections
     def __add__(self, other):
```

### Comparing `pear_ebi-0.1.57/pear_ebi.egg-info/PKG-INFO` & `pear_ebi-0.1.58/pear_ebi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pear-ebi
-Version: 0.1.57
+Version: 0.1.58
 Summary: Embeds phylogenetic tree distances and produce representations
 Home-page: https://github.com/AndreaRubbi/TreeEmbedding
 Author: Andrea Rubbi
 Author-email: andrea.rubbi.98@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pear-ebi Version: 0.1.57 Summary: Embeds
+Metadata-Version: 2.1 Name: pear-ebi Version: 0.1.58 Summary: Embeds
 phylogenetic tree distances and produce representations Home-page: https://
 github.com/AndreaRubbi/TreeEmbedding Author: Andrea Rubbi Author-email:
 andrea.rubbi.98@gmail.com License: MIT License Description-Content-Type: text/
 markdown License-File: LICENSE.txt
 ****** Phylogeny Embedding &
 Approximate Representation ******
 [logos/LOGO_PEAR.png] ## Goldman Group - European Bioinformatics Institute
```

### Comparing `pear_ebi-0.1.57/pear_ebi.egg-info/SOURCES.txt` & `pear_ebi-0.1.58/pear_ebi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.57/setup.py` & `pear_ebi-0.1.58/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="pear_ebi",
-    version="0.1.57",
+    version="0.1.58",
     license="MIT License",
     description="Embeds phylogenetic tree distances and produce representations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Andrea Rubbi",
     author_email="andrea.rubbi.98@gmail.com",
     url="https://github.com/AndreaRubbi/TreeEmbedding",
```

### Comparing `pear_ebi-0.1.57/test/test.py` & `pear_ebi-0.1.58/test/test.py`

 * *Files identical despite different names*

