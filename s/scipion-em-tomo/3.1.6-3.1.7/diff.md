# Comparing `tmp/scipion-em-tomo-3.1.6.tar.gz` & `tmp/scipion-em-tomo-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-tomo-3.1.6.tar", last modified: Thu Apr 20 14:35:09 2023, max compression
+gzip compressed data, was "scipion-em-tomo-3.1.7.tar", last modified: Fri Apr 21 09:07:25 2023, max compression
```

## Comparing `scipion-em-tomo-3.1.6.tar` & `scipion-em-tomo-3.1.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.131913 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 14:35:09.000000 scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.131913 scipion-em-tomo-3.1.6/tomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.131913 scipion-em-tomo-3.1.6/tomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/convert/mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    99969 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/tomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_assignTransformationTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_assign_tomo2subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_assign_tomo2tomoMask.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_consensus_classes_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ctf_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_extract_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_fit_ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_coordinates_from_scipion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_tomomasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_misalignTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_particles_to_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_rotate_astigmatism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_split_evenodd_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_tomo_to_mics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_consensus_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_convert_coords3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_correct_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_estimate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    41419 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/tomo/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/HIV-Picking-with-Dynamo.json.template
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/HIV-Reconstruction.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/HIV-Subtomogram-averaging.json.template
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/Membrane picking-with-PySeg.json.template
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/templates/Ribosomes-Subtomogram-averaging.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/tomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_base_centralized_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_compose_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_fit_vesicles.py
--rw-r--r--   0 runner    (1001) docker     (123)    41397 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    43270 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_tomo_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:09.135913 scipion-em-tomo-3.1.6/tomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/viewer_split_evenodd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    40940 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-20 14:30:24.000000 scipion-em-tomo-3.1.6/tomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.681352 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 09:07:25.000000 scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.681352 scipion-em-tomo-3.1.7/tomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.685353 scipion-em-tomo-3.1.7/tomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/convert/mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100531 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.693353 scipion-em-tomo-3.1.7/tomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_assignTransformationTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_assign_tomo2subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_assign_tomo2tomoMask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_consensus_classes_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ctf_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_extract_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_fit_ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_coordinates_from_scipion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_tomomasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_misalignTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_particles_to_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_rotate_astigmatism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_split_evenodd_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_tomo_to_mics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_consensus_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_convert_coords3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_correct_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_estimate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41419 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.693353 scipion-em-tomo-3.1.7/tomo/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/HIV-Picking-with-Dynamo.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/HIV-Reconstruction.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/HIV-Subtomogram-averaging.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/Membrane picking-with-PySeg.json.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/templates/Ribosomes-Subtomogram-averaging.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/tomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_base_centralized_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_compose_TS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_fit_vesicles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41397 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43270 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_tomo_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:25.697353 scipion-em-tomo-3.1.7/tomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/viewer_split_evenodd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40940 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-21 09:01:34.000000 scipion-em-tomo-3.1.7/tomo/wizards.py
```

### Comparing `scipion-em-tomo-3.1.6/LICENSE` & `scipion-em-tomo-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/PKG-INFO` & `scipion-em-tomo-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-tomo
-Version: 3.1.6
+Version: 3.1.7
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
```

### Comparing `scipion-em-tomo-3.1.6/README.rst` & `scipion-em-tomo-3.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/PKG-INFO` & `scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-em-tomo
-Version: 3.1.6
+Version: 3.1.7
 Summary: Plugin to use electron tomography software within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomo
 Author: J.M. De la Rosa, Estrella Fernandez, David Herreros, Adrian Quintana
 Author-email: delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomo/
```

### Comparing `scipion-em-tomo-3.1.6/scipion_em_tomo.egg-info/SOURCES.txt` & `scipion-em-tomo-3.1.7/scipion_em_tomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/setup.py` & `scipion-em-tomo-3.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/__init__.py` & `scipion-em-tomo-3.1.7/tomo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pwem
 
-__version__ = '3.1.6'
+__version__ = '3.1.7'
 _logo = "icon.png"
 _references = []
 
 
 class Plugin(pwem.Plugin):
     @classmethod
     def _defineVariables(cls):
```

### Comparing `scipion-em-tomo-3.1.6/tomo/constants.py` & `scipion-em-tomo-3.1.7/tomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/convert/__init__.py` & `scipion-em-tomo-3.1.7/tomo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/convert/convert.py` & `scipion-em-tomo-3.1.7/tomo/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/convert/mdoc.py` & `scipion-em-tomo-3.1.7/tomo/convert/mdoc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/icon.png` & `scipion-em-tomo-3.1.7/tomo/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/objects.py` & `scipion-em-tomo-3.1.7/tomo/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         return fileName + suffix + fileExtension
 
 
 TS_IGNORE_ATTRS = ['_mapperPath', '_size', '_hasAlignment']
 
 
 class TiltSeriesBase(data.SetOfImages):
-
+    TS_ID_FIELD = '_tsId'
     def __init__(self, **kwargs):
         data.SetOfImages.__init__(self, **kwargs)
         self._tsId = String(kwargs.get('tsId', None))
         # TiltSeries will always be used inside a SetOfTiltSeries
         # so, let's do not store the mapper path by default
         self._mapperPath.setStore(False)
         self._acquisition = TomoAcquisition()
@@ -736,14 +736,20 @@
     def getScannedPixelSize(self):
         mag = self._acquisition.getMagnification()
         return self._samplingRate.get() * 1e-4 * mag
 
     def getTiltSeriesFromTsId(self, tsId):
         return self[{"_tsId": tsId}]
 
+    def getTSIds(self):
+        """ Returns al the Tilt series ids involved in the set."""
+        tsIds = self.aggregate(["MAX"], TiltSeries.TS_ID_FIELD, [TiltSeries.TS_ID_FIELD])
+        tsIds = [d[TiltSeries.TS_ID_FIELD] for d in tsIds]
+        return tsIds
+
 
 class SetOfTiltSeries(SetOfTiltSeriesBase):
     ITEM_TYPE = TiltSeries
 
     def _dimStr(self):
         """ Return the string representing the dimensions. """
 
@@ -1545,14 +1551,21 @@
         return self._tomos
 
     def append(self, item: Coordinate3D):
         if self.getBoxSize() is None and item._boxSize:
             self.setBoxSize(item._boxSize)
         super().append(item)
 
+    def getTSIds(self):
+        """ Returns all the TS ID (tomoId) present in this set"""
+        volIds = self.aggregate(["MAX"], Coordinate3D.TOMO_ID_ATTR, [Coordinate3D.TOMO_ID_ATTR])
+        volIds = [d[Coordinate3D.TOMO_ID_ATTR] for d in volIds]
+        return volIds
+
+
 
 class SubTomogram(data.Volume):
     """The coordinate associated to each subtomogram is not scaled. To do that, the coordinates and the subtomograms
     sampling rates should be compared (because of how the extraction protocol works). But when shifts are applied to
     the coordinates, it has to be considered that if we're operating with coordinates coming from subtomogrmas, those
     shifts will be scaled, but if the coordinates come from coordinates, they won't be."""
```

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/__init__.py` & `scipion-em-tomo-3.1.7/tomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_alignment_assign.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_assignTransformationTS.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_assignTransformationTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_assign_tomo2subtomo.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_assign_tomo2subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_assign_tomo2tomoMask.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_assign_tomo2tomoMask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_base.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_compose_TS.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_compose_TS.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
             time.sleep(self.time4NextMic.get())
             len_mics_input_2 = self._loadInputList()
             if len_mics_input_2 == len_mics_input_1:
                 return False
             len_mics_input_1 = self._loadInputList()
 
         self.info('Tilts in the mdoc file: {}\n'
-                  'Micrographs abailables: {}'.format(
+                  'Micrographs availables: {}'.format(
             len(mdoc_order_angle_list), len(self.listOfMics)))
 
         # MATCH
         list_mdoc_files = [os.path.basename(fp[0]) for fp in mdoc_order_angle_list]
         list_mics_matched = []
         for x, mic in enumerate(self.listOfMics):
             if mic.getMicName() in list_mdoc_files:
```

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_consensus_classes_subtomo.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_consensus_classes_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ctf_validate.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ctf_validate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_extract_coordinates.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_fit_ellipsoid.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_fit_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_coordinates.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_coordinates_from_scipion.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_coordinates_from_scipion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_subtomograms.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_tomograms.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_tomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_import_tomomasks.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_import_tomomasks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_misalignTS.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_misalignTS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_particles_to_subtomograms.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_particles_to_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_rotate_astigmatism.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_rotate_astigmatism.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_split_evenodd_subtomos.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_split_evenodd_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_tomo_to_mics.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_tomo_to_mics.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_base.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_consensus_alignment.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_consensus_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_convert_coords3d.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_convert_coords3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_correct_motion.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_correct_motion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_estimate_ctf.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_estimate_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols/protocol_ts_import.py` & `scipion-em-tomo-3.1.7/tomo/protocols/protocol_ts_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/protocols.conf` & `scipion-em-tomo-3.1.7/tomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/templates/HIV-Picking-with-Dynamo.json.template` & `scipion-em-tomo-3.1.7/tomo/templates/HIV-Picking-with-Dynamo.json.template`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Course 2022, day 2: Non vectorial picking with Dynamo and Eman on HIV (EMPIAR-10164) tomogram
+Non vectorial picking with Dynamo and Eman on HIV (EMPIAR-10164) tomogram
 You'll need to download its dataset -> scipion3 testdata --download tomo-tutorial
 [
     {
         "object.className": "ProtImportTomograms",
         "object.id": "2",
         "object.label": "Tomo Curso",
         "object.comment": "",
```

### Comparing `scipion-em-tomo-3.1.6/tomo/templates/HIV-Reconstruction.json.template` & `scipion-em-tomo-3.1.7/tomo/templates/HIV-Reconstruction.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/templates/HIV-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.1.7/tomo/templates/HIV-Subtomogram-averaging.json.template`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "hostName": "localhost",
         "numberOfThreads": 12,
-        "numberOfMpi": 1,
+        "numberOfMpi": 5,
         "boxSize": 192,
         "croppedBoxSize": 96,
         "binningFactor": 4.0,
         "symmetry": "C6",
         "snrWiener": 0.0,
         "inReParticles": "270.relionParticles"
     },
@@ -307,15 +307,15 @@
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "hostName": "localhost",
         "numberOfThreads": 12,
-        "numberOfMpi": 1,
+        "numberOfMpi": 5,
         "boxSize": 192,
         "croppedBoxSize": 96,
         "binningFactor": 4.0,
         "applyConeWeight": false,
         "coneAngle": 10.0,
         "applyOffsets": false,
         "outputInFloat16": false,
@@ -405,15 +405,15 @@
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "hostName": "localhost",
         "numberOfThreads": 12,
-        "numberOfMpi": 1,
+        "numberOfMpi": 5,
         "boxSize": 192,
         "croppedBoxSize": 96,
         "binningFactor": 4.0,
         "symmetry": "C6",
         "snrWiener": 0.0,
         "inReParticles": "717.relionParticles"
     },
@@ -499,16 +499,16 @@
         "object.comment": "",
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "hostName": "localhost",
-        "numberOfThreads": 20,
-        "numberOfMpi": 1,
+        "numberOfThreads": 12,
+        "numberOfMpi": 5,
         "boxSize": 256,
         "croppedBoxSize": 128,
         "binningFactor": 2.0,
         "symmetry": "C6",
         "snrWiener": 0.0,
         "inReParticles": "924.relionParticles"
     },
@@ -520,15 +520,15 @@
         "_useQueue": false,
         "_prerequisites": "",
         "_queueParams": null,
         "runName": null,
         "runMode": 0,
         "hostName": "localhost",
         "numberOfThreads": 12,
-        "numberOfMpi": 1,
+        "numberOfMpi": 5,
         "boxSize": 256,
         "croppedBoxSize": 128,
         "binningFactor": 2.0,
         "applyConeWeight": false,
         "coneAngle": 10.0,
         "applyOffsets": false,
         "outputInFloat16": false,
```

### Comparing `scipion-em-tomo-3.1.6/tomo/templates/Membrane picking-with-PySeg.json.template` & `scipion-em-tomo-3.1.7/tomo/templates/Membrane picking-with-PySeg.json.template`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Course 2022, day 2: Vectorial picking with PySeg on Mice Intact P19 cells (emd_10439) tomogram.
+Vectorial picking with PySeg on Mice Intact P19 cells (emd_10439) tomogram.
 [
     {
         "object.className": "ProtImportVolumes",
         "object.id": "2",
         "object.label": "Download emd 10439 map",
         "object.comment": "",
         "_useQueue": false,
```

### Comparing `scipion-em-tomo-3.1.6/tomo/templates/Ribosomes-Subtomogram-averaging.json.template` & `scipion-em-tomo-3.1.7/tomo/templates/Ribosomes-Subtomogram-averaging.json.template`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Course 2022, day 3 :Subtomogram averaging on ribosomes (EMPIAR-10045)
+Subtomogram averaging on ribosomes (EMPIAR-10045)
 You'll need to download its dataset -> scipion3 testdata --download tomo-tutorial
 [
     {
         "object.className": "ProtImportTomograms",
         "object.id": "2",
         "object.label": "tomo - import tomograms",
         "object.comment": "",
```

### Comparing `scipion-em-tomo-3.1.6/tomo/tests/__init__.py` & `scipion-em-tomo-3.1.7/tomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/tests/test_base_centralized_layer.py` & `scipion-em-tomo-3.1.7/tomo/tests/test_base_centralized_layer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/tests/test_compose_TS.py` & `scipion-em-tomo-3.1.7/tomo/tests/test_compose_TS.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/tests/test_fit_vesicles.py` & `scipion-em-tomo-3.1.7/tomo/tests/test_fit_vesicles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/tests/test_import.py` & `scipion-em-tomo-3.1.7/tomo/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/tests/test_objects.py` & `scipion-em-tomo-3.1.7/tomo/tests/test_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
         coords.setPrecedents(tomos)
 
         coords.write()
 
         # Test precedents involved
         self.assertEqual(len(coords.getPrecedentsInvolved()), 1, "getPrecedentsInvolved does not seem to work")
 
+        self.assertEqual(coords.getTSIds(), [TS_1], "SetOfCoordinates.getTSIds not working.")
+
         subtomos = SetOfSubTomograms.create(self.outputPath)
         subtomos.setCoordinates3D(coords)
 
         subtomo = SubTomogram()
         subtomo.setCoordinate3D(coord1)
         subtomos.append(subtomo)
 
@@ -143,15 +145,15 @@
     def test_set_of_tilt_series(self):
         """ Tests the SetOfTiltSeries model"""
 
         # Create the set
         tiltseries = SetOfTiltSeries.create(self.outputPath)
         tiltseries.setAnglesCount(3)
         ts = TiltSeries()
-        ts.setTsId("TS1")
+        ts.setTsId(TS_1)
 
         # We need to append the tilt series before adding tilt images
         tiltseries.append(ts)
 
         # Add tilt images
         ti = TiltImage()
         ti.setTiltAngle(-3)
@@ -165,14 +167,16 @@
 
         # Persist the whole set, this should persist properties of the set
         tiltseries.write()
 
         tiltSerieFromFile = SetOfTiltSeries(filename=tiltseries.getFileName())
         tiltSerieFromFile.loadAllProperties()
 
+        self.assertEqual(tiltSerieFromFile.getTSIds(), [TS_1], "SetOfTiltSeries.getTSIds not working.")
+
     def test_landmarks(self):
         """ Test the Landmark model"""
 
         temp_name = next(tempfile._get_candidate_names())
         # Verify the count
         lm = LandmarkModel(fileName=temp_name)
```

### Comparing `scipion-em-tomo-3.1.6/tomo/tests/test_tomo_base.py` & `scipion-em-tomo-3.1.7/tomo/tests/test_tomo_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/tests/test_transformations.py` & `scipion-em-tomo-3.1.7/tomo/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/utils.py` & `scipion-em-tomo-3.1.7/tomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/viewers/__init__.py` & `scipion-em-tomo-3.1.7/tomo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/viewers/viewer_split_evenodd.py` & `scipion-em-tomo-3.1.7/tomo/viewers/viewer_split_evenodd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/viewers/viewers_data.py` & `scipion-em-tomo-3.1.7/tomo/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/viewers/views.py` & `scipion-em-tomo-3.1.7/tomo/viewers/views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/viewers/views_tkinter_tree.py` & `scipion-em-tomo-3.1.7/tomo/viewers/views_tkinter_tree.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomo-3.1.6/tomo/wizards.py` & `scipion-em-tomo-3.1.7/tomo/wizards.py`

 * *Files identical despite different names*

