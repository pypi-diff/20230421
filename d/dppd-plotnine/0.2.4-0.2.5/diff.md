# Comparing `tmp/dppd_plotnine-0.2.4.tar.gz` & `tmp/dppd_plotnine-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dppd_plotnine-0.2.4.tar", last modified: Wed Apr 22 07:49:22 2020, max compression
+gzip compressed data, was "dppd_plotnine-0.2.5.tar", last modified: Fri Apr 21 12:38:00 2023, max compression
```

## Comparing `dppd_plotnine-0.2.4.tar` & `dppd_plotnine-0.2.5.tar`

### file list

```diff
@@ -1,97 +1,22 @@
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/
--rw-rw-r--   0 g         (1000) g         (1000)      537 2020-04-22 07:16:36.000000 dppd_plotnine-0.2.4/.gitignore
--rw-rw-r--   0 g         (1000) g         (1000)      561 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/.hgignore
--rw-rw-r--   0 g         (1000) g         (1000)       93 2020-04-22 07:16:36.000000 dppd_plotnine-0.2.4/.readthedocs.yml
--rw-rw-r--   0 g         (1000) g         (1000)     1646 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/.travis.yml
--rw-rw-r--   0 g         (1000) g         (1000)       95 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/AUTHORS.rst
--rw-rw-r--   0 g         (1000) g         (1000)      746 2020-04-22 07:49:05.000000 dppd_plotnine-0.2.4/CHANGELOG.rst
--rw-rw-r--   0 g         (1000) g         (1000)     1086 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/LICENSE.txt
--rw-rw-r--   0 g         (1000) g         (1000)     2544 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)     1629 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/README.md
--rwxrwxr-x   0 g         (1000) g         (1000)      422 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/accept_generated_images.py
--rw-rw-r--   0 g         (1000) g         (1000)      934 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/autobuild_docs.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/docs/
--rw-rw-r--   0 g         (1000) g         (1000)     7610 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/Makefile
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/docs/_static/
--rw-rw-r--   0 g         (1000) g         (1000)       18 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/_static/.gitignore
--rw-rw-r--   0 g         (1000) g         (1000)    15516 2020-04-22 07:46:08.000000 dppd_plotnine-0.2.4/docs/_static/index.png
--rw-rw-r--   0 g         (1000) g         (1000)      281 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/_static/my-styles.css
--rw-rw-r--   0 g         (1000) g         (1000)     2448 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/aes.md
--rw-rw-r--   0 g         (1000) g         (1000)       41 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/authors.rst
--rw-rw-r--   0 g         (1000) g         (1000)       43 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/changelog.rst
--rw-rw-r--   0 g         (1000) g         (1000)    10384 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/conf.py
--rw-rw-r--   0 g         (1000) g         (1000)     2675 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/index.rst
--rw-rw-r--   0 g         (1000) g         (1000)       67 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/license.rst
--rw-rw-r--   0 g         (1000) g         (1000)       36 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/docs/requirements.txt
--rw-rw-r--   0 g         (1000) g         (1000)     1529 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/setup.cfg
--rw-rw-r--   0 g         (1000) g         (1000)      569 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/setup.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine/
--rw-rw-r--   0 g         (1000) g         (1000)      169 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/src/dppd_plotnine/__init__.py
--rw-rw-r--   0 g         (1000) g         (1000)     6417 2020-04-22 07:20:52.000000 dppd_plotnine-0.2.4/src/dppd_plotnine/dppd_plotnine.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine/geoms/
--rw-rw-r--   0 g         (1000) g         (1000)       74 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/src/dppd_plotnine/geoms/__init__.py
--rw-rw-r--   0 g         (1000) g         (1000)     3965 2020-04-22 07:44:54.000000 dppd_plotnine-0.2.4/src/dppd_plotnine/geoms/annotation_stripes_dppd.py
--rw-rw-r--   0 g         (1000) g         (1000)    13329 2020-04-22 07:25:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine/plotnine_extensions.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine.egg-info/
--rw-rw-r--   0 g         (1000) g         (1000)     2544 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine.egg-info/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)     3839 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine.egg-info/SOURCES.txt
--rw-rw-r--   0 g         (1000) g         (1000)        1 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine.egg-info/dependency_links.txt
--rw-rw-r--   0 g         (1000) g         (1000)        1 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/src/dppd_plotnine.egg-info/not-zip-safe
--rw-rw-r--   0 g         (1000) g         (1000)      118 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine.egg-info/requires.txt
--rw-rw-r--   0 g         (1000) g         (1000)       14 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/src/dppd_plotnine.egg-info/top_level.txt
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/tests/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/tests/baseline_images/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_annotations/
--rw-rw-r--   0 g         (1000) g         (1000)     8461 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_annotations/test_annotation_strips.png
--rw-rw-r--   0 g         (1000) g         (1000)     8153 2020-04-22 07:45:53.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_annotations/test_annotation_strips_coord_flip.png
--rw-rw-r--   0 g         (1000) g         (1000)     7569 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_annotations/test_annotation_strips_horiontal.png
--rw-rw-r--   0 g         (1000) g         (1000)     8121 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_annotations/test_annotation_strips_horiontal_coord_flip.png
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/
--rw-rw-r--   0 g         (1000) g         (1000)     4724 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_bar_identity_stat_default.png
--rw-rw-r--   0 g         (1000) g         (1000)     5549 2020-04-22 07:23:43.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_chained-failed-diff.png
--rw-rw-r--   0 g         (1000) g         (1000)    14513 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_chained.png
--rw-rw-r--   0 g         (1000) g         (1000)     6072 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_coord_flip.png
--rw-rw-r--   0 g         (1000) g         (1000)     5445 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_default_order.png
--rw-rw-r--   0 g         (1000) g         (1000)     7626 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_expression_outside_variables.png
--rw-rw-r--   0 g         (1000) g         (1000)     7002 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_expression_vs_column.png
--rw-rw-r--   0 g         (1000) g         (1000)     8384 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_facet_wrap.png
--rw-rw-r--   0 g         (1000) g         (1000)     9891 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_hline.png
--rw-rw-r--   0 g         (1000) g         (1000)     6325 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_mapped_data_as_all_scalar.png
--rw-rw-r--   0 g         (1000) g         (1000)     5740 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_mapped_data_as_list.png
--rw-rw-r--   0 g         (1000) g         (1000)     5713 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_mapped_data_as_list_mixing_unmapped_scalar.png
--rw-rw-r--   0 g         (1000) g         (1000)     5713 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_mapped_data_as_list_unmapped.png
--rw-rw-r--   0 g         (1000) g         (1000)     5808 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_passing_in_lists.png
--rw-rw-r--   0 g         (1000) g         (1000)     5299 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_passing_in_scalar.png
--rw-rw-r--   0 g         (1000) g         (1000)     9525 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_scale.png
--rw-rw-r--   0 g         (1000) g         (1000)     6326 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_scatter.png
--rw-rw-r--   0 g         (1000) g         (1000)     8405 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_simple.png
--rw-rw-r--   0 g         (1000) g         (1000)     8405 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_simple_add.png
--rw-rw-r--   0 g         (1000) g         (1000)     5185 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_stat_count.png
--rw-rw-r--   0 g         (1000) g         (1000)     6567 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_theme_bw.png
--rw-rw-r--   0 g         (1000) g         (1000)     7869 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_title.png
--rw-rw-r--   0 g         (1000) g         (1000)     9884 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_unmapped.png
--rw-rw-r--   0 g         (1000) g         (1000)     5674 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_dppd_plotnine/test_unmapped_list.png
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2020-04-22 07:49:22.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/
--rw-rw-r--   0 g         (1000) g         (1000)     7905 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_axis_ticks.png
--rw-rw-r--   0 g         (1000) g         (1000)     8027 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_axis_ticks_x.png
--rw-rw-r--   0 g         (1000) g         (1000)     7900 2020-04-22 07:23:43.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_axis_ticks_y-failed-diff.png
--rw-rw-r--   0 g         (1000) g         (1000)     7941 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_axis_ticks_y.png
--rw-rw-r--   0 g         (1000) g         (1000)     7595 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_background.png
--rw-rw-r--   0 g         (1000) g         (1000)     7306 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_facet_labels.png
--rw-rw-r--   0 g         (1000) g         (1000)     6621 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_x_axis_labels.png
--rw-rw-r--   0 g         (1000) g         (1000)     7601 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_x_axis_title.png
--rw-rw-r--   0 g         (1000) g         (1000)     5470 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_y_axis_labels.png
--rw-rw-r--   0 g         (1000) g         (1000)     7765 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_hide_y_axis_title.png
--rw-rw-r--   0 g         (1000) g         (1000)     7107 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_reverse_transform.png
--rw-rw-r--   0 g         (1000) g         (1000)     8256 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_scale_color_many_categories.png
--rw-rw-r--   0 g         (1000) g         (1000)     6136 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_scale_fill_many_categories.png
--rw-rw-r--   0 g         (1000) g         (1000)     8469 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_turn_x_axis_labels.png
--rw-rw-r--   0 g         (1000) g         (1000)     8465 2020-04-22 07:37:26.000000 dppd_plotnine-0.2.4/tests/baseline_images/test_extensions/test_turn_y_axis_labels.png
--rw-rw-r--   0 g         (1000) g         (1000)     1670 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/tests/conftest.py
--rw-rw-r--   0 g         (1000) g         (1000)     1635 2020-04-22 07:42:07.000000 dppd_plotnine-0.2.4/tests/test_annotations.py
--rw-rw-r--   0 g         (1000) g         (1000)     7015 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/tests/test_dppd_plotnine.py
--rw-rw-r--   0 g         (1000) g         (1000)     2853 2020-04-22 07:19:55.000000 dppd_plotnine-0.2.4/tests/test_extensions.py
--rw-rw-r--   0 g         (1000) g         (1000)      413 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/tests/test_flake8.py
--rw-rw-r--   0 g         (1000) g         (1000)      288 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/tests/test_other.py
--rw-rw-r--   0 g         (1000) g         (1000)      114 2020-04-22 07:16:35.000000 dppd_plotnine-0.2.4/tox.ini
+drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.532075 dppd_plotnine-0.2.5/
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)       95 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/AUTHORS.rst
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)     1086 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/LICENSE.txt
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)     2105 2023-04-21 12:38:00.532075 dppd_plotnine-0.2.5/PKG-INFO
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)     1629 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/README.md
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)     1435 2023-04-21 12:38:00.533075 dppd_plotnine-0.2.5/setup.cfg
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)      398 2023-04-21 12:36:22.000000 dppd_plotnine-0.2.5/setup.py
+drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.529075 dppd_plotnine-0.2.5/src/
+drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.530075 dppd_plotnine-0.2.5/src/dppd_plotnine/
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)      169 2023-04-21 12:36:43.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/__init__.py
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)     6406 2023-04-21 12:35:55.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/dppd_plotnine.py
+drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.532075 dppd_plotnine-0.2.5/src/dppd_plotnine/geoms/
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)       74 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/geoms/__init__.py
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)     3907 2023-04-21 12:34:54.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/geoms/annotation_stripes_dppd.py
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)    13552 2023-04-21 12:35:55.000000 dppd_plotnine-0.2.5/src/dppd_plotnine/plotnine_extensions.py
+drwxr-xr-x   0 finkernagel  (1001) zti       (2000)        0 2023-04-21 12:38:00.531075 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)     2105 2023-04-21 12:37:59.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/PKG-INFO
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)      489 2023-04-21 12:38:00.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/SOURCES.txt
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)        1 2023-04-21 12:38:00.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/dependency_links.txt
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)        1 2023-04-21 12:37:59.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/not-zip-safe
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)      118 2023-04-21 12:38:00.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/requires.txt
+-rw-r--r--   0 finkernagel  (1001) zti       (2000)       14 2023-04-21 12:38:00.000000 dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dppd_plotnine-0.2.4/LICENSE.txt` & `dppd_plotnine-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dppd_plotnine-0.2.4/PKG-INFO` & `dppd_plotnine-0.2.5/src/dppd_plotnine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 Metadata-Version: 2.1
-Name: dppd_plotnine
-Version: 0.2.4
+Name: dppd-plotnine
+Version: 0.2.5
 Summary: Combines plotnine and dppd
 Home-page: https://github.com/TyberiusPrime/dppd_plotnine
 Author: Florian Finkernagel
 Author-email: finkernagel@imt.uni-marburg.de
 License: mit
-Description: # dppd_plotnine
-        
-        | Build status: | [![Build Status](https://travis-ci.com/TyberiusPrime/dppd_plotnine.svg?branch=master)](https://travis-ci.com/TyberiusPrime/dppd_plotnine)|
-        |---------------|-----------------------------------------------------------------------------|
-        | Documentation | https://dppd_plotnine.readthedocs.io/en/latest/
-        
-        dppd_plotnine combines the power of
-        [plotnine](https://plotnine.readthedocs.io/en/stable) and
-        [dppd](https://dppd.readthedocs.io/en/latest/)
-        
-        It allows you to use code like this
-        
-        
-        ```python
-           import numpy as np
-           from dppd import dppd
-           import dppd_plotnine
-           from plotnine.data import mtcars
-           import plotnine as p9
-           dp, X = dppd()
-        
-           plot = (
-              dp(mtcars)
-              .assign(kwh=X.hp * 0.74)
-              .categorize("cyl")
-              .p9()
-              .add_point(
-                    "cyl",
-                    "kwh",
-                    color="cyl",
-                    position=p9.position_jitter(height=0, random_state=500),
-              )
-              .add_errorbar(
-                    x="cyl",
-                    y="kwh_median",
-                    ymin="kwh_median",
-                    ymax="kwh_median",
-                    data=dp(X.data)
-                    .groupby("cyl")
-                    .summarize(("kwh", np.median, "kwh_median"))
-                    .pd,
-              )
-              .scale_color_manual(
-                    ["red", "blue", "purple"]
-              )  # after pd, X is what it was before
-              .pd
-            )
-            plot.save("test.png")
-            
-        
-        ```
-        
-        ![Example
-        image](https://github.com/TyberiusPrime/dppd_plotnine/raw/master/docs/_static/index.png)
-        
-        Please see our full documentation at https://dppd_plotnine.readthedocs.io/en/latest/
-        for more details of the straight and enhanced plotnine mappings available.
-        
-        
-        
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: doc
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+# dppd_plotnine
+
+| Build status: | [![Build Status](https://travis-ci.com/TyberiusPrime/dppd_plotnine.svg?branch=master)](https://travis-ci.com/TyberiusPrime/dppd_plotnine)|
+|---------------|-----------------------------------------------------------------------------|
+| Documentation | https://dppd_plotnine.readthedocs.io/en/latest/
+
+dppd_plotnine combines the power of
+[plotnine](https://plotnine.readthedocs.io/en/stable) and
+[dppd](https://dppd.readthedocs.io/en/latest/)
+
+It allows you to use code like this
+
+
+```python
+   import numpy as np
+   from dppd import dppd
+   import dppd_plotnine
+   from plotnine.data import mtcars
+   import plotnine as p9
+   dp, X = dppd()
+
+   plot = (
+      dp(mtcars)
+      .assign(kwh=X.hp * 0.74)
+      .categorize("cyl")
+      .p9()
+      .add_point(
+            "cyl",
+            "kwh",
+            color="cyl",
+            position=p9.position_jitter(height=0, random_state=500),
+      )
+      .add_errorbar(
+            x="cyl",
+            y="kwh_median",
+            ymin="kwh_median",
+            ymax="kwh_median",
+            data=dp(X.data)
+            .groupby("cyl")
+            .summarize(("kwh", np.median, "kwh_median"))
+            .pd,
+      )
+      .scale_color_manual(
+            ["red", "blue", "purple"]
+      )  # after pd, X is what it was before
+      .pd
+    )
+    plot.save("test.png")
+    
+
+```
+
+![Example
+image](https://github.com/TyberiusPrime/dppd_plotnine/raw/master/docs/_static/index.png)
+
+Please see our full documentation at https://dppd_plotnine.readthedocs.io/en/latest/
+for more details of the straight and enhanced plotnine mappings available.
+
+
+
+
+
```

### Comparing `dppd_plotnine-0.2.4/README.md` & `dppd_plotnine-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dppd_plotnine-0.2.4/setup.cfg` & `dppd_plotnine-0.2.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = dppd_plotnine
 description = Combines plotnine and dppd
 author = Florian Finkernagel
 author-email = finkernagel@imt.uni-marburg.de
-version = 0.2.4
+version = 0.2.5
 license = mit
 url = https://github.com/TyberiusPrime/dppd_plotnine
 long-description = file: README.md
 long_description_content_type = text/markdown
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
@@ -15,15 +15,14 @@
 
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
-setup_requires = pyscaffold>=3.1a0,<3.2a0
 install_requires = 
 	plotnine
 	dppd
 
 [options.packages.find]
 where = src
 exclude = 
@@ -82,15 +81,11 @@
 exclude = 
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
 
-[pyscaffold]
-version = 3.1
-package = dppd_plotnine
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dppd_plotnine-0.2.4/src/dppd_plotnine/dppd_plotnine.py` & `dppd_plotnine-0.2.5/src/dppd_plotnine/dppd_plotnine.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 @register_verb("p9", types=pd.DataFrame)
 def p9_DataFrame(df, mapping=None):
     return p9.ggplot(mapping=mapping, data=df, environment=EvalEnvironment.capture(2))
 
 
 never_map = set(["data", "stat", "position"])
-other_args = set(["DEFAULT_AES"])
+other_args = set(['DEFAULT_AES'])
 
 add_funcs = {}
 
 
 def sensible_aes_order(required_aes):
     order = []
     if "x" in required_aes:
@@ -27,14 +27,17 @@
         order.append("y")
     for a in sorted(required_aes):
         if a != "x" and a != "y":
             order.append(a)
     return order
 
 
+
+
+
 def iter_elements():
     for name in dir(p9):
         if "_" in name and name[: name.find("_")] in (
             "geom",
             "annotate",
             "annotation",
             "scale",
@@ -51,15 +54,15 @@
 
 
 aliases = {
     "scale_y_continuous": ["syc"],
     "scale_x_continuous": ["sxc"],
 }
 
-for name, cls in iter_elements():  # noqa: C901
+for name, cls in iter_elements():
 
     if name in aliases:
         register_name = aliases[name] + [name]
     else:
         register_name = name
 
     @register_verb(register_name, types=p9.ggplot)
@@ -123,17 +126,17 @@
                     else:
                         raise
 
                 mapped = {k: k for k in cls.REQUIRED_AES if k in mapped}
                 non_mapped["data"] = data
 
             geom = cls(p9.aes(**mapped), **non_mapped)
-            if "DEFAULT_AES" in other:
+            if 'DEFAULT_AES' in other:
                 geom.DEFAULT_AES = geom.DEFAULT_AES.copy()
-                geom.DEFAULT_AES.update(other["DEFAULT_AES"])
+                geom.DEFAULT_AES.update(other['DEFAULT_AES'])
             return plot + geom
 
         add_funcs[add_name] = add_add_geom
 
 
 @register_verb(["save", "render"], types=p9.ggplot)
 def save(plot, *args, **kwargs):
```

### Comparing `dppd_plotnine-0.2.4/src/dppd_plotnine/plotnine_extensions.py` & `dppd_plotnine-0.2.5/src/dppd_plotnine/plotnine_extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,21 +62,21 @@
 
 @register_verb(types=p9.ggplot)
 def hide_axis_ticks(plot):
     """Hide the ticks on both axis"""
     return _change_theme(plot, "axis_ticks", p9.element_blank())
 
 
-@register_verb(['hide_x_axis_ticks', 'hide_axis_ticks_x'], types=p9.ggplot)
+@register_verb(types=p9.ggplot)
 def hide_x_axis_ticks(plot):
     """Hide the ticks on the X axis"""
     return _change_theme(plot, "axis_ticks_major_x", p9.element_blank())
 
 
-@register_verb(['hide_y_axis_ticks', 'hide_axis_ticks_y'], types=p9.ggplot)
+@register_verb(types=p9.ggplot)
 def hide_y_axis_ticks(plot):
     """Hide the ticks on the Y axis"""
     return _change_theme(plot, "axis_ticks_major_y", p9.element_blank())
 
 
 @register_verb(types=p9.ggplot)
 def hide_x_axis_title(plot):
@@ -92,14 +92,19 @@
 
 @register_verb(types=p9.ggplot)
 def hide_facet_labels(plot):
     """Hide the facet labels"""
     _change_theme(plot, "strip_background", p9.element_blank())
     return _change_theme(plot, "strip_text_x", p9.element_blank())
 
+@register_verb(types=p9.ggplot)
+def hide_legend_title(plot):
+    """Hide the legend label"""
+    return _change_theme(plot, "legend_title", p9.element_blank())
+
 
 _many_cat_colors = [
     "#1C86EE",
     "#E31A1C",  # red
     "#008B00",
     "#6A3D9A",  # purple
     "#FF7F00",  # orange
@@ -271,14 +276,17 @@
     plot.layers._org_compute_aesthetics = plot.layers.compute_aesthetics
     # advanced monkey patching for the win!
     plot.layers.compute_aesthetics = types.MethodType(
         my_compute_aesthetics, plot.layers
     )
     return plot
 
+@register_verb('sc10', types=p9.ggplot)
+def sc10(plot):
+    return plot + p9.scale_x_continuous(trans='log10') + p9.scale_y_continuous(trans='log10')
 
 @register_verb("sxc10", types=p9.ggplot)
 def sxc10(plot, *args, **kwargs):
     """scale_x_continuous(trans='log10',...)"""
     if not "trans" in kwargs:
         kwargs["trans"] = "log10"
     return plot + p9.scale_x_continuous(*args, **kwargs)
```

### Comparing `dppd_plotnine-0.2.4/src/dppd_plotnine.egg-info/PKG-INFO` & `dppd_plotnine-0.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 Metadata-Version: 2.1
-Name: dppd-plotnine
-Version: 0.2.4
+Name: dppd_plotnine
+Version: 0.2.5
 Summary: Combines plotnine and dppd
 Home-page: https://github.com/TyberiusPrime/dppd_plotnine
 Author: Florian Finkernagel
 Author-email: finkernagel@imt.uni-marburg.de
 License: mit
-Description: # dppd_plotnine
-        
-        | Build status: | [![Build Status](https://travis-ci.com/TyberiusPrime/dppd_plotnine.svg?branch=master)](https://travis-ci.com/TyberiusPrime/dppd_plotnine)|
-        |---------------|-----------------------------------------------------------------------------|
-        | Documentation | https://dppd_plotnine.readthedocs.io/en/latest/
-        
-        dppd_plotnine combines the power of
-        [plotnine](https://plotnine.readthedocs.io/en/stable) and
-        [dppd](https://dppd.readthedocs.io/en/latest/)
-        
-        It allows you to use code like this
-        
-        
-        ```python
-           import numpy as np
-           from dppd import dppd
-           import dppd_plotnine
-           from plotnine.data import mtcars
-           import plotnine as p9
-           dp, X = dppd()
-        
-           plot = (
-              dp(mtcars)
-              .assign(kwh=X.hp * 0.74)
-              .categorize("cyl")
-              .p9()
-              .add_point(
-                    "cyl",
-                    "kwh",
-                    color="cyl",
-                    position=p9.position_jitter(height=0, random_state=500),
-              )
-              .add_errorbar(
-                    x="cyl",
-                    y="kwh_median",
-                    ymin="kwh_median",
-                    ymax="kwh_median",
-                    data=dp(X.data)
-                    .groupby("cyl")
-                    .summarize(("kwh", np.median, "kwh_median"))
-                    .pd,
-              )
-              .scale_color_manual(
-                    ["red", "blue", "purple"]
-              )  # after pd, X is what it was before
-              .pd
-            )
-            plot.save("test.png")
-            
-        
-        ```
-        
-        ![Example
-        image](https://github.com/TyberiusPrime/dppd_plotnine/raw/master/docs/_static/index.png)
-        
-        Please see our full documentation at https://dppd_plotnine.readthedocs.io/en/latest/
-        for more details of the straight and enhanced plotnine mappings available.
-        
-        
-        
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: doc
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+# dppd_plotnine
+
+| Build status: | [![Build Status](https://travis-ci.com/TyberiusPrime/dppd_plotnine.svg?branch=master)](https://travis-ci.com/TyberiusPrime/dppd_plotnine)|
+|---------------|-----------------------------------------------------------------------------|
+| Documentation | https://dppd_plotnine.readthedocs.io/en/latest/
+
+dppd_plotnine combines the power of
+[plotnine](https://plotnine.readthedocs.io/en/stable) and
+[dppd](https://dppd.readthedocs.io/en/latest/)
+
+It allows you to use code like this
+
+
+```python
+   import numpy as np
+   from dppd import dppd
+   import dppd_plotnine
+   from plotnine.data import mtcars
+   import plotnine as p9
+   dp, X = dppd()
+
+   plot = (
+      dp(mtcars)
+      .assign(kwh=X.hp * 0.74)
+      .categorize("cyl")
+      .p9()
+      .add_point(
+            "cyl",
+            "kwh",
+            color="cyl",
+            position=p9.position_jitter(height=0, random_state=500),
+      )
+      .add_errorbar(
+            x="cyl",
+            y="kwh_median",
+            ymin="kwh_median",
+            ymax="kwh_median",
+            data=dp(X.data)
+            .groupby("cyl")
+            .summarize(("kwh", np.median, "kwh_median"))
+            .pd,
+      )
+      .scale_color_manual(
+            ["red", "blue", "purple"]
+      )  # after pd, X is what it was before
+      .pd
+    )
+    plot.save("test.png")
+    
+
+```
+
+![Example
+image](https://github.com/TyberiusPrime/dppd_plotnine/raw/master/docs/_static/index.png)
+
+Please see our full documentation at https://dppd_plotnine.readthedocs.io/en/latest/
+for more details of the straight and enhanced plotnine mappings available.
+
+
+
+
+
```

