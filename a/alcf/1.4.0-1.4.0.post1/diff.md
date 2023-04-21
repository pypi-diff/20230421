# Comparing `tmp/alcf-1.4.0.tar.gz` & `tmp/alcf-1.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcf-1.4.0.tar", last modified: Fri Apr 21 17:24:58 2023, max compression
+gzip compressed data, was "alcf-1.4.0.post1.tar", last modified: Fri Apr 21 17:41:23 2023, max compression
```

## Comparing `alcf-1.4.0.tar` & `alcf-1.4.0.post1.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/
--rw-r--r--   0 peter     (1000) peter     (1000)      239 2023-04-21 17:22:09.000000 alcf-1.4.0/.editorconfig
--rw-r--r--   0 peter     (1000) peter     (1000)     1144 2023-04-21 17:22:09.000000 alcf-1.4.0/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)      160 2023-04-21 17:22:09.000000 alcf-1.4.0/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     1275 2023-04-21 17:22:09.000000 alcf-1.4.0/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     1016 2023-04-21 17:24:58.460616 alcf-1.4.0/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      764 2023-04-21 17:22:09.000000 alcf-1.4.0/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/
--rw-r--r--   0 peter     (1000) peter     (1000)       27 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/calibration/
--rw-r--r--   0 peter     (1000) peter     (1000)       62 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/calibration/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      373 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/calibration/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/cloud_base_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       71 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/cloud_base_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      930 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/cloud_base_detection/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/cloud_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       66 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/cloud_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      798 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/cloud_detection/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2029 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/couple.py
--rw-r--r--   0 peter     (1000) peter     (1000)   259682 2023-04-21 17:24:18.000000 alcf-1.4.0/alcf/algorithms/interp.c
--rw-r--r--   0 peter     (1000) peter     (1000)      781 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/lidar_ratio.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf/algorithms/noise_removal/
--rw-r--r--   0 peter     (1000) peter     (1000)       64 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/noise_removal/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      981 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/noise_removal/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1682 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/output_sample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     9415 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1120 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/tsample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1776 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/algorithms/zsample.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      408 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3555 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/cmds/auto_cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      141 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto_cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      843 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto_cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1671 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto_cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1086 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/auto_cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2804 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/calibrate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2148 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3429 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/convert.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10693 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1395 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6342 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)    17038 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/plot.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6425 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/simulate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3569 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/cmds/stats.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/fonts/
--rw-r--r--   0 peter     (1000) peter     (1000)     6709 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)    56032 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/PublicSans-Bold.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60100 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/PublicSans-BoldItalic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60316 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/PublicSans-Italic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    56792 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/fonts/PublicSans-Regular.otf
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/lidars/
--rw-r--r--   0 peter     (1000) peter     (1000)     1426 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2033 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/blview.py
--rw-r--r--   0 peter     (1000) peter     (1000)      101 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/caliop.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1632 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/chm15k.py
--rw-r--r--   0 peter     (1000) peter     (1000)      410 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/cl31.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2157 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/cl51.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1709 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/cl61.py
--rw-r--r--   0 peter     (1000) peter     (1000)      996 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3358 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/mpl.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1873 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/lidars/mpl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3867 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/misc.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/alcf/models/
--rw-r--r--   0 peter     (1000) peter     (1000)     2156 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2214 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/amps.py
--rw-r--r--   0 peter     (1000) peter     (1000)      359 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/cmip5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2719 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2570 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/icon.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2802 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/jra55.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1871 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/merra2.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2013 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/nzcsm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3092 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/nzesm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2414 2023-04-21 17:22:09.000000 alcf-1.4.0/alcf/models/um.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.448616 alcf-1.4.0/alcf.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1016 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     4446 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 17:24:19.000000 alcf-1.4.0/alcf.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)      158 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        5 2023-04-21 17:24:58.000000 alcf-1.4.0/alcf.egg-info/top_level.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.452616 alcf-1.4.0/bin/
--rwxr-xr-x   0 peter     (1000) peter     (1000)      282 2023-04-21 17:22:09.000000 alcf-1.4.0/bin/alcf
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2023-04-21 17:22:09.000000 alcf-1.4.0/build_doc
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/MISR_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    16546 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/MISR_simulator/MISR_simulator.f
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/MODIS_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    64835 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/MODIS_simulator/modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     7387 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/MODIS_simulator/test_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5167 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     7506 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/Makefile.cmor1
--rw-r--r--   0 peter     (1000) peter     (1000)     7515 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/Makefile.ibm
--rw-r--r--   0 peter     (1000) peter     (1000)      842 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)    48320 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/README.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      467 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/README_v1.4.1.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/actsim/
--rw-r--r--   0 peter     (1000) peter     (1000)    35248 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/lidar_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    38101 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/lmd_ipsl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11672 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/mie_backscatter_1064.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11571 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/mie_backscatter_532.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11642 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/actsim/mie_backscatter_910.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.456616 alcf-1.4.0/cosp/cfmip2/
--rw-r--r--   0 peter     (1000) peter     (1000)     2508 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7271 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7400 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3320 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3261 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    31979 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    15220 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_constants.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     1881 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_defs.h
--rw-r--r--   0 peter     (1000) peter     (1000)     2644 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_htfrtc.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6934 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_input_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    40704 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_io.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4292 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_isccp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4123 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_lidar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3561 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_misr_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    25019 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3646 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_output_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    26091 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_rttov.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5694 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_rttov_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     9657 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13744 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    70107 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_types.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13287 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/cosp_utils.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/
--rw-r--r--   0 peter     (1000) peter     (1000)     2957 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)    59127 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/README
--rw-r--r--   0 peter     (1000) peter     (1000)      165 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/congvec.expected
--rw-r--r--   0 peter     (1000) peter     (1000)     2545 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/congvec.f
--rw-r--r--   0 peter     (1000) peter     (1000)    43978 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/icarus.f
--rw-r--r--   0 peter     (1000) peter     (1000)      869 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/input.data
--rw-r--r--   0 peter     (1000) peter     (1000)     1042 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/input.data.halved
--rw-r--r--   0 peter     (1000) peter     (1000)    13495 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
--rw-r--r--   0 peter     (1000) peter     (1000)     1845 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/license
--rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/rcsid
--rw-r--r--   0 peter     (1000) peter     (1000)    11849 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)     2539 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
--rw-r--r--   0 peter     (1000) peter     (1000)    13385 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/cosp/llnl/
--rw-r--r--   0 peter     (1000) peter     (1000)     7918 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/llnl/cosp_radar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6082 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/llnl/llnl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5703 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/llnl/pf_to_mr.f
--rw-r--r--   0 peter     (1000) peter     (1000)     9585 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/llnl/prec_scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)    75040 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/mac_info.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1317 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/predict_mom07.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/cosp/quickbeam/
--rw-r--r--   0 peter     (1000) peter     (1000)     1563 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/README
--rw-r--r--   0 peter     (1000) peter     (1000)     4166 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/array_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     5500 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/atmos_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7260 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/calc_Re.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    10671 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/dsd.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4282 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/format_input.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7774 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/gases.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1665 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/load_hydrometeor_classes.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1761 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/load_mie_table.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     9299 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/math_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    17248 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/mrgrnk.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    36058 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/optics_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4211 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/predict_psd07.f
--rw-r--r--   0 peter     (1000) peter     (1000)    18284 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/radar_simulator.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4867 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/radar_simulator_init.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     2934 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/radar_simulator_types.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4039 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/scale_LUTs_io.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4852 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/quickbeam/zeff.f90
--rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/replace_tabs.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/tests.sh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/cosp/utils/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/utils/COSP_plots.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2021-11-30 13:13:22.000000 alcf-1.4.0/cosp/utils/append_cf3hr_files.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      326 2023-04-21 17:22:09.000000 alcf-1.4.0/download_cosp
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     4118 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-auto.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2261 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-calibrate.1
--rw-r--r--   0 peter     (1000) peter     (1000)      792 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-compare.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1985 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-convert.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5366 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-lidar.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3035 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-model.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5220 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-plot.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1962 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-simulate.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1390 2023-04-21 17:22:09.000000 alcf-1.4.0/man/alcf.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-21 17:24:58.460616 alcf-1.4.0/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1971 2023-04-21 17:22:09.000000 alcf-1.4.0/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:24:58.460616 alcf-1.4.0/src/
--rw-r--r--   0 peter     (1000) peter     (1000)    12585 2023-04-21 17:22:09.000000 alcf-1.4.0/src/cosp_run.f03
--rw-r--r--   0 peter     (1000) peter     (1000)    10920 2023-04-21 17:22:09.000000 alcf-1.4.0/src/main.f03
--rw-r--r--   0 peter     (1000) peter     (1000)     8501 2023-04-21 17:22:09.000000 alcf-1.4.0/src/nc_utils.f03
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.838101 alcf-1.4.0.post1/
+-rw-r--r--   0 peter     (1000) peter     (1000)      239 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/.editorconfig
+-rw-r--r--   0 peter     (1000) peter     (1000)     1144 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      181 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     1275 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     1022 2023-04-21 17:41:23.834101 alcf-1.4.0.post1/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      764 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.818101 alcf-1.4.0.post1/alcf/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf/algorithms/
+-rw-r--r--   0 peter     (1000) peter     (1000)       27 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf/algorithms/calibration/
+-rw-r--r--   0 peter     (1000) peter     (1000)       62 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/calibration/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      373 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/calibration/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf/algorithms/cloud_base_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       71 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/cloud_base_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      930 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/cloud_base_detection/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf/algorithms/cloud_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       66 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/cloud_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      798 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/cloud_detection/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2029 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/couple.py
+-rw-r--r--   0 peter     (1000) peter     (1000)   259682 2023-04-21 17:41:23.000000 alcf-1.4.0.post1/alcf/algorithms/interp.c
+-rw-r--r--   0 peter     (1000) peter     (1000)     1018 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/interp.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)      781 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/lidar_ratio.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf/algorithms/noise_removal/
+-rw-r--r--   0 peter     (1000) peter     (1000)       64 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/noise_removal/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      981 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/noise_removal/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1682 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/output_sample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9415 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1120 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/tsample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1776 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/algorithms/zsample.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf/cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      408 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3555 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/auto.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf/cmds/auto_cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      141 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/auto_cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      843 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/auto_cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1671 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/auto_cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1086 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/auto_cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2804 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/calibrate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2148 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3429 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/convert.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10693 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1395 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6342 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    17038 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/plot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6425 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/simulate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3569 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/cmds/stats.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf/fonts/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6709 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/fonts/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    56032 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/fonts/PublicSans-Bold.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60100 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/fonts/PublicSans-BoldItalic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60316 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/fonts/PublicSans-Italic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    56792 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/fonts/PublicSans-Regular.otf
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.826100 alcf-1.4.0.post1/alcf/lidars/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1426 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2033 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/blview.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      101 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/caliop.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1632 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/chm15k.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      410 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/cl31.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2157 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/cl51.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1709 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/cl61.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      996 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3358 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/mpl.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1873 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/lidars/mpl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3867 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/misc.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.826100 alcf-1.4.0.post1/alcf/models/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2156 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2214 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/amps.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      359 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/cmip5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2719 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2570 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/icon.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2802 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/jra55.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1871 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/merra2.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2013 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/nzcsm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3092 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/nzesm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2414 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/alcf/models/um.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.822100 alcf-1.4.0.post1/alcf.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1022 2023-04-21 17:41:23.000000 alcf-1.4.0.post1/alcf.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     4473 2023-04-21 17:41:23.000000 alcf-1.4.0.post1/alcf.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 17:41:23.000000 alcf-1.4.0.post1/alcf.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 17:41:23.000000 alcf-1.4.0.post1/alcf.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)      158 2023-04-21 17:41:23.000000 alcf-1.4.0.post1/alcf.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        5 2023-04-21 17:41:23.000000 alcf-1.4.0.post1/alcf.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.826100 alcf-1.4.0.post1/bin/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      282 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/bin/alcf
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/build_doc
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.830100 alcf-1.4.0.post1/cosp/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.830100 alcf-1.4.0.post1/cosp/MISR_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    16546 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/MISR_simulator/MISR_simulator.f
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.830100 alcf-1.4.0.post1/cosp/MODIS_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    64835 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/MODIS_simulator/modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7387 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/MODIS_simulator/test_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5167 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     7506 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/Makefile.cmor1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7515 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/Makefile.ibm
+-rw-r--r--   0 peter     (1000) peter     (1000)      842 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    48320 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/README.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      467 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/README_v1.4.1.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.830100 alcf-1.4.0.post1/cosp/actsim/
+-rw-r--r--   0 peter     (1000) peter     (1000)    35248 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/actsim/lidar_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    38101 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/actsim/lmd_ipsl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11672 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/actsim/mie_backscatter_1064.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11571 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/actsim/mie_backscatter_532.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11642 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/actsim/mie_backscatter_910.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.830100 alcf-1.4.0.post1/cosp/cfmip2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2508 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7271 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7400 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3320 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3261 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    31979 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    15220 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_constants.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1881 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_defs.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     2644 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_htfrtc.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6934 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_input_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    40704 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_io.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4292 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_isccp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4123 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_lidar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3561 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_misr_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    25019 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3646 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_output_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    26091 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_rttov.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5694 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_rttov_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9657 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13744 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    70107 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_types.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13287 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/cosp_utils.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.830100 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2957 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)    59127 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/README
+-rw-r--r--   0 peter     (1000) peter     (1000)      165 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/congvec.expected
+-rw-r--r--   0 peter     (1000) peter     (1000)     2545 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/congvec.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    43978 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/icarus.f
+-rw-r--r--   0 peter     (1000) peter     (1000)      869 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/input.data
+-rw-r--r--   0 peter     (1000) peter     (1000)     1042 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/input.data.halved
+-rw-r--r--   0 peter     (1000) peter     (1000)    13495 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     1845 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/license
+-rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/rcsid
+-rw-r--r--   0 peter     (1000) peter     (1000)    11849 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     2539 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/test_congvec.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
+-rw-r--r--   0 peter     (1000) peter     (1000)    13385 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.834101 alcf-1.4.0.post1/cosp/llnl/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7918 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/llnl/cosp_radar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6082 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/llnl/llnl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5703 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/llnl/pf_to_mr.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     9585 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/llnl/prec_scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    75040 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/mac_info.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1317 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/predict_mom07.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.834101 alcf-1.4.0.post1/cosp/quickbeam/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1563 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/README
+-rw-r--r--   0 peter     (1000) peter     (1000)     4166 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/array_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5500 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/atmos_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7260 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/calc_Re.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    10671 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/dsd.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4282 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/format_input.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7774 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/gases.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1665 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/load_hydrometeor_classes.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1761 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/load_mie_table.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9299 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/math_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    17248 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/mrgrnk.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    36058 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/optics_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4211 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/predict_psd07.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    18284 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/radar_simulator.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4867 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/radar_simulator_init.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     2934 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/radar_simulator_types.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4039 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/scale_LUTs_io.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4852 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/quickbeam/zeff.f90
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/replace_tabs.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/tests.sh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.834101 alcf-1.4.0.post1/cosp/utils/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/utils/COSP_plots.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2021-11-30 13:13:22.000000 alcf-1.4.0.post1/cosp/utils/append_cf3hr_files.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      326 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/download_cosp
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.834101 alcf-1.4.0.post1/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     4118 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-auto.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2261 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-calibrate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      792 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-compare.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1985 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-convert.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5366 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-lidar.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3035 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-model.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5220 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-plot.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1962 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-simulate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1390 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/man/alcf.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-21 17:41:23.838101 alcf-1.4.0.post1/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1977 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 17:41:23.834101 alcf-1.4.0.post1/src/
+-rw-r--r--   0 peter     (1000) peter     (1000)    12585 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/src/cosp_run.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)    10920 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/src/main.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)     8501 2023-04-21 17:39:47.000000 alcf-1.4.0.post1/src/nc_utils.f03
```

### Comparing `alcf-1.4.0/LICENSE.md` & `alcf-1.4.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/Makefile` & `alcf-1.4.0.post1/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/PKG-INFO` & `alcf-1.4.0.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alcf
-Version: 1.4.0
+Version: 1.4.0.post1
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
```

### Comparing `alcf-1.4.0/README.md` & `alcf-1.4.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/cloud_base_detection/default.py` & `alcf-1.4.0.post1/alcf/algorithms/cloud_base_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/cloud_detection/default.py` & `alcf-1.4.0.post1/alcf/algorithms/cloud_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/couple.py` & `alcf-1.4.0.post1/alcf/algorithms/couple.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/interp.c` & `alcf-1.4.0.post1/alcf/algorithms/interp.c`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/lidar_ratio.py` & `alcf-1.4.0.post1/alcf/algorithms/lidar_ratio.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/noise_removal/default.py` & `alcf-1.4.0.post1/alcf/algorithms/noise_removal/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/output_sample.py` & `alcf-1.4.0.post1/alcf/algorithms/output_sample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/stats.py` & `alcf-1.4.0.post1/alcf/algorithms/stats.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/tsample.py` & `alcf-1.4.0.post1/alcf/algorithms/tsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/algorithms/zsample.py` & `alcf-1.4.0.post1/alcf/algorithms/zsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/auto.py` & `alcf-1.4.0.post1/alcf/cmds/auto.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/auto_cmds/compare.py` & `alcf-1.4.0.post1/alcf/cmds/auto_cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/auto_cmds/lidar.py` & `alcf-1.4.0.post1/alcf/cmds/auto_cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/auto_cmds/model.py` & `alcf-1.4.0.post1/alcf/cmds/auto_cmds/model.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/calibrate.py` & `alcf-1.4.0.post1/alcf/cmds/calibrate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/compare.py` & `alcf-1.4.0.post1/alcf/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/convert.py` & `alcf-1.4.0.post1/alcf/cmds/convert.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/lidar.py` & `alcf-1.4.0.post1/alcf/cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/main.py` & `alcf-1.4.0.post1/alcf/cmds/main.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/model.py` & `alcf-1.4.0.post1/alcf/cmds/model.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/plot.py` & `alcf-1.4.0.post1/alcf/cmds/plot.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/simulate.py` & `alcf-1.4.0.post1/alcf/cmds/simulate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/cmds/stats.py` & `alcf-1.4.0.post1/alcf/cmds/stats.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/fonts/LICENSE.md` & `alcf-1.4.0.post1/alcf/fonts/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/fonts/PublicSans-Bold.otf` & `alcf-1.4.0.post1/alcf/fonts/PublicSans-Bold.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/fonts/PublicSans-BoldItalic.otf` & `alcf-1.4.0.post1/alcf/fonts/PublicSans-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/fonts/PublicSans-Italic.otf` & `alcf-1.4.0.post1/alcf/fonts/PublicSans-Italic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/fonts/PublicSans-Regular.otf` & `alcf-1.4.0.post1/alcf/fonts/PublicSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/lidars/__init__.py` & `alcf-1.4.0.post1/alcf/lidars/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/lidars/blview.py` & `alcf-1.4.0.post1/alcf/lidars/blview.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/lidars/chm15k.py` & `alcf-1.4.0.post1/alcf/lidars/chm15k.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/lidars/cl51.py` & `alcf-1.4.0.post1/alcf/lidars/cl51.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/lidars/cl61.py` & `alcf-1.4.0.post1/alcf/lidars/cl61.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/lidars/default.py` & `alcf-1.4.0.post1/alcf/lidars/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/lidars/mpl.py` & `alcf-1.4.0.post1/alcf/lidars/mpl.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/lidars/mpl2nc.py` & `alcf-1.4.0.post1/alcf/lidars/mpl2nc.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/misc.py` & `alcf-1.4.0.post1/alcf/misc.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/__init__.py` & `alcf-1.4.0.post1/alcf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/amps.py` & `alcf-1.4.0.post1/alcf/models/amps.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/era5.py` & `alcf-1.4.0.post1/alcf/models/era5.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/icon.py` & `alcf-1.4.0.post1/alcf/models/icon.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/jra55.py` & `alcf-1.4.0.post1/alcf/models/jra55.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/merra2.py` & `alcf-1.4.0.post1/alcf/models/merra2.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/nzcsm.py` & `alcf-1.4.0.post1/alcf/models/nzcsm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/nzesm.py` & `alcf-1.4.0.post1/alcf/models/nzesm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf/models/um.py` & `alcf-1.4.0.post1/alcf/models/um.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/alcf.egg-info/PKG-INFO` & `alcf-1.4.0.post1/alcf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alcf
-Version: 1.4.0
+Version: 1.4.0.post1
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
```

### Comparing `alcf-1.4.0/alcf.egg-info/SOURCES.txt` & `alcf-1.4.0.post1/alcf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 alcf.egg-info/dependency_links.txt
 alcf.egg-info/not-zip-safe
 alcf.egg-info/requires.txt
 alcf.egg-info/top_level.txt
 alcf/algorithms/__init__.py
 alcf/algorithms/couple.py
 alcf/algorithms/interp.c
+alcf/algorithms/interp.pyx
 alcf/algorithms/lidar_ratio.py
 alcf/algorithms/output_sample.py
 alcf/algorithms/stats.py
 alcf/algorithms/tsample.py
 alcf/algorithms/zsample.py
 alcf/algorithms/calibration/__init__.py
 alcf/algorithms/calibration/default.py
```

### Comparing `alcf-1.4.0/build_doc` & `alcf-1.4.0.post1/build_doc`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/MISR_simulator/MISR_simulator.f` & `alcf-1.4.0.post1/cosp/MISR_simulator/MISR_simulator.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/MODIS_simulator/modis_simulator.F90` & `alcf-1.4.0.post1/cosp/MODIS_simulator/modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/MODIS_simulator/test_modis_simulator.F90` & `alcf-1.4.0.post1/cosp/MODIS_simulator/test_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/Makefile` & `alcf-1.4.0.post1/cosp/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/Makefile.cmor1` & `alcf-1.4.0.post1/cosp/Makefile.cmor1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/Makefile.ibm` & `alcf-1.4.0.post1/cosp/Makefile.ibm`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/README.md` & `alcf-1.4.0.post1/cosp/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/README.txt` & `alcf-1.4.0.post1/cosp/README.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/actsim/lidar_simulator.F90` & `alcf-1.4.0.post1/cosp/actsim/lidar_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/actsim/lmd_ipsl_stats.F90` & `alcf-1.4.0.post1/cosp/actsim/lmd_ipsl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/actsim/mie_backscatter_1064.F90` & `alcf-1.4.0.post1/cosp/actsim/mie_backscatter_1064.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/actsim/mie_backscatter_532.F90` & `alcf-1.4.0.post1/cosp/actsim/mie_backscatter_532.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/actsim/mie_backscatter_910.F90` & `alcf-1.4.0.post1/cosp/actsim/mie_backscatter_910.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt` & `alcf-1.4.0.post1/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt` & `alcf-1.4.0.post1/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt` & `alcf-1.4.0.post1/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt` & `alcf-1.4.0.post1/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt` & `alcf-1.4.0.post1/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt` & `alcf-1.4.0.post1/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp.F90` & `alcf-1.4.0.post1/cosp/cosp.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_constants.F90` & `alcf-1.4.0.post1/cosp/cosp_constants.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_defs.h` & `alcf-1.4.0.post1/cosp/cosp_defs.h`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_htfrtc.F90` & `alcf-1.4.0.post1/cosp/cosp_htfrtc.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_input_nl.txt` & `alcf-1.4.0.post1/cosp/cosp_input_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_io.F90` & `alcf-1.4.0.post1/cosp/cosp_io.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_isccp_simulator.F90` & `alcf-1.4.0.post1/cosp/cosp_isccp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_lidar.F90` & `alcf-1.4.0.post1/cosp/cosp_lidar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_misr_simulator.F90` & `alcf-1.4.0.post1/cosp/cosp_misr_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_modis_simulator.F90` & `alcf-1.4.0.post1/cosp/cosp_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_output_nl.txt` & `alcf-1.4.0.post1/cosp/cosp_output_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_rttov.F90` & `alcf-1.4.0.post1/cosp/cosp_rttov.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_rttov_simulator.F90` & `alcf-1.4.0.post1/cosp/cosp_rttov_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_simulator.F90` & `alcf-1.4.0.post1/cosp/cosp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_stats.F90` & `alcf-1.4.0.post1/cosp/cosp_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_types.F90` & `alcf-1.4.0.post1/cosp/cosp_types.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/cosp_utils.F90` & `alcf-1.4.0.post1/cosp/cosp_utils.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/Makefile` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/README` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/README`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/congvec.f` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/icarus.f` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/icarus.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/input.data` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/input.data`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/input.data.halved` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/input.data.halved`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/license` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/license`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/scops.f` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_congvec.f` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/test_congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/test_congvec.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh` & `alcf-1.4.0.post1/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/llnl/cosp_radar.F90` & `alcf-1.4.0.post1/cosp/llnl/cosp_radar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/llnl/llnl_stats.F90` & `alcf-1.4.0.post1/cosp/llnl/llnl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/llnl/pf_to_mr.f` & `alcf-1.4.0.post1/cosp/llnl/pf_to_mr.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/llnl/prec_scops.f` & `alcf-1.4.0.post1/cosp/llnl/prec_scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/mac_info.txt` & `alcf-1.4.0.post1/cosp/mac_info.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/predict_mom07.F90` & `alcf-1.4.0.post1/cosp/predict_mom07.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/README` & `alcf-1.4.0.post1/cosp/quickbeam/README`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/array_lib.f90` & `alcf-1.4.0.post1/cosp/quickbeam/array_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/atmos_lib.f90` & `alcf-1.4.0.post1/cosp/quickbeam/atmos_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/calc_Re.f90` & `alcf-1.4.0.post1/cosp/quickbeam/calc_Re.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/dsd.f90` & `alcf-1.4.0.post1/cosp/quickbeam/dsd.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/format_input.f90` & `alcf-1.4.0.post1/cosp/quickbeam/format_input.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/gases.f90` & `alcf-1.4.0.post1/cosp/quickbeam/gases.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/load_hydrometeor_classes.f90` & `alcf-1.4.0.post1/cosp/quickbeam/load_hydrometeor_classes.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/load_mie_table.f90` & `alcf-1.4.0.post1/cosp/quickbeam/load_mie_table.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/math_lib.f90` & `alcf-1.4.0.post1/cosp/quickbeam/math_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/mrgrnk.f90` & `alcf-1.4.0.post1/cosp/quickbeam/mrgrnk.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/optics_lib.f90` & `alcf-1.4.0.post1/cosp/quickbeam/optics_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/predict_psd07.f` & `alcf-1.4.0.post1/cosp/quickbeam/predict_psd07.f`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/radar_simulator.f90` & `alcf-1.4.0.post1/cosp/quickbeam/radar_simulator.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/radar_simulator_init.f90` & `alcf-1.4.0.post1/cosp/quickbeam/radar_simulator_init.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/radar_simulator_types.f90` & `alcf-1.4.0.post1/cosp/quickbeam/radar_simulator_types.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/scale_LUTs_io.f90` & `alcf-1.4.0.post1/cosp/quickbeam/scale_LUTs_io.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/quickbeam/zeff.f90` & `alcf-1.4.0.post1/cosp/quickbeam/zeff.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/utils/COSP_plots.py` & `alcf-1.4.0.post1/cosp/utils/COSP_plots.py`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/cosp/utils/append_cf3hr_files.sh` & `alcf-1.4.0.post1/cosp/utils/append_cf3hr_files.sh`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-auto.1` & `alcf-1.4.0.post1/man/alcf-auto.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-calibrate.1` & `alcf-1.4.0.post1/man/alcf-calibrate.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-compare.1` & `alcf-1.4.0.post1/man/alcf-compare.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-convert.1` & `alcf-1.4.0.post1/man/alcf-convert.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-lidar.1` & `alcf-1.4.0.post1/man/alcf-lidar.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-model.1` & `alcf-1.4.0.post1/man/alcf-model.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-plot.1` & `alcf-1.4.0.post1/man/alcf-plot.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-simulate.1` & `alcf-1.4.0.post1/man/alcf-simulate.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf-stats.1` & `alcf-1.4.0.post1/man/alcf-stats.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/man/alcf.1` & `alcf-1.4.0.post1/man/alcf.1`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/setup.py` & `alcf-1.4.0.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	def run(self):
 		subprocess.run('make', cwd='cosp', check=True)
 		subprocess.run('make', check=True)
 		build_py.run(self)
 
 setup(
 	name='alcf',
-	version='1.4.0',
+	version='1.4.0.post1',
 	description='Automatic Lidar and Ceilometer Framework (ALCF)',
 	author='Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn',
 	author_email='peter@peterkuma.net',
 	license='MIT',
 	scripts=['bin/alcf'],
 	packages=find_packages(),
 	ext_modules=cythonize('alcf/algorithms/interp.pyx', language_level=3),
```

### Comparing `alcf-1.4.0/src/cosp_run.f03` & `alcf-1.4.0.post1/src/cosp_run.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/src/main.f03` & `alcf-1.4.0.post1/src/main.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.4.0/src/nc_utils.f03` & `alcf-1.4.0.post1/src/nc_utils.f03`

 * *Files identical despite different names*

