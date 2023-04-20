# Comparing `tmp/scipion-em-xmipptomo-3.23.3.3.tar.gz` & `tmp/scipion-em-xmipptomo-3.23.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-xmipptomo-3.23.3.3.tar", last modified: Wed Apr 19 08:35:26 2023, max compression
+gzip compressed data, was "scipion-em-xmipptomo-3.23.3.4.tar", last modified: Thu Apr 20 22:01:49 2023, max compression
```

## Comparing `scipion-em-xmipptomo-3.23.3.3.tar` & `scipion-em-xmipptomo-3.23.3.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.769371 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 08:35:26.000000 scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.769371 scipion-em-xmipptomo-3.23.3.3/xmipptomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_align_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_applyAlignmentTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_coords_roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_crop_resize_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_crop_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_flexalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_half_maps_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_phantom_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_project_top.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resizeTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resize_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_roiIJ.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_score_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_score_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_splitTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_subtomo_map_back.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_subtraction_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_xmipptomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:35:26.773371 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/monotomo_tree_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_phantom_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_score_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-19 08:32:21.000000 scipion-em-xmipptomo-3.23.3.3/xmipptomo/xmipp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.815284 scipion-em-xmipptomo-3.23.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-20 22:01:49.811284 scipion-em-xmipptomo-3.23.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.807284 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 22:01:49.000000 scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:01:49.815284 scipion-em-xmipptomo-3.23.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.807284 scipion-em-xmipptomo-3.23.3.4/xmipptomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.811284 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_align_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_applyAlignmentTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_coords_roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_crop_resize_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_crop_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_flexalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_half_maps_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_phantom_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_project_top.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resizeTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resize_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_roiIJ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_score_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_score_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_splitTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_subtomo_map_back.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_subtraction_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.811284 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_xmipptomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:01:49.811284 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/monotomo_tree_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_phantom_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_score_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-20 22:00:03.000000 scipion-em-xmipptomo-3.23.3.4/xmipptomo/xmipp_logo.png
```

### Comparing `scipion-em-xmipptomo-3.23.3.3/CHANGES.txt` & `scipion-em-xmipptomo-3.23.3.4/CHANGES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+V3.23.03.4:
+ - Mapback waits now when scheduled and not the reference is needed (validation added)
+
 V3.23.03.3:
  - Fit vesicles removed (moved to tomo)
- -
+
 V3.23.03.2:
  - Mapback scales any reference to match the tomogram sampling.
 V3.23.03.1:
  - Subtomo projector compatible with hdf stacks. Test fixed. Projections keep orientation.
 
 V3.23.03.0:
  - New protocol and test extract_subtomos
```

### Comparing `scipion-em-xmipptomo-3.23.3.3/LICENSE` & `scipion-em-xmipptomo-3.23.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/PKG-INFO` & `scipion-em-xmipptomo-3.23.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.3
+Version: 3.23.3.4
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/PKG-INFO` & `scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.3
+Version: 3.23.3.4
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.3/scipion_em_xmipptomo.egg-info/SOURCES.txt` & `scipion-em-xmipptomo-3.23.3.4/scipion_em_xmipptomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/setup.py` & `scipion-em-xmipptomo-3.23.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/__init__.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # **************************************************************************
 import xmipp3
 import subprocess, os
 import pyworkflow.utils as pwutils
 
 _logo = "xmipp_logo.png"
 _references = ['delaRosaTrevin2013']
-__version__ = "3.23.03.3" #X.YY.MM.sv
+__version__ = "3.23.03.4" #X.YY.MM.sv
         # X.Y.M = version of the xmipp release associated.
         # sv = Set this to ".0" on each xmipp  release.
         # For not release version (hotfix) increase it --> ".1", ".2", ...
 
 class Plugin(xmipp3.Plugin):
 
     @classmethod
```

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/bibtex.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/__init__.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_align_transform.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_align_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_applyAlignmentTS.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_applyAlignmentTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_apply_alignment_subtomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_apply_alignment_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_cltomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_connected_components.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_connected_components.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_coords_roi.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_coords_roi.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_crop_resize_base.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_crop_resize_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_crop_tomograms.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_crop_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_extract_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_filter_coordinates_by_map.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_filter_coordinates_by_map.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_flexalign.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_flexalign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_half_maps_subtomos.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_half_maps_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_phantom_tomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_phantom_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_project_top.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_project_top.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resizeTS.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resizeTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resize_tomograms.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resize_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_roiIJ.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_roiIJ.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_score_coordinates.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_score_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_score_transform.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_score_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_splitTS.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_splitTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_subtomo_map_back.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_subtomo_map_back.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
 from tomo.objects import Tomogram, SetOfCoordinates3D, SetOfSubTomograms, SetOfClassesSubTomograms, SubTomogram, \
     MATRIX_CONVERSION, SetOfTomograms
 from tomo.protocols import ProtTomoBase
 from xmipp3.convert import alignmentToRow
 import tomo.constants as const
 
+REFERENCE = 'Reference'
+
 
 # Painting types
 class PAINTING_TYPES:
     COPY=0
     AVERAGE=1
     HIGHLIGHT=2
     BINARIZE=3
@@ -83,15 +85,15 @@
                       condition='selection==0', allowsNull=True,
                       help="Subtomogram class from which the coordinates of the subtomograms and the reference will be "
                            "used. It should be a SetOfClassesSubTomograms with just 1 item.")
         form.addParam('inputSubtomos', PointerParam, pointerClass=[SetOfSubTomograms, SetOfCoordinates3D], label='Subtomograms/coordinates',
                       condition='selection==1', allowsNull=True,
                       help="Subtomograms to be mapped back, they should have alignment and coordinates.")
         form.addParam('inputRef', PointerParam, pointerClass="Volume, SubTomogram, AverageSubTomogram",
-                      label='Reference', condition='selection==1', allowsNull=True,
+                      label=REFERENCE, condition='selection==1', allowsNull=True,
                       help="Subtomogram reference, average, representative or initial model of the subtomograms.")
         form.addParam('inputTomograms', PointerParam, pointerClass="SetOfTomograms",
                       label='Original tomograms', help="Original tomograms from which the subtomograms were extracted", allowsNull=True)
         form.addParam('invertContrast', BooleanParam, default=False, label='Invert reference contrast',
                       help="Invert the contrast if the reference is black over a white background.  Xmipp, Spider, "
                            "Relion and Eman require white particles over a black background. ")
         form.addParam('paintingType', EnumParam,
@@ -338,29 +340,30 @@
         else:
             self._defineSourceRelation(inputTomosSet, outputTomos)
 
     # --------------------------- INFO functions --------------------------------
     def _validate(self):
         validateMsgs = []
         if self._useClasses():
-            for subtomo in self.inputClasses.get().getFirstItem().iterItems():
-                if not subtomo.hasCoordinate3D():
-                    validateMsgs.append('Please provide a class which contains subtomograms with 3D coordinates.')
-                    break
-                if not subtomo.hasTransform():
-                    validateMsgs.append('Please provide a class which contains subtomograms with alignment.')
-                    break
-        elif self._isInputASetOfSubtomograms():
-            subtomo = self.inputSubtomos.get().getFirstItem()
+            subtomo = self.inputClasses.get().getFirstItem().getFirstItem()
             if not subtomo.hasCoordinate3D():
-                validateMsgs.append('Please provide a set of subtomograms which contains subtomograms with 3D '
-                                        'coordinates.')
+                validateMsgs.append('Please provide a class which contains subtomograms with 3D coordinates.')
+
             if not subtomo.hasTransform():
-                validateMsgs.append('Please provide a set of subtomograms which contains subtomograms with '
-                                        'alignment.')
+                validateMsgs.append('Please provide a class which contains subtomograms with alignment.')
+
+        else:
+            if not self.inputRef.get():
+                validateMsgs.append("When using coordinates or subtomograms the %s is mandatory." % REFERENCE)
+
+            if self._isInputASetOfSubtomograms():
+                subtomo = self.inputSubtomos.get().getFirstItem()
+                if not subtomo.hasCoordinate3D():
+                    validateMsgs.append('Please provide a set of subtomograms which contains subtomograms with 3D '
+                                            'coordinates.')
         return validateMsgs
 
     def _summary(self):
         summary = []
         if self._useClasses():
             summary.append("Using a class with its reference.")
         elif self._isInputASetOfSubtomograms():
```

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols/protocol_subtraction_subtomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols/protocol_subtraction_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/protocols.conf` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/__init__.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_extract_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_monotomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_crop.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_crop.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_resize.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/tests/test_protocols_xmipptomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/tests/test_protocols_xmipptomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/utils.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/__init__.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/monotomo_tree_provider.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/monotomo_tree_provider.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_cltomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_phantom_create.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_phantom_create.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/viewers/viewer_score_subtomos.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/viewers/viewer_score_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/wizards.py` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.3/xmipptomo/xmipp_logo.png` & `scipion-em-xmipptomo-3.23.3.4/xmipptomo/xmipp_logo.png`

 * *Files identical despite different names*

