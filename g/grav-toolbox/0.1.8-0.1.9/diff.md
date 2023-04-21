# Comparing `tmp/grav-toolbox-0.1.8.tar.gz` & `tmp/grav-toolbox-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grav-toolbox-0.1.8.tar", last modified: Thu Apr 13 12:58:31 2023, max compression
+gzip compressed data, was "grav-toolbox-0.1.9.tar", last modified: Fri Apr 21 17:58:22 2023, max compression
```

## Comparing `grav-toolbox-0.1.8.tar` & `grav-toolbox-0.1.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.310593 grav-toolbox-0.1.8/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/LICENSE
--rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-13 12:58:31.310593 grav-toolbox-0.1.8/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.1.8/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.286594 grav-toolbox-0.1.8/bev_legacy/
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/__init__.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/adjust.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/adjust_reilly1970.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/command_line.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/const.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/drift_mlr.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/init.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/output.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/plots.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/schwaus.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.1.8/bev_legacy/settings.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/bev_legacy/utils.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.286594 grav-toolbox-0.1.8/grav_toolbox.egg-info/
--rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2021 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)      320 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-04-13 12:58:31.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.1.8/grav_toolbox.egg-info/zip-safe
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.290593 grav-toolbox-0.1.8/gravtools/
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.290593 grav-toolbox-0.1.8/gravtools/CG5_utils/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/CG5_utils/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32616 2023-03-22 14:22:41.000000 grav-toolbox-0.1.8/gravtools/CG5_utils/cg5_survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-04-13 12:47:38.000000 grav-toolbox-0.1.8/gravtools/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/const.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.302594 grav-toolbox-0.1.8/gravtools/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    60214 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_autoselection_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9024 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_estimation_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_export_results.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_gis_export_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_load_stations.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_new_campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_options.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1805 2023-04-05 13:15:14.000000 grav-toolbox-0.1.8/gravtools/gui/dialog_setup_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)   191439 2023-04-05 13:08:26.000000 grav-toolbox-0.1.8/gravtools/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_observation_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_correlation_matrix_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_drift_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_obs_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_stat_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_results_vg_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_setup_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_station_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.1.8/gravtools/gui/gui_model_survey_table.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.306594 grav-toolbox-0.1.8/gravtools/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    47182 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/models/campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/models/exceptions.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    37918 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/models/lsm.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    39571 2023-04-13 12:34:11.000000 grav-toolbox-0.1.8/gravtools/models/lsm_diff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    35903 2023-04-13 12:34:49.000000 grav-toolbox-0.1.8/gravtools/models/lsm_nondiff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/models/misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18647 2023-04-13 12:35:28.000000 grav-toolbox-0.1.8/gravtools/models/mlr_bev_legacy.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    21920 2023-04-13 12:57:26.000000 grav-toolbox-0.1.8/gravtools/models/station.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    86806 2023-04-04 07:26:18.000000 grav-toolbox-0.1.8/gravtools/models/survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32345 2023-04-13 12:35:06.000000 grav-toolbox-0.1.8/gravtools/models/vg_lsm.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.306594 grav-toolbox-0.1.8/gravtools/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/scripts/run_gui.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9492 2023-04-05 12:55:15.000000 grav-toolbox-0.1.8/gravtools/settings.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-13 12:58:31.310593 grav-toolbox-0.1.8/gravtools/tides/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/tides/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/gravtools/tides/longman1959.py
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.1.8/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)     1105 2023-04-13 12:58:31.310593 grav-toolbox-0.1.8/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.253033 grav-toolbox-0.1.9/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/LICENSE
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-21 17:58:22.253033 grav-toolbox-0.1.9/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.1.9/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.225033 grav-toolbox-0.1.9/bev_legacy/
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/__init__.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/adjust.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/adjust_reilly1970.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/command_line.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/const.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/drift_mlr.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/init.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/output.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/plots.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/schwaus.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.1.9/bev_legacy/settings.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/utils.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.229033 grav-toolbox-0.1.9/grav_toolbox.egg-info/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2021 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)      320 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/zip-safe
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.229033 grav-toolbox-0.1.9/gravtools/
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.229033 grav-toolbox-0.1.9/gravtools/CG5_utils/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/CG5_utils/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32616 2023-03-22 14:22:41.000000 grav-toolbox-0.1.9/gravtools/CG5_utils/cg5_survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-04-21 17:58:03.000000 grav-toolbox-0.1.9/gravtools/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/const.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.241033 grav-toolbox-0.1.9/gravtools/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    61145 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_autoselection_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9024 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_estimation_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_export_results.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_gis_export_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-04-21 17:28:55.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_load_stations.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-04-21 17:28:55.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_new_campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_options.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1805 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_setup_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   193329 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_observation_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_correlation_matrix_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_drift_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_obs_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_stat_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_vg_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_setup_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_station_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_survey_table.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.245033 grav-toolbox-0.1.9/gravtools/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    48441 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/models/campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/models/exceptions.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    37918 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/models/lsm.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    39571 2023-04-13 12:34:11.000000 grav-toolbox-0.1.9/gravtools/models/lsm_diff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35903 2023-04-13 12:34:49.000000 grav-toolbox-0.1.9/gravtools/models/lsm_nondiff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/models/misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18647 2023-04-13 12:35:28.000000 grav-toolbox-0.1.9/gravtools/models/mlr_bev_legacy.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/models/station.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    86806 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/models/survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32345 2023-04-13 12:35:06.000000 grav-toolbox-0.1.9/gravtools/models/vg_lsm.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.249033 grav-toolbox-0.1.9/gravtools/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/scripts/run_gui.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9521 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/settings.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.249033 grav-toolbox-0.1.9/gravtools/tides/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/tides/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/tides/longman1959.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1105 2023-04-21 17:58:22.253033 grav-toolbox-0.1.9/setup.cfg
```

### Comparing `grav-toolbox-0.1.8/LICENSE` & `grav-toolbox-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/PKG-INFO` & `grav-toolbox-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.1.8
+Version: 0.1.9
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `grav-toolbox-0.1.8/README.md` & `grav-toolbox-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/adjust.py` & `grav-toolbox-0.1.9/bev_legacy/adjust.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/adjust_reilly1970.py` & `grav-toolbox-0.1.9/bev_legacy/adjust_reilly1970.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/command_line.py` & `grav-toolbox-0.1.9/bev_legacy/command_line.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/drift_mlr.py` & `grav-toolbox-0.1.9/bev_legacy/drift_mlr.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/init.py` & `grav-toolbox-0.1.9/bev_legacy/init.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/output.py` & `grav-toolbox-0.1.9/bev_legacy/output.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/plots.py` & `grav-toolbox-0.1.9/bev_legacy/plots.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/schwaus.py` & `grav-toolbox-0.1.9/bev_legacy/schwaus.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/settings.py` & `grav-toolbox-0.1.9/bev_legacy/settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/bev_legacy/utils.py` & `grav-toolbox-0.1.9/bev_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/grav_toolbox.egg-info/PKG-INFO` & `grav-toolbox-0.1.9/grav_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.1.8
+Version: 0.1.9
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `grav-toolbox-0.1.8/grav_toolbox.egg-info/SOURCES.txt` & `grav-toolbox-0.1.9/grav_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/CG5_utils/__init__.py` & `grav-toolbox-0.1.9/gravtools/CG5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/CG5_utils/cg5_survey.py` & `grav-toolbox-0.1.9/gravtools/CG5_utils/cg5_survey.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/__init__.py` & `grav-toolbox-0.1.9/gravtools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (andreas.hellerschmied@bev.gv.at)
 """
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 __author__ = 'Andreas Hellerschmied'
 __git_repo__ = 'https://github.com/ahellers/GravTools'
 __pypi_repo__ = 'https://pypi.org/project/grav-toolbox/'
 __email__ = 'andreas.hellerschmied@bev.gv.at'
 __copyright__ = '(c) 2022 Andreas Hellerschmied'
```

### Comparing `grav-toolbox-0.1.8/gravtools/const.py` & `grav-toolbox-0.1.9/gravtools/const.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/MainWindow.py` & `grav-toolbox-0.1.9/gravtools/gui/MainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,14 +496,17 @@
         self.menubar.setGeometry(QtCore.QRect(0, 0, 1337, 22))
         self.menubar.setObjectName("menubar")
         self.menu_File = QtWidgets.QMenu(self.menubar)
         self.menu_File.setObjectName("menu_File")
         self.menuAdd_Survey = QtWidgets.QMenu(self.menu_File)
         self.menuAdd_Survey.setEnabled(False)
         self.menuAdd_Survey.setObjectName("menuAdd_Survey")
+        self.menu_Add_Stations = QtWidgets.QMenu(self.menu_File)
+        self.menu_Add_Stations.setEnabled(False)
+        self.menu_Add_Stations.setObjectName("menu_Add_Stations")
         self.menu_Observations = QtWidgets.QMenu(self.menubar)
         self.menu_Observations.setEnabled(False)
         self.menu_Observations.setTearOffEnabled(False)
         self.menu_Observations.setObjectName("menu_Observations")
         self.menuEstimation_settings = QtWidgets.QMenu(self.menubar)
         self.menuEstimation_settings.setEnabled(True)
         self.menuEstimation_settings.setObjectName("menuEstimation_settings")
@@ -571,23 +574,30 @@
         self.action_About = QtWidgets.QAction(MainWindow)
         self.action_About.setObjectName("action_About")
         self.action_License = QtWidgets.QAction(MainWindow)
         self.action_License.setObjectName("action_License")
         self.action_Gis_Export_settings = QtWidgets.QAction(MainWindow)
         self.action_Gis_Export_settings.setEnabled(False)
         self.action_Gis_Export_settings.setObjectName("action_Gis_Export_settings")
+        self.action_from_oesgn_table = QtWidgets.QAction(MainWindow)
+        self.action_from_oesgn_table.setObjectName("action_from_oesgn_table")
+        self.action_from_csv_file = QtWidgets.QAction(MainWindow)
+        self.action_from_csv_file.setObjectName("action_from_csv_file")
         self.menuAdd_Survey.addAction(self.action_from_CG5_observation_file)
         self.menuAdd_Survey.addAction(self.action_from_BEV_observation_file)
+        self.menu_Add_Stations.addAction(self.action_from_oesgn_table)
+        self.menu_Add_Stations.addAction(self.action_from_csv_file)
         self.menu_File.addAction(self.action_New_Campaign)
         self.menu_File.addAction(self.action_Change_output_directory)
         self.menu_File.addAction(self.action_Change_Campaign_name)
         self.menu_File.addAction(self.action_Save_Campaign)
         self.menu_File.addAction(self.action_Load_Campaign)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.menuAdd_Survey.menuAction())
+        self.menu_File.addAction(self.menu_Add_Stations.menuAction())
         self.menu_File.addAction(self.action_Add_Stations)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Export_Results)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Options)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Exit)
@@ -708,14 +718,15 @@
         self.radioButton_results_vg_plot_full_polynomial.setToolTip(_translate("MainWindow", "Plot the full estimated VG polynomial versus height above the reference."))
         self.radioButton_results_vg_plot_full_polynomial.setText(_translate("MainWindow", "Plot full polynomial"))
         self.tabWidget_results.setTabText(self.tabWidget_results.indexOf(self.tab_vg_plot), _translate("MainWindow", "VG Plot"))
         self.tabWidget_Main.setTabText(self.tabWidget_Main.indexOf(self.tab_main_results), _translate("MainWindow", "Results"))
         self.tabWidget_Main.setTabToolTip(self.tabWidget_Main.indexOf(self.tab_main_results), _translate("MainWindow", "Setup data: Corrected and reduces observation data accumulated for each instrument setup."))
         self.menu_File.setTitle(_translate("MainWindow", "File"))
         self.menuAdd_Survey.setTitle(_translate("MainWindow", "Add Survey"))
+        self.menu_Add_Stations.setTitle(_translate("MainWindow", "Add Stations"))
         self.menu_Observations.setTitle(_translate("MainWindow", "Observations"))
         self.menuEstimation_settings.setTitle(_translate("MainWindow", "Settings"))
         self.menuHelp.setTitle(_translate("MainWindow", "Help"))
         self.action_New_Campaign.setText(_translate("MainWindow", "&New Campaign"))
         self.action_Save_Campaign.setText(_translate("MainWindow", "&Save Campaign"))
         self.action_Load_Campaign.setText(_translate("MainWindow", "&Load Campaign"))
         self.action_Load_Campaign.setToolTip(_translate("MainWindow", "Load campaign"))
@@ -739,8 +750,10 @@
         self.action_Setup_data_options.setText(_translate("MainWindow", "Setup data options"))
         self.action_Flag_observations.setText(_translate("MainWindow", "Load flags from obs. list file"))
         self.action_Flag_observations.setToolTip(_translate("MainWindow", "Flag observations based ob observations file"))
         self.action_Change_Campaign_name.setText(_translate("MainWindow", "Change Campaign name"))
         self.action_About.setText(_translate("MainWindow", "About"))
         self.action_License.setText(_translate("MainWindow", "License"))
         self.action_Gis_Export_settings.setText(_translate("MainWindow", "GIS export settings"))
+        self.action_from_oesgn_table.setText(_translate("MainWindow", "From OESGN file"))
+        self.action_from_csv_file.setText(_translate("MainWindow", "From CSV file"))
 from pyqtgraph import GraphicsLayoutWidget
```

### Comparing `grav-toolbox-0.1.8/gravtools/gui/__init__.py` & `grav-toolbox-0.1.9/gravtools/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_about.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_about.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_autoselection_settings.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_autoselection_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_corrections.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_corrections.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_estimation_settings.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_estimation_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_export_results.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_export_results.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_gis_export_settings.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_gis_export_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_load_stations.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_load_stations.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_new_campaign.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_new_campaign.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_options.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_options.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/dialog_setup_data.py` & `grav-toolbox-0.1.9/gravtools/gui/dialog_setup_data.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_main.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,14 @@
         # GUI:
         super().__init__()
         self.setupUi(self)
 
         # Connect signals and slots
         self.action_Exit.triggered.connect(self.exit_application)
         self.action_New_Campaign.triggered.connect(self.on_menu_file_new_campaign)
-        self.action_Add_Stations.triggered.connect(self.on_menu_file_load_stations)
         self.action_Corrections.triggered.connect(self.on_menu_observations_corrections)
         self.action_Flag_observations.triggered.connect(self.on_manu_observations_flag_observations)
         self.action_Autoselection_settings.triggered.connect(self.on_menu_observations_autoselection_settings)
         self.action_Estimation_settings.triggered.connect(self.on_menu_estimation_settings)
         self.action_Gis_Export_settings.triggered.connect(self.on_menu_gis_export_settings)
         self.action_Setup_data_options.triggered.connect(self.on_menu_observations_setup_data)
         self.action_Export_Results.triggered.connect(self.on_menu_file_export_results)
@@ -126,14 +125,16 @@
         self.action_About.triggered.connect(self.on_menu_help_about)
         self.pushButton_obs_apply_autoselect_current_data.pressed.connect(self.on_apply_autoselection)
         self.pushButton_obs_comp_setup_data.pressed.connect(self.on_pushbutton_obs_comp_setup_data)
         self.pushButton_obs_run_estimation.pressed.connect(self.on_pushbutton_obs_run_estimation)
         self.pushButton_results_delete_lsm_run.pressed.connect(self.on_pushbutton_results_delete_lsm_run)
         self.pushButton_results_export_shapefile.pressed.connect(self.on_pushButton_results_export_shapefile)
         self.action_from_CG5_observation_file.triggered.connect(self.on_menu_file_load_survey_from_cg5_observation_file)
+        self.action_from_oesgn_table.triggered.connect(self.on_menu_file_load_stations_from_oesgn_table)
+        self.action_from_csv_file.triggered.connect(self.on_menu_file_load_stations_from_csv_file)
         self.lineEdit_filter_stat_name.textChanged.connect(self.on_lineEdit_filter_stat_name_textChanged)
         self.checkBox_filter_observed_stat_only.stateChanged.connect(self.on_checkBox_filter_observed_stat_only_toggled)
         self.checkBox_obs_plot_setup_data.stateChanged.connect(self.on_checkBox_obs_plot_setup_data_state_changed)
         self.treeWidget_observations.itemSelectionChanged.connect(self.on_obs_tree_widget_item_selected)
         self.treeWidget_observations.itemChanged.connect(self.on_tree_widget_item_changed)
         self.checkBox_obs_plot_reduced_observations.clicked.connect(self.on_obs_tree_widget_item_selected)
         self.comboBox_results_lsm_run_selection.currentIndexChanged.connect(
@@ -447,15 +448,15 @@
                 QMessageBox.critical(self, 'Error!', str(e))
                 self.statusBar().showMessage(f"No campaign data loaded.")
             else:
                 # Update GUI:
 
                 # Enable/disable main menu items:
                 self.menuAdd_Survey.setEnabled(True)
-                self.action_Add_Stations.setEnabled(True)
+                self.menu_Add_Stations.setEnabled(True)
                 self.action_Export_Results.setEnabled(True)
                 self.action_Save_Campaign.setEnabled(True)
                 self.action_Change_output_directory.setEnabled(True)
                 self.action_Change_Campaign_name.setEnabled(True)
 
                 # Set up view models and views for this campaign:
                 # - Stations tab:
@@ -2234,15 +2235,15 @@
                                 flag_export_successful = exporter.export(os.path.join(output_path, filename_png))
                         except Exception as e:
                             QMessageBox.critical(self, 'Error!', str(e))
                             flag_export_successful = False
 
                     # Save shapefile:
                     if lsm_run.lsm_method in settings.LSM_METHODS_GIS_EXPORT:
-                        if dlg.checkBox_gis_write_shapefile:
+                        if dlg.checkBox_gis_write_shapefile.isChecked():
                             if self.dlg_gis_export_settings.radioButton_campaign_output_dir.isChecked():
                                 gis_output_dir = self.campaign.output_directory
                             else:
                                 gis_output_dir = self.dlg_gis_export_settings.lineEdit_gis_output_dir.text()
                             if not os.path.isdir(gis_output_dir):
                                 QMessageBox.critical(self, 'Error!',
                                                      f'Invalid output directory for GIS files: {gis_output_dir}')
@@ -2800,15 +2801,15 @@
                 campaign_name=dlg.lineEdit_campaign_name.text(),
                 output_directory=dlg.lineEdit_output_directory.text(),
                 surveys=None,  # Always use non-mutable default arguments!
                 stations=None,  # Always use non-mutable default arguments!
             )
             # Enable/disable main menu items:
             self.menuAdd_Survey.setEnabled(True)
-            self.action_Add_Stations.setEnabled(True)
+            self.menu_Add_Stations.setEnabled(True)
             self.action_Export_Results.setEnabled(True)
             self.action_Save_Campaign.setEnabled(True)
             self.action_Change_output_directory.setEnabled(True)
             self.action_Change_Campaign_name.setEnabled(True)
 
             # Set up GUI (models and widgets):
             # - Stations Tab:
@@ -2845,72 +2846,104 @@
             self.groupBox_obs_view_options.setEnabled(True)
             self.groupBox_obs_data_manipulation.setEnabled(True)
         else:
             self.menu_Observations.setEnabled(False)
             self.groupBox_obs_view_options.setEnabled(False)
             self.groupBox_obs_data_manipulation.setEnabled(False)
 
-    @pyqtSlot()
-    def on_menu_file_load_stations(self):
-        """Launch dialog to load stations to project."""
-        dlg = DialogLoadStations(campaign_output_dir=self.campaign.output_directory)
-        return_value = dlg.exec()
-        if return_value == QDialog.Accepted:
-            # Load Stations to campaign
-            number_of_stations_old = self.campaign.stations.get_number_of_stations
-            try:
-                # WARNING: The following line is required in order to prevent a memory error with
-                # "QSortFilterProxyModelPrivate::proxy_to_source()"
-                # => When adding stations to the model do the follwong steps:
-                # 1.) connect the station model ("self.station_model")
-                # 2.) Add station data
-                # 3.) Set up an connect the proxy model for sorting and filtering ("self.set_up_proxy_station_model")
-                self.connect_station_model_to_table_view()
-
-                # WARNING: Whenever new station data is loaded with "self.campaign.add_stations_from_oesgn_table_file",
-                # the reference between the "view model" () and the "campaign stations dataframe"
-                # (self.campaign.stations.stat_df) is broken!
-                # => Therefore, these two have to be reassigned in order to mirror the same data! This is done by
-                #    calling the method "self.station_model.load_stat_df(self.campaign.stations.stat_df)".
-                self.campaign.add_stations_from_oesgn_table_file(dlg.lineEdit_oesgn_table_file_path.text(),
+    def on_menu_file_load_stations_from_oesgn_table(self):
+        """Load stations from OESGN table file."""
+        options = QFileDialog.Options()
+        options |= QFileDialog.DontUseNativeDialog
+        oesgn_filename, _ = QFileDialog.getOpenFileName(self,
+                                                               'Select OESGN table file',
+                                                               self.campaign.output_directory,
+                                                               "OESGN table file (*.tab)",
+                                                               options=options)
+        if oesgn_filename:
+            # Returns pathName with the '/' separators converted to separators that are appropriate for the underlying
+            # operating system.
+            # On Windows, toNativeSeparators("c:/winnt/system32") returns "c:\winnt\system32".
+            oesgn_filename = QDir.toNativeSeparators(oesgn_filename)
+            self.load_stations(file_type='oesgn', filename=oesgn_filename)
+
+    def on_menu_file_load_stations_from_csv_file(self):
+        """Load stations from a CSV file."""
+        options = QFileDialog.Options()
+        options |= QFileDialog.DontUseNativeDialog
+        csv_filename, _ = QFileDialog.getOpenFileName(self,
+                                                        'Select station CSV file',
+                                                        self.campaign.output_directory,
+                                                        "Station CSV file (*.csv)",
+                                                        options=options)
+        if csv_filename:
+            # Returns pathName with the '/' separators converted to separators that are appropriate for the underlying
+            # operating system.
+            # On Windows, toNativeSeparators("c:/winnt/system32") returns "c:\winnt\system32".
+            csv_filename = QDir.toNativeSeparators(csv_filename)
+            self.load_stations(file_type='csv', filename=csv_filename)
+
+    def load_stations(self, file_type, filename):
+        """Load stations from stations file to the campaign and update the GUI."""
+
+        # Load Stations to campaign
+        number_of_stations_old = self.campaign.stations.get_number_of_stations
+        try:
+            # WARNING: The following line is required in order to prevent a memory error with
+            # "QSortFilterProxyModelPrivate::proxy_to_source()"
+            # => When adding stations to the model do the follwong steps:
+            # 1.) connect the station model ("self.station_model")
+            # 2.) Add station data
+            # 3.) Set up an connect the proxy model for sorting and filtering ("self.set_up_proxy_station_model")
+            self.connect_station_model_to_table_view()
+
+            # WARNING: Whenever new station data is loaded with "self.campaign.add_stations_from_oesgn_table_file",
+            # the reference between the "view model" () and the "campaign stations dataframe"
+            # (self.campaign.stations.stat_df) is broken!
+            # => Therefore, these two have to be reassigned in order to mirror the same data! This is done by
+            #    calling the method "self.station_model.load_stat_df(self.campaign.stations.stat_df)".
+            if file_type == 'oesgn':
+                self.campaign.add_stations_from_oesgn_table_file(filename,
                                                                  is_datum=settings.INIT_OESGN_STATION_AS_DATUM,
                                                                  verbose=IS_VERBOSE)
-                self.campaign.synchronize_stations_and_surveys(verbose=IS_VERBOSE)
-                self.refresh_stations_table_model_and_view()
-                self.set_up_proxy_station_model()
-                self.on_checkBox_filter_observed_stat_only_toggled(
-                    state=self.checkBox_filter_observed_stat_only.checkState())
-
-            except FileNotFoundError:
-                QMessageBox.critical(self, 'File not found error', f'"{dlg.lineEdit_oesgn_table_file_path.text()}" '
-                                                                   f'not found.')
-                self.statusBar().showMessage(f"No stations added.")
-            except Exception as e:
-                QMessageBox.critical(self, 'Error!', str(e))
-                self.statusBar().showMessage(f"No stations added.")
+            elif file_type == 'csv':
+                self.campaign.add_stations_from_csv_file(filename, verbose=IS_VERBOSE)
             else:
-                self.enable_station_view_options_based_on_model()
-                # Show observed stations only based on Checkbox state:
-                self.on_checkBox_filter_observed_stat_only_toggled(self.checkBox_filter_observed_stat_only.checkState(),
-                                                                   auto_range_stations_plot=True)
-                # self.update_stations_map() => Called in self.on_checkBox_filter_observed_stat_only_toggled() above!
-                number_of_stations_added = self.campaign.stations.get_number_of_stations - number_of_stations_old
-
-                # Re-calculate observation corrections, based on the new station data (VG is relevant for height
-                # reduction!):
-                self.apply_observation_corrections()
-
-                # Update the observations table and plot (in case the reduced obs. changed):
-                survey_name, setup_id = self.get_obs_tree_widget_selected_item()
-                self.update_obs_table_view(survey_name, setup_id)
-                self.plot_observations(survey_name)
+                raise AssertionError(f'Unknown station file type: {file_type}!')
+            self.campaign.synchronize_stations_and_surveys(verbose=IS_VERBOSE)
+            self.refresh_stations_table_model_and_view()
+            self.set_up_proxy_station_model()
+            self.on_checkBox_filter_observed_stat_only_toggled(
+                state=self.checkBox_filter_observed_stat_only.checkState())
 
-                self.statusBar().showMessage(f"{number_of_stations_added} stations added.")
-        else:
+        except FileNotFoundError:
+            QMessageBox.critical(self, 'File not found error', f'"{filename}" not found.')
+            self.statusBar().showMessage(f"No stations added.")
+        except Exception as e:
+            QMessageBox.critical(self, 'Error!', str(e))
             self.statusBar().showMessage(f"No stations added.")
+        else:
+            self.enable_station_view_options_based_on_model()
+            # Show observed stations only based on Checkbox state:
+            self.on_checkBox_filter_observed_stat_only_toggled(self.checkBox_filter_observed_stat_only.checkState(),
+                                                               auto_range_stations_plot=True)
+            # self.update_stations_map() => Called in self.on_checkBox_filter_observed_stat_only_toggled() above!
+            number_of_stations_added = self.campaign.stations.get_number_of_stations - number_of_stations_old
+
+            # Re-calculate observation corrections, based on the new station data (VG is relevant for height
+            # reduction!):
+            self.apply_observation_corrections()
+
+            # Update the observations table and plot (in case the reduced obs. changed):
+            survey_name, setup_id = self.get_obs_tree_widget_selected_item()
+            self.update_obs_table_view(survey_name, setup_id)
+            self.plot_observations(survey_name)
+
+            self.statusBar().showMessage(f"{number_of_stations_added} stations added.")
+
 
     def enable_station_view_options_based_on_model(self):
         """Enable or disable the station view options based on the number of stations in the model."""
         if len(self.station_model._data) > 0:
             self.groupBox_filter_options.setEnabled(True)
             self.groupBox_edit_options.setEnabled(True)
             self.groupBox_stations_map_view_options.setEnabled(True)
```

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_misc.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_observation_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_observation_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_correlation_matrix_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_correlation_matrix_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_drift_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_drift_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_obs_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_obs_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_stat_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_stat_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_results_vg_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_vg_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_setup_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_setup_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_station_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_station_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/gui/gui_model_survey_table.py` & `grav-toolbox-0.1.9/gravtools/gui/gui_model_survey_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/__init__.py` & `grav-toolbox-0.1.9/gravtools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/campaign.py` & `grav-toolbox-0.1.9/gravtools/models/campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,14 +386,26 @@
         is_datum : bool, optional (default = False)
             `True` indicates that all loaded OESGN stations are initially selected as datum stations (is_datum=True)
         verbose : bool, optional (default=False)
             If `True`, status messages are printed to the command line.
         """
         self.stations.add_stations_from_oesgn_table(filename=oesgn_filename, is_datum=is_datum, verbose=verbose)
 
+    def add_stations_from_csv_file(self, csv_filename, verbose=False):
+        """Add station from a CSV file.
+
+        Parameters
+        ----------
+        csv_filename : string, specifying the path and filename of the station csv file
+            Stations in this csv file are added to the campaign.
+        verbose : bool, optional (default=False)
+            If `True`, status messages are printed to the command line.
+        """
+        self.stations.add_stations_from_csv_file(filename=csv_filename, verbose=verbose)
+
     def synchronize_stations_and_surveys(self, verbose=False):
         """Synchronize information between station and survey data in the campaign.
 
         The following information is synchronized:
 
         - The `is_observed` flags in the :py:obj:`.Campaign.stations.stat_df` are set according to the surveys in
           :py:obj:`.Campaign.surveys`. `True` indicated that the station as observed at least once.
@@ -658,21 +670,33 @@
                         dhb_m = dhb_list_m[0]
                         dhf_m = dhf_list_m[0]
                     elif vertical_offset_mode == 'mean':
                         dhb_m = np.mean(dhb_list_m)
                         dhf_m = np.mean(dhf_list_m)
 
                     # Get gravimeter S/N and gravimeter type of first survey in the list:
-                    if verbose:
-                        if len(observed_in_surveys) > 1:
+
+                    if len(observed_in_surveys) > 1:
+                        if verbose:
                             print(f'WARNING: station {station_name} was observed in {len(observed_in_surveys)} surveys! Hence, '
-                                  f'the gravimeter serial number and type may be ambiguous in the nsb file!')
-                    gravimeter_type = self.surveys[observed_in_surveys[0]].gravimeter_type
-                    gravimeter_serial_number = self.surveys[observed_in_surveys[0]].gravimeter_serial_number
-                    date_str = self.surveys[observed_in_surveys[0]].date.strftime('%Y%m%d')
+                                  f'the gravimeter serial number/type and the observation date may be ambiguous in the nsb file!')
+                            print(
+                                f' - {station_name} was observed the following surveys: {", ".join(observed_in_surveys)}')
+                        # Get the latest survey in which the station was observed:
+                        latest_survey_name = ''
+                        latest_survey_date = dt.date(1900,1,1)
+                        for survey in observed_in_surveys:
+                            if self.surveys[survey].date > latest_survey_date:
+                                latest_survey_date = self.surveys[survey].date
+                                latest_survey_name = survey
+                    else:
+                        latest_survey_name = observed_in_surveys[0]
+                    gravimeter_type = self.surveys[latest_survey_name].gravimeter_type
+                    gravimeter_serial_number = self.surveys[latest_survey_name].gravimeter_serial_number
+                    date_str = self.surveys[latest_survey_name].date.strftime('%Y%m%d')
 
                     # Comment string:
                     # - Max. 5 characters!
                     if WRITE_COMMENT_TO_NSB == 'cg5_serial_number':
                         comment_str = str(gravimeter_serial_number)
                     elif WRITE_COMMENT_TO_NSB == 'inst_id':
                         comment_str = GRAVIMETER_SERIAL_NUMBER_TO_ID_LOOKUPTABLE[gravimeter_serial_number]
```

### Comparing `grav-toolbox-0.1.8/gravtools/models/exceptions.py` & `grav-toolbox-0.1.9/gravtools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/lsm.py` & `grav-toolbox-0.1.9/gravtools/models/lsm.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/lsm_diff.py` & `grav-toolbox-0.1.9/gravtools/models/lsm_diff.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/lsm_nondiff.py` & `grav-toolbox-0.1.9/gravtools/models/lsm_nondiff.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/misc.py` & `grav-toolbox-0.1.9/gravtools/models/misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/mlr_bev_legacy.py` & `grav-toolbox-0.1.9/gravtools/models/mlr_bev_legacy.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/station.py` & `grav-toolbox-0.1.9/gravtools/models/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,19 +158,19 @@
         """
         widths = (
             10,  # Punktnummer im ÖSGN
             24,  # Anmerkung
             8,  # Geograph. Breite [deg] 34
             8,  # Geograph. Länge [deg] 42
             8,  # Höhe [m] 50
-            7,  # g [µGal] 58
-            3,  # mittlerer Fehler von g [?] 65
+            7,  # g - 9.8e8 [µGal] 58
+            3,  # mittlerer Fehler von g [µGal] 65
             4,  # Vertikalgradient der Schwere [µGal/m] 68
             6,  # Datum 73
-            12,  # Punktidentität 79
+            12, # Punktidentität 79
         )
         column_names = (
             'station_name',
             'notes',
             'lat_deg',
             'long_deg',
             'height_m',
@@ -407,15 +407,15 @@
 
         # Add stations to a temp. copy of self.stat_df:
         stat_df_old = self.stat_df.copy(deep=True)
 
         # Add missing stations to stat_df by matching the station names only (location parameters of observed stations
         # may differ!):
         # - From station files => Drop existing entries with the same name in any case!
-        if data_source_type == 'oesgn_table':
+        if data_source_type == 'oesgn_table' or data_source_type == 'csv_stat_file':
             stat_df_new = pd.concat([stat_df_old, stat_df_add]).drop_duplicates(
                 subset=['station_name'],
                 keep='last'
             ).reset_index(drop=True)
         # From observation file  => Drop existing entries with the same name!
         elif data_source_type == 'obs_file':
             # => Replace entries with data_source = obs_file:
@@ -435,14 +435,36 @@
         if verbose:
             number_of_new_stations = len(stat_df_add)
             number_of_stations = len(self.stat_df)
             stations_added = number_of_stations - number_of_existing_stations
             print(f"{number_of_new_stations} stations loaded. "
                   f"{stations_added} stations added ({number_of_new_stations - stations_added} already listed).")
 
+
+    def add_stations_from_csv_file(self, filename, verbose=False):
+        """Adds (appends) all stations of the input OESGN table to the station dataframe.
+
+        Parameters
+        ----------
+        filename : str
+            Name (and path) of the OESGN table file.
+        verbose : bool, optional
+            Print notifications, if `True` (default=`False`)
+        """
+        if verbose:
+            print(f'Read station csv file: {filename}')
+        stat_df_new = pd.read_csv(filename, comment='#')
+        stat_df_new = self._stat_df_add_columns(stat_df_new)
+        stat_df_new = self._stat_df_reorder_columns(stat_df_new)
+        stat_df_new['is_observed'] = False  # Default = False
+        stat_df_new['is_datum'] = False
+        stat_df_new['source_type'] = 'csv_stat_file'
+        stat_df_new['source_name'] = os.path.basename(filename)
+        self.add_stations(stat_df_new, data_source_type='csv_stat_file', verbose=verbose)
+
     def set_datum_stations(self, station_names: list, is_datum: bool, verbose=False):
         """
         Dependent on the `is_datum` flag set the datum status of all stations in the list
 
         Parameters
         ----------
         station_names : list of str
```

### Comparing `grav-toolbox-0.1.8/gravtools/models/survey.py` & `grav-toolbox-0.1.9/gravtools/models/survey.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/models/vg_lsm.py` & `grav-toolbox-0.1.9/gravtools/models/vg_lsm.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/scripts/__init__.py` & `grav-toolbox-0.1.9/gravtools/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/scripts/run_gui.py` & `grav-toolbox-0.1.9/gravtools/scripts/run_gui.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/settings.py` & `grav-toolbox-0.1.9/gravtools/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 
 SURVEY_DATA_SOURCE_TYPES = {
     'cg5_obs_file_txt': 'Scintrex CG5 observation file (text format)',
     'bev_obs_file': 'Simple observation file format used by BEV',
 }
 
 STATION_DATA_SOURCE_TYPES = {
-    'oesgn_table': 'Control points of the Austrian gravity base network (OESGN).',
-    'obs_file': 'From an observation file'
+    'oesgn_table': 'Austrian gravity base network stations (OESGN).',
+    'csv_stat_file': 'CVS station file',
+    'obs_file': 'From an observation file',
 }
 
 TIDE_CORRECTION_TYPES = {
     'cg5_longman1959': 'Instrument-implemented tidal correction of the Scintrex CG-5',
     'longman1959': 'Tidal corrections by the model of Longman (1959)',
     'no_tide_corr': 'No tide correction applied',
     'unknown': 'Unknown whether a tide correction was applied',
```

### Comparing `grav-toolbox-0.1.8/gravtools/tides/__init__.py` & `grav-toolbox-0.1.9/gravtools/tides/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/gravtools/tides/longman1959.py` & `grav-toolbox-0.1.9/gravtools/tides/longman1959.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.8/setup.cfg` & `grav-toolbox-0.1.9/setup.cfg`

 * *Files identical despite different names*

