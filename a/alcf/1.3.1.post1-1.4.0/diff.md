# Comparing `tmp/alcf-1.3.1.post1.tar.gz` & `tmp/alcf-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcf-1.3.1.post1.tar", last modified: Thu Mar 16 21:05:16 2023, max compression
+gzip compressed data, was "alcf-1.4.0.tar", last modified: Fri Apr 21 17:24:58 2023, max compression
```

## Comparing `alcf-1.3.1.post1.tar` & `alcf-1.4.0.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.317148 alcf-1.3.1.post1/
--rw-r--r--   0 peter     (1000) peter     (1000)      239 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/.editorconfig
--rw-r--r--   0 peter     (1000) peter     (1000)     1144 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)      160 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     1275 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)      979 2023-03-16 21:05:16.317148 alcf-1.3.1.post1/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      764 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.305148 alcf-1.3.1.post1/alcf/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.305148 alcf-1.3.1.post1/alcf/algorithms/
--rw-r--r--   0 peter     (1000) peter     (1000)       27 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.305148 alcf-1.3.1.post1/alcf/algorithms/calibration/
--rw-r--r--   0 peter     (1000) peter     (1000)       62 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/calibration/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      373 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/calibration/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.305148 alcf-1.3.1.post1/alcf/algorithms/cloud_base_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       71 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/cloud_base_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      930 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/cloud_base_detection/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.305148 alcf-1.3.1.post1/alcf/algorithms/cloud_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       66 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/cloud_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      798 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/cloud_detection/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2029 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/couple.py
--rw-r--r--   0 peter     (1000) peter     (1000)      757 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/interp.py
--rw-r--r--   0 peter     (1000) peter     (1000)      781 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/lidar_ratio.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.305148 alcf-1.3.1.post1/alcf/algorithms/noise_removal/
--rw-r--r--   0 peter     (1000) peter     (1000)       64 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/noise_removal/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      981 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/noise_removal/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1682 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/output_sample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     9415 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1131 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/tsample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1776 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/algorithms/zsample.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.309148 alcf-1.3.1.post1/alcf/cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      408 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3555 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/auto.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.309148 alcf-1.3.1.post1/alcf/cmds/auto_cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      141 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/auto_cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      843 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/auto_cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1671 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/auto_cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/auto_cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2804 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/calibrate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2148 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3429 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/convert.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10466 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1395 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5299 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)    17038 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/plot.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6425 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/simulate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3569 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/cmds/stats.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.309148 alcf-1.3.1.post1/alcf/fonts/
--rw-r--r--   0 peter     (1000) peter     (1000)     6709 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/fonts/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)    56032 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/fonts/PublicSans-Bold.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60100 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/fonts/PublicSans-BoldItalic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60316 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/fonts/PublicSans-Italic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    56792 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/fonts/PublicSans-Regular.otf
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.309148 alcf-1.3.1.post1/alcf/lidars/
--rw-r--r--   0 peter     (1000) peter     (1000)     1426 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1649 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/blview.py
--rw-r--r--   0 peter     (1000) peter     (1000)      101 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/caliop.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1322 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/chm15k.py
--rw-r--r--   0 peter     (1000) peter     (1000)      410 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/cl31.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1591 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/cl51.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1364 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/cl61.py
--rw-r--r--   0 peter     (1000) peter     (1000)      763 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2996 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/mpl.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1525 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/lidars/mpl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3323 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/misc.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.309148 alcf-1.3.1.post1/alcf/models/
--rw-r--r--   0 peter     (1000) peter     (1000)     2156 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2227 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/amps.py
--rw-r--r--   0 peter     (1000) peter     (1000)      359 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/cmip5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2719 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2581 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/icon.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2802 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/jra55.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1871 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/merra2.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2013 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/nzcsm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3092 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/nzesm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2414 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/alcf/models/um.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.305148 alcf-1.3.1.post1/alcf.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)      979 2023-03-16 21:05:16.000000 alcf-1.3.1.post1/alcf.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     4447 2023-03-16 21:05:16.000000 alcf-1.3.1.post1/alcf.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-03-16 21:05:16.000000 alcf-1.3.1.post1/alcf.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-03-16 21:02:12.000000 alcf-1.3.1.post1/alcf.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)      158 2023-03-16 21:05:16.000000 alcf-1.3.1.post1/alcf.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        5 2023-03-16 21:05:16.000000 alcf-1.3.1.post1/alcf.egg-info/top_level.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.309148 alcf-1.3.1.post1/bin/
--rwxr-xr-x   0 peter     (1000) peter     (1000)      301 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/bin/alcf
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/build_doc
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.313148 alcf-1.3.1.post1/cosp/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.313148 alcf-1.3.1.post1/cosp/MISR_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    16546 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/MISR_simulator/MISR_simulator.f
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.313148 alcf-1.3.1.post1/cosp/MODIS_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    64835 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/MODIS_simulator/modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     7387 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/MODIS_simulator/test_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5167 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     7506 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/Makefile.cmor1
--rw-r--r--   0 peter     (1000) peter     (1000)     7515 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/Makefile.ibm
--rw-r--r--   0 peter     (1000) peter     (1000)      842 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)    48320 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/README.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      467 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/README_v1.4.1.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.313148 alcf-1.3.1.post1/cosp/actsim/
--rw-r--r--   0 peter     (1000) peter     (1000)    35248 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/actsim/lidar_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    38101 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/actsim/lmd_ipsl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11672 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/actsim/mie_backscatter_1064.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11571 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/actsim/mie_backscatter_532.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11642 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/actsim/mie_backscatter_910.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.313148 alcf-1.3.1.post1/cosp/cfmip2/
--rw-r--r--   0 peter     (1000) peter     (1000)     2508 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7271 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7400 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3320 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3261 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    31979 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    15220 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_constants.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     1881 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_defs.h
--rw-r--r--   0 peter     (1000) peter     (1000)     2644 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_htfrtc.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6934 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_input_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    40704 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_io.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4292 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_isccp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4123 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_lidar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3561 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_misr_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    25019 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3646 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_output_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    26091 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_rttov.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5694 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_rttov_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     9657 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13744 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    70107 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_types.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13287 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/cosp_utils.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.313148 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/
--rw-r--r--   0 peter     (1000) peter     (1000)     2957 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)    59127 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/README
--rw-r--r--   0 peter     (1000) peter     (1000)      165 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/congvec.expected
--rw-r--r--   0 peter     (1000) peter     (1000)     2545 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/congvec.f
--rw-r--r--   0 peter     (1000) peter     (1000)    43978 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/icarus.f
--rw-r--r--   0 peter     (1000) peter     (1000)      869 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/input.data
--rw-r--r--   0 peter     (1000) peter     (1000)     1042 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/input.data.halved
--rw-r--r--   0 peter     (1000) peter     (1000)    13495 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
--rw-r--r--   0 peter     (1000) peter     (1000)     1845 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/license
--rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/rcsid
--rw-r--r--   0 peter     (1000) peter     (1000)    11849 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)     2539 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/test_congvec.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
--rw-r--r--   0 peter     (1000) peter     (1000)    13385 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.313148 alcf-1.3.1.post1/cosp/llnl/
--rw-r--r--   0 peter     (1000) peter     (1000)     7918 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/llnl/cosp_radar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6082 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/llnl/llnl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5703 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/llnl/pf_to_mr.f
--rw-r--r--   0 peter     (1000) peter     (1000)     9585 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/llnl/prec_scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)    75040 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/mac_info.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1317 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/predict_mom07.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.317148 alcf-1.3.1.post1/cosp/quickbeam/
--rw-r--r--   0 peter     (1000) peter     (1000)     1563 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/README
--rw-r--r--   0 peter     (1000) peter     (1000)     4166 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/array_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     5500 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/atmos_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7260 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/calc_Re.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    10671 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/dsd.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4282 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/format_input.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7774 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/gases.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1665 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/load_hydrometeor_classes.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1761 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/load_mie_table.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     9299 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/math_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    17248 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/mrgrnk.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    36058 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/optics_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4211 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/predict_psd07.f
--rw-r--r--   0 peter     (1000) peter     (1000)    18284 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/radar_simulator.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4867 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/radar_simulator_init.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     2934 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/radar_simulator_types.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4039 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/scale_LUTs_io.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4852 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/quickbeam/zeff.f90
--rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/replace_tabs.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/tests.sh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.317148 alcf-1.3.1.post1/cosp/utils/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/utils/COSP_plots.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2021-11-30 13:13:22.000000 alcf-1.3.1.post1/cosp/utils/append_cf3hr_files.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      326 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/download_cosp
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.317148 alcf-1.3.1.post1/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     4118 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-auto.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2261 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-calibrate.1
--rw-r--r--   0 peter     (1000) peter     (1000)      792 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-compare.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1985 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-convert.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5366 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-lidar.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2922 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-model.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5220 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-plot.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1962 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-simulate.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1390 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/man/alcf.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-03-16 21:05:16.317148 alcf-1.3.1.post1/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1800 2023-03-16 21:04:58.000000 alcf-1.3.1.post1/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-16 21:05:16.317148 alcf-1.3.1.post1/src/
--rw-r--r--   0 peter     (1000) peter     (1000)    12585 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/src/cosp_run.f03
--rw-r--r--   0 peter     (1000) peter     (1000)    10920 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/src/main.f03
--rw-r--r--   0 peter     (1000) peter     (1000)     8501 2023-03-16 14:31:44.000000 alcf-1.3.1.post1/src/nc_utils.f03
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)      239 2023-04-21 17:22:09.000000 alcf-1.4.0/.editorconfig
+-rw-r--r--   0 peter     (1000) peter     (1000)     1144 2023-04-21 17:22:09.000000 alcf-1.4.0/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      160 2023-04-21 17:22:09.000000 alcf-1.4.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     1275 2023-04-21 17:22:09.000000 alcf-1.4.0/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     1016 2023-04-21 17:24:58.460616 alcf-1.4.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      764 2023-04-21 17:22:09.000000 alcf-1.4.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/
+-rw-r--r--   0 peter     (1000) peter     (1000)       27 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/calibration/
+-rw-r--r--   0 peter     (1000) peter     (1000)       62 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/calibration/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      373 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/calibration/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/cloud_base_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       71 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/cloud_base_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      930 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/cloud_base_detection/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/cloud_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       66 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/cloud_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      798 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/cloud_detection/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2029 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/couple.py
+-rw-r--r--   0 peter     (1000) peter     (1000)   259682 2023-04-21 17:24:18.000000 alcf-1.4.0/alcf/algorithms/interp.c
+-rw-r--r--   0 peter     (1000) peter     (1000)      781 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/lidar_ratio.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/noise_removal/
+-rw-r--r--   0 peter     (1000) peter     (1000)       64 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/noise_removal/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      981 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/noise_removal/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1682 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/output_sample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9415 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1120 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/tsample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1776 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/zsample.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      408 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3555 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/cmds/auto_cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      141 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto_cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      843 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto_cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1671 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto_cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1086 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto_cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2804 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/calibrate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2148 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3429 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/convert.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10693 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1395 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6342 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    17038 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/plot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6425 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/simulate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3569 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/stats.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/fonts/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6709 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    56032 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/PublicSans-Bold.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60100 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/PublicSans-BoldItalic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60316 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/PublicSans-Italic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    56792 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/PublicSans-Regular.otf
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/lidars/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1426 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2033 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/blview.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      101 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/caliop.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1632 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/chm15k.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      410 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/cl31.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2157 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/cl51.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1709 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/cl61.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      996 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3358 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/mpl.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1873 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/mpl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3867 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/misc.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/models/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2156 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2214 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/amps.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      359 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/cmip5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2719 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2570 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/icon.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2802 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/jra55.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1871 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/merra2.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2013 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/nzcsm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3092 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/nzesm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2414 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/um.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1016 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     4446 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 17:24:19.000000 alcf-1.4.0/alcf.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)      158 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        5 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/bin/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      282 2023-04-21 17:22:09.000000 alcf-1.4.0/bin/alcf
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2023-04-21 17:22:09.000000 alcf-1.4.0/build_doc
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/MISR_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    16546 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/MISR_simulator/MISR_simulator.f
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/MODIS_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    64835 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/MODIS_simulator/modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7387 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/MODIS_simulator/test_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5167 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     7506 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/Makefile.cmor1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7515 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/Makefile.ibm
+-rw-r--r--   0 peter     (1000) peter     (1000)      842 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    48320 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/README.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      467 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/README_v1.4.1.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/actsim/
+-rw-r--r--   0 peter     (1000) peter     (1000)    35248 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/lidar_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    38101 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/lmd_ipsl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11672 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/mie_backscatter_1064.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11571 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/mie_backscatter_532.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11642 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/mie_backscatter_910.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/cfmip2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2508 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7271 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7400 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3320 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3261 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    31979 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    15220 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_constants.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1881 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_defs.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     2644 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_htfrtc.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6934 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_input_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    40704 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_io.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4292 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_isccp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4123 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_lidar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3561 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_misr_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    25019 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3646 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_output_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    26091 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_rttov.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5694 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_rttov_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9657 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13744 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    70107 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_types.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13287 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_utils.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2957 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)    59127 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/README
+-rw-r--r--   0 peter     (1000) peter     (1000)      165 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/congvec.expected
+-rw-r--r--   0 peter     (1000) peter     (1000)     2545 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/congvec.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    43978 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/icarus.f
+-rw-r--r--   0 peter     (1000) peter     (1000)      869 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/input.data
+-rw-r--r--   0 peter     (1000) peter     (1000)     1042 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/input.data.halved
+-rw-r--r--   0 peter     (1000) peter     (1000)    13495 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     1845 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/license
+-rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/rcsid
+-rw-r--r--   0 peter     (1000) peter     (1000)    11849 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     2539 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
+-rw-r--r--   0 peter     (1000) peter     (1000)    13385 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/cosp/llnl/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7918 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/llnl/cosp_radar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6082 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/llnl/llnl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5703 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/llnl/pf_to_mr.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     9585 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/llnl/prec_scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    75040 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/mac_info.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1317 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/predict_mom07.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/cosp/quickbeam/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1563 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/README
+-rw-r--r--   0 peter     (1000) peter     (1000)     4166 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/array_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5500 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/atmos_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7260 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/calc_Re.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    10671 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/dsd.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4282 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/format_input.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7774 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/gases.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1665 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/load_hydrometeor_classes.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1761 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/load_mie_table.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9299 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/math_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    17248 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/mrgrnk.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    36058 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/optics_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4211 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/predict_psd07.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    18284 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/radar_simulator.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4867 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/radar_simulator_init.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     2934 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/radar_simulator_types.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4039 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/scale_LUTs_io.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4852 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/zeff.f90
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/replace_tabs.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/tests.sh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/cosp/utils/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/utils/COSP_plots.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/utils/append_cf3hr_files.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      326 2023-04-21 17:22:09.000000 alcf-1.4.0/download_cosp
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     4118 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-auto.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2261 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-calibrate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      792 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-compare.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1985 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-convert.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5366 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-lidar.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3035 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-model.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5220 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-plot.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1962 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-simulate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1390 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-21 17:24:58.460616 alcf-1.4.0/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1971 2023-04-21 17:22:09.000000 alcf-1.4.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/src/
+-rw-r--r--   0 peter     (1000) peter     (1000)    12585 2023-04-21 17:22:09.000000 alcf-1.4.0/src/cosp_run.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)    10920 2023-04-21 17:22:09.000000 alcf-1.4.0/src/main.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)     8501 2023-04-21 17:22:09.000000 alcf-1.4.0/src/nc_utils.f03
```

### Comparing `alcf-1.3.1.post1/LICENSE.md` & `alcf-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/Makefile` & `alcf-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/PKG-INFO` & `alcf-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 1.1
 Name: alcf
-Version: 1.3.1.post1
+Version: 1.4.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `alcf-1.3.1.post1/README.md` & `alcf-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/algorithms/cloud_base_detection/default.py` & `alcf-1.4.0/alcf/algorithms/cloud_base_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/algorithms/cloud_detection/default.py` & `alcf-1.4.0/alcf/algorithms/cloud_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/algorithms/couple.py` & `alcf-1.4.0/alcf/algorithms/couple.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/algorithms/lidar_ratio.py` & `alcf-1.4.0/alcf/algorithms/lidar_ratio.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/algorithms/noise_removal/default.py` & `alcf-1.4.0/alcf/algorithms/noise_removal/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/algorithms/output_sample.py` & `alcf-1.4.0/alcf/algorithms/output_sample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/algorithms/stats.py` & `alcf-1.4.0/alcf/algorithms/stats.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/algorithms/tsample.py` & `alcf-1.4.0/alcf/algorithms/tsample.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 			continue
 		i = d['.'][var]['.dims'].index('time')
 		shape = list(d[var].shape)
 		d[var] = np.average(d[var], axis=i, weights=w)
 		shape[i] = 1
 		d[var] = d[var].reshape(shape)
 
-def stream(dd, state, tres=None, tlim=None, **options):
+def stream(dd, state, tres=None, **options):
 	if tres is not None:
 		state['aggregate_state'] = state.get('aggregate_state', {})
 		dd = misc.aggregate(dd, state['aggregate_state'], tres)
 		return misc.stream(dd, state, tsample, tres=tres)
 	return dd
```

### Comparing `alcf-1.3.1.post1/alcf/algorithms/zsample.py` & `alcf-1.4.0/alcf/algorithms/zsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/auto.py` & `alcf-1.4.0/alcf/cmds/auto.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/auto_cmds/compare.py` & `alcf-1.4.0/alcf/cmds/auto_cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/auto_cmds/lidar.py` & `alcf-1.4.0/alcf/cmds/auto_cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/auto_cmds/model.py` & `alcf-1.4.0/alcf/cmds/auto_cmds/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,8 +27,13 @@
 		model.run(model_type, input_, model_dir, *args, **kwargs)
 	if i < STEPS.index('simulate'):
 		print('-> %s' % simulate_dir)
 		try: os.mkdir(simulate_dir)
 		except OSError: pass
 		print('! alcf simulate')
 		simulate.run(lidar_type, model_dir, simulate_dir)
-	auto_lidar.run('cosp', simulate_dir, output, *args, **kwargs)
+
+	lidar_skip = skip if i > STEPS.index('simulate') else None
+	auto_lidar.run('cosp', simulate_dir, output, *args,
+		skip=lidar_skip,
+		**kwargs
+	)
```

### Comparing `alcf-1.3.1.post1/alcf/cmds/calibrate.py` & `alcf-1.4.0/alcf/cmds/calibrate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/compare.py` & `alcf-1.4.0/alcf/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/convert.py` & `alcf-1.4.0/alcf/cmds/convert.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/lidar.py` & `alcf-1.4.0/alcf/cmds/lidar.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def read_calibration_file(filename):
 	with open(filename, 'rb') as f:
 		return pst.decode(f.read())
 
 def run(type_, input_, output,
 	altitude=None,
 	tres=300,
-	tlim=None,
+	time=None,
 	tshift=0.,
 	zres=50,
 	zlim=[0., 15000.],
 	cloud_detection='default',
 	cloud_base_detection='default',
 	noise_removal='default',
 	calibration='default',
@@ -111,15 +111,15 @@
 - `cloud_base_detection: <algorithm>`: Cloud base detection algorithm. Available algorithms: `default`, `none`. Default: `default`.
 - `--fix_cl_range`: Fix CL31/CL51 range correction (if `noise_h2` firmware option if off). The critical range is taken from `cl_crit_range`.
 - `lat: <lat>`: Latitude of the instrument (degrees North). Default: Taken from lidar data or `none` if not available.
 - `lon: <lon>`: Longitude of the instrument (degrees East). Default: Taken from lidar data or `none` if not available.
 - `noise_removal: <algorithm>`: Noise removal algorithm. Available algorithms: `default`, `none`.  Default: `default`.
 - `output_sampling: <period>`: Output sampling period (seconds). Default: `86400` (24 hours).
 - `-r`: Process the input directory recursively.
-- `tlim: { <low> <high> }`: Time limits (see Time format below). Default: `none`.
+- `time: { <low> <high> }`: Time limits (see Time format below). Default: `none`.
 - `tres: <tres>`: Time resolution (seconds). Default: `300` (5 min).
 - `tshift: <tshift>`: Time shift (seconds). Default: `0`.
 - `zlim: { <low> <high> }`: Height limits (m). Default: `{ 0 15000 }`.
 - `zres: <zres>`: Height resolution (m). Default: `50`.
 
 Cloud detection options
 -----------------------
@@ -176,14 +176,22 @@
 	# if time is not None:
 	# 	start, end = misc.parse_time(time)
 
 	lidar = LIDARS.get(type_)
 	if lidar is None:
 		raise ValueError('Invalid type: %s' % type_)
 
+	time1 = None
+	if time is not None:
+		time1 = [None, None]
+		for i in 0, 1:
+			time1[i] = aq.from_iso(time[i])
+			if time1[i] is None:
+				raise ValueError('Invalid time format: %s' % time[i])
+
 	noise_removal_mod = None
 	calibration_mod = None
 	cloud_detection_mod = None
 	cloud_base_detection_mod = None
 
 	if type_ not in ('default', 'cosp') and noise_removal is not None:
 		noise_removal_mod = NOISE_REMOVAL.get(noise_removal)
@@ -252,16 +260,16 @@
 			dd = couple_mod.stream(dd, state['couple'], couple)
 		if noise_removal_mod is not None:
 			dd = noise_removal_mod.stream(dd, state['noise_removal'], **options)
 		if calibration_mod is not None:
 			dd = calibration_mod.stream(dd, state['calibration'], **options)
 		if zres is not None or zlim is not None:
 			dd = zsample.stream(dd, state['zsample'], zres=zres, zlim=zlim)
-		if tres is not None or tlim is not None:
-			dd = tsample.stream(dd, state['tsample'], tres=tres/86400., tlim=tlim)
+		if tres is not None or time is not None:
+			dd = tsample.stream(dd, state['tsample'], tres=tres/86400.)
 		if output_sampling is not None:
 			dd = output_sample.stream(dd, state['output_sample'],
 				tres=tres/86400.,
 				output_sampling=output_sampling/86400.,
 			)
 			dd = misc.aggregate(dd, state['output_sample'], output_sampling/86400.)
 		if cloud_detection_mod is not None:
@@ -289,15 +297,17 @@
 			try:
 				d = lidar.read(file_, VARIABLES,
 					altitude=altitude,
 					lon=lon,
 					lat=lat,
 					fix_cl_range=fix_cl_range,
 					cl_crit_range=cl_crit_range,
+					time=time1,
 				)
+				if d is None: continue
 				dd = process([d], state, **options)
 			except SystemExit:
 				raise
 			except SystemError:
 				raise
 			except:
 				logging.warning(traceback.format_exc())
```

### Comparing `alcf-1.3.1.post1/alcf/cmds/main.py` & `alcf-1.4.0/alcf/cmds/main.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/model.py` & `alcf-1.4.0/alcf/cmds/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import sys
 import os
+import traceback
+from concurrent.futures import ProcessPoolExecutor, as_completed
 import numpy as np
 import aquarius_time as aq
 import ds_format as ds
 from alcf.models import MODELS
 
 def get_track_segment(track, t1, t2):
 	mask = (track['time'] >= t1) & (track['time'] < t2)
@@ -22,51 +24,65 @@
 	return {
 		'time': time,
 		'lon': lon,
 		'lat': lat,
 		'.': track['.']
 	}
 
-def model(type_, input_, point=None, time=None, track=None, debug=False,
-	recursive=False):
-	model = MODELS.get(type_)
-	warnings = []
-	if model is None:
-		raise ValueError('Invalid type: %s' % type_)
+def process_model(model, input_, index, point=None, time=None, track=None,
+	debug=False, recursive=False, warnings=[]):
 	if track is not None:
 		track_segment = get_track_segment(track, time[0], time[1])
-		d = model.read(input_, track_segment, warnings=warnings,
+		d = model.read(input_, index, track_segment, warnings=warnings,
 			recursive=recursive)
 	else:
 		lon = np.array([point[0], point[0]], dtype=np.float64)
 		lat = np.array([point[1], point[1]], dtype=np.float64)
 		time = np.array([time[0], time[1]], dtype=np.float64)
 		track = {
 			'lon': lon,
 			'lat': lat,
 			'time': time,
 		}
-		d = model.read(input_, track, warnings=warnings, recursive=recursive)
-	for w in warnings:
-		if len(w) == 2:
-			print('Warning: %s' % w[0], file=sys.stderr)
-			if debug: print(w[1], file=sys.stderr)
-			else: print('Use --debug to print debugging information.', file=sys.stderr)
-		else:
-			print('Warning: %s' % w, file=sys.stderr)
+		d = model.read(input_, index, track, warnings=warnings,
+			recursive=recursive)
 	return d
 
+def worker(type_, input_, index, output, point, t, track1, debug, r):
+	try:
+		model = MODELS[type_]
+		output_filename = os.path.join(output, '%s.nc' % \
+			aq.to_iso(t).replace(':', ''))
+		warnings = []
+		d = process_model(model, input_, index, point, time=[t, t + 1.],
+			track=track1, debug=debug, recursive=r, warnings=warnings)
+		for w in warnings:
+			if len(w) == 2:
+				print('Warning: %s' % w[0], file=sys.stderr)
+				if debug: print(w[1], file=sys.stderr)
+				else: print('Use --debug to print debugging information.', file=sys.stderr)
+			else:
+				print('Warning: %s' % w, file=sys.stderr)
+		if d is not None:
+			ds.write(output_filename, d)
+			print('-> %s' % output_filename)
+	except Exception as e:
+		print('Warning: %s' % str(e), file=sys.stderr)
+		if debug: print(traceback.format_exc(), file=sys.stderr)
+		else: print('Use --debug to print debugging information.', file=sys.stderr)
+
 def run(type_, input_, output,
 	point=None,
 	time=None,
 	track=None,
 	track_override_year=None,
 	track_lon_180=False,
 	debug=False,
 	r=False,
+	njobs=None,
 	**kwargs
 ):
 	'''
 alcf-model -- Extract model data at a point or along a track.
 ==========
 
 Synopsis
@@ -93,14 +109,15 @@
 - `end`: End time (see Time format below).
 - `track`: Track NetCDF file (see Files below).
 - `options`: See Options below.
 
 Options
 -------
 
+- `njobs: <n>`: Number of parallel jobs. Default: number of CPU cores.
 - `-r`: Process the input directory recursively.
 - `--track_lon_180`: Expect track longitude between -180 and 180 degrees.
 - `track_override_year: <year>`: Override year in track. Use if comparing observations with a model statistically. Default: `none`.
 
 Types
 -----
 
@@ -117,15 +134,15 @@
 -----------
 
 `YYYY-MM-DD[THH:MM[:SS]]`, where `YYYY` is year, `MM` is month, `DD` is day, `HH` is hour, `MM` is minute, `SS` is second. Example: `2000-01-01T00:00:00`.
 
 Files
 -----
 
-The track file is a NetCDF file containing 1D variables `lon`, `lat`, and `time`. `time` is time in format conforming with the NetCDF standard, `lon` is longitude between 0 and 360 degrees and `lat` is latitude between -90 and 90 degrees.
+The track file is a NetCDF file containing 1D variables `lon`, `lat`, and `time`. `time` is time in format conforming with the CF Conventions (has a valid `units` attribute), `lon` is longitude between 0 and 360 degrees and `lat` is latitude between -90 and 90 degrees.
 
 Examples
 --------
 
 Extract MERRA-2 model data in `M2I3NVASM.5.12.4` at 45 S, 170 E between 1 and 2 January 2020 and store the output in the directory `alcf_merra2_model`.
 
     alcf model merra2 point: { -45.0 170.0 } time: { 2020-01-01 2020-01-02 } M2I3NVASM.5.12.4 alcf_merra2_model
@@ -147,28 +164,42 @@
 		time1 = track1['time'][0], track1['time'][-1]
 	elif point is not None and time is not None:
 		pass
 	else:
 		raise ValueError('Point and time or track is required')
 
 	if time is not None:
-			time1 = [None, None]
-			for i in 0, 1:
-				time1[i] = aq.from_iso(time[i])
-				if time1[i] is None:
-					raise ValueError('Invalid time format: %s' % time[i])
+		time1 = [None, None]
+		for i in 0, 1:
+			time1[i] = aq.from_iso(time[i])
+			if time1[i] is None:
+				raise ValueError('Invalid time format: %s' % time[i])
 
 	# if os.path.isdir(output):
+
+	model = MODELS.get(type_)
+	if model is None:
+		raise ValueError('Invalid type: %s' % type_)
+
 	t1, t2 = time1[0], time1[1]
-	for t in np.arange(np.floor(t1 - 0.5), np.ceil(t2 - 0.5)) + 0.5:
-		output_filename = os.path.join(output, '%s.nc' % \
-			aq.to_iso(t).replace(':', ''))
-		d = model(type_, input_, point, time=[t, t + 1.],
-			track=track1, debug=debug, recursive=r)
-		if d is not None:
-			ds.write(output_filename, d)
-			print('-> %s' % output_filename)
-	# else:
-	# 	d = model(type_, input_, point, time=time1, track=track1)
-	# 	if d is not None:
-	# 		ds.to_netcdf(output, d)
-	# 		print('-> %s' % output)
+
+	if njobs is None: njobs = os.cpu_count()
+
+	warnings = []
+	index = None
+	if hasattr(model, 'index'):
+		index = model.index(input_, warnings=warnings, recursive=r, njobs=njobs)
+
+	with ProcessPoolExecutor(max_workers=njobs) as ex:
+		fs = []
+		for t in np.arange(np.floor(t1 - 0.5), np.ceil(t2 - 0.5)) + 0.5:
+			f = ex.submit(worker,
+				type_, input_, index, output, point, t, track1, debug, r)
+			fs += [f]
+
+	for w in warnings:
+		if len(w) == 2:
+			print('Warning: %s' % w[0], file=sys.stderr)
+			if debug: print(w[1], file=sys.stderr)
+			else: print('Use --debug to print debugging information.', file=sys.stderr)
+		else:
+			print('Warning: %s' % w, file=sys.stderr)
```

### Comparing `alcf-1.3.1.post1/alcf/cmds/plot.py` & `alcf-1.4.0/alcf/cmds/plot.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/simulate.py` & `alcf-1.4.0/alcf/cmds/simulate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/cmds/stats.py` & `alcf-1.4.0/alcf/cmds/stats.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/fonts/LICENSE.md` & `alcf-1.4.0/alcf/fonts/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/fonts/PublicSans-Bold.otf` & `alcf-1.4.0/alcf/fonts/PublicSans-Bold.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/fonts/PublicSans-BoldItalic.otf` & `alcf-1.4.0/alcf/fonts/PublicSans-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/fonts/PublicSans-Italic.otf` & `alcf-1.4.0/alcf/fonts/PublicSans-Italic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/fonts/PublicSans-Regular.otf` & `alcf-1.4.0/alcf/fonts/PublicSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/lidars/__init__.py` & `alcf-1.4.0/alcf/lidars/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/lidars/blview.py` & `alcf-1.4.0/alcf/lidars/blview.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,22 +15,34 @@
 	'time_bnds': ['time'],
 	'zfull': ['time', 'range', 'altitude'],
 	'altitude': ['time', 'altitude'],
 	'lon': ['time'],
 	'lat': ['time'],
 }
 
-def read(filename, vars, altitude=None, lon=None, lat=None, **kwargs):
+def read(filename, vars, altitude=None, lon=None, lat=None, time=None, **kwargs):
+	sel = None
+	tres = None
+	if time is not None:
+		d = ds.read(filename, 'time')
+		d['time'] = d['time']/86400. + 2440587.5
+		tres = d['time'][1] - d['time'][0]
+		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		mask = misc.time_mask(d['time_bnds'], time[0], time[1])
+		if np.sum(mask) == 0: return None
+		sel = { 'timeDim': mask }
+
 	dep_vars = list(set([y for x in vars if x in VARS for y in VARS[x]]))
-	d = ds.read(filename, dep_vars)
+	d = ds.read(filename, dep_vars, sel=sel)
 	dx = {}
 	if 'time' in vars:
 		n = len(d['time'])
 		dx['time'] = d['time']/86400. + 2440587.5
-		dx['time_bnds'] = misc.time_bnds(dx['time'], dx['time'][1] - dx['time'][0])
+		if tres is None: tres = dx['time'][1] - dx['time'][0]
+		dx['time_bnds'] = misc.time_bnds(dx['time'], tres)
 	if 'altitude' in vars:
 		dx['altitude'] = d['altitude'][:,0].astype(np.float64).filled(np.nan)
 	if 'zfull' in vars:
 		range_ = d['range'].astype(np.float64).filled(np.nan)
 		dx['zfull'] = np.tile(range_, (n, 1))
 		dx['zfull'] = (dx['zfull'].T + dx['altitude']).T
 	if 'lon' in vars:
```

### Comparing `alcf-1.3.1.post1/alcf/lidars/chm15k.py` & `alcf-1.4.0/alcf/lidars/chm15k.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,27 +15,35 @@
 	'time_bnds': ['time'],
 	'zfull': ['range', 'altitude'],
 	'altitude': ['altitude'],
 	'lon': [],
 	'lat': [],
 }
 
-def read(filename, vars, altitude=None, lon=None, lat=None, **kwargs):
+def read(filename, vars, altitude=None, lon=None, lat=None, time=None, **kwargs):
+	sel = None
+	tres = None
+	if time is not None:
+		d = ds.read(filename, 'time', jd=True)
+		tres = d['time'][1] - d['time'][0]
+		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		mask = misc.time_mask(d['time_bnds'], time[0], time[1])
+		if np.sum(mask) == 0: return None
+		sel = {'time': mask}
+
 	dep_vars = list(set([y for x in vars if x in VARS for y in VARS[x]]))
-	d = ds.from_netcdf(
-		filename,
-		dep_vars,
-	)
+	d = ds.read(filename, dep_vars, jd=True, sel=sel)
 	dx = {}
 	n, m = d['beta_raw'].shape
 	if altitude is None:
 		altitude = d['altitude']
 	if 'time' in vars:
-		dx['time'] = d['time']/(24.0*60.0*60.0) + 2416480.5
-		dx['time_bnds'] = misc.time_bnds(dx['time'], dx['time'][1] - dx['time'][0])
+		dx['time'] = d['time']
+		if tres is None: tres = dx['time'][1] - dx['time'][0]
+		dx['time_bnds'] = misc.time_bnds(dx['time'], tres)
 	if 'backscatter' in vars:
 		dx['backscatter'] = d['beta_raw']*1e-11*CALIBRATION_COEFF
 	if 'zfull' in vars:
 		zfull1 = d['range'] + altitude
 		dx['zfull'] = np.tile(zfull1, (n, 1))
 	if 'altitude' in vars:
 		dx['altitude'] = np.full(n, altitude, np.float64)
```

### Comparing `alcf-1.3.1.post1/alcf/lidars/cl51.py` & `alcf-1.4.0/alcf/lidars/cl51.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,47 +13,62 @@
 VARS = {
 	'backscatter': ['backscatter'],
 }
 
 DEFAULT_VARS = [
 	'vertical_resolution',
 	'level',
+	'range',
 	'time',
 	'detection_status',
 ]
 
 def read(filename, vars,
 	altitude=None,
 	lon=None,
 	lat=None,
 	calibration_coeff=CALIBRATION_COEFF,
 	fix_cl_range=False,
 	cl_crit_range=6000,
+	time=None,
 	**kwargs
 ):
+	sel = None
+	tres = None
+	if time is not None:
+		d = ds.read(filename, 'time', jd=True)
+		tres = d['time'][1] - d['time'][0]
+		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		mask = misc.time_mask(d['time_bnds'], time[0], time[1])
+		if np.sum(mask) == 0: return None
+		sel = {'time': mask}
+
 	dep_vars = list(set([y for x in vars if x in VARS for y in VARS[x]]))
 	required_vars = dep_vars + DEFAULT_VARS
-	d = ds.read(
-		filename,
-		required_vars,
-		jd=True
-	)
+
+	d = ds.read(filename, required_vars, jd=True, sel=sel)
 	dx = {}
 	dx['time'] = d['time']
-	dx['time_bnds'] = misc.time_bnds(dx['time'], dx['time'][1] - dx['time'][0])
+	if tres is None: tres = dx['time'][1] - dx['time'][0]
+	dx['time_bnds'] = misc.time_bnds(dx['time'], tres)
 
 	n = len(dx['time'])
-	range_ = d['vertical_resolution'][0]*d['level']
+	if 'range' in d: # ARM CL51 format.
+		range_ = d['range']
+	else: # Generic CL51 format.
+		range_ = d['vertical_resolution'][0]*d['level']
 	if 'zfull' in vars:
 		zfull1 = range_
 		dx['zfull'] = np.tile(zfull1, (n, 1))
 		if altitude is not None:
 			dx['zfull'] += altitude
 	if 'backscatter' in vars:
-		dx['backscatter'] = d['backscatter']*calibration_coeff
+		factor = 1e-4 if (d['.']['backscatter']['units'] == '1/(sr*km*10000)') \
+			else 1 # Factor of 1e-4 if ARM CL51 format.
+		dx['backscatter'] = d['backscatter']*calibration_coeff*factor
 		mask = range_ > 6000
 		if fix_cl_range is True:
 			for i in range(n):
 				if d['detection_status'][i] == b'0':
 					dx['backscatter'][i,mask] *= (range_[mask]/6000)**2
 	if 'altitude' in vars:
 		dx['altitude'] = np.full(n, altitude, np.float64)
```

### Comparing `alcf-1.3.1.post1/alcf/lidars/default.py` & `alcf-1.4.0/alcf/lidars/default.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import numpy as np
 import ds_format as ds
+from alcf import misc
 from alcf.lidars import META
 
 WAVELENGTH = 1064 # nm
 CALIBRATION_COEFF = 1.0
 SURFACE_LIDAR = None
 SC_LR = None
 
-def read(filename, vars, altitude=None, lon=None, lat=None, **kwargs):
-	d = ds.from_netcdf(filename, vars)
+def read(filename, vars, altitude=None, lon=None, lat=None, time=None, **kwargs):
+	sel = None
+	if time is not None:
+		d = ds.read(filename, 'time_bnds', jd=True)
+		mask = misc.time_mask(d['time_bnds'], time[0], time[1])
+		if np.sum(mask) == 0: return None
+		sel = {'time': mask}
+
+	d = ds.read(filename, vars, sel=sel)
 	n = d['backscatter'].shape[0]
 	d['altitude'] = d['altitude'] if altitude is None and 'altitude' in d else \
 		np.full(n, altitude, np.float64)
 	d['lon'] = d['lon'] if lon is None and 'longitude' in d else \
 		np.full(n, lon, np.float64)
 	d['lat'] = d['lat'] if lat is None and 'latitude' in d else \
 		np.full(n, lat, np.float64)
```

### Comparing `alcf-1.3.1.post1/alcf/lidars/mpl.py` & `alcf-1.4.0/alcf/lidars/mpl.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 
 VARS = {
 	'backscatter': ['copol_nrb', 'crosspol_nrb'],
 	'backscatter_x': ['copol_nrb', 'crosspol_nrb'],
 	'backscatter_y': ['copol_nrb', 'crosspol_nrb'],
 }
 
-DEFAULT_VARS = [
-	'range_nrb',
-	'elevation_angle',
+TIME_VARS = [
 	'year',
 	'month',
 	'day',
 	'hour',
 	'minute',
 	'second',
+]
+
+DEFAULT_VARS = TIME_VARS + [
+	'range_nrb',
+	'elevation_angle',
 	'altitude',
 	'latitude',
 	'longitude',
 ]
 
 def parse_temporal_resolution(s):
 	errmsg = 'Unrecognized temporal resolution "%s"' % s
@@ -45,40 +48,50 @@
 	except:
 		raise ValueError(errmsg)
 	for item in FACTOR:
 		if x[1] in item[0]:
 			return f*item[1]
 	raise ValueError(errmsg)
 
-def read(filename, vars, altitude=None, lon=None, lat=None, **kwargs):
+def convert_time(d):
+	time = np.array([
+		(dt.datetime(y, m, day, H, M, S) - dt.datetime(1970, 1, 1)).total_seconds()/(24*60*60) + 2440587.5
+		for y, m, day, H, M, S
+		in zip(d['year'], d['month'], d['day'], d['hour'], d['minute'], d['second'])
+	], np.float64)
+	tres = parse_temporal_resolution(d['.']['.']['temporal_resolution'])
+	time_bnds = misc.time_bnds(time, tres)
+	return time, time_bnds, tres
+
+def read(filename, vars, altitude=None, lon=None, lat=None, time=None, **kwargs):
+	sel = None
+	tres = None
+	if time is not None:
+		d = ds.read(filename, TIME_VARS)
+		d['time'], d['time_bnds'], tres = convert_time(d)
+		mask = misc.time_mask(d['time_bnds'], time[0], time[1])
+		if np.sum(mask) == 0: return None
+		sel = {'time': mask}
+
 	dep_vars = list(set([y for x in vars if x in VARS for y in VARS[x]]))
 	required_vars = dep_vars + DEFAULT_VARS
-	d = ds.from_netcdf(
-		filename,
-		required_vars
-	)
+	d = ds.read(filename, required_vars, sel=sel)
 	mask = d['elevation_angle'] == 0.0
 	dx = {}
 	n = len(d['year'])
 
 	altitude = d['altitude'] if altitude is None else \
 		np.full(n, altitude, np.float64)
 	lon = d['longitude'] if lon is None else \
 		np.full(n, lon, np.float64)
 	lat = d['latitude'] if lat is None else \
 		np.full(n, lat, np.float64)
 
 	if 'time' in vars:
-		dx['time'] = np.array([
-			(dt.datetime(y, m, day, H, M, S) - dt.datetime(1970, 1, 1)).total_seconds()/(24.0*60.0*60.0) + 2440587.5
-			for y, m, day, H, M, S
-			in zip(d['year'], d['month'], d['day'], d['hour'], d['minute'], d['second'])
-		], np.float64)
-		tres = parse_temporal_resolution(d['.']['.']['temporal_resolution'])
-		dx['time_bnds'] = misc.time_bnds(dx['time'], tres)
+		dx['time'], dx['time_bnds'], tres = convert_time(d)
 		# dx['time'] += 13.0/24.0
 	if 'zfull' in vars:
 		zfull1 = np.outer(
 			np.sin(d['elevation_angle']/180.0*np.pi),
 			d['range_nrb']*1e3
 		)
 		dx['zfull'] = np.tile(zfull1, (n, 1))
```

### Comparing `alcf-1.3.1.post1/alcf/lidars/mpl2nc.py` & `alcf-1.4.0/alcf/lidars/mpl2nc.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,30 +18,41 @@
 	'time',
 	'elevation_angle',
 	'gps_altitude',
 	'gps_longitude',
 	'gps_latitude',
 ]
 
-def read(filename, vars, altitude=None, lon=None, lat=None, **kwargs):
-	d = ds.read(filename, VARIABLES, jd=True)
+def read(filename, vars, altitude=None, lon=None, lat=None, time=None, **kwargs):
+	sel = None
+	tres = None
+	if time is not None:
+		d = ds.read(filename, 'time', jd=True)
+		tres = d['time'][1] - d['time'][0]
+		d['time_bnds'] = misc.time_bnds(d['time'], tres)
+		mask = misc.time_mask(d['time_bnds'], time[0], time[1])
+		if np.sum(mask) == 0: return None
+		sel = {'profile': mask}
+
+	d = ds.read(filename, VARIABLES, jd=True, sel=sel)
 	mask = d['elevation_angle'] == 0.0
 	dx = {}
 	n, m = d['nrb_copol'].shape
 
 	altitude = d['gps_altitude'] if altitude is None else \
 		np.full(n, altitude, np.float64)
 	lon = d['gps_longitude'] if lon is None else \
 		np.full(n, lon, np.float64)
 	lat = d['gps_latitude'] if lat is None else \
 		np.full(n, lat, np.float64)
 
 	if 'time' in vars:
 		dx['time'] = d['time']
-		dx['time_bnds'] = misc.time_bnds(dx['time'], dx['time'][1] - dx['time'][0])
+		if tres is None: tres = dx['time'][1] - dx['time'][0]
+		dx['time_bnds'] = misc.time_bnds(dx['time'], tres)
 	if 'zfull' in vars:
 		dx['zfull'] = np.full((n, m), np.nan, np.float64)
 		for i in range(n):
 			range_ = 0.5*d['bin_time'][i]*d['c']*(np.arange(m) + 0.5)
 			dx['zfull'][i,:] = range_*np.sin(d['elevation_angle'][i]/180.0*np.pi)
 			dx['zfull'][i,:] += altitude[i]
 	if 'backscatter' in vars:
```

### Comparing `alcf-1.3.1.post1/alcf/misc.py` & `alcf-1.4.0/alcf/misc.py`

 * *Files 17% similar despite different names*

```diff
@@ -113,16 +113,38 @@
 	for v in variables:
 		if v not in d:
 			raise ValueError('Variable "%s" is required' % v)
 
 def geo_distance(lon1, lat1, lon2, lat2, method='gc'):
 	lon1, lat1, lon2, lat2 = [x/180*np.pi for x in (lon1, lat1, lon2, lat2)]
 	if method == 'gc':
-		return 6371*(np.arccos(np.sin(lat1)*np.sin(lat2) + \
-			np.cos(lat1)*np.cos(lat2)*np.cos(lon1 - lon2)))
+		x = np.sin(lat1)*np.sin(lat2) + \
+			np.cos(lat1)*np.cos(lat2)*np.cos(lon1 - lon2)
+		return 6371*(np.arccos(np.maximum(np.minimum(x, 1), -1)))
 	elif method == 'hs':
 		dlon = lon2 - lon1
 		dlat = lat2 - lat1
 		a = np.sin(dlat/2)**2 + np.cos(lat1)*np.cos(lat2)*np.sin(dlon/2)**2
 		return 2*6371*np.arcsin(np.sqrt(a))
 	else:
 		raise ValueError('Unrecognized method "%s"' % method)
+
+def time_mask(bnds, t1, t2):
+	return ~(((bnds[:,0] < t1) & (bnds[:,1] < t1)) |
+	         ((bnds[:,0] > t2) & (bnds[:,1] > t2)))
+
+def track_at(track, t):
+	ii = np.arange(len(track['time']))
+	i = np.interp(t, track['time'], ii, left=np.nan, right=np.nan)
+	mask = np.isnan(i)
+	i = np.where(mask, 0, i)
+	ilow = np.floor(i).astype(int)
+	ihigh = np.ceil(i).astype(int)
+	ires = i % 1
+	return [
+		np.where(
+			mask,
+			np.nan,
+			(1 - ires)*track[k][ilow] + ires*track[k][ihigh]
+		)
+		for k in ['lon', 'lat']
+	]
```

### Comparing `alcf-1.3.1.post1/alcf/models/__init__.py` & `alcf-1.4.0/alcf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/models/amps.py` & `alcf-1.4.0/alcf/models/amps.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 	'PHB',
 	'PH',
 	'HGT',
 	'XTIME',
 	'XLONG',
 	'XLAT',
 	'T',
-	'T00',
 ]
 
 def read(dirname, track, warnings=[], step=3./24., recursive=False):
 	dd_index = ds.readdir(dirname, variables=['XTIME'], jd=True,
 		recursive=recursive)
 	start_time = track['time'][0]
 	end_time = track['time'][-1]
@@ -50,15 +49,15 @@
 			cli = d['QICE'][:,i,j]
 			cl = 100.*np.ones(len(clw), dtype=np.float64)
 			ps = d['PSFC'][i,j]
 			orog = d['HGT'][i,j]
 			pfull = d['PB'][:,i,j] + d['P'][:,i,j]
 			zfull = (d['PHB'][:,i,j] + d['PH'][:,i,j])/9.81
 			zfull = 0.5*(zfull[1:] + zfull[:-1])
-			theta = d['T'][:,i,j] + d['T00']
+			theta = d['T'][:,i,j] + 300
 			ta = theta*(pfull/ps)**KAPPA
 			newshape3 = [1] + list(clw.shape)
 			newshape2 = [1] + list(ps.shape)
 			d_new = {
 				'clw': clw.reshape(newshape3),
 				'cli': cli.reshape(newshape3),
 				'ta': ta.reshape(newshape3),
```

### Comparing `alcf-1.3.1.post1/alcf/models/era5.py` & `alcf-1.4.0/alcf/models/era5.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/models/icon.py` & `alcf-1.4.0/alcf/models/icon.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,82 +10,81 @@
 	'cli',
 	'clw',
 	'pfull',
 	'ta',
 	'ps',
 ]
 
-def read(dirname, track, warnings=[], step=6./24., recursive=False):
-	d_g = ds.read(os.path.join(dirname, 'vgrid.nc'), [
-		'clon', 'clat'
-	], full=True)
-	d_g['clon'] *= 180/np.pi
-	d_g['clat'] *= 180/np.pi
-
-	n = len(track['time'])
-	ncells = ds.dim(d_g, 'ncells')
-	cell = np.zeros(n, np.int64)
-
-	for i in range(n):
-		dist = misc.geo_distance(
-			np.full(ncells, track['lon'][i]),
-			np.full(ncells, track['lat'][i]),
-			d_g['clon'],
-			d_g['clat'],
-			method='gc'
-		)
-		cell[i] = np.argmin(dist)
-
-	d_g2 = ds.read(os.path.join(dirname, 'vgrid.nc'), ['zg', 'zghalf'], sel={
-		'ncells': cell,
-		'height': ds.dim(d_g, 'height') - 1,
-	})
-
-	dd_idx = ds.readdir(dirname,
+def index(dirname, warnings=[], recursive=False, njobs=1):
+	dd = ds.readdir(dirname,
 		variables=['time'],
 		jd=True,
 		full=True,
 		warnings=warnings,
 		recursive=recursive,
+		parallel=(njobs > 1),
+		njobs=njobs,
 	)
 
+	d_g = ds.read(os.path.join(dirname, 'vgrid.nc'), [
+		'clon', 'clat'
+	], full=True)
+	d_g['clon'] *= 180/np.pi
+	d_g['clat'] *= 180/np.pi
+
+	return [dd, d_g]
+
+def read(dirname, index, track, warnings=[], step=6./24., recursive=False):
 	start_time = track['time'][0]
 	end_time = track['time'][-1]
+	vgrid_filename = os.path.join(dirname, 'vgrid.nc')
 	dd_out = []
+	dd_idx, d_g = index
+	ncells = ds.dim(d_g, 'ncells')
 
 	for var in VARS:
-		print(var)
 		dd = []
 		for d_idx in dd_idx:
 			if var not in d_idx['.']:
 				continue
 			time = d_idx['time']
 			filename = d_idx['filename']
 			ii = np.nonzero(
 				(time >= start_time - step*0.5) &
 				(time < end_time + step*0.5)
 			)[0]
 			for i in ii:
-				i2 = np.argmin(np.abs(track['time'] - time[i]))
-				lat0 = track['lat'][i2]
-				lon0 = track['lon'][i2]
-				print(filename)
+				lon0, lat0 = misc.track_at(track, time[i])
+				dist = misc.geo_distance(
+					np.full(ncells, lon0),
+					np.full(ncells, lat0),
+					d_g['clon'],
+					d_g['clat'],
+					method='gc'
+				)
+				cell = np.argmin(dist)
+
+				d_g2 = ds.read(vgrid_filename, ['zg', 'zghalf'], sel={
+					'ncells': cell,
+					'height': ds.dim(d_g, 'height') - 1,
+				})
+
 				d = ds.read(filename, [var],
 					sel={
 						'time': [i],
-						'ncells': cell[i2],
+						'ncells': cell,
 					},
 					jd=True,
 				)
 				ds.rename_dim(d, 'height', 'level')
 				d['time'] = np.array([time[i]])
-				d['lat'] = np.array([d_g['clat'][cell[i2]]])
-				d['lon'] = np.array([d_g['clon'][cell[i2]]])
-				d['orog'] = np.array([d_g2['zghalf'][i2]])
-				d['zfull'] = d_g2['zg'][::-1,i2]
+				d['lat'] = np.array([d_g['clat'][cell]])
+				d['lon'] = np.array([d_g['clon'][cell]])
+				d['orog'] = np.array([d_g2['zghalf']])
+				d['zfull'] = d_g2['zg'][::-1]
 				d['zfull'] = d['zfull'].reshape((1, len(d['zfull'])))
 				ds.dims(d, 'time', ['time'])
 				ds.dims(d, 'lat', ['time'])
 				ds.dims(d, 'lon', ['time'])
 				ds.dims(d, 'orog', ['time'])
 				ds.dims(d, 'zfull', ['time', 'level'])
 				if d[var].ndim == 2:
```

### Comparing `alcf-1.3.1.post1/alcf/models/jra55.py` & `alcf-1.4.0/alcf/models/jra55.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/models/merra2.py` & `alcf-1.4.0/alcf/models/merra2.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/models/nzcsm.py` & `alcf-1.4.0/alcf/models/nzcsm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/models/nzesm.py` & `alcf-1.4.0/alcf/models/nzesm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf/models/um.py` & `alcf-1.4.0/alcf/models/um.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/alcf.egg-info/PKG-INFO` & `alcf-1.4.0/alcf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 1.1
 Name: alcf
-Version: 1.3.1.post1
+Version: 1.4.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

### Comparing `alcf-1.3.1.post1/alcf.egg-info/SOURCES.txt` & `alcf-1.4.0/alcf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 alcf.egg-info/SOURCES.txt
 alcf.egg-info/dependency_links.txt
 alcf.egg-info/not-zip-safe
 alcf.egg-info/requires.txt
 alcf.egg-info/top_level.txt
 alcf/algorithms/__init__.py
 alcf/algorithms/couple.py
-alcf/algorithms/interp.py
+alcf/algorithms/interp.c
 alcf/algorithms/lidar_ratio.py
 alcf/algorithms/output_sample.py
 alcf/algorithms/stats.py
 alcf/algorithms/tsample.py
 alcf/algorithms/zsample.py
 alcf/algorithms/calibration/__init__.py
 alcf/algorithms/calibration/default.py
```

### Comparing `alcf-1.3.1.post1/build_doc` & `alcf-1.4.0/build_doc`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/MISR_simulator/MISR_simulator.f` & `alcf-1.4.0/cosp/MISR_simulator/MISR_simulator.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/MODIS_simulator/modis_simulator.F90` & `alcf-1.4.0/cosp/MODIS_simulator/modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/MODIS_simulator/test_modis_simulator.F90` & `alcf-1.4.0/cosp/MODIS_simulator/test_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/Makefile` & `alcf-1.4.0/cosp/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/Makefile.cmor1` & `alcf-1.4.0/cosp/Makefile.cmor1`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/Makefile.ibm` & `alcf-1.4.0/cosp/Makefile.ibm`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/README.md` & `alcf-1.4.0/cosp/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/README.txt` & `alcf-1.4.0/cosp/README.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/actsim/lidar_simulator.F90` & `alcf-1.4.0/cosp/actsim/lidar_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/actsim/lmd_ipsl_stats.F90` & `alcf-1.4.0/cosp/actsim/lmd_ipsl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/actsim/mie_backscatter_1064.F90` & `alcf-1.4.0/cosp/actsim/mie_backscatter_1064.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/actsim/mie_backscatter_532.F90` & `alcf-1.4.0/cosp/actsim/mie_backscatter_532.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/actsim/mie_backscatter_910.F90` & `alcf-1.4.0/cosp/actsim/mie_backscatter_910.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt` & `alcf-1.4.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt` & `alcf-1.4.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt` & `alcf-1.4.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt` & `alcf-1.4.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt` & `alcf-1.4.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt` & `alcf-1.4.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp.F90` & `alcf-1.4.0/cosp/cosp.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_constants.F90` & `alcf-1.4.0/cosp/cosp_constants.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_defs.h` & `alcf-1.4.0/cosp/cosp_defs.h`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_htfrtc.F90` & `alcf-1.4.0/cosp/cosp_htfrtc.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_input_nl.txt` & `alcf-1.4.0/cosp/cosp_input_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_io.F90` & `alcf-1.4.0/cosp/cosp_io.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_isccp_simulator.F90` & `alcf-1.4.0/cosp/cosp_isccp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_lidar.F90` & `alcf-1.4.0/cosp/cosp_lidar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_misr_simulator.F90` & `alcf-1.4.0/cosp/cosp_misr_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_modis_simulator.F90` & `alcf-1.4.0/cosp/cosp_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_output_nl.txt` & `alcf-1.4.0/cosp/cosp_output_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_rttov.F90` & `alcf-1.4.0/cosp/cosp_rttov.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_rttov_simulator.F90` & `alcf-1.4.0/cosp/cosp_rttov_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_simulator.F90` & `alcf-1.4.0/cosp/cosp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_stats.F90` & `alcf-1.4.0/cosp/cosp_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_types.F90` & `alcf-1.4.0/cosp/cosp_types.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/cosp_utils.F90` & `alcf-1.4.0/cosp/cosp_utils.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/Makefile` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/README` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/README`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/congvec.f` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/icarus.f` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/icarus.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/input.data` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/input.data`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/input.data.halved` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/input.data.halved`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/license` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/license`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/scops.f` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/test_congvec.f` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/test_congvec.ksh` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh` & `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/llnl/cosp_radar.F90` & `alcf-1.4.0/cosp/llnl/cosp_radar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/llnl/llnl_stats.F90` & `alcf-1.4.0/cosp/llnl/llnl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/llnl/pf_to_mr.f` & `alcf-1.4.0/cosp/llnl/pf_to_mr.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/llnl/prec_scops.f` & `alcf-1.4.0/cosp/llnl/prec_scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/mac_info.txt` & `alcf-1.4.0/cosp/mac_info.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/predict_mom07.F90` & `alcf-1.4.0/cosp/predict_mom07.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/README` & `alcf-1.4.0/cosp/quickbeam/README`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/array_lib.f90` & `alcf-1.4.0/cosp/quickbeam/array_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/atmos_lib.f90` & `alcf-1.4.0/cosp/quickbeam/atmos_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/calc_Re.f90` & `alcf-1.4.0/cosp/quickbeam/calc_Re.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/dsd.f90` & `alcf-1.4.0/cosp/quickbeam/dsd.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/format_input.f90` & `alcf-1.4.0/cosp/quickbeam/format_input.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/gases.f90` & `alcf-1.4.0/cosp/quickbeam/gases.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/load_hydrometeor_classes.f90` & `alcf-1.4.0/cosp/quickbeam/load_hydrometeor_classes.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/load_mie_table.f90` & `alcf-1.4.0/cosp/quickbeam/load_mie_table.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/math_lib.f90` & `alcf-1.4.0/cosp/quickbeam/math_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/mrgrnk.f90` & `alcf-1.4.0/cosp/quickbeam/mrgrnk.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/optics_lib.f90` & `alcf-1.4.0/cosp/quickbeam/optics_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/predict_psd07.f` & `alcf-1.4.0/cosp/quickbeam/predict_psd07.f`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/radar_simulator.f90` & `alcf-1.4.0/cosp/quickbeam/radar_simulator.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/radar_simulator_init.f90` & `alcf-1.4.0/cosp/quickbeam/radar_simulator_init.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/radar_simulator_types.f90` & `alcf-1.4.0/cosp/quickbeam/radar_simulator_types.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/scale_LUTs_io.f90` & `alcf-1.4.0/cosp/quickbeam/scale_LUTs_io.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/quickbeam/zeff.f90` & `alcf-1.4.0/cosp/quickbeam/zeff.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/utils/COSP_plots.py` & `alcf-1.4.0/cosp/utils/COSP_plots.py`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/cosp/utils/append_cf3hr_files.sh` & `alcf-1.4.0/cosp/utils/append_cf3hr_files.sh`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/man/alcf-auto.1` & `alcf-1.4.0/man/alcf-auto.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-AUTO" "1" "March 2023" ""
+.TH "ALCF\-AUTO" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-auto\fR \- Peform automatic processing of model or lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf auto model <model_type> <lidar_type> point: { <lon> <lat> } time: { <start> <end> } [<options>] [<model_options>] [<lidar_options>] [\-\-] <input> <output>
 
 alcf auto model <model_type> <lidar_type> track: <track> [<options>] [<model_options>] [<lidar_options>] [\-\-] <input> <output>
```

### Comparing `alcf-1.3.1.post1/man/alcf-calibrate.1` & `alcf-1.4.0/man/alcf-calibrate.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-CALIBRATE" "1" "March 2023" ""
+.TH "ALCF\-CALIBRATE" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-calibrate\fR \- Calibrate ALC backscatter\.
 .SH "SYNOPSIS"
 .nf
 alcf calibrate <type> [\-\-] <time_periods> <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.3.1.post1/man/alcf-compare.1` & `alcf-1.4.0/man/alcf-compare.1`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-COMPARE" "1" "March 2023" ""
+.TH "ALCF\-COMPARE" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-compare\fR \- Calculate comparison statistics from multiple lidar time series\.
 .SH "SYNOPSIS"
 .nf
 alcf compare <input_1> <input_2> [<input_n>\|\.\|\.\|\.] <output>
 .fi
 .SH "ARGUMENTS"
```

### Comparing `alcf-1.3.1.post1/man/alcf-convert.1` & `alcf-1.4.0/man/alcf-convert.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-CONVERT" "1" "March 2023" ""
+.TH "ALCF\-CONVERT" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-convert\fR \- Convert input instrument or model data to NetCDF\.
 .SH "SYNOPSIS"
 .nf
 alcf convert [options] <type> [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.3.1.post1/man/alcf-lidar.1` & `alcf-1.4.0/man/alcf-lidar.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-LIDAR" "1" "March 2023" ""
+.TH "ALCF\-LIDAR" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-lidar\fR \- Process lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf lidar <type> [<options>] [<algorithm_options>] [\-\-] <lidar> <output>
 .fi
 .SH "DESCRIPTION"
@@ -105,15 +105,15 @@
 .TP
 \fBoutput_sampling: <period>\fR
 Output sampling period (seconds)\. Default: \fB86400\fR (24 hours)\.
 .TP
 \fB\-r\fR
 Process the input directory recursively\.
 .TP
-\fBtlim: { <low> <high> }\fR
+\fBtime: { <low> <high> }\fR
 Time limits (see Time format below)\. Default: \fBnone\fR\.
 .TP
 \fBtres: <tres>\fR
 Time resolution (seconds)\. Default: \fB300\fR (5 min)\.
 .TP
 \fBtshift: <tshift>\fR
 Time shift (seconds)\. Default: \fB0\fR\.
```

### Comparing `alcf-1.3.1.post1/man/alcf-model.1` & `alcf-1.4.0/man/alcf-model.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-MODEL" "1" "March 2023" ""
+.TH "ALCF\-MODEL" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-model\fR \- Extract model data at a point or along a track\.
 .SH "SYNOPSIS"
 .nf
 alcf model <type> point: { <lon> <lat> } time: { <start> <end> } [options] [\-\-] <input> <output>
 
 alcf model <type> track: <track> [\-\-] <input> <output>
@@ -37,14 +37,17 @@
 \fBtrack\fR
 Track NetCDF file (see Files below)\.
 .TP
 \fBoptions\fR
 See Options below\.
 .SH "OPTIONS"
 .TP
+\fBnjobs: <n>\fR
+Number of parallel jobs\. Default: number of CPU cores\.
+.TP
 \fB\-r\fR
 Process the input directory recursively\.
 .TP
 \fB\-\-track_lon_180\fR
 Expect track longitude between \-180 and 180 degrees\.
 .TP
 \fBtrack_override_year: <year>\fR
@@ -73,15 +76,15 @@
 New Zealand Earth System Model (NZESM)\. [Experimental]
 .TP
 \fBum\fR
 UK Met Office Unified Model (UM)\.
 .SH "TIME FORMAT"
 \fBYYYY\-MM\-DD[THH:MM[:SS]]\fR, where \fBYYYY\fR is year, \fBMM\fR is month, \fBDD\fR is day, \fBHH\fR is hour, \fBMM\fR is minute, \fBSS\fR is second\. Example: \fB2000\-01\-01T00:00:00\fR\.
 .SH "FILES"
-The track file is a NetCDF file containing 1D variables \fBlon\fR, \fBlat\fR, and \fBtime\fR\. \fBtime\fR is time in format conforming with the NetCDF standard, \fBlon\fR is longitude between 0 and 360 degrees and \fBlat\fR is latitude between \-90 and 90 degrees\.
+The track file is a NetCDF file containing 1D variables \fBlon\fR, \fBlat\fR, and \fBtime\fR\. \fBtime\fR is time in format conforming with the CF Conventions (has a valid \fBunits\fR attribute), \fBlon\fR is longitude between 0 and 360 degrees and \fBlat\fR is latitude between \-90 and 90 degrees\.
 .SH "EXAMPLES"
 Extract MERRA\-2 model data in \fBM2I3NVASM\.5\.12\.4\fR at 45 S, 170 E between 1 and 2 January 2020 and store the output in the directory \fBalcf_merra2_model\fR\.
 .IP "" 4
 .nf
 alcf model merra2 point: { \-45\.0 170\.0 } time: { 2020\-01\-01 2020\-01\-02 } M2I3NVASM\.5\.12\.4 alcf_merra2_model
 .fi
 .IP "" 0
```

### Comparing `alcf-1.3.1.post1/man/alcf-plot.1` & `alcf-1.4.0/man/alcf-plot.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-PLOT" "1" "March 2023" ""
+.TH "ALCF\-PLOT" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-plot\fR \- Plot lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf plot <plot_type> [<options>] [<plot_options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.3.1.post1/man/alcf-simulate.1` & `alcf-1.4.0/man/alcf-simulate.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-SIMULATE" "1" "March 2023" ""
+.TH "ALCF\-SIMULATE" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-simulate\fR \- Simulate lidar measurements from model data using COSP\.
 .SH "SYNOPSIS"
 .nf
 alcf simulate <type> [<options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.3.1.post1/man/alcf-stats.1` & `alcf-1.4.0/man/alcf-stats.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-STATS" "1" "March 2023" ""
+.TH "ALCF\-STATS" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\-stats\fR \- Calculate cloud occurrence statistics\.
 .SH "SYNOPSIS"
 .nf
 alcf stats [<options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.3.1.post1/man/alcf.1` & `alcf-1.4.0/man/alcf.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF" "1" "March 2023" ""
+.TH "ALCF" "1" "April 2023" ""
 .SH "NAME"
 \fBalcf\fR \- Tool for processing of automatic lidar and ceilometer (ALC) data and intercomparison with atmospheric models\.
 .SH "SYNOPSIS"
 .nf
 alcf <cmd> [<options>]
 alcf <cmd> \-\-help
 .fi
```

### Comparing `alcf-1.3.1.post1/setup.py` & `alcf-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 from setuptools.command.build_py import build_py
+from Cython.Build import cythonize
 import os
 import os.path
 import subprocess
 
 class BuildCOSP(build_py):
 	def run(self):
 		subprocess.run('make', cwd='cosp', check=True)
 		subprocess.run('make', check=True)
 		build_py.run(self)
 
 setup(
 	name='alcf',
-	version='1.3.1.post1',
+	version='1.4.0',
 	description='Automatic Lidar and Ceilometer Framework (ALCF)',
 	author='Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn',
 	author_email='peter@peterkuma.net',
 	license='MIT',
 	scripts=['bin/alcf'],
 	packages=find_packages(),
+	ext_modules=cythonize('alcf/algorithms/interp.pyx', language_level=3),
 	zip_safe=False,
 	package_data={'alcf': ['cosp_alcf'] + \
 		[os.path.join('fonts', x) for x in os.listdir('alcf/fonts')]},
 	data_files=[('share/man/man1',
 		[os.path.join('man', x) for x in os.listdir('man')])],
+	setup_requires=[
+		'cython',
+	],
 	install_requires=[
 		'numpy>=1.16.2',
 		'scipy>=1.1.0',
 		'matplotlib>=3.0.2',
 		'netCDF4>=1.2.9',
 		'cl2nc>=3.3.0',
 		'aquarius-time>=0.1.0',
@@ -43,14 +48,15 @@
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: Console',
 		'Intended Audience :: Science/Research',
 		'License :: OSI Approved :: MIT License',
 		'Operating System :: POSIX',
 		'Programming Language :: Python :: 3',
+		'Programming Language :: Cython',
 		'Programming Language :: Fortran',
 		'Topic :: Scientific/Engineering :: Atmospheric Science',
 		'Topic :: Scientific/Engineering :: Physics',
 		'Topic :: Scientific/Engineering :: Visualization',
 	],
 	cmdclass={
 		'build_py': BuildCOSP,
```

### Comparing `alcf-1.3.1.post1/src/cosp_run.f03` & `alcf-1.4.0/src/cosp_run.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/src/main.f03` & `alcf-1.4.0/src/main.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.3.1.post1/src/nc_utils.f03` & `alcf-1.4.0/src/nc_utils.f03`

 * *Files identical despite different names*

