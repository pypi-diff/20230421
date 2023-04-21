# Comparing `tmp/scipion-em-reliontomo-3.1.4.tar.gz` & `tmp/scipion-em-reliontomo-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-reliontomo-3.1.4.tar", last modified: Thu Apr 20 14:27:22 2023, max compression
+gzip compressed data, was "scipion-em-reliontomo-3.1.5.tar", last modified: Fri Apr 21 08:17:52 2023, max compression
```

## Comparing `scipion-em-reliontomo-3.1.4.tar` & `scipion-em-reliontomo-3.1.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.832166 scipion-em-reliontomo-3.1.4/reliontomo/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.832166 scipion-em-reliontomo-3.1.4/reliontomo/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/cmd/compareStarFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.832166 scipion-em-reliontomo-3.1.4/reliontomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/convert/convert30_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    21665 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/convert/convert40_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/convert/convertBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/reliontomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_3d_classify_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_import_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_per_part_per_tilt.py
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_relion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_ctf_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_de_novo_initial_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_edit_particles_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_import_coordinates_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_import_subtomograms_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_make_pseudo_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_matching_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    17346 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_rec_tomogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_refine_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_tomo_frame_align.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/relion_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/reliontomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/test_compare_star_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/test_import_star_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    33801 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/tests/test_refine_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/reliontomo/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:22.836166 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 14:27:22.000000 scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:27:22.840166 scipion-em-reliontomo-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-20 14:25:25.000000 scipion-em-reliontomo-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.372264 scipion-em-reliontomo-3.1.5/reliontomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.372264 scipion-em-reliontomo-3.1.5/reliontomo/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/cmd/compareStarFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.372264 scipion-em-reliontomo-3.1.5/reliontomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/convert/convert30_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21765 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/convert/convert40_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/convert/convertBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/reliontomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_3d_classify_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_import_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_per_part_per_tilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_relion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_ctf_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_de_novo_initial_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_edit_particles_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_import_coordinates_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_import_subtomograms_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_make_pseudo_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_matching_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_rec_tomogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_refine_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_tomo_frame_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/relion_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/reliontomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/test_compare_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/test_import_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33801 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/tests/test_refine_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/reliontomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 08:17:52.000000 scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:17:52.376264 scipion-em-reliontomo-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-21 08:15:39.000000 scipion-em-reliontomo-3.1.5/setup.py
```

### Comparing `scipion-em-reliontomo-3.1.4/LICENSE` & `scipion-em-reliontomo-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/PKG-INFO` & `scipion-em-reliontomo-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-reliontomo
-Version: 3.1.4
+Version: 3.1.5
 Summary: Plugin to use Relion programs for tomography within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-reliontomo
 Author: CNB-CSIC
 Author-email: jjimenez@cnb.csic.es, scipion-users@lists.sourceforge.net
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-reliontomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-reliontomo/
```

### Comparing `scipion-em-reliontomo-3.1.4/README.rst` & `scipion-em-reliontomo-3.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/__init__.py` & `scipion-em-reliontomo-3.1.5/reliontomo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import pwem
 import relion
 from reliontomo.constants import RELIONTOMO_HOME, RELIONTOMO_DEFAULT, RELION, RELIONTOMO_CUDA_LIB, V4_0
 
 _logo = "relion_logo.png"
 _references = ['Scheres2012a', 'Scheres2012b', 'Kimanius2016', 'Zivanov2018']
-__version__ = '3.1.4'
+__version__ = '3.1.5'
 
 
 class Plugin(relion.Plugin):
     _supportedVersions = [V4_0]
     _homeVar = RELIONTOMO_HOME
     _pathVars = [RELIONTOMO_HOME]
```

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/bibtex.py` & `scipion-em-reliontomo-3.1.5/reliontomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/cmd/compareStarFiles.py` & `scipion-em-reliontomo-3.1.5/reliontomo/cmd/compareStarFiles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/constants.py` & `scipion-em-reliontomo-3.1.5/reliontomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/convert/__init__.py` & `scipion-em-reliontomo-3.1.5/reliontomo/convert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 
 def createWriterTomo40(**kwargs):
     """ Create a new Writer instance for Relion 4."""
     Writer = convert40_tomo.Writer
     return Writer(**kwargs)
 
 
-def writeSetOfCoordinates(coordSet, starFile, **kwargs):
-    return createWriterTomo40().coordinates2Star(coordSet, starFile, **kwargs)
+def writeSetOfCoordinates(coordSet, starFile, whitelist, **kwargs):
+    return createWriterTomo40().coordinates2Star(coordSet, starFile, whitelist, **kwargs)
 
 
 def writeSetOfSubtomograms(particlesSet, starFile, **kwargs):
     """ Convenience function to write a SetOfSubtomograms as Relion metadata using a Writer."""
     writer = createWriterTomo(**kwargs)
     return writer.subtomograms2Star(particlesSet, starFile)
```

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/convert/convert30_tomo.py` & `scipion-em-reliontomo-3.1.5/reliontomo/convert/convert30_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/convert/convert40_tomo.py` & `scipion-em-reliontomo-3.1.5/reliontomo/convert/convert40_tomo.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,23 +76,28 @@
                                self._genCulledFileName(prot, tsId)  # _rlnTomoImportCulledFile #7
                                )
             else:
                 logger.info("Tilt series %s excluded." % tsId)
         # Write the STAR file
         tsTable.write(outStarFileName)
 
-    def coordinates2Star(self, coordSet, subtomosStar, sRate=1, coordsScale=1):
+    def coordinates2Star(self, coordSet, subtomosStar, whitelist, sRate=1, coordsScale=1):
         """Input coordsScale is used to scale the coordinates so they are expressed in bin 1, as expected by Relion 4"""
         tomoTable = Table(columns=self._getCoordinatesStarFileLabels())
         i = 0
         for coord in coordSet.iterCoordinates():
+            tsId = coord.getTomoId()
+
+            if tsId not in whitelist:
+                continue
+
             angles, shifts = getTransformInfoFromCoordOrSubtomo(coord, coordSet.getSamplingRate())
             # Add row to the table which will be used to generate the STAR file
             tomoTable.addRow(
-                coord.getTomoId(),  # 1 _rlnTomoName
+                tsId,  # 1 _rlnTomoName
                 coord.getObjId(),  # 2 _rlnTomoParticleId
                 coord.getGroupId() if coord.getGroupId() else 1,  # 3 _rlnTomoManifoldIndex
                 # coord in pix at scale of bin1
                 coord.getX(RELION_3D_COORD_ORIGIN) * coordsScale,  # 4 _rlnCoordinateX
                 coord.getY(RELION_3D_COORD_ORIGIN) * coordsScale,  # 5 _rlnCoordinateY
                 coord.getZ(RELION_3D_COORD_ORIGIN) * coordsScale,  # 6 _rlnCoordinateZ
                 # pix * Å/pix = [shifts in Å]
```

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/convert/convertBase.py` & `scipion-em-reliontomo-3.1.5/reliontomo/convert/convertBase.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/objects.py` & `scipion-em-reliontomo-3.1.5/reliontomo/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/__init__.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_3d_classify_subtomograms.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_3d_classify_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_import_from_star.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_import_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_per_part_per_tilt.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_per_part_per_tilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_refine.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_base_relion.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_base_relion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_ctf_refine.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_ctf_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_de_novo_initial_model.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_de_novo_initial_model.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_edit_particles_star.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_edit_particles_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_import_coordinates_from_star.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_import_coordinates_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_import_subtomograms_from_star.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_import_subtomograms_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_make_pseudo_subtomos.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_make_pseudo_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_matching_coordinates.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_matching_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_post_process.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_post_process.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_prepare_data.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_prepare_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from pyworkflow.utils import makePath, Message
 from reliontomo import Plugin
 from reliontomo.objects import createSetOfRelionPSubtomograms, RelionSetOfPseudoSubtomograms
 from reliontomo.constants import (IN_TOMOS_STAR, OUT_TOMOS_STAR, IN_COORDS_STAR,
                                   OPTIMISATION_SET_STAR, OUT_PARTICLES_STAR, PSUBTOMOS_SQLITE)
 from reliontomo.convert import writeSetOfTomograms, writeSetOfCoordinates, readSetOfPseudoSubtomograms
 from reliontomo.utils import generateProjections
-from tomo.utils import getNonInterpolatedTsFromRelations
 import tomo.objects as tomoObj
 from tomo.protocols.protocol_base import ProtTomoBase
 
 # Other constants
 DEFOCUS = 'defocus'
 THICKNESS = 'thickness'
 X_SIZE = 'x'
@@ -64,15 +63,15 @@
     _possibleOutputs = outputObjects
 
     def __init__(self, **args):
         EMProtocol.__init__(self, **args)
         self.tsSet = None
         self.tomoSet = None
         self.tsReducedSet = None  # Reduced list of tiltseries with only those in the coordinates
-        self.coordsVolIds = None  # Unique tomogram identifiers volId used in the coordinate set. In case is a subset
+        self.matchingTSIds = None  # Unique tomogram identifiers volId used in the coordinate set. In case is a subset
         self.coordScale = Float(1)
 
     # -------------------------- DEFINE param functions -----------------------
 
     def _defineParams(self, form):
         form.addSection(label=Message.LABEL_INPUT)
 
@@ -140,79 +139,94 @@
 
     # -------------------------- STEPS functions ------------------------------
     def _initialize(self):
         defocusDir = self._getExtraPath(DEFOCUS)
         if not exists(defocusDir):  # It can exist in case of Continue execution
             mkdir(defocusDir)
         self.coords = self.inputCoords.get()
-        self.coordsVolIds = self._getTSIDFromCoordinates()
         self.tsSet = self._getTiltSeriesNonInterpolated()
+
+        # Compute matching TS id among coordinates and tilt series, both could be a subset
+        coordsTsIds = self.coords.getTSIds()
+        self.info("Tilt series present in coordinates are: %s" % coordsTsIds)
+
+        tsIds = self.tsSet.getTSIds()
+        self.info("Tilt series present in Tilt series are: %s" % tsIds)
+
+        # Intersection
+        self.matchingTSIds = set(coordsTsIds).intersection(tsIds)
+        if len(self.matchingTSIds):
+            self.info("Tilt series associated in both, coordinates and tilt series are %s" % self.matchingTSIds)
+        else:
+            raise Exception("There isn't any common tilt series among the coordinates and tilt series chosen.")
+
         self.tomoSet = self.coords.getPrecedents()
         self.inputCtfs = self.inputCtfTs.get()
         # If coordinates are referred to a set of tomograms, they'll be rescaled
         # to be expressed in bin 1, as the ts images
         if self.tomoSet:
             self.coordScale.set(self.tomoSet.getSamplingRate() / self.tsSet.getSamplingRate())
 
-    def _getTiltSeriesNonInterpolated(self):
+    def _getTiltSeriesNonInterpolated(self) ->tomoObj.SetOfTiltSeries:
         return self.inputTS.get() # if self.inputTS.get() is not None else \
             #getNonInterpolatedTsFromRelations(self.inputCoords.get(), self)
 
-    def _getTSIDFromCoordinates(self):
-        # TODO: Add this functionality to the SetOFCoordinates. May be useful for other cases
-        volIds = self.coords.aggregate(["MAX"], "_tomoId", ["_tomoId"])
-        volIds = [d['_tomoId'] for d in volIds]
-        self.info("Involved tomograms in the coordinates: %s" % volIds)
-        return volIds
-
     def convertInputStep(self):
         # Generate defocus files
         for ctfTomo in self.inputCtfs:
+            tsId = ctfTomo.getTsId()
+            if tsId not in self.matchingTSIds:
+                continue
             defocusPath = self._getExtraPath(DEFOCUS, ctfTomo.getTsId())
             if not exists(defocusPath):  # It can exist in case of mode Continue execution
                 mkdir(defocusPath)
             generateDefocusIMODFileFromObject(ctfTomo,
                                               join(defocusPath, ctfTomo.getTsId() + '.' + DEFOCUS),
                                               isRelion=True)
         # Thickness of the tomogram and shifts
         tomoSizeDict = {}
         tomoShiftsDict ={}
         tomoList = [tomo.clone() for tomo in self.coords.getPrecedents()]
         coordScale = self.coordScale.get()
         for tomo in tomoList:
+            tsId = tomo.getTsId()
+            if tsId not in self.matchingTSIds:
+                continue
+
             x, y, thickness = tomo.getDim()
-            tomoSizeDict[tomo.getTsId()] = {X_SIZE: x * coordScale,
+            tomoSizeDict[tsId] = {X_SIZE: x * coordScale,
                                             Y_SIZE: y * coordScale,
                                             THICKNESS: thickness * coordScale}
 
             # Based on this: https://github.com/3dem/relion/blob/ver4.0/src/jaz/tomography/programs/convert_projections.cpp#L368
             # First element is X, second Z!
             shiftsAngs = tomo.getShiftsFromOrigin()
 
             # shifts are stored in Angstrom, we convert to tomo SR and then add the half and the to TS pixel size
             shiftX = int(((shiftsAngs[0] / tomo.getSamplingRate()) + x/2) * self.coordScale.get())
             shiftZ = int(((shiftsAngs[2] / tomo.getSamplingRate()) + thickness/2) * self.coordScale.get())
-            tomoShiftsDict[tomo.getTsId()] = (shiftX, shiftZ)
+            tomoShiftsDict[tsId] = (shiftX, shiftZ)
 
             self.info("Shifts detected for %s are: %s" % (tomo.getTsId(), (shiftX, shiftZ)))
 
         # Simulate the etomo files that serve as entry point to relion4
         self._simulateETomoFiles(self.tsSet, tomoSizeDict, tomoShiftsDict, binned=1, binByFactor=self.coordScale,
-                                 whiteList=self.coordsVolIds, swapDims=self.swapXY.get())
+                                 whiteList=self.matchingTSIds, swapDims=self.swapXY.get())
 
         # Write the tomograms star file
         writeSetOfTomograms(self.tsSet,
                             self._getStarFilename(IN_TOMOS_STAR),
                             prot=self,
                             ctfPlotterParentDir=self._getExtraPath(DEFOCUS),
                             eTomoParentDir=self._getTmpPath(),
-                            whiteList=self.coordsVolIds)
+                            whiteList=self.matchingTSIds)
         # Write the particles star file
         writeSetOfCoordinates(self.inputCoords.get(),
                               self._getStarFilename(IN_COORDS_STAR),
+                              self.matchingTSIds,
                               sRate=self.tsSet.getSamplingRate(),
                               coordsScale=self.coordScale.get())
 
     def relionImportTomograms(self):
         Plugin.runRelionTomo(self, 'relion_tomo_import_tomograms', self._genImportTomosCmd())
 
     def relionImportParticles(self):
@@ -247,14 +261,17 @@
         fiducialModelGaps = self._createSetOfLandmarkModels(suffix='Gaps')
         fiducialModelGaps.copyInfo(self.tsSet)
         fiducialModelGaps.setSetOfTiltSeries(self.inputTS) # Use the pointer better when scheduling
 
         pos = 0
         for ts in self.tsSet:
             tsId = ts.getTsId()
+
+            if tsId not in self.matchingTSIds:
+                continue
             landmarkModelGapsFilePath = os.path.join(self._getExtraPath(),
                                                      str(tsId) + "_gaps.sfid")
 
             landmarkModelGaps = tomoObj.LandmarkModel(tsId=tsId,
                                                       tiltSeriesPointer=ts,
                                                       fileName=landmarkModelGapsFilePath,
                                                       modelName=None,
```

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_rec_tomogram.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_rec_tomogram.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_refine_subtomograms.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_refine_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols/protocol_tomo_frame_align.py` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols/protocol_tomo_frame_align.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/protocols.conf` & `scipion-em-reliontomo-3.1.5/reliontomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/relion_logo.png` & `scipion-em-reliontomo-3.1.5/reliontomo/relion_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/tests/__init__.py` & `scipion-em-reliontomo-3.1.5/reliontomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/tests/test_compare_star_files.py` & `scipion-em-reliontomo-3.1.5/reliontomo/tests/test_compare_star_files.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/tests/test_conversion.py` & `scipion-em-reliontomo-3.1.5/reliontomo/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/tests/test_import_star_files.py` & `scipion-em-reliontomo-3.1.5/reliontomo/tests/test_import_star_files.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/tests/test_refine_cycle.py` & `scipion-em-reliontomo-3.1.5/reliontomo/tests/test_refine_cycle.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/utils.py` & `scipion-em-reliontomo-3.1.5/reliontomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/reliontomo/wizards.py` & `scipion-em-reliontomo-3.1.5/reliontomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/PKG-INFO` & `scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-reliontomo
-Version: 3.1.4
+Version: 3.1.5
 Summary: Plugin to use Relion programs for tomography within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-reliontomo
 Author: CNB-CSIC
 Author-email: jjimenez@cnb.csic.es, scipion-users@lists.sourceforge.net
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-reliontomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-reliontomo/
```

### Comparing `scipion-em-reliontomo-3.1.4/scipion_em_reliontomo.egg-info/SOURCES.txt` & `scipion-em-reliontomo-3.1.5/scipion_em_reliontomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.4/setup.py` & `scipion-em-reliontomo-3.1.5/setup.py`

 * *Files identical despite different names*

