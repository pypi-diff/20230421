# Comparing `tmp/Simba-UW-tf-dev-1.56.9.tar.gz` & `tmp/Simba-UW-tf-dev-1.57.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.9.tar", last modified: Thu Apr 20 01:49:27 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.2.tar", last modified: Fri Apr 21 19:35:06 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.56.9.tar` & `Simba-UW-tf-dev-1.57.2.tar`

### file list

```diff
@@ -1,393 +1,394 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/
--rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.56.9/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.9/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11585 2023-04-19 14:00:17.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     3364 2023-04-20 00:29:41.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-19 14:11:27.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7088 2023-04-19 15:24:28.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5375 2023-04-19 17:04:26.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-19 18:57:16.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)    10253 2023-04-19 15:20:53.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    43774 2023-04-20 00:55:59.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2267 2023-04-19 15:23:44.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)     8383 2023-04-19 19:54:15.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.56.9/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.56.9/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-19 18:06:57.000000 Simba-UW-tf-dev-1.56.9/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-18 15:20:17.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.9/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.9/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.9/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8217 2023-04-18 15:24:14.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.56.9/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.56.9/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.9/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.56.9/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.9/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.9/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.9/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.9/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.9/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.56.9/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.9/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.9/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    47110 2023-04-20 01:48:23.000000 Simba-UW-tf-dev-1.56.9/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.9/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.9/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.9/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.56.9/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.9/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.9/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9874 2023-04-14 13:15:44.000000 Simba-UW-tf-dev-1.56.9/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.9/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.9/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.9/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.9/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56935 2023-04-18 14:46:46.000000 Simba-UW-tf-dev-1.56.9/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.9/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.56.9/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.9/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.9/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.9/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    64354 2023-04-13 18:53:02.000000 Simba-UW-tf-dev-1.56.9/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-18 15:20:17.000000 Simba-UW-tf-dev-1.56.9/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.9/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.9/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.56.9/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     8101 2023-04-15 18:49:21.000000 Simba-UW-tf-dev-1.56.9/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.9/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.56.9/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.9/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.9/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.9/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.9/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13424 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.9/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.9/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.9/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-20 01:49:18.000000 Simba-UW-tf-dev-1.56.9/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-20 01:49:27.000000 Simba-UW-tf-dev-1.56.9/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.57.2/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.2/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11938 2023-04-20 14:29:24.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     3354 2023-04-20 14:05:40.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-20 13:38:50.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7569 2023-04-20 15:20:31.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4812 2023-04-20 14:48:41.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-20 15:04:13.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9907 2023-04-20 12:55:14.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41552 2023-04-20 14:49:52.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2331 2023-04-20 12:56:44.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)     8421 2023-04-20 13:33:19.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.57.2/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-20 15:30:01.000000 Simba-UW-tf-dev-1.57.2/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     1959 2023-04-20 20:07:38.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    26890 2023-04-20 18:25:40.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-21 18:44:23.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.2/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.2/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.57.2/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8292 2023-04-21 12:36:21.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.57.2/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.2/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.57.2/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.57.2/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.2/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.2/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.2/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.57.2/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.57.2/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.57.2/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.2/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    47395 2023-04-20 01:59:56.000000 Simba-UW-tf-dev-1.57.2/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.2/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.57.2/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.2/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.57.2/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.57.2/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.57.2/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    10872 2023-04-21 16:14:46.000000 Simba-UW-tf-dev-1.57.2/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.57.2/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.57.2/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.57.2/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.57.2/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56353 2023-04-20 15:18:16.000000 Simba-UW-tf-dev-1.57.2/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.57.2/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.57.2/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.2/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    19358 2023-04-21 19:25:08.000000 Simba-UW-tf-dev-1.57.2/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64335 2023-04-21 19:27:47.000000 Simba-UW-tf-dev-1.57.2/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-21 16:17:45.000000 Simba-UW-tf-dev-1.57.2/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.57.2/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     9460 2023-04-21 14:18:35.000000 Simba-UW-tf-dev-1.57.2/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.57.2/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.57.2/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.2/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13500 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.2/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.2/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.2/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-21 19:34:57.000000 Simba-UW-tf-dev-1.57.2/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.56.9/PKG-INFO` & `Simba-UW-tf-dev-1.57.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.9
+Version: 1.57.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/video_processing.py` & `Simba-UW-tf-dev-1.57.2/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/dbcv_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os.path
 import pandas as pd
-from simba.unsupervised.misc import check_directory_exists
+from simba.train_model_functions import check_if_dir_exists
 from simba.misc_tools import SimbaTimer, check_file_exist_and_readable
 import numpy as np
 from numba import jit, prange
 from numba.typed import List
 from scipy.sparse.csgraph import minimum_spanning_tree
 from scipy.sparse import csgraph
 from simba.unsupervised.enums import Unsupervised, Clustering
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 from simba.mixins.config_reader import ConfigReader
-from simba.utils.printing import stdout_success
+from simba.utils.printing import stdout_success, stdout_warning
 
 
 CLUSTERER_NAME = 'CLUSTERER_NAME'
 CLUSTER_COUNT = 'CLUSTER_COUNT'
 EMBEDDER_NAME = 'EMBEDDER_NAME'
 DBCV = 'DBCV'
 
@@ -50,15 +50,15 @@
     def __init__(self,
                  config_path: str,
                  data_path: str):
 
         ConfigReader.__init__(self, config_path=config_path)
         UnsupervisedMixin.__init__(self)
         if os.path.isdir(data_path):
-            check_directory_exists(data_path)
+            check_if_dir_exists(in_dir=data_path)
             self.data = self.read_pickle(data_path=data_path)
         else:
             check_file_exist_and_readable(file_path=data_path)
             self.data = {0: self.read_pickle(data_path=data_path)}
         self.save_path = os.path.join(self.logs_path, f'DBCV_{self.datetime}.xlsx')
         with pd.ExcelWriter(self.save_path, mode='w') as writer:
             pd.DataFrame().to_excel(writer, sheet_name=' ', index=True)
@@ -75,18 +75,22 @@
             cluster_lbls = v[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value].labels_
             x = v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_
             self.results[k] = {**self.results[k], **v[Clustering.CLUSTER_MODEL.value][Unsupervised.PARAMETERS.value], **v[Unsupervised.DR_MODEL.value][Unsupervised.PARAMETERS.value]}
             cluster_cnt = self.get_cluster_cnt(data=cluster_lbls, clusterer_name=v[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value], minimum_clusters=1)
 
             if cluster_cnt > 1:
                 dbcv_results = self.DBCV(x, cluster_lbls)
+            else:
+                stdout_warning(msg=f'No DBCV calculated for clusterer {self.results[k][CLUSTERER_NAME]}: Less than two clusters identified.')
             self.results[k] = {**self.results[k], **{DBCV: dbcv_results}, **{CLUSTER_COUNT: cluster_cnt}}
             model_timer.stop_timer()
             stdout_success(msg=f"DBCV complete for model {self.results[k][CLUSTERER_NAME]}", elapsed_time=model_timer.elapsed_time_str)
         self.__save_results()
+        self.timer.stop_timer()
+        stdout_success(msg=f"ALL DBCV calculations complete and saved in {self.save_path}", elapsed_time=self.timer.elapsed_time_str)
 
     def __save_results(self):
         for k, v in self.results.items():
             df = pd.DataFrame.from_dict(v, orient='index', columns=['VALUE'])
             with pd.ExcelWriter(self.save_path, mode='a') as writer:
                 df.to_excel(writer, sheet_name=v[CLUSTERER_NAME], index=True)
 
@@ -271,11 +275,11 @@
     @jit(nopython=True)
     def _cluster_density_sparseness(MST, labels, cluster):
         indices = np.where(labels == cluster)[0]
         cluster_MST = MST[indices][:, indices]
         cluster_density_sparseness = np.max(cluster_MST)
         return cluster_density_sparseness
 
-test = DBCVCalculator(data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models',
-                      config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
-test.run()
+# test = DBCVCalculator(data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models',
+#                       config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,23 +59,24 @@
     MIN_CLUSTER_SIZE = 'min_cluster_size'
     MIN_SAMPLES = 'min_samples'
     EPSILON = 'cluster_selection_epsilon'
     CLUSTER_MODEL = 'CLUSTER_MODEL'
 
 
 class UnsupervisedOptions(Enum):
-    FEATURE_SLICE_OPTIONS = [Unsupervised.ALL_FEATURES_INCLUDING_POSE,
-                          Unsupervised.ALL_FEATURES_INCLUDING_POSE.value,
+    FEATURE_SLICE_OPTIONS = [Unsupervised.ALL_FEATURES_INCLUDING_POSE.value,
+                          Unsupervised.ALL_FEATURES_EXCLUDING_POSE.value,
                           Unsupervised.USER_DEFINED_SET.value]
     BOUT_AGGREGATION_METHODS = ['MEAN', 'MEDIAN']
     DATA_FORMATS = ['NONE', 'SCALED', 'RAW']
     SAVE_FORMATS = ['CSV', 'PICKLE']
-    CATEGORICAL_OPTIONS = ['VIDEO NAMES', 'CLASSIFIER', 'CLUSTER']
     CORRELATION_OPTIONS = ['SPEARMAN', 'PEARSONS', 'KENDALL']
-    CONTINUOUS_OPTIONS = ['START FRAME', 'END_FRAME', 'CLASSIFIER PROBABILITY']
+
+    CATEGORICAL_OPTIONS = ['VIDEO', 'CLASSIFIER', 'CLUSTER']
+    CONTINUOUS_OPTIONS = ['START_FRAME', 'END_FRAME', 'PROBABILITY']
     SPEED_OPTIONS = [round(x, 1) for x in list(np.arange(0.1, 2.1, 0.1))]
     SHAP_CLUSTER_METHODS = ['Paired clusters']
     DR_ALGO_OPTIONS = ['UMAP', 'TSNE']
     CLUSTERING_ALGO_OPTIONS = ['HDBSCAN']
     VARIANCE_OPTIONS = list(range(0, 100, 10))
     GRAPH_CNT = list(range(1, 11))
     SCATTER_SIZE = list(range(10, 110, 10))
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/.DS_Store`

 * *Files 26% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0003 35e3 0000 000b 005f 005f 0070  ....5......_._.p
+00000130: 0000 0003 855e 0000 000b 005f 005f 0070  .....^....._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 4a51 769d  moDDblob....JQv.
-00000160: ddf6 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 4d55 fc8e  moDDblob....MU..
+00000160: bbf8 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 4a51 769d ddf6  dDblob....JQv...
+00000180: 6444 626c 6f62 0000 0008 4d55 fc8e bbf8  dDblob....MU....
 00000190: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0004 0000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0004 a000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/dataset_creator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import os
 import pandas as pd
+import numpy as np
 from simba.read_config_unit_tests import (check_if_filepath_list_is_empty,
                                           check_file_exist_and_readable)
 from simba.unsupervised.bout_aggregator import bout_aggregator
 from simba.misc_tools import get_fn_ext
 from simba.unsupervised.enums import Unsupervised
 from simba.mixins.config_reader import ConfigReader
+from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 from simba.drop_bp_cords import getBpNames
 from simba.rw_dfs import read_df
 from simba.utils.errors import NoDataError
 from simba.utils.printing import stdout_success
 import pickle
+import sys
 
 
-class DatasetCreator(ConfigReader):
+class DatasetCreator(ConfigReader, UnsupervisedMixin):
     def __init__(self,
                  config_path: str,
                  settings: dict):
 
         print('Creating unsupervised learning dataset...')
-        super().__init__(config_path=config_path)
+        ConfigReader.__init__(self, config_path=config_path)
+        UnsupervisedMixin.__init__(self)
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths, error_msg='NO MACHINE LEARNING DATA FOUND')
         self.settings = settings
         self.clf_type, self.feature_lst = None, None
         self.save_path = os.path.join(self.logs_path, 'unsupervised_data_{}.pickle'.format(self.datetime))
         self.log_save_path = os.path.join(self.logs_path, 'unsupervised_data_log_{}.csv'.format(self.datetime))
         self.clf_probability_cols = ['Probability_' + x for x in self.clf_names]
         self.clf_cols = self.clf_names + self.clf_probability_cols
@@ -96,22 +100,21 @@
         if len(self.bouts_x_df) == 0:
             raise NoDataError(msg='The data contains zero frames after the chosen slice setting')
         results = {}
         results['DATETIME'] = self.datetime
         results['AGGREGATION_METHOD'] = self.settings[Unsupervised.BOUT_AGGREGATION_TYPE.value]
         results['MIN_BOUT'] = self.settings[Unsupervised.MIN_BOUT_LENGTH.value]
         results['FEATURE_NAMES'] = self.feature_names
-        results['FRAME_FEATURES'] = self.raw_x_df
-        results['FRAME_POSE'] = self.raw_bp_df
-        results['FRAME_TARGETS'] = self.raw_y_df
-        results['BOUTS_FEATURES'] = self.bouts_x_df
+        results['FRAME_FEATURES'] = self.raw_x_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float16)
+        results['FRAME_POSE'] = self.raw_bp_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float16)
+        results['FRAME_TARGETS'] = self.raw_y_df.set_index([Unsupervised.VIDEO.value, Unsupervised.FRAME.value]).astype(np.float16)
+        results['BOUTS_FEATURES'] = self.bouts_x_df.set_index([Unsupervised.VIDEO.value, Unsupervised.START_FRAME.value, Unsupervised.END_FRAME.value]).astype(np.float16)
         results['BOUTS_TARGETS'] = self.bouts_y_df
 
-        with open(self.save_path, 'wb') as f:
-            pickle.dump(results, f, protocol=pickle.HIGHEST_PROTOCOL)
+        self.write_pickle(data=results, save_path=self.save_path)
         self.timer.stop_timer()
         self.__aggregate_dataset_stats()
         stdout_success(msg=f'Dataset for unsupervised learning saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
 # settings = {'data_slice': 'ALL FEATURES (EXCLUDING POSE)',
 #             'clf_slice': 'Attack',
 #             'bout_aggregation_type': 'MEDIAN',
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/grid_search_visualizers.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,59 +19,53 @@
         super().__init__()
         check_if_dir_exists(in_dir=save_dir)
         check_if_dir_exists(in_dir=model_dir)
         self.save_dir, self.settings, self.model_dir = save_dir, settings, model_dir
         self.data_path = glob.glob(model_dir + '/*.pickle')
         check_if_filepath_list_is_empty(filepaths=self.data_path, error_msg=f'SIMBA ERROR: No pickle files in {model_dir}')
 
-    def cluster_visualizer(self):
-        data = self.read_pickle(self.model_dir)
-        for k, v in data.items():
-            self.check_key_exist_in_object(object=v, key=Clustering.CLUSTER_MODEL.value)
-        for k, v in data.items():
-            save_path = os.path.join(self.save_dir, f'{v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{v[Clustering.CLUSTER_MODEL.value][Unsupervised.HASHED_NAME.value]}.png')
-            data = pd.DataFrame(v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_, columns=['X', 'Y'])
-            data['CLUSTER'] = v[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value].labels_.reshape(-1, 1).astype(np.int8)
-            plot = sns.scatterplot(data=data, x='X', y='Y', hue="CLUSTER", palette=self.settings['PALETTE'])
-            plt.savefig(save_path)
-            stdout_success(msg=f'Saved {save_path}...')
-            plt.close('all')
-        self.timer.stop_timer()
-        stdout_success(msg='All cluster images created.', elapsed_time=self.timer.elapsed_time_str)
+    def __join_data(self, data: object):
+        embedding_data = pd.DataFrame(data[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_, columns=['X', 'Y'])
+        bouts_data = data[Unsupervised.DATA.value][Unsupervised.BOUTS_FEATURES.value]
+        target_data = data[Unsupervised.DATA.value][Unsupervised.BOUTS_TARGETS.value]
+        cluster_data = pd.DataFrame(data[Clustering.CLUSTER_MODEL.value][Unsupervised.MODEL.value].labels_.reshape(-1, 1).astype(np.int8), columns=['CLUSTER'])
+        data = pd.concat([embedding_data, bouts_data, target_data, cluster_data], axis=1)
+        return data.loc[:, ~data.columns.duplicated()].copy()
 
     def categorical_visualizer(self,
                                categoricals: list):
         data = self.read_pickle(self.model_dir)
         for k, v in data.items():
             self.check_key_exist_in_object(object=v, key=Unsupervised.DR_MODEL.value)
         for k, v in data.items():
+            data = self.__join_data(data=v)
             for variable in categoricals:
                 save_path = os.path.join(self.save_dir, f'{v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{variable}.png')
-                data = pd.DataFrame(v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_, columns=['X', 'Y'])
-                data = pd.concat([v[Unsupervised.DATA.value][Unsupervised.BOUTS_FEATURES.value][variable], data], axis=1)
-                plot = sns.scatterplot(data=data, x='X', y='Y', hue=variable, palette=self.settings['CATEGORICAL_PALETTE'])
-                plt.savefig(save_path)
-                stdout_success(msg=f'Saved {save_path}...')
-                plt.close('all')
+                if os.path.isfile(save_path):
+                    continue
+                else:
+                    sns.scatterplot(data=data, x='X', y='Y', hue=variable, palette=sns.color_palette(self.settings['CATEGORICAL_PALETTE'], len(data[variable].unique())))
+                    plt.savefig(save_path)
+                    stdout_success(msg=f'Saved {save_path}...')
+                    plt.close('all')
         self.timer.stop_timer()
         stdout_success(msg='All cluster images created.', elapsed_time=self.timer.elapsed_time_str)
 
     def continuous_visualizer(self,
                              continuous_vars: list):
         data = self.read_pickle(self.model_dir)
         for k, v in data.items():
             self.check_key_exist_in_object(object=v, key=Unsupervised.DR_MODEL.value)
         for k, v in data.items():
+            data = self.__join_data(data=v)
             for variable in continuous_vars:
                 save_path = os.path.join(self.save_dir, f'{v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]}_{variable}.png')
                 fig, ax = plt.subplots()
                 plt.xlabel('X')
                 plt.ylabel('Y')
-                data = pd.DataFrame(v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value].embedding_, columns=['X', 'Y'])
-                data = pd.concat([v[Unsupervised.DATA.value][Unsupervised.BOUTS_FEATURES.value][variable], data], axis=1)
                 points = ax.scatter(data['X'], data['Y'], c=data[variable], s=self.settings['SCATTER_SIZE'], cmap=self.settings['CONTINUOUS_PALETTE'])
                 cbar = fig.colorbar(points)
                 cbar.set_label(variable, loc='center')
                 title = v[Unsupervised.DR_MODEL.value][Unsupervised.HASHED_NAME.value]
                 plt.title(title, ha="center", fontsize=15, bbox={"facecolor": "orange", "alpha": 0.5, "pad": 0})
                 fig.savefig(save_path)
                 plt.close('all')
@@ -84,12 +78,13 @@
 # settings = {'PALETTE': 'Pastel1'}
 # test = GridSearchVisualizer(model_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models',
 #                             save_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/images',
 #                             settings=settings)
 # test.cluster_visualizer()
 
 
-# settings = {'PALETTE': 'Pastel1', 'SCATTER_SIZE': 10}
-# test = GridSearchVisualizer(model_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models',
+# settings = {'CATEGORICAL_PALETTE': 'Pastel1', 'SCATTER_SIZE': 10}
+# test = GridSearchVisualizer(model_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models_042023',
 #                             save_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/images',
 #                             settings=settings)
-# test.continuous_visualizer(continuous_vars=['START_FRAME'])
+# #test.continuous_visualizer(continuous_vars=['START_FRAME'])
+# test.categorical_visualizer(categoricals=['CLUSTER'])
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-from simba.read_config_unit_tests import (read_config_entry,
-                                          read_config_file,
-                                          read_project_path_and_file_type)
 from tkinter import *
 from simba.tkinter_functions import (hxtScrollbar,
                                      Entry_Box,
                                      DropDownMenu,
                                      FileSelect)
-from PIL import ImageTk
-import PIL.Image
-import os
-from simba.utils.lookups import get_icons_paths
 import tkinter.ttk as ttk
 from simba.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
-from simba.unsupervised.enums import Options, Unsupervised
-from simba.enums import ReadConfig, Dtypes
-from simba.train_model_functions import get_all_clf_names
+from simba.unsupervised.enums import UnsupervisedOptions, Unsupervised
 from simba.unsupervised.dataset_creator import DatasetCreator
-from simba.unsupervised.pop_up_classes import (GridSearchClusterVisualizerPopUp,
-                                               BatchDataExtractorPopUp,
+from simba.unsupervised.pop_up_classes import (GridSearchVisualizerPopUp,
+                                               DataExtractorPopUp,
                                                FitDimReductionPopUp,
                                                FitClusterModelsPopUp,
                                                TransformDimReductionPopUp,
                                                TransformClustererPopUp,
                                                ClusterVisualizerPopUp,
                                                ClusterFrequentistStatisticsPopUp,
-                                               ClusterMLStatisticsPopUp,
+                                               ClusterXAIPopUp,
                                                EmbedderCorrelationsPopUp,
                                                PrintEmBeddingInfoPopUp,
                                                DBCVPopUp)
 
 class UnsupervisedGUI(ConfigReader, PopUpMixin):
     def __init__(self,
                  config_path: str):
 
         ConfigReader.__init__(self, config_path=config_path)
         PopUpMixin.__init__(self, title="UNSUPERVISED ANALYSIS", config_path=config_path, size=(1000, 800))
+        self.main_frm = Toplevel()
+        self.main_frm.minsize(1000, 800)
+        self.main_frm.wm_title("UNSUPERVISED ANALYSIS")
         self.main_frm.columnconfigure(0, weight=1)
         self.main_frm.rowconfigure(0, weight=1)
         self.main_frm = ttk.Notebook(hxtScrollbar(self.main_frm))
         self.create_dataset_tab = ttk.Frame(self.main_frm)
         self.dimensionality_reduction_tab = ttk.Frame(self.main_frm)
         self.clustering_tab = ttk.Frame(self.main_frm)
         self.visualization_tab = ttk.Frame(self.main_frm)
@@ -49,27 +43,26 @@
         self.main_frm.add(self.create_dataset_tab, text=f'{"[CREATE DATASET]": ^20s}', compound='left', image=self.menu_icons['features']['img'])
         self.main_frm.add(self.dimensionality_reduction_tab, text=f'{"[DIMENSIONALITY REDUCTION]": ^20s}', compound='left', image=self.menu_icons['dimensionality_reduction']['img'])
         self.main_frm.add(self.clustering_tab, text=f'{"[CLUSTERING]": ^20s}', compound='left', image=self.menu_icons['cluster']['img'])
         self.main_frm.add(self.visualization_tab, text=f'{"[VISUALIZATION]": ^20s}', compound='left', image=self.menu_icons['visualize']['img'])
         self.main_frm.add(self.metrics_tab, text=f'{"[METRICS]": ^20s}', compound='left', image=self.menu_icons['metrics']['img'])
         self.main_frm.grid(row=0)
 
-        self.clf_slice_options = [f'ALL CLASSIFIERS ({len(self.clf_names)}']
+        self.clf_slice_options = [f'ALL CLASSIFIERS ({len(self.clf_names)})']
         for clf_name in self.clf_names: self.clf_slice_options.append(f'{clf_name}')
-
         create_dataset_frm = LabelFrame(self.create_dataset_tab, text='CREATE DATASET', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
         self.feature_file_selected = FileSelect(create_dataset_frm, "FEATURE FILE (CSV)", lblwidth=25)
 
-        self.data_slice_dropdown = DropDownMenu(create_dataset_frm, 'FEATURE SLICE:', Options.FEATURE_SLICE_OPTIONS.value, '25', com= lambda x: self.change_status_of_file_select())
-        self.data_slice_dropdown.setChoices(Options.FEATURE_SLICE_OPTIONS.value[0])
+        self.data_slice_dropdown = DropDownMenu(create_dataset_frm, 'FEATURE SLICE:', UnsupervisedOptions.FEATURE_SLICE_OPTIONS.value, '25', com= lambda x: self.change_status_of_file_select())
+        self.data_slice_dropdown.setChoices(UnsupervisedOptions.FEATURE_SLICE_OPTIONS.value[0])
         self.clf_slice_dropdown = DropDownMenu(create_dataset_frm, 'CLASSIFIER SLICE:', self.clf_slice_options, '25')
         self.clf_slice_dropdown.setChoices(self.clf_slice_options[0])
         self.change_status_of_file_select()
-        self.bout_dropdown = DropDownMenu(create_dataset_frm, 'BOUT AGGREGATION METHOD:', Options.BOUT_AGGREGATION_METHODS.value, '25')
-        self.bout_dropdown.setChoices(choice=Options.BOUT_AGGREGATION_METHODS.value[0])
+        self.bout_dropdown = DropDownMenu(create_dataset_frm, 'BOUT AGGREGATION METHOD:', UnsupervisedOptions.BOUT_AGGREGATION_METHODS.value, '25')
+        self.bout_dropdown.setChoices(choice=UnsupervisedOptions.BOUT_AGGREGATION_METHODS.value[0])
         self.min_bout_length = Entry_Box(create_dataset_frm, 'MINIMUM BOUT LENGTH (MS): ', '25', validation='numeric')
         self.min_bout_length.entry_set(val=0)
         self.create_btn = Button(create_dataset_frm, text='CREATE DATASET', fg='blue', command= lambda: self.create_dataset())
 
         create_dataset_frm.grid(row=0, column=0, sticky=NW)
         self.data_slice_dropdown.grid(row=0, column=0, sticky=NW)
         self.clf_slice_dropdown.grid(row=1, column=0, sticky=NW)
@@ -89,25 +82,25 @@
         self.cluster_fit_btn = Button(self.clustering_frm, text='CLUSTERING: FIT ', fg='blue', command= lambda: FitClusterModelsPopUp())
         self.cluster_transform_btn = Button(self.clustering_frm, text='CLUSTERING: TRANSFORM ', fg='red', command=lambda: TransformClustererPopUp())
         self.clustering_frm.grid(row=0, column=0, sticky=NW)
         self.cluster_fit_btn.grid(row=1, column=0, sticky=NW)
         self.cluster_transform_btn.grid(row=2, column=0, sticky=NW)
 
         self.visualization_frm = LabelFrame(self.visualization_tab, text='VISUALIZATIONS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.grid_search_visualization_btn = Button(self.visualization_frm, text='GRID-SEARCH VISUALIZATION', fg='blue', command= lambda: self.launch_grid_search_visualization_pop_up())
+        self.grid_search_visualization_btn = Button(self.visualization_frm, text='GRID-SEARCH VISUALIZATION', fg='blue', command= lambda: GridSearchVisualizerPopUp(config_path=self.config_path))
         self.cluster_visualizer = Button(self.visualization_frm, text='DATA VISUALIZERS', fg='red', command= lambda: ClusterVisualizerPopUp(config_path=self.config_path))
         self.visualization_frm.grid(row=0, column=0, sticky='NW')
         self.grid_search_visualization_btn.grid(row=0, column=0, sticky='NW')
         self.cluster_visualizer.grid(row=1, column=0, sticky='NW')
 
         self.metrics_frm = LabelFrame(self.metrics_tab, text='METRICS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.dbcv_btn = Button(self.metrics_frm, text='DENSITY-BASED CLUSTER VALIDATION', fg='blue', command=lambda: DBCVPopUp(config_path=self.config_path))
-        self.extract_single_metrics_btn = Button(self.metrics_frm, text='EXTRACT DATA', fg='red', command=lambda: BatchDataExtractorPopUp())
+        self.extract_single_metrics_btn = Button(self.metrics_frm, text='EXTRACT DATA', fg='red', command=lambda: DataExtractorPopUp(config_path=self.config_path))
         self.cluster_descriptives_btn = Button(self.metrics_frm, text='CLUSTER FREQUENTIST STATISTICS', fg='green', command=lambda: ClusterFrequentistStatisticsPopUp(config_path=self.config_path))
-        self.cluster_xai_btn = Button(self.metrics_frm, text='CLUSTER XAI STATISTICS', fg='blue', command=lambda: ClusterMLStatisticsPopUp(config_path=self.config_path))
+        self.cluster_xai_btn = Button(self.metrics_frm, text='CLUSTER XAI STATISTICS', fg='blue', command=lambda: ClusterXAIPopUp(config_path=self.config_path))
         self.embedding_corr_btn = Button(self.metrics_frm, text='EMBEDDING CORRELATIONS', fg='orange', command=lambda: EmbedderCorrelationsPopUp(config_path=self.config_path))
         self.print_embedding_info_btn = Button(self.metrics_frm, text='PRINT MODEL INFO', fg='black', command=lambda: PrintEmBeddingInfoPopUp(config_path=self.config_path))
 
         self.metrics_frm.grid(row=0, column=0, sticky='NW')
         self.dbcv_btn.grid(row=0, column=0, sticky='NW')
         self.extract_single_metrics_btn.grid(row=1, column=0, sticky='NW')
         self.cluster_descriptives_btn.grid(row=2, column=0, sticky='NW')
@@ -128,18 +121,16 @@
         classifier_slice_type = self.clf_slice_dropdown.getChoices()
         bout_selection = self.bout_dropdown.getChoices()
         bout_length = self.min_bout_length.entry_get
         feature_file_path = None
         if data_slice_type is Unsupervised.USER_DEFINED_SET.value:
             feature_file_path = self.feature_file_selected.file_path
 
-        settings = {'feature_slice': data_slice_type,
+        settings = {'data_slice': data_slice_type,
                     'clf_slice': classifier_slice_type,
-                    'bout_aggregation_method': bout_selection,
+                    'bout_aggregation_type': bout_selection,
                     'min_bout_length': bout_length,
                     'feature_file_path': feature_file_path}
         _ = DatasetCreator(settings=settings, config_path=self.config_path)
 
-    def launch_grid_search_visualization_pop_up(self):
-        _ = GridSearchClusterVisualizerPopUp(config_path=self.config_path)
 
-_ = UnsupervisedGUI(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
+_ = UnsupervisedGUI(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/visualizers.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/data_plotter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,193 @@
-import numpy as np
-import matplotlib.pyplot as plt
-from simba.unsupervised.misc import (read_pickle,
-                                     check_directory_exists)
+__author__ = "Simon Nilsson"
+
 import pandas as pd
-from simba.misc_tools import (check_file_exist_and_readable,
-                              get_video_meta_data,
-                              find_all_videos_in_directory,
-                              check_multi_animal_status,
-                              SimbaTimer)
-from simba.drop_bp_cords import getBpNames, create_body_part_dictionary, createColorListofList
-from simba.read_config_unit_tests import read_config_file, read_config_entry, read_project_path_and_file_type
-from simba.enums import Paths, Formats, ReadConfig, Dtypes
+from joblib import Parallel, delayed
 import os
-import warnings
+from simba.feature_extractors.unit_tests import read_video_info
+from simba.movement_processor import MovementProcessor
+from simba.misc_tools import (check_multi_animal_status,
+                              get_fn_ext,
+                              SimbaTimer,
+                              get_color_dict,
+                              )
+from simba.utils.printing import stdout_success
+import numpy as np
 import cv2
+from simba.enums import Formats
+from simba.mixins.config_reader import ConfigReader
+from simba.utils.errors import NoSpecifiedOutputError
+
+
+class DataPlotter(ConfigReader):
+    """
+    Class for tabular data visualizations of animal movement and distances in the current frame and their aggregate
+    statistics.
+
+    Parameters
+    ----------
+    config_path: str
+        path to SimBA project config file in Configparser format
+
+    Notes
+    ----------
+    `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-data-tables`__.
+
+    Examples
+    -----
+    >>> data_plotter = DataPlotter(config_path='MyConfigPath')
+    >>> data_plotter.process_movement()
+    >>> data_plotter.create_data_plots()
+    """
 
-
-class GridSearchClusterVisualizer(object):
-    def __init__(self,
-                 clusterers_path: str,
-                 save_dir: str,
-                 settings: dict):
-
-        self.timer = SimbaTimer()
-        self.timer.start_timer()
-        check_directory_exists(save_dir)
-        self.save_dir = save_dir
-        self.settings = settings
-        self.clusterers = None
-        if clusterers_path:
-            check_directory_exists(clusterers_path)
-            self.clusterers = read_pickle(data_path=clusterers_path)
-
-    def create_datasets(self):
-        self.img_data = {}
-        print('Retrieving models for visualization...')
-        for k, v in self.clusterers.items():
-            self.img_data[k] = {}
-            self.img_data[k]['categorical_legends'] = set()
-            self.img_data[k]['continuous_legends'] = set()
-            embedder = v['EMBEDDER']
-            cluster_data = v['MODEL'].labels_.reshape(-1, 1).astype(np.int8)
-            embedding_data = embedder['MODEL'].embedding_
-            data = np.hstack((embedding_data, cluster_data))
-            self.img_data[k]['DATA'] = pd.DataFrame(data, columns=['X', 'Y', 'CLUSTER'])
-            self.img_data[k]['HASH'] = v['HASH']
-            self.img_data[k]['EMBEDDER'] = embedder
-            self.img_data[k]['CLUSTERER_NAME'] = v['NAME']
-            self.img_data[k]['categorical_legends'].add('CLUSTER')
-
-        if self.settings['HUE']:
-            for hue_id, hue_settings in self.settings['HUE'].items():
-                field_type, field_name = hue_settings['FIELD_TYPE'], hue_settings['FIELD_NAME']
-                for k, v in self.img_data.items():
-                    embedder = v['EMBEDDER']
-                    if not 'categorical_legends' in self.img_data[k].keys():
-                        self.img_data[k]['categorical_legends'] = set()
-                        self.img_data[k]['continuous_legends'] = set()
-                    if (field_type == 'CLASSIFIER'):
-                        self.img_data[k]['categorical_legends'].add(field_name)
-                    if (field_type == 'VIDEO NAMES'):
-                        self.img_data[k]['categorical_legends'].add(field_type)
-                    elif (field_type == 'CLASSIFIER PROBABILITY') or (field_type == 'START FRAME'):
-                        if field_name != 'None' and field_name != '':
-                            self.img_data[k]['continuous_legends'].add(field_name)
-                        else:
-                            self.img_data[k]['continuous_legends'].add(field_type)
-                    if field_name != 'None' and field_name != '':
-                        self.img_data[k]['DATA'][field_name] = embedder[field_type][field_name]
-                    else:
-                        self.img_data[k]['DATA'][field_type] = embedder[field_type]
-
-
-    def create_imgs(self):
-        print('Creating plots...')
-        plots = {}
-        for k, v in self.img_data.items():
-            for categorical in v['categorical_legends']:
-                fig, ax = plt.subplots()
-                colmap = {name: n for n, name in enumerate(set(list(v['DATA'][categorical].unique())))}
-                scatter = ax.scatter(v['DATA']['X'], v['DATA']['Y'], c=[colmap[name] for name in v['DATA'][categorical]], cmap=self.settings['CATEGORICAL_PALETTE'], s=self.settings['SCATTER_SIZE'])
-                plt.legend(*scatter.legend_elements()).set_title(categorical)
-                plt.xlabel('X')
-                plt.ylabel('Y')
-                plt_key = v['HASH'] + '_' + v['CLUSTERER_NAME'] + '_' + categorical
-                title = 'EMBEDDER: {} \n CLUSTERER: {}'.format(v['HASH'], v['CLUSTERER_NAME'])
-                if categorical != 'CLUSTER':
-                    title = 'EMBEDDER: {}'.format(v['HASH'])
-                plt.title(title, ha="center", fontsize=15, bbox={"facecolor": "orange", "alpha": 0.5, "pad": 0})
-                plots[plt_key] = fig
-                plt.close('all')
-
-            for continuous in v['continuous_legends']:
-                fig, ax = plt.subplots()
-                plt.xlabel('X')
-                plt.ylabel('Y')
-                points = ax.scatter(v['DATA']['X'], v['DATA']['Y'], c=v['DATA'][continuous], s=self.settings['SCATTER_SIZE'], cmap=self.settings['CONTINUOUS_PALETTE'])
-                cbar = fig.colorbar(points)
-                cbar.set_label(continuous, loc='center')
-                title = 'EMBEDDER: {}'.format(v['HASH'])
-                plt_key = v['HASH'] + v['CLUSTERER_NAME'] + '_' + continuous
-                plt.title(title, ha="center", fontsize=15, bbox={"facecolor": "orange", "alpha": 0.5, "pad": 0})
-                plots[plt_key] = fig
-                plt.close('all')
-
-        for plt_key, fig in plots.items():
-            save_path = os.path.join(self.save_dir, f'{plt_key}.png')
-            print(f'Saving scatterplot {plt_key} ...')
-            fig.savefig(save_path)
-        self.timer.stop_timer()
-        print(f'SIMBA COMPLETE: {str(len(plots.keys()))} plots saved in {self.save_dir} (elapsed time: {self.timer.elapsed_time_str}s)')
-
-
-
-class ClusterVisualizer(object):
     def __init__(self,
                  config_path: str,
-                 video_dir: str,
-                 data_path: str,
-                 settings: dict):
-
-        self.config, self.settings = read_config_file(ini_path=config_path), settings
-        self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
-        self.save_parent_dir = os.path.join(self.project_path, Paths.CLUSTER_EXAMPLES.value)
-        if not os.path.exists(self.save_parent_dir): os.makedirs(self.save_parent_dir)
-        check_file_exist_and_readable(file_path=data_path)
-        self.x_cols, self.y_cols, self.pcols = getBpNames(config_path)
-        self.no_animals = read_config_entry(self.config, ReadConfig.GENERAL_SETTINGS.value, ReadConfig.ANIMAL_CNT.value, Dtypes.INT.value)
-        self.pose_colors = createColorListofList(self.no_animals, int(len(self.x_cols) + 1))
-        self.multi_animal_status, self.multi_animal_id_lst = check_multi_animal_status(self.config, self.no_animals)
-        self.animal_bp_dict = create_body_part_dictionary(self.multi_animal_status, self.multi_animal_id_lst, self.no_animals, self.x_cols, self.y_cols, [], self.pose_colors)
-        self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
-        self.video_files = find_all_videos_in_directory(directory=video_dir, as_dict=True)
-        self.data = read_pickle(data_path=data_path)
-        self.video_dir, self.pose_df = video_dir, None
-        self.cluster_ids = self.data['MODEL'].labels_
-
-    def create(self):
-        for cluster_id in np.unique(self.cluster_ids):
-            self.cluster_id = cluster_id
-            cluster_idx = [i for i, e in enumerate(self.cluster_ids) if e == self.cluster_id]
-            for idx in cluster_idx:
-                self.video_name = self.data['EMBEDDER']['VIDEO NAMES'].loc[idx].values[0]
-                if self.video_name not in self.video_files.keys():
-                    warnings.warn(f'SIMBA WARNING: Video {self.video_name} not found in video directory {self.video_dir}')
-                    continue
-                self.start_frm, self.end_frm = self.data['EMBEDDER']['START FRAME'].loc[idx].values[0], self.data['EMBEDDER']['END FRAME'].loc[idx].values[0]
-                self.__cluster_video_creator()
-
-    def __cluster_video_creator(self):
-        self.save_directory = os.path.join(self.save_parent_dir, str(self.cluster_id), self.video_name)
-        if self.settings['pose']['include']:
-            self.pose_df = self.data['EMBEDDER']['POSE'][self.data['EMBEDDER']['POSE']['VIDEO'] == self.video_name].drop(['FRAME', 'VIDEO'], axis=1).reset_index(drop=True)
-        if not os.path.exists(self.save_directory): os.makedirs(self.save_directory)
-        video_meta_data = get_video_meta_data(video_path=self.video_files[self.video_name])
-        print(self.video_files[self.video_name])
-        output_fps = int(video_meta_data['fps'] * self.settings['video_speed'])
-
-        if output_fps < 1: output_fps = 1
-        cap = cv2.VideoCapture(self.video_files[self.video_name])
-        cap.set(1, self.start_frm)
-        file_name = os.path.join(self.save_directory, f'Event_{str(int(self.start_frm))}_{str(int(self.end_frm))}.mp4')
-        self.writer = cv2.VideoWriter(file_name, self.fourcc, output_fps,(video_meta_data['width'], video_meta_data['height']))
-        current_frm = self.start_frm
-        event_frms = self.end_frm - self.start_frm
-        frm_cnt = 1
-        while current_frm < self.end_frm:
-            _, img = cap.read()
-            if self.settings['pose']['include']:
-                bp_data = self.pose_df.iloc[current_frm]
-                for cnt, (animal_name, animal_bps) in enumerate(self.animal_bp_dict.items()):
-                    for bp in zip(animal_bps['X_bps'], animal_bps['Y_bps']):
-                        x_bp, y_bp = bp_data[bp[0]], bp_data[bp[1]]
-                        cv2.circle(img, (int(x_bp), int(y_bp)), self.settings['pose']['circle_size'], self.animal_bp_dict[animal_name]['colors'][cnt], -1)
-
-
-
-            self.writer.write(img)
-            print(f'Writing frame {str(frm_cnt)}/{str(event_frms)}, Cluster: {self.cluster_id}, Video: {self.video_name}...')
-            current_frm += 1
-            frm_cnt += 1
-        cap.release()
-        self.writer.release()
-
-
-
+                 style_attr: dict,
+                 body_part_attr: list,
+                 data_paths: list,
+                 video_setting: bool,
+                 frame_setting: bool,
+                 ):
+
+        super().__init__(config_path=config_path)
+        self.video_setting, self.frame_setting = video_setting, frame_setting
+        if (not self.video_setting) and (not self.frame_setting):
+            raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please choose to create video and/or frames data plots. SimBA found that you ticked neither video and/or frames')
+        self.files_found, self.style_attr, self.body_part_attr = data_paths, style_attr, body_part_attr
+        if not os.path.exists(self.data_table_path):
+            os.makedirs(self.data_table_path)
+        self.multi_animal_status, self.multi_animal_id_list = check_multi_animal_status(self.config, len(self.body_part_attr))
+        self.__compute_spacings()
+        self.process_movement()
+        print('Processing {} video(s)...'.format(str(len(self.files_found))))
+
+    def __compute_spacings(self):
+        """
+        Private helper to compute appropriate spacing between printed text.
+        """
+        self.loc_dict = {}
+        self.loc_dict['Animal'] = (50, 20)
+        self.loc_dict['total_movement_header'] = (250, 20)
+        self.loc_dict['current_velocity_header'] = (475, 20)
+        self.loc_dict['animals'] = {}
+        y_cord, x_cord = 75, 15
+        for animal_cnt, animal_name in enumerate(self.multi_animal_id_list):
+            self.loc_dict['animals'][animal_name] = {}
+            self.loc_dict['animals'][animal_name]['index_loc'] = (50, y_cord)
+            self.loc_dict['animals'][animal_name]['total_movement_loc'] = (250, y_cord)
+            self.loc_dict['animals'][animal_name]['current_velocity_loc'] = (475, y_cord)
+            y_cord += 50
+
+    def process_movement(self):
+        """
+        Method to create movement data for visualization
+
+        Returns
+        -------
+        Attribute: pd.Dataframe
+            movement
+        """
+        self.config.set('process movements', 'no_of_animals', str(len(self.body_part_attr)))
+        self.config.set('process movements', 'probability_threshold', str(0.00))
+        for animal_cnt, animal in enumerate(self.body_part_attr):
+            self.config.set('process movements', 'animal_{}_bp'.format(animal_cnt + 1), animal[0])
+        with open(self.config_path, 'w') as file:
+            self.config.write(file)
+        movement_processor = MovementProcessor(config_path=self.config_path, visualization=True, files=self.files_found)
+        movement_processor.process_movement()
+        self.movement = movement_processor.movement_dict
+
+    def create_data_plots(self):
+        """
+        Method to create and save visualizations on disk from data created in
+        :meth:`~simba.DataPlotter.process_movement`. Results are stored in the `project_folder/frames/output/live_data_table`.
+
+        Returns
+        -------
+        None
+        """
+
+        def multiprocess_img_creation(video_data_slice: list,
+                                      location_dict: dict,
+                                      animal_ids: list,
+                                      video_data: pd.DataFrame,
+                                      style_attr: dict,
+                                      body_part_attr: dict):
+
+            color_dict = get_color_dict()
+            img = np.zeros((style_attr['size'][1], style_attr['size'][0], 3))
+            img[:] = color_dict[style_attr['bg_color']]
+            cv2.putText(img, 'Animal', location_dict['Animal'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, color_dict[style_attr['header_color']], style_attr['font_thickness'])
+            cv2.putText(img, 'Total movement (cm)', location_dict['total_movement_header'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, color_dict[style_attr['header_color']], style_attr['font_thickness'])
+            cv2.putText(img, 'Velocity (cm/s)',location_dict['current_velocity_header'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, color_dict[style_attr['header_color']], style_attr['font_thickness'])
+            for animal_cnt, animal_name in enumerate(animal_ids):
+                clr = color_dict[body_part_attr[animal_cnt][1]]
+                total_movement = str(round(video_data[animal_name].iloc[0:video_data_slice.index.max()].sum() / 10, style_attr['data_accuracy']))
+                current_velocity = str(round(video_data_slice[animal_name].sum() / 10, style_attr['data_accuracy']))
+                cv2.putText(img, animal_name, location_dict['animals'][animal_name]['index_loc'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, clr, 1)
+                cv2.putText(img, total_movement, location_dict['animals'][animal_name]['total_movement_loc'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, clr, 1)
+                cv2.putText(img, current_velocity, location_dict['animals'][animal_name]['current_velocity_loc'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, clr, 1)
+            return img
+
+        for file_cnt, file_path in enumerate(self.files_found):
+            video_timer = SimbaTimer()
+            video_timer.start_timer()
+            _, video_name, _ = get_fn_ext(file_path)
+            video_data = pd.DataFrame(self.movement[video_name])
+            _, _, self.fps = read_video_info(vid_info_df=self.video_info_df, video_name=video_name)
+            if self.video_setting:
+                self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
+                self.video_save_path = os.path.join(self.data_table_path, video_name + '.mp4')
+                self.writer = cv2.VideoWriter(self.video_save_path, self.fourcc, self.fps, self.style_attr['size'])
+            if self.frame_setting:
+                self.frame_save_path = os.path.join(self.data_table_path, video_name)
+                if not os.path.exists(self.frame_save_path): os.makedirs(self.frame_save_path)
+            video_data_lst = np.array_split(pd.DataFrame(video_data), int(len(video_data) / self.fps))
+            self.imgs = Parallel(n_jobs=self.cpu_to_use, verbose=1, backend="threading")(delayed(multiprocess_img_creation)(x, self.loc_dict, self.multi_animal_id_list, video_data, self.style_attr, self.body_part_attr) for x in video_data_lst)
+            frm_cnt = 0
+            for img_cnt, img in enumerate(self.imgs):
+                for frame_cnt in range(int(self.fps)):
+                    if self.video_setting:
+                        self.writer.write(np.uint8(img))
+                    if self.frame_setting:
+                        frm_save_name = os.path.join(self.frame_save_path, '{}.png'.format(str(frm_cnt)))
+                        cv2.imwrite(frm_save_name, np.uint8(img))
+                    frm_cnt += 1
+                    print('Frame: {} / {}. Video: {} ({}/{})'.format(str(frm_cnt), str(len(video_data)),
+                                                                   video_name, str(file_cnt + 1),
+                                                                   len(self.files_found)))
+
+            print('Data tables created for video {}...'.format(video_name))
+            if self.video_setting:
+                self.writer.release()
+                video_timer.stop_timer()
+                print('Video {} complete (elapsed time {}s)...'.format(video_name, video_timer.elapsed_time_str))
 
+        self.timer.stop_timer()
+        stdout_success(msg=f'All data table videos created inside {self.data_table_path}', elapsed_time=self.timer.elapsed_time_str)
 
-# settings = {'video_speed': 0.001, 'pose': {'include': True, 'circle_size': 5}}
-# test = ClusterVisualizer(video_dir='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/videos',
-#                          data_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/my_cluster_models/sharp_hopper.pickle',
-#                          settings=settings,
-#                          config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
-# test.create()
-
-
-# settings = {'HUE': {'FIELD_TYPE': 'VIDEO_NAMES', 'FIELD_NAME': None}}
-# settings = {'SCATTER_SIZE': 50, 'CATEGORICAL_PALETTE': 'Set1', 'CONTINUOUS_PALETTE': 'magma', 'HUE': {0: {'FIELD_TYPE': 'CLASSIFIER PROBABILITY', 'FIELD_NAME': 'None'}, 1: {'FIELD_TYPE': 'CLASSIFIER', 'FIELD_NAME': 'Attack'}}}
-# test = GridSearchClusterVisualizer(clusterers_path= '/Users/simon/Desktop/envs/troubleshooting/unsupervised/cluster_models',
-#                                    save_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/images',
-#                                    settings=settings)
-# test.create_datasets()
-# test.create_imgs()
+# style_attr = {'bg_color': 'White', 'header_color': 'Black', 'font_thickness': 1, 'size': (640, 480), 'data_accuracy': 2}
+# body_part_attr = [['Ear_left_1', 'Grey'], ['Ear_right_2', 'Red']]
+# data_paths = ['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv']
+#
+#
+# test = DataPlotter(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                    style_attr=style_attr,
+#                    body_part_attr=body_part_attr,
+#                    data_paths=data_paths,
+#                    video_setting=True,
+#                    frame_setting=False)
+# test.create_data_plots()
+
+# style_attr = {'bg_color': 'White', 'header_color': 'Black', 'font_thickness': 1, 'size': (640, 480), 'data_accuracy': 2}
+# body_part_attr = [['Ear_left_1', 'Grey'], ['Ear_right_2', 'Red']]
+# data_paths = ['/Users/simon/Desktop/envs/simba_dev/tests/test_data/two_C57_madlc/project_folder/csv/outlier_corrected_movement_location/Together_1.csv']
+#
+#
+# test = DataPlotter(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/two_C57_madlc/project_folder/project_config.ini',
+#                    style_attr=style_attr,
+#                    body_part_attr=body_part_attr,
+#                    data_paths=data_paths,
+#                    video_setting=True,
+#                    frame_setting=False)
+# test.create_data_plots()
 
-#{0: {'FIELD_TYPE': 'CLASSIFIER PROBABILITY', 'FIELD_NAME': 'None'}, 1: {'FIELD_TYPE': 'CLASSIFIER', 'FIELD_NAME': 'Attack'}}
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/pop_up_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os, glob
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.mixins.config_reader import ConfigReader
+from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 from tkinter import *
 from simba.enums import Formats, Options
-from simba.misc_tools import check_file_exist_and_readable
+from simba.misc_tools import check_file_exist_and_readable, check_if_filepath_list_is_empty
 from simba.unsupervised.enums import UnsupervisedOptions, Unsupervised, Clustering
 import numpy as np
 from simba.tkinter_functions import (FolderSelect,
                                      DropDownMenu,
                                      FileSelect,
                                      Entry_Box)
 from simba.train_model_functions import check_if_dir_exists
@@ -18,35 +19,16 @@
 from simba.unsupervised.umap_embedder import UmapEmbedder
 from simba.unsupervised.tsne import TSNEGridSearch
 from simba.unsupervised.hdbscan_clusterer import HDBSCANClusterer
 from simba.unsupervised.cluster_visualizer import ClusterVisualizer
 from simba.unsupervised.cluster_statistics import (ClusterFrequentistCalculator,
                                                    ClusterXAICalculator,
                                                    EmbeddingCorrelationCalculator)
-# from simba.enums import Formats, Options
-# from simba.unsupervised.visualizers import (GridSearchClusterVisualizer,
-#                                             ClusterVisualizer)
-# from simba.unsupervised.data_extractors import DataExtractorMultipleModels
-# from simba.unsupervised.umap_embedder import (UMAPGridSearch, UMAPTransform)
-
-# from simba.unsupervised.hdbscan_clusterer import (HDBSCANClusterer,
-#                                                   HDBSCANTransform)
-# from simba.unsupervised.dbcv import DBCVCalculator
-# from simba.read_config_unit_tests import (check_float,
-#                                           check_int,
-#                                           check_file_exist_and_readable,
-#                                           check_if_dir_exists,
-#                                           check_if_filepath_list_is_empty)
-# from simba.unsupervised.misc import read_pickle
-# from simba.unsupervised.cluster_statistics import (ClusterFrequentistCalculator,
-#                                                    ClusterXAICalculator,
-#                                                    EmbeddingCorrelationCalculator)
-# from simba.mixins.pop_up_mixin import PopUpMixin
+from simba.unsupervised.dbcv_calculator import DBCVCalculator
 
-#
 class GridSearchVisualizerPopUp(PopUpMixin):
     def __init__(self,
                  config_path: str):
 
         super().__init__(config_path=config_path, title='GRID SEARCH VISUALIZER')
 
         data_frm = LabelFrame(self.main_frm, text='DATA', fg='black', font=Formats.LABELFRAME_HEADER_FORMAT.value)
@@ -97,16 +79,14 @@
             self.plot_data[idx]['label'].grid(row=idx+1, column=0, sticky=NW)
             self.plot_data[idx]['variable'].grid(row=idx+1, column=1, sticky=NW)
         self.plot_table.grid(row=1, column=0, sticky=NW)
 
     def run(self):
         if len(self.plot_data.keys()) < 1:
             raise NoSpecifiedOutputError(msg='Specify at least one plot')
-        #check_if_dir_exists(in_dir=self.save_dir_select.folder_path)
-        #check_if_dir_exists(in_dir=self.data_dir_select.folder_path)
         settings = {}
         settings['SCATTER_SIZE'] = int(self.scatter_size_dropdown.getChoices())
         settings['CATEGORICAL_PALETTE'] = self.categorical_palette_dropdown.getChoices()
         settings['CONTINUOUS_PALETTE'] = self.continuous_palette_dropdown.getChoices()
 
         continuous_vars, categorical_vars = [], []
         for k, v in self.plot_data.items():
@@ -268,15 +248,15 @@
 
     def __get_settings(self):
         self.variance_selected = int(self.var_threshold_dropdown.getChoices()[:-1]) / 100
         self.save_path = self.save_dir.folder_path
         self.data_path = self.dataset_file_selected.file_path
         self.scaler = self.scaling_dropdown.getChoices()
         check_if_dir_exists(self.save_path)
-        check_if_dir_exists(self.data_path)
+        check_file_exist_and_readable(self.data_path)
 
 
 # _ = FitDimReductionPopUp()
 
 class TransformDimReductionPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='DIMENSIONALITY REDUCTION: TRANSFORM')
@@ -312,15 +292,15 @@
 
 #_ = TransformDimReductionPopUp()
 
 class FitClusterModelsPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='CLUSTERING FIT: GRID SEARCH')
         self.dataset_frm = LabelFrame(self.main_frm, text='DATASET', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.data_dir_selected = FolderSelect(self.dataset_frm, "DATA DIRECTORY: ", lblwidth=25)
+        self.data_dir_selected = FolderSelect(self.dataset_frm, "DATA DIRECTORY (PICKLES): ", lblwidth=25)
         self.save_frm = LabelFrame(self.main_frm, text='SAVE', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.save_dir = FolderSelect(self.save_frm, "SAVE DIRECTORY: ", lblwidth=25)
         self.algo_frm = LabelFrame(self.main_frm, text='ALGORITHM', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
         self.algo_dropdown = DropDownMenu(self.algo_frm, 'ALGORITHM:', UnsupervisedOptions.CLUSTERING_ALGO_OPTIONS.value, '25', com=lambda x: self.show_hyperparameters())
         self.algo_dropdown.setChoices(UnsupervisedOptions.CLUSTERING_ALGO_OPTIONS.value[0])
         self.value_frm = LabelFrame(self.main_frm, fg='black')
         self.value_entry_box = Entry_Box(self.value_frm, 'VALUE:', '25')
@@ -361,15 +341,15 @@
             epsilon_add_btn = Button(self.hyperparameters_frm, text='ADD', fg='blue', command=lambda: self.add_to_listbox_from_entrybox(list_box=self.epsilon_listbox, entry_box=self.value_entry_box))
 
             alpha_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command= lambda: self.remove_from_listbox(list_box=self.alpha_listbox))
             min_cluster_size_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.min_cluster_size_listbox))
             min_samples_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.min_samples_listbox))
             epsilon_remove_btn = Button(self.hyperparameters_frm, text='REMOVE', fg='red', command=lambda: self.remove_from_listbox(list_box=self.epsilon_listbox))
 
-            self.add_values_to_several_listboxes(list_boxes=[self.alpha_listbox, self.min_cluster_size_listbox, self.min_samples_listbox, self.epsilon_listbox], values= [15, 5, 0, 1])
+            self.add_values_to_several_listboxes(list_boxes=[self.alpha_listbox, self.min_cluster_size_listbox, self.min_samples_listbox, self.epsilon_listbox], values= [1, 15, 1, 1])
 
             self.hyperparameters_frm.grid(row=4, column=0, sticky=NW)
             alpha_add_btn.grid(row=2, column=0)
             min_cluster_size_add_btn.grid(row=2, column=1)
             min_samples_add_btn.grid(row=2, column=2)
             epsilon_add_btn.grid(row=2, column=3)
 
@@ -382,32 +362,32 @@
             self.min_cluster_size_listbox.grid(row=4, column=1, sticky=NW)
             self.min_samples_listbox.grid(row=4, column=2, sticky=NW)
             self.epsilon_listbox.grid(row=4, column=3, sticky=NW)
 
             self.create_run_frm(run_function=self.run_hdbscan_clustering)
 
     def __get_settings(self):
-        self.data_path = self.data_dir_selected.folder_path
-        self.save_dir = self.save_dir.folder_path
-        check_if_dir_exists(self.data_path)
-        check_if_dir_exists(self.save_dir)
+        self.data_directory = self.data_dir_selected.folder_path
+        self.save_directory = self.save_dir.folder_path
+        check_if_dir_exists(self.data_dir_selected.folder_path)
+        check_if_dir_exists(self.save_dir.folder_path)
 
 
     def run_hdbscan_clustering(self):
         self.__get_settings()
         alphas = [float(x) for x in self.alpha_listbox.get(0, END)]
         min_cluster_sizes = [int(x) for x in self.min_cluster_size_listbox.get(0, END)]
         min_samples = [int(x) for x in self.min_samples_listbox.get(0, END)]
         epsilons = [float(x) for x in self.epsilon_listbox.get(0, END)]
         hyper_parameters = {'alpha': alphas,
                             'min_cluster_size': min_cluster_sizes,
                             'min_samples': min_samples,
                             'cluster_selection_epsilon': epsilons}
         clusterer = HDBSCANClusterer()
-        clusterer.fit(data_path=self.data_path, save_dir=self.save_dir, hyper_parameters=hyper_parameters)
+        clusterer.fit(data_path=self.data_directory, save_dir=self.save_directory, hyper_parameters=hyper_parameters)
 
 #_ = FitClusterModelsPopUp()
 
 class TransformClustererPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='CLUSTERING: TRANSFORM')
         self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
@@ -446,15 +426,15 @@
 
 class ClusterVisualizerPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
         PopUpMixin.__init__(self, title='CLUSTER VIDEO VISUALIZATIONS')
         ConfigReader.__init__(self, config_path=config_path)
-        self.include_pose_var = BooleanVar(value=True)
+        self.include_pose_var = BooleanVar(value=False)
 
         self.data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.videos_dir_select = FolderSelect(self.data_frm, "VIDEOS DIRECTORY:", lblwidth=25)
         self.dataset_file_selected = FileSelect(self.data_frm, "DATASET (PICKLE): ", lblwidth=25)
         self.data_frm.grid(row=0, column=0, sticky=NW)
         self.videos_dir_select.grid(row=0, column=0, sticky=NW)
 
@@ -638,81 +618,53 @@
                                                    data_path=self.data_file_selected.file_path,
                                                    settings=settings)
         calculator.run()
 
 #_ = EmbedderCorrelationsPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
 
 
-#
-#
-# class PrintEmBeddingInfoPopUp(PopUpMixin):
-#     def __init__(self,
-#                  config_path: str):
-#         super().__init__(title='PRINT EMBEDDING MODEL INFO')
-#         self.config_path = config_path
-#         self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-#         self.dataset_file_selected = FileSelect(self.data_frm, "DATASET (PICKLE): ")
-#
-#         self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-#         run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
-#
-#         self.data_frm.grid(row=0, column=0, sticky=NW)
-#         self.dataset_file_selected.grid(row=0, column=0, sticky=NW)
-#         self.run_frm.grid(row=1, column=0, sticky=NW)
-#         run_btn.grid(row=1, column=0, sticky=NW)
-#
-#     def run(self):
-#         check_file_exist_and_readable(file_path=self.dataset_file_selected.file_path)
-#         data = read_pickle(data_path=self.dataset_file_selected.file_path)
-#         parameters = {**data['PARAMETERS'], **data['EMBEDDER']['PARAMETERS']}
-#         print(parameters)
-#
-# class DBCVPopUp(PopUpMixin):
-#     def __init__(self,
-#                  config_path: str):
-#         super().__init__(title='DENSITY BASED CLUSTER VALIDATION')
-#         self.config_path = config_path
-#
-#         self.data_frm = LabelFrame(self.main_frm, text='DATA', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-#         self.folder_selected = FolderSelect(self.data_frm, "DATASET (FOLDER WITH PICKLES): ")
-#
-#         self.run_frm = LabelFrame(self.main_frm, text='RUN', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-#         run_btn = Button(self.run_frm, text='RUN', fg='blue', command=lambda: self.run())
-#
-#         self.data_frm.grid(row=0, column=0, sticky=NW)
-#         self.folder_selected.grid(row=0, column=0, sticky=NW)
-#         self.run_frm.grid(row=1, column=0, sticky=NW)
-#         run_btn.grid(row=1, column=0, sticky=NW)
-#
-#     def run(self):
-#         check_if_dir_exists(in_dir=self.folder_selected.folder_path)
-#         data_paths = glob.glob(self.folder_selected.folder_path + '/*.pickle')
-#         check_if_filepath_list_is_empty(filepaths=data_paths, error_msg=f'No pickle files in {self.folder_selected.folder_path}')
-#         dbcv_calculator = DBCVCalculator(clusterers_path=self.folder_selected.folder_path, config_path=self.config_path)
-#         dbcv_calculator.run()
-
-
-
-
-
-#_ = PrintEmBeddingInfoPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
-
-
-
+class PrintEmBeddingInfoPopUp(PopUpMixin, ConfigReader, UnsupervisedMixin):
+    def __init__(self,
+                 config_path: str):
+        PopUpMixin.__init__(self, title='PRINT EMBEDDING MODEL INFO')
+        ConfigReader.__init__(self, config_path=config_path)
+        UnsupervisedMixin.__init__(self)
+        self.data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.dataset_file_selected = FileSelect(self.data_frm, "DATASET (PICKLE): ", lblwidth=25)
+        self.data_frm.grid(row=0, column=0, sticky=NW)
+        self.dataset_file_selected.grid(row=0, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
+        self.main_frm.mainloop()
 
-#_ = ClusterFrequentistStatisticsPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+    def run(self):
+        check_file_exist_and_readable(file_path=self.dataset_file_selected.file_path)
+        data = self.read_pickle(data_path=self.dataset_file_selected.file_path)
+        parameters = {**data[Unsupervised.DR_MODEL.value][Unsupervised.PARAMETERS.value]}
+        print(parameters)
 
+#_ = PrintEmBeddingInfoPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
 
-# settings = {'video_speed': 0.01, 'pose': {'include': True, 'circle_size': 5}}
-# test = ClusterVisualizer(video_dir='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/videos',
-#                          data_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models/dreamy_spence_awesome_elion.pickle',
-#                          settings=settings,
-#                          config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
-# test.create()
+class DBCVPopUp(PopUpMixin, ConfigReader, UnsupervisedMixin):
+    def __init__(self,
+                 config_path: str):
 
+        PopUpMixin.__init__(self, title='DENSITY BASED CLUSTER VALIDATION')
+        ConfigReader.__init__(self, config_path=config_path)
+        UnsupervisedMixin.__init__(self)
 
+        self.data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        self.folder_selected = FolderSelect(self.data_frm, "DATASETS (DIRECTORY WITH PICKLES):", lblwidth=35)
+        self.data_frm.grid(row=0, column=0, sticky=NW)
+        self.folder_selected.grid(row=0, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
 
+        self.main_frm.mainloop()
 
+    def run(self):
+        check_if_dir_exists(in_dir=self.folder_selected.folder_path)
+        data_paths = glob.glob(self.folder_selected.folder_path + '/*.pickle')
+        check_if_filepath_list_is_empty(filepaths=data_paths, error_msg=f'No pickle files in {self.folder_selected.folder_path}')
+        dbcv_calculator = DBCVCalculator(data_path=self.folder_selected.folder_path, config_path=self.config_path)
+        dbcv_calculator.run()
 
 
-#_ = BatchDataExtractorPopUp()
-#_ = GridSearchClusterVisualizerPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
+#_ = DBCVPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/bout_aggregator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 from joblib.externals.loky import get_reusable_executor
 from joblib import Parallel, delayed
+from simba.feature_extractors.unit_tests import read_video_info
 from simba.misc_tools import detect_bouts
 
 
 def bout_aggregator(data: pd.DataFrame,
                     clfs: list,
                     feature_names: list,
                     aggregator: str,
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/hdbscan_clusterer.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,15 @@
             save_dir: str,
             hyper_parameters: dict):
 
         self.save_dir, self.data_path = save_dir, data_path
         self.check_that_directory_is_empty(directory=self.save_dir)
         if os.path.isdir(data_path):
             check_if_dir_exists(in_dir=data_path)
-            self.data_path = glob.glob(data_path + '/*.pickle')
-            check_if_filepath_list_is_empty(filepaths=self.data_path, error_msg=f'SIMBA ERROR: No pickle files in {data_path}')
+            check_if_filepath_list_is_empty(filepaths=glob.glob(data_path + '/*.pickle'), error_msg=f'SIMBA ERROR: No pickle files in {data_path}')
         else:
             check_file_exist_and_readable(file_path=data_path)
             self.data_path = data_path
 
         self.search_space = list(itertools.product(*[hyper_parameters[Clustering.ALPHA.value],
                                                      hyper_parameters[Clustering.MIN_CLUSTER_SIZE.value],
                                                      hyper_parameters[Clustering.MIN_SAMPLES.value],
@@ -45,20 +44,22 @@
         self.embeddings = self.read_pickle(data_path=self.data_path)
         print(f'Fitting {str(len(self.search_space) * len(self.embeddings.keys()))} HDBSCAN model(s)...')
         self.__fit_hdbscan()
         self.timer.stop_timer()
         stdout_success(msg=f'{str(len(self.search_space) * len(self.embeddings.keys()))} saved in {self.save_dir}', elapsed_time=self.timer.elapsed_time_str)
 
     def __fit_hdbscan(self):
+        self.model_counter = 0
         for k, v in self.embeddings.items():
             fit_timer = SimbaTimer()
             fit_timer.start_timer()
             embedder = v[Unsupervised.DR_MODEL.value][Unsupervised.MODEL.value]
             for cnt, h in enumerate(self.search_space):
-                results, self.model, self.model_count = {}, {}, cnt
+                results, self.model = {}, {}
+                self.model_counter += 1
                 self.model_timer = SimbaTimer()
                 self.model_timer.start_timer()
                 self.model[Unsupervised.HASHED_NAME.value] = random.sample(self.model_names, 1)[0]
                 self.model[Unsupervised.PARAMETERS.value] = {Clustering.ALPHA.value: h[0],
                                                              Clustering.MIN_CLUSTER_SIZE.value: h[1],
                                                              Clustering.MIN_SAMPLES.value: h[2],
                                                              Clustering.EPSILON.value: h[3]}
@@ -78,15 +79,15 @@
                 results[Unsupervised.DR_MODEL.value] = v[Unsupervised.DR_MODEL.value]
                 results[Clustering.CLUSTER_MODEL.value] = self.model
                 self.__save(data=results)
 
     def __save(self, data: dict) -> None:
         self.write_pickle(data=data, save_path=os.path.join(self.save_dir, f'{self.model[Unsupervised.HASHED_NAME.value]}.pickle'))
         self.model_timer.stop_timer()
-        stdout_success(msg=f'Model {self.model_count + 1}/{len(self.search_space)} ({self.model[Unsupervised.HASHED_NAME.value]}) saved...', elapsed_time=self.model_timer.elapsed_time)
+        stdout_success(msg=f'Model {self.model_counter}/{len(self.search_space) * len(list(self.embeddings.keys()))} ({self.model[Unsupervised.HASHED_NAME.value]}) saved...', elapsed_time=self.model_timer.elapsed_time)
 
 
     def transform(self,
                   data_path: str,
                   model: str or dict,
                   save_dir: str or None=None,
                   settings: dict or None=None):
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.57.2/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/enums.py` & `Simba-UW-tf-dev-1.57.2/simba/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 0010 0000 000c  ................
 00001010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
 00001020: 0069 0073 0065 0064 6c67 3153 636f 6d70  .i.s.e.dlg1Scomp
-00001030: 0000 0000 0005 fd3a 0000 000c 0075 006e  .......:.....u.n
+00001030: 0000 0000 0005 d88e 0000 000c 0075 006e  .............u.n
 00001040: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
 00001050: 0065 0064 6c73 7643 626c 6f62 0000 0297  .e.dlsvCblob....
 00001060: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
 00001070: 0809 0a0b 1949 4a0a 4c5f 1012 7669 6577  .....IJ.L_..view
 00001080: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
 00001090: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 000010a0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
@@ -340,21 +340,21 @@
 00001530: 5a01 6301 6501 6601 6801 6901 7201 7401  Z.c.e.f.h.i.r.t.
 00001540: 7501 7701 7801 8101 8301 8401 8701 8801  u.w.x...........
 00001550: 9101 9201 9301 9401 9d01 a201 a300 0000  ................
 00001560: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 00001570: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 00001580: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
 00001590: 7600 6900 7300 6500 646d 6f44 4462 6c6f  v.i.s.e.dmoDDblo
-000015a0: 6200 0000 08b0 f569 2d29 f8c4 4100 0000  b......i-)..A...
+000015a0: 6200 0000 08f8 5284 dfc7 f8c4 4100 0000  b.....R.....A...
 000015b0: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
 000015c0: 7600 6900 7300 6500 646d 6f64 4462 6c6f  v.i.s.e.dmodDblo
-000015d0: 6200 0000 08b0 f569 2d29 f8c4 4100 0000  b......i-)..A...
+000015d0: 6200 0000 08f8 5284 dfc7 f8c4 4100 0000  b.....R.....A...
 000015e0: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
 000015f0: 7600 6900 7300 6500 6470 6831 5363 6f6d  v.i.s.e.dph1Scom
-00001600: 7000 0000 0000 0740 0000 0000 0c00 7500  p......@......u.
+00001600: 7000 0000 0000 0760 0000 0000 0c00 7500  p......`......u.
 00001610: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
 00001620: 7300 6500 6476 5372 6e6c 6f6e 6700 0000  s.e.dvSrnlong...
 00001630: 0100 0000 0500 7500 7400 6900 6c00 7362  ......u.t.i.l.sb
 00001640: 7773 7062 6c6f 6200 0000 c962 706c 6973  wspblob....bplis
 00001650: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
 00001660: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
 00001670: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
@@ -509,18 +509,18 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0013 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0042 0f84 0000 000b 005f 005f 0070  ...B......._._.p
+00002030: 0000 0042 1115 0000 000b 005f 005f 0070  ...B......._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 5692 9a09  moDDblob....V...
-00002060: 1cf8 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 4af4 9086  moDDblob....J...
+00002060: aef8 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00002080: 6444 626c 6f62 0000 0008 6a13 8953 eaf6  dDblob....j..S..
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 0050 0000 0000 0006  comp.....P......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
@@ -1049,21 +1049,21 @@
 00004180: 6465 6261 7208 0809 0809 5f10 187b 7b33  debar....._..{{3
 00004190: 3934 2c20 3138 317d 2c20 7b37 3730 2c20  94, 181}, {770, 
 000041a0: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
 000041b0: 7b7c 7d7e 9900 0000 0000 0001 0100 0000  {|}~............
 000041c0: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 000041d0: 0000 0000 9a00 0000 0600 6d00 6900 7800  ..........m.i.x.
 000041e0: 6900 6e00 736c 6731 5363 6f6d 7000 0000  i.n.slg1Scomp...
-000041f0: 0000 01aa ba00 0000 0600 6d00 6900 7800  ..........m.i.x.
+000041f0: 0000 01b8 da00 0000 0600 6d00 6900 7800  ..........m.i.x.
 00004200: 6900 6e00 736d 6f44 4462 6c6f 6200 0000  i.n.smoDDblob...
-00004210: 08cd 7da0 ce1e f8c4 4100 0000 0600 6d00  ..}.....A.....m.
+00004210: 0821 b3af 405b f8c4 4100 0000 0600 6d00  .!..@[..A.....m.
 00004220: 6900 7800 6900 6e00 736d 6f64 4462 6c6f  i.x.i.n.smodDblo
-00004230: 6200 0000 08cd 7da0 ce1e f8c4 4100 0000  b.....}.....A...
+00004230: 6200 0000 0821 b3af 405b f8c4 4100 0000  b....!..@[..A...
 00004240: 0600 6d00 6900 7800 6900 6e00 7370 6831  ..m.i.x.i.n.sph1
-00004250: 5363 6f6d 7000 0000 0000 01f0 0000 0000  Scomp...........
+00004250: 5363 6f6d 7000 0000 0000 0210 0000 0000  Scomp...........
 00004260: 0600 6d00 6900 7800 6900 6e00 7376 5372  ..m.i.x.i.n.svSr
 00004270: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
 00004280: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
 00004290: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
 000042a0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000042b0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 000042c0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
@@ -1885,15 +1885,15 @@
 000075c0: e500 0000 0000 0002 0100 0000 0000 0000  ................
 000075d0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
 000075e0: e600 0000 0700 0000 0e00 7000 6f00 7300  ..........p.o.s.
 000075f0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00007600: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
 00007610: 0100 0000 0800 0000 0c00 7500 6e00 7300  ..........u.n.s.
 00007620: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-00007630: 6464 7363 6c62 6f6f 6c01 0009 0072 006f  ddsclbool....r.o
+00007630: 6464 7363 6c62 6f6f 6c00 0009 0072 006f  ddsclbool....r.o
 00007640: 0069 005f 0074 006f 006f 006c 0073 6d6f  .i._.t.o.o.l.smo
 00007650: 4444 626c 6f62 0000 0008 6030 99e3 46f2  DDblob....`0..F.
 00007660: c441 0000 0009 0072 006f 0069 005f 0074  .A.....r.o.i._.t
 00007670: 006f 006f 006c 0073 6d6f 6444 626c 6f62  .o.o.l.smodDblob
 00007680: 0000 0008 6030 99e3 46f2 c441 0000 0009  ....`0..F..A....
 00007690: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
 000076a0: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
@@ -2013,15 +2013,15 @@
 00007dc0: e500 0000 0000 0002 0100 0000 0000 0000  ................
 00007dd0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
 00007de0: e600 0000 0700 0000 0e00 7000 6f00 7300  ..........p.o.s.
 00007df0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00007e00: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
 00007e10: 0100 0000 0800 0000 0c00 7500 6e00 7300  ..........u.n.s.
 00007e20: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-00007e30: 6464 7363 6c62 6f6f 6c01 0009 0072 006f  ddsclbool....r.o
+00007e30: 6464 7363 6c62 6f6f 6c00 0009 0072 006f  ddsclbool....r.o
 00007e40: 0069 005f 0074 006f 006f 006c 0073 6d6f  .i._.t.o.o.l.smo
 00007e50: 4444 626c 6f62 0000 0008 6030 99e3 46f2  DDblob....`0..F.
 00007e60: c441 0000 0009 0072 006f 0069 005f 0074  .A.....r.o.i._.t
 00007e70: 006f 006f 006c 0073 6d6f 6444 626c 6f62  .o.o.l.smodDblob
 00007e80: 0000 0008 6030 99e3 46f2 c441 0000 0009  ....`0..F..A....
 00007e90: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
 00007ea0: 0073 7068 3153 636f 6d70 0000 0000 0005  .sph1Scomp......
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 000012d0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 000012e0: 6261 7208 0809 0809 5f10 177b 7b33 342c  bar....._..{{34,
 000012f0: 2039 307d 2c20 7b31 3031 352c 2037 3637   90}, {1015, 767
 00001300: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
 00001310: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
 00001320: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00001330: 0099 0000 0004 006d 0069 0073 0063 6c67  .......m.i.s.clg
-00001340: 3153 636f 6d70 0000 0000 0002 7de9 0000  1Scomp......}...
+00001340: 3153 636f 6d70 0000 0000 0002 e73a 0000  1Scomp.......:..
 00001350: 0004 006d 0069 0073 0063 6c73 7643 626c  ...m.i.s.clsvCbl
 00001360: 6f62 0000 02b0 6270 6c69 7374 3030 da01  ob....bplist00..
 00001370: 0203 0405 0607 0809 0a0b 0c0d 1848 4948  .............HIH
 00001380: 4a4b 0c5f 1012 7669 6577 4f70 7469 6f6e  JK._..viewOption
 00001390: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 000013a0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
 000013b0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
@@ -391,19 +391,19 @@
 00001860: 6b01 6d01 6e01 6f01 7801 7a01 7c01 7d01  k.m.n.o.x.z.|.}.
 00001870: 7e01 8701 8901 8b01 8c01 8d01 9601 9801  ~...............
 00001880: 9a01 9b01 9c01 a501 a701 a901 aa01 ab01  ................
 00001890: b401 b501 b801 b901 bb01 bc01 c501 ce01  ................
 000018a0: d301 dc00 0000 0000 0002 0100 0000 0000  ................
 000018b0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
 000018c0: 0001 dd00 0000 0400 6d00 6900 7300 636d  ........m.i.s.cm
-000018d0: 6f44 4462 6c6f 6200 0000 08d6 e178 04e6  oDDblob......x..
-000018e0: f6c4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
-000018f0: 6f64 4462 6c6f 6200 0000 081a 1af6 afc4  odDblob.........
-00001900: f6c4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
-00001910: 6831 5363 6f6d 7000 0000 0000 0360 0000  h1Scomp......`..
+000018d0: 6f44 4462 6c6f 6200 0000 083b a5ee 5cdb  oDDblob....;..\.
+000018e0: f8c4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
+000018f0: 6f64 4462 6c6f 6200 0000 083b a5ee 5cdb  odDblob....;..\.
+00001900: f8c4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
+00001910: 6831 5363 6f6d 7000 0000 0000 03d0 0000  h1Scomp.........
 00001920: 0000 0400 6d00 6900 7300 6376 5372 6e6c  ....m.i.s.cvSrnl
 00001930: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
 00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.57.2/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/requirements.txt` & `Simba-UW-tf-dev-1.57.2/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/severity_processor.py` & `Simba-UW-tf-dev-1.57.2/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.57.2/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.57.2/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.57.2/simba/mixins/config_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self.heatmap_location_dir = os.path.join(self.project_path, Paths.HEATMAP_LOCATION_DIR.value)
         self.line_plot_dir = os.path.join(self.project_path, Paths.LINE_PLOT_DIR.value)
         self.probability_plot_dir = os.path.join(self.project_path, Paths.PROBABILITY_PLOTS_DIR.value)
         self.gantt_plot_dir = os.path.join(self.project_path, Paths.GANTT_PLOT_DIR.value)
         self.path_plot_dir = os.path.join(self.project_path, Paths.PATH_PLOT_DIR.value)
         self.font = cv2.FONT_HERSHEY_COMPLEX
         self.roi_features_save_dir = os.path.join(self.project_path, Paths.ROI_FEATURES.value)
+        self.configs_meta_dir = os.path.join(self.project_path, 'configs')
         self.sklearn_plot_dir = os.path.join(self.project_path, Paths.SKLEARN_RESULTS.value)
         self.detailed_roi_data_dir = os.path.join(self.project_path, Paths.DETAILED_ROI_DATA_DIR.value)
         self.directing_animals_video_output_path = os.path.join(self.project_path, Paths.DIRECTING_BETWEEN_ANIMALS_OUTPUT_PATH.value)
         self.animal_cnt = read_config_entry(config=self.config, section=ReadConfig.GENERAL_SETTINGS.value, option=ReadConfig.ANIMAL_CNT.value, data_type=Dtypes.INT.value)
         self.clf_cnt = read_config_entry(self.config, ReadConfig.SML_SETTINGS.value, ReadConfig.TARGET_CNT.value, Dtypes.INT.value)
         self.clf_names = get_all_clf_names(config=self.config, target_cnt=self.clf_cnt)
         self.feature_file_paths = glob.glob(self.features_dir + '/*.' + self.file_type)
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.57.2/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.57.2/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.57.2/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.57.2/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.57.2/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.57.2/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.57.2/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/video_info_table.py` & `Simba-UW-tf-dev-1.57.2/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.57.2/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.57.2/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.57.2/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/utils/errors.py` & `Simba-UW-tf-dev-1.57.2/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/utils/printing.py` & `Simba-UW-tf-dev-1.57.2/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.57.2/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.2/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.57.2/simba/train_model_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,16 +95,18 @@
             df_concat = pd.concat([df_concat, df], axis=0).astype(np.float16)
     try:
         df_concat = df_concat.set_index('scorer').astype(np.float16)
     except KeyError:
         pass
     if len(df_concat) == 0:
         raise NoDataError(msg='SimBA found 0 annotated frames in the project_folder/csv/targets_inserted directory')
-    df_concat = df_concat.loc[:, ~df_concat.columns.str.contains('^Unnamed')]
+    df_concat = df_concat.loc[:, ~df_concat.columns.str.contains('^Unnamed')].astype(np.float16)
     timer.stop_timer()
+    data_size = df_concat.memory_usage(index=True).sum()
+    print(f'Dataset size: {round(data_size / 1000000, 6)}MB / {round(data_size / 1000000000, 6)}GB')
     print('{} file(s) read (elapsed time: {}s) ...'.format(str(len(file_paths)), timer.elapsed_time_str))
     return df_concat.reset_index(drop=True).astype(np.float16)
 
 
 def read_in_all_model_names_to_remove(config, model_cnt, clf_name):
     """
     Helper to find all field names that contain annotations but are not the target.
@@ -1083,14 +1085,15 @@
                 df_lst.append(res)
         df_concat = pd.concat(df_lst, axis=0).astype(np.float16)
         if 'scorer' in df_concat.columns:
             df_concat = df_concat.set_index('scorer')
         if len(df_concat) == 0:
             raise ValueError('ANNOTATION ERROR: SimBA found 0 observations (frames) in the project_folder/csv/targets_inserted directory')
         df_concat = df_concat.loc[:, ~df_concat.columns.str.contains('^Unnamed')].astype(np.float16)
-        #print(df_concat.memory_usage(index=True).sum())
+        data_size = df_concat.memory_usage(index=True).sum()
+        print(f'Dataset size: {round(data_size/1000000, 6)}MB / {round(data_size/1000000000, 6)}GB')
         return df_concat.reset_index(drop=True)
 
     except BrokenProcessPool:
         return read_all_files_in_folder(file_paths=file_paths,
                                         file_type=file_type,
                                         classifier_names=classifier_names)
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.57.2/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.57.2/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.57.2/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/movement_processor.py` & `Simba-UW-tf-dev-1.57.2/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pybursts.py` & `Simba-UW-tf-dev-1.57.2/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.57.2/simba/rw_dfs.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.57.2/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.57.2/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.57.2/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.57.2/simba/tkinter_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 __author__ = "Simon Nilsson", "JJ Choong"
 
 from tkinter import *
 import platform
-from simba.enums import Defaults
+from simba.enums import Defaults, Formats
 from tkinter.filedialog import askopenfilename, askdirectory
 from simba.utils.lookups import get_icons_paths
 from PIL import ImageTk
 import PIL.Image
-from simba.enums import Formats
 import webbrowser
 
 MENU_ICONS = get_icons_paths()
 
 def onMousewheel(event, canvas):
     try:
         scrollSpeed = event.delta
@@ -268,12 +267,33 @@
                     cmd: object or None=None):
 
     scale = Scale(parent, from_=min, to=max, orient=HORIZONTAL, length=200, label=name, command=cmd)
     scale.set(0)
     return scale
 
 
-
-
-
+class TwoOptionQuestionPopUp(object):
+    def __init__(self,
+                 question: str,
+                 option_one: str,
+                 option_two: str,
+                 title: str
+                 ):
+
+        self.main_frm = Toplevel()
+        self.main_frm.geometry('600x200')
+        self.main_frm.title(title)
+
+        question_frm = Frame(self.main_frm)
+        question_frm.pack(expand=True, fill='both')
+        Label(question_frm, text=question, font=Formats.LABELFRAME_HEADER_FORMAT.value).pack()
+        button_one = Button(question_frm, text=option_one, fg='blue', command= lambda: self.run(option_one))
+        button_two = Button(question_frm, text=option_two, fg='red', command=lambda: self.run(option_two))
+        button_one.place(relx=0.5, rely=0.50, anchor=CENTER)
+        button_two.place(relx=0.5, rely=0.70, anchor=CENTER)
+        self.main_frm.wait_window()
+
+    def run(self, selected_option):
+        self.selected_option = selected_option
+        self.main_frm.destroy()
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/setting_menu.py` & `Simba-UW-tf-dev-1.57.2/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.57.2/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/run_inference.py` & `Simba-UW-tf-dev-1.57.2/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.57.2/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.57.2/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/dash_app.py` & `Simba-UW-tf-dev-1.57.2/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.57.2/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.57.2/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.57.2/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/misc_tools.py` & `Simba-UW-tf-dev-1.57.2/simba/misc_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1453,32 +1453,13 @@
 def create_logger(path: str):
     logger = logging.getLogger()
     logger.setLevel(logging.INFO)
     handler = logging.FileHandler(filename=path, encoding='utf-8')  # or whatever
     handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s %(message)s'))
     logger.addHandler(handler)
 
-
-    #
-    #
-    # logger = logging.getLogger("test")
-    # logger.setLevel(level=logging.WARNING)
-    # log_format = logging.Formatter(fmt=f"%(levelname)s %(asctime)s (%(relativeCreated)d) \t %(pathname)s %(funcName)s L%(lineno)s - %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
-    # log_file = logging.FileHandler(filename=path)
-    # log_file.setFormatter(log_format)
-    # log_file.setLevel(level=logging.INFO)
-    # logger.addHandler(log_file)
-    #
-    #
-    #
-
-# logging.basicConfig(filename='example.log',level=logging.DEBUG)
-
-
-
-
-
-
-
-# run_user_defined_feature_extraction_class(file_path='/Users/simon/Desktop/envs/simba_dev/simba/features_scripts/misc/fish_feature_extractor.py',
-#                                           config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/zebrafish/project_folder/project_config.ini')
-
+def get_memory_usage_of_df(df: pd.DataFrame) -> dict:
+    results = {}
+    results['bytes'] = df.memory_usage(index=True).sum()
+    results['megabytes'] = round(results['bytes'] / 1000000, 6)
+    results['gigabytes'] = round(results['bytes'] / 1000000000, 6)
+    return results
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.2/simba/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.57.2/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.57.2/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.57.2/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/pose_reset.py` & `Simba-UW-tf-dev-1.57.2/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.57.2/simba/train_mutiple_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __author__ = "Simon Nilsson"
 
-import os, glob, ast
-from simba.train_model_functions import (read_all_files_in_folder,
-                                         read_in_all_model_names_to_remove,
+import os, glob
+
+import pandas as pd
+from simba.train_model_functions import (read_in_all_model_names_to_remove,
                                          delete_other_annotation_columns,
                                          split_df_to_x_y,
                                          random_undersampler,
                                          smoteen_oversampler,
                                          smote_oversampler,
                                          calc_permutation_importance,
                                          calc_learning_curve,
@@ -28,34 +29,32 @@
 
 from simba.read_config_unit_tests import (check_int,
                                           check_str,
                                           check_float,
                                           read_config_entry,
                                           read_simba_meta_files,
                                           read_meta_file,
-                                          read_config_file,
                                           check_if_filepath_list_is_empty,
-                                          check_if_valid_input,
-                                          read_project_path_and_file_type)
+                                          check_if_valid_input)
+
+from simba.tkinter_functions import TwoOptionQuestionPopUp
 from simba.utils.printing import stdout_success
 from simba.drop_bp_cords import drop_bp_cords
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
-from simba.utils.errors import InvalidInputError
+from simba.utils.errors import InvalidInputError, NoDataError
 from simba.enums import (Options,
                          ReadConfig,
-                         Paths,
                          Dtypes,
                          Methods,
-                         MetaKeys,
-                         Defaults,
-                         TagNames)
+                         MetaKeys)
+from simba.mixins.config_reader import ConfigReader
 
 
-class TrainMultipleModelsFromMeta(object):
+class TrainMultipleModelsFromMeta(ConfigReader):
     """
     Class for grid-searching random forest models from hyperparameter setting and sampling methods
     stored within the `project_folder/configs` directory of a SimBA project.
 
     Parameters
     ----------
     config_path: str
@@ -66,158 +65,180 @@
     >>> model_trainer = TrainMultipleModelsFromMeta(config_path='MyConfigPath')
     >>> model_trainer.train_models_from_meta()
     """
 
     def __init__(self,
                  config_path: str):
 
-        self.config = read_config_file(ini_path=config_path)
-        self.ini_path = config_path
-        self.project_path, self.file_type = read_project_path_and_file_type(config=self.config)
-        self.data_in_path = os.path.join(self.project_path, Paths.TARGETS_INSERTED_DIR.value)
+        ConfigReader.__init__(self, config_path=config_path)
+
         self.model_dir_out = os.path.join(read_config_entry(self.config, ReadConfig.SML_SETTINGS.value, ReadConfig.MODEL_DIR.value, data_type=Dtypes.STR.value), 'validations')
         if not os.path.exists(self.model_dir_out): os.makedirs(self.model_dir_out)
-        self.model_cnt = read_config_entry(self.config, ReadConfig.SML_SETTINGS.value, ReadConfig.TARGET_CNT.value, data_type=Dtypes.INT.value)
-        self.annotation_file_paths = glob.glob(self.data_in_path + '/*.' + self.file_type)
-        self.meta_files_folder = os.path.join(self.project_path, 'configs')
-        if not os.path.exists(self.meta_files_folder): os.makedirs(self.meta_files_folder)
-        self.meta_file_lst = sorted(read_simba_meta_files(self.meta_files_folder))
-        self.annotation_file_paths = glob.glob(self.data_in_path + '/*.' + self.file_type)
-        check_if_filepath_list_is_empty(filepaths=self.annotation_file_paths,
-                                        error_msg='SIMBA ERROR: Zero annotation files found in project_folder/csv/targets_inserted, cannot create models.')
-        print('Reading in {} annotated files...'.format(str(len(self.annotation_file_paths))))
-        self.in_df = read_all_files_in_folder_mp(self.annotation_file_paths, self.file_type)
-        self.data_df_wo_cords = drop_bp_cords(self.in_df, config_path)
-
-    def perform_sampling(self):
-        if self.tt_split_type == Methods.SPLIT_TYPE_FRAMES.value:
-            self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(self.x_df, self.y_df, test_size=self.meta_dict['train_test_size'])
-        elif self.tt_split_type == Methods.SPLIT_TYPE_BOUTS.value:
-            self.x_train, self.x_test, self.y_train, self.y_test = bout_train_test_splitter(x_df=self.x_df, y_df=self.y_df, test_size=self.meta_dict['train_test_size'])
+        check_if_filepath_list_is_empty(filepaths=self.target_file_paths,
+                                        error_msg='Zero annotation files found in project_folder/csv/targets_inserted, cannot create models.')
+        if not os.path.exists(self.configs_meta_dir): os.makedirs(self.configs_meta_dir)
+        self.meta_file_lst = sorted(read_simba_meta_files(self.configs_meta_dir))
+        print('Reading in {} annotated files...'.format(str(len(self.target_file_paths))))
+        self.data_df = read_all_files_in_folder_mp(self.target_file_paths, self.file_type)
+        self.data_df = drop_bp_cords(self.data_df, config_path)
+
+    def perform_sampling(self, meta_dict: dict):
+        if meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value] == Methods.SPLIT_TYPE_FRAMES.value:
+            self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(self.x_df, self.y_df, test_size=meta_dict['train_test_size'])
+        elif meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value] == Methods.SPLIT_TYPE_BOUTS.value:
+            self.x_train, self.x_test, self.y_train, self.y_test = bout_train_test_splitter(x_df=self.x_df, y_df=self.y_df, test_size=meta_dict['train_test_size'])
         else:
-            raise InvalidInputError(msg=f'{self.tt_split_type} is not recognized as a valid SPLIT TYPE (OPTIONS: FRAMES, BOUTS')
-        if self.meta_dict[ReadConfig.UNDERSAMPLE_SETTING.value].lower() == Methods.RANDOM_UNDERSAMPLE.value:
-            self.x_train, self.y_train = random_undersampler(self.x_train, self.y_train, self.meta_dict[ReadConfig.UNDERSAMPLE_RATIO.value])
-        if self.meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower() == Methods.SMOTEENN.value:
-            self.x_train, self.y_train = smoteen_oversampler(self.x_train, self.y_train, self.meta_dict[ReadConfig.OVERSAMPLE_RATIO.value])
-        elif self.meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower() == Methods.SMOTE.value:
-            self.x_train, self.y_train = smote_oversampler(self.x_train, self.y_train, self.meta_dict[ReadConfig.OVERSAMPLE_RATIO.value])
-
-    def train_models_from_meta(self):
-        print(f'Training {str(len(self.meta_file_lst))} models...')
-        for config_cnt, file_path in enumerate(self.meta_file_lst):
-            print('Training model {}/{}...'.format(str(config_cnt+1), str(len(self.meta_file_lst))))
-            self.meta_dict = read_meta_file(file_path)
-            self.meta_dict = {k.lower(): v for k, v in self.meta_dict.items()}
-            check_str(name=self.meta_dict[MetaKeys.CLF_NAME.value], value=self.meta_dict[MetaKeys.CLF_NAME.value])
-            check_int(name=MetaKeys.RF_ESTIMATORS.value, value=self.meta_dict[MetaKeys.RF_ESTIMATORS.value], min_value=1)
-            check_str(name=MetaKeys.CRITERION.value, value=self.meta_dict[MetaKeys.CRITERION.value], options=Options.CLF_CRITERION.value)
-            check_str(name=MetaKeys.RF_MAX_FEATURES.value, value=self.meta_dict[MetaKeys.RF_MAX_FEATURES.value], options=Options.CLF_MAX_FEATURES.value)
-            check_float(name=MetaKeys.TT_SIZE.value, value=self.meta_dict[MetaKeys.TT_SIZE.value])
-            check_int(name=MetaKeys.MIN_LEAF.value, value=self.meta_dict[MetaKeys.MIN_LEAF.value])
-            check_if_valid_input(name=MetaKeys.META_FILE.value, input=self.meta_dict[MetaKeys.META_FILE.value], options=Options.RUN_OPTIONS_FLAGS.value)
-            check_if_valid_input(MetaKeys.EX_DECISION_TREE.value, input=self.meta_dict[MetaKeys.EX_DECISION_TREE.value], options=Options.RUN_OPTIONS_FLAGS.value)
-            check_if_valid_input(MetaKeys.CLF_REPORT.value, input=self.meta_dict[MetaKeys.CLF_REPORT.value], options=Options.RUN_OPTIONS_FLAGS.value)
-            check_if_valid_input(MetaKeys.IMPORTANCE_LOG.value, input=self.meta_dict[MetaKeys.IMPORTANCE_LOG.value], options=Options.RUN_OPTIONS_FLAGS.value)
-            check_if_valid_input(MetaKeys.IMPORTANCE_BAR_CHART.value, input=self.meta_dict[MetaKeys.IMPORTANCE_BAR_CHART.value], options=Options.RUN_OPTIONS_FLAGS.value)
-            check_if_valid_input(MetaKeys.PERMUTATION_IMPORTANCE.value, input=self.meta_dict[MetaKeys.PERMUTATION_IMPORTANCE.value], options=Options.RUN_OPTIONS_FLAGS.value)
-            check_if_valid_input(MetaKeys.LEARNING_CURVE.value, input=self.meta_dict[MetaKeys.LEARNING_CURVE.value], options=Options.RUN_OPTIONS_FLAGS.value)
-            check_if_valid_input(MetaKeys.PRECISION_RECALL.value, input=self.meta_dict[MetaKeys.PRECISION_RECALL.value], options=Options.RUN_OPTIONS_FLAGS.value)
-            check_str(ReadConfig.UNDERSAMPLE_SETTING.value, self.meta_dict[ReadConfig.UNDERSAMPLE_SETTING.value].lower(), options=[x.lower() for x in Options.UNDERSAMPLE_OPTIONS.value])
-            check_str(ReadConfig.OVERSAMPLE_SETTING.value, self.meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower(), options=[x.lower() for x in Options.OVERSAMPLE_OPTIONS.value])
-            if self.meta_dict[MetaKeys.RF_MAX_FEATURES.value] == Dtypes.NONE.value:
-                self.meta_dict[MetaKeys.RF_MAX_FEATURES.value] = None
-            if self.meta_dict[MetaKeys.LEARNING_CURVE.value] in Options.PERFORM_FLAGS.value:
-                check_int(name=MetaKeys.LEARNING_CURVE_K_SPLITS.value, value=self.meta_dict[MetaKeys.LEARNING_CURVE_K_SPLITS.value])
-                check_int(name=MetaKeys.LEARNING_CURVE_DATA_SPLITS.value, value=self.meta_dict[MetaKeys.LEARNING_CURVE_DATA_SPLITS.value])
-            if self.meta_dict[MetaKeys.IMPORTANCE_BAR_CHART.value] in Options.PERFORM_FLAGS.value:
-                check_int(name=MetaKeys.N_FEATURE_IMPORTANCE_BARS.value, value=self.meta_dict[MetaKeys.N_FEATURE_IMPORTANCE_BARS.value])
-            if MetaKeys.SHAP_SCORES.value in self.meta_dict.keys():
-                if self.meta_dict[MetaKeys.SHAP_SCORES.value] in Options.PERFORM_FLAGS.value:
-                    check_int(name=MetaKeys.SHAP_PRESENT.value, value=self.meta_dict[MetaKeys.SHAP_PRESENT.value])
-                    check_int(name=MetaKeys.SHAP_ABSENT.value, value=self.meta_dict[MetaKeys.SHAP_ABSENT.value])
-            if MetaKeys.PARTIAL_DEPENDENCY.value in self.meta_dict.keys():
-                check_if_valid_input(MetaKeys.PARTIAL_DEPENDENCY.value, input=self.meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value],options=Options.RUN_OPTIONS_FLAGS.value)
-            if self.meta_dict[ReadConfig.UNDERSAMPLE_SETTING.value].lower() == Methods.RANDOM_UNDERSAMPLE.value:
-                check_float(name=ReadConfig.UNDERSAMPLE_RATIO.value, value=self.meta_dict[ReadConfig.UNDERSAMPLE_RATIO.value])
-            if (self.meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower() == Methods.SMOTEENN.value.lower()) or (self.meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower() == Methods.SMOTE.value.lower()):
-                check_float(name=ReadConfig.OVERSAMPLE_RATIO.value, value=self.meta_dict[ReadConfig.OVERSAMPLE_RATIO.value])
-
-            if ReadConfig.CLASS_WEIGHTS.value in self.meta_dict.keys():
-                class_weights = self.meta_dict[ReadConfig.CLASS_WEIGHTS.value]
-                if class_weights == 'custom':
-                    class_weights = self.meta_dict['custom_weights']
-                    for k, v in class_weights.items():
-                        class_weights[k] = int(v)
-                if class_weights == Dtypes.NONE.value:
-                    class_weights = None
+            raise InvalidInputError(msg=f'{meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value]} is not recognized as a valid SPLIT TYPE (OPTIONS: FRAMES, BOUTS')
+        if meta_dict[ReadConfig.UNDERSAMPLE_SETTING.value].lower() == Methods.RANDOM_UNDERSAMPLE.value:
+            self.x_train, self.y_train = random_undersampler(self.x_train, self.y_train, meta_dict[ReadConfig.UNDERSAMPLE_RATIO.value])
+        if meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower() == Methods.SMOTEENN.value:
+            self.x_train, self.y_train = smoteen_oversampler(self.x_train, self.y_train, meta_dict[ReadConfig.OVERSAMPLE_RATIO.value])
+        elif meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower() == Methods.SMOTE.value:
+            self.x_train, self.y_train = smote_oversampler(self.x_train, self.y_train, meta_dict[ReadConfig.OVERSAMPLE_RATIO.value])
+
+    def __check_validity_of_meta_files(self, meta_file_paths: list):
+        meta_dicts, errors = {}, []
+        for config_cnt, path in enumerate(meta_file_paths):
+            meta_dict = read_meta_file(path)
+            meta_dict = {k.lower(): v for k, v in meta_dict.items()}
+            errors.append(check_str(name=meta_dict[MetaKeys.CLF_NAME.value], value=meta_dict[MetaKeys.CLF_NAME.value], raise_error=False)[1])
+            errors.append(check_str(name=MetaKeys.CRITERION.value, value=meta_dict[MetaKeys.CRITERION.value], options=Options.CLF_CRITERION.value, raise_error=False)[1])
+            errors.append(check_str(name=MetaKeys.RF_MAX_FEATURES.value, value=meta_dict[MetaKeys.RF_MAX_FEATURES.value], options=Options.CLF_MAX_FEATURES.value, raise_error=False)[1])
+            errors.append(check_str(ReadConfig.UNDERSAMPLE_SETTING.value, meta_dict[ReadConfig.UNDERSAMPLE_SETTING.value].lower(), options=[x.lower() for x in Options.UNDERSAMPLE_OPTIONS.value], raise_error=False)[1])
+            errors.append(check_str(ReadConfig.OVERSAMPLE_SETTING.value, meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower(), options=[x.lower() for x in Options.OVERSAMPLE_OPTIONS.value], raise_error=False)[1])
+            if MetaKeys.TRAIN_TEST_SPLIT_TYPE.value in meta_dict.keys():
+                errors.append(check_str(name=meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value], value=meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value], options=Options.TRAIN_TEST_SPLIT.value, raise_error=False)[1])
+
+            errors.append(check_int(name=MetaKeys.RF_ESTIMATORS.value, value=meta_dict[MetaKeys.RF_ESTIMATORS.value], min_value=1, raise_error=False)[1])
+            errors.append(check_int(name=MetaKeys.MIN_LEAF.value, value=meta_dict[MetaKeys.MIN_LEAF.value], raise_error=False)[1])
+            if meta_dict[MetaKeys.LEARNING_CURVE.value] in Options.PERFORM_FLAGS.value:
+                errors.append(check_int(name=MetaKeys.LEARNING_CURVE_K_SPLITS.value, value=meta_dict[MetaKeys.LEARNING_CURVE_K_SPLITS.value], raise_error=False)[1])
+                errors.append(check_int(name=MetaKeys.LEARNING_CURVE_DATA_SPLITS.value, value=meta_dict[MetaKeys.LEARNING_CURVE_DATA_SPLITS.value], raise_error=False)[1])
+            if meta_dict[MetaKeys.IMPORTANCE_BAR_CHART.value] in Options.PERFORM_FLAGS.value:
+                errors.append(check_int(name=MetaKeys.N_FEATURE_IMPORTANCE_BARS.value, value=meta_dict[MetaKeys.N_FEATURE_IMPORTANCE_BARS.value], raise_error=False)[1])
+            if MetaKeys.SHAP_SCORES.value in meta_dict.keys():
+                if meta_dict[MetaKeys.SHAP_SCORES.value] in Options.PERFORM_FLAGS.value:
+                    errors.append(check_int(name=MetaKeys.SHAP_PRESENT.value, value=meta_dict[MetaKeys.SHAP_PRESENT.value], raise_error=False)[1])
+                    errors.append(check_int(name=MetaKeys.SHAP_ABSENT.value, value=meta_dict[MetaKeys.SHAP_ABSENT.value], raise_error=False)[1])
+
+            errors.append(check_float(name=MetaKeys.TT_SIZE.value, value=meta_dict[MetaKeys.TT_SIZE.value], raise_error=False)[1])
+            if meta_dict[ReadConfig.UNDERSAMPLE_SETTING.value].lower() == Methods.RANDOM_UNDERSAMPLE.value:
+                errors.append(check_float(name=ReadConfig.UNDERSAMPLE_RATIO.value, value=meta_dict[ReadConfig.UNDERSAMPLE_RATIO.value], raise_error=False)[1])
+                try:
+                    present_len, absent_len = len(self.data_df[self.data_df[meta_dict[MetaKeys.CLF_NAME.value]] == 1]), len(self.data_df[self.data_df[meta_dict[MetaKeys.CLF_NAME.value]] == 0])
+                    ratio_n = int(present_len * meta_dict[ReadConfig.UNDERSAMPLE_RATIO.value])
+                    if absent_len < ratio_n:
+                        errors.append(f'The under-sample ratio of {meta_dict[ReadConfig.UNDERSAMPLE_RATIO.value]} in \n classifier {meta_dict[MetaKeys.CLF_NAME.value]} demands {ratio_n} behavior-absent annotations.')
+                except:
+                    pass
+
+            if (meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower() == Methods.SMOTEENN.value.lower()) or (meta_dict[ReadConfig.OVERSAMPLE_SETTING.value].lower() == Methods.SMOTE.value.lower()):
+                errors.append(check_float(name=ReadConfig.OVERSAMPLE_RATIO.value, value=meta_dict[ReadConfig.OVERSAMPLE_RATIO.value], raise_error=False)[1])
+
+            errors.append(check_if_valid_input(name=MetaKeys.META_FILE.value, input=meta_dict[MetaKeys.META_FILE.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            errors.append(check_if_valid_input(MetaKeys.EX_DECISION_TREE.value, input=meta_dict[MetaKeys.EX_DECISION_TREE.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            errors.append(check_if_valid_input(MetaKeys.CLF_REPORT.value, input=meta_dict[MetaKeys.CLF_REPORT.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            errors.append(check_if_valid_input(MetaKeys.IMPORTANCE_LOG.value, input=meta_dict[MetaKeys.IMPORTANCE_LOG.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            errors.append(check_if_valid_input(MetaKeys.IMPORTANCE_BAR_CHART.value, input=meta_dict[MetaKeys.IMPORTANCE_BAR_CHART.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            errors.append(check_if_valid_input(MetaKeys.PERMUTATION_IMPORTANCE.value, input=meta_dict[MetaKeys.PERMUTATION_IMPORTANCE.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            errors.append(check_if_valid_input(MetaKeys.LEARNING_CURVE.value, input=meta_dict[MetaKeys.LEARNING_CURVE.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            errors.append(check_if_valid_input(MetaKeys.PRECISION_RECALL.value, input=meta_dict[MetaKeys.PRECISION_RECALL.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            if MetaKeys.PARTIAL_DEPENDENCY.value in meta_dict.keys():
+                errors.append(check_if_valid_input(MetaKeys.PARTIAL_DEPENDENCY.value, input=meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value],options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+
+            if meta_dict[MetaKeys.RF_MAX_FEATURES.value] == Dtypes.NONE.value: meta_dict[MetaKeys.RF_MAX_FEATURES.value] = None
+            if MetaKeys.TRAIN_TEST_SPLIT_TYPE.value not in meta_dict.keys(): meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value] = Methods.SPLIT_TYPE_FRAMES.value
+
+            if ReadConfig.CLASS_WEIGHTS.value in meta_dict.keys():
+                meta_dict[ReadConfig.CLASS_WEIGHTS.value] = meta_dict[ReadConfig.CLASS_WEIGHTS.value]
+                if meta_dict[ReadConfig.CLASS_WEIGHTS.value] == 'custom':
+                    meta_dict[ReadConfig.CLASS_WEIGHTS.value] = meta_dict['custom_weights']
+                    for k, v in meta_dict[ReadConfig.CLASS_WEIGHTS.value].items():
+                        meta_dict[ReadConfig.CLASS_WEIGHTS.value][k] = int(v)
+                if meta_dict[ReadConfig.CLASS_WEIGHTS.value] == Dtypes.NONE.value:
+                    meta_dict[ReadConfig.CLASS_WEIGHTS.value] = None
             else:
-                class_weights = None
+                meta_dict[ReadConfig.CLASS_WEIGHTS.value] = None
 
-            if MetaKeys.TRAIN_TEST_SPLIT_TYPE.value in self.meta_dict.keys():
-                check_str(name=self.meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value], value=self.meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value], options=Options.TRAIN_TEST_SPLIT.value)
-                self.tt_split_type = self.meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value]
+            errors = [x for x in errors if x != '']
+            if errors:
+                option = TwoOptionQuestionPopUp(question=f'{errors[0]} \n \n  Do you want to skip this meta file or terminate training ?',
+                                                title='META CONFIG FILE ERROR',
+                                                option_one='SKIP',
+                                                option_two='TERMINATE')
+
+                if option.selected_option == 'SKIP':
+                    continue
+                else:
+                    raise InvalidInputError(msg=errors[0])
             else:
-                self.tt_split_type = Methods.SPLIT_TYPE_FRAMES.value
+                meta_dicts[config_cnt] = meta_dict
 
-            self.clf_name = self.meta_dict[MetaKeys.CLF_NAME.value]
-            self.class_names = ['Not_' + self.clf_name, self.clf_name]
-            annotation_cols_to_remove = read_in_all_model_names_to_remove(self.config, self.model_cnt, self.clf_name)
-            self.x_y_df = delete_other_annotation_columns(self.data_df_wo_cords, annotation_cols_to_remove)
-            self.x_df, self.y_df = split_df_to_x_y(self.x_y_df, self.clf_name)
+        return meta_dicts
+
+    def run(self):
+        self.meta_dicts = self.__check_validity_of_meta_files(meta_file_paths=self.meta_file_lst)
+        if len(self.meta_dicts.keys()) == 0:
+            raise NoDataError(msg='No valid hyper-parameter config files')
+        for config_cnt, meta_dict in self.meta_dicts.items():
+            self.clf_name = meta_dict[MetaKeys.CLF_NAME.value]
+            print(f'Training model {config_cnt+1}/{len(self.meta_dicts.keys())} ({meta_dict[MetaKeys.CLF_NAME.value]})...')
+            self.class_names = [f'Not_{meta_dict[MetaKeys.CLF_NAME.value]}', meta_dict[MetaKeys.CLF_NAME.value]]
+            annotation_cols_to_remove = read_in_all_model_names_to_remove(self.config, self.clf_cnt, meta_dict[MetaKeys.CLF_NAME.value])
+            self.x_y_df = delete_other_annotation_columns(self.data_df, annotation_cols_to_remove)
+            self.x_df, self.y_df = split_df_to_x_y(self.x_y_df, meta_dict[MetaKeys.CLF_NAME.value])
             self.feature_names = self.x_df.columns
             check_dataset_integrity(x_df=self.x_df, y_df=self.y_df)
-            self.perform_sampling()
-            print('MODEL {} settings'.format(str(config_cnt)))
-            print_machine_model_information(self.meta_dict)
+            self.perform_sampling(meta_dict=meta_dict)
+            print(f'MODEL {config_cnt+1} settings')
+            print_machine_model_information(meta_dict)
             print('# {} features.'.format(len(self.feature_names)))
-
-            self.rf_clf = RandomForestClassifier(n_estimators=self.meta_dict[MetaKeys.RF_ESTIMATORS.value],
-                                                 max_features=self.meta_dict[MetaKeys.RF_MAX_FEATURES.value],
+            self.rf_clf = RandomForestClassifier(n_estimators=meta_dict[MetaKeys.RF_ESTIMATORS.value],
+                                                 max_features=meta_dict[MetaKeys.RF_MAX_FEATURES.value],
                                                  n_jobs=-1,
-                                                 criterion=self.meta_dict[MetaKeys.CRITERION.value],
-                                                 min_samples_leaf=self.meta_dict[MetaKeys.MIN_LEAF.value],
+                                                 criterion=meta_dict[MetaKeys.CRITERION.value],
+                                                 min_samples_leaf=meta_dict[MetaKeys.MIN_LEAF.value],
                                                  bootstrap=True,
                                                  verbose=1,
-                                                 class_weight=class_weights)
+                                                 class_weight=meta_dict[ReadConfig.CLASS_WEIGHTS.value])
 
             print(f'Fitting {self.clf_name} model...')
             self.rf_clf = clf_fit(clf=self.rf_clf, x_df=self.x_train, y_df=self.y_train)
-            if self.meta_dict[MetaKeys.PERMUTATION_IMPORTANCE.value] in Options.PERFORM_FLAGS.value:
+            if meta_dict[MetaKeys.PERMUTATION_IMPORTANCE.value] in Options.PERFORM_FLAGS.value:
                 calc_permutation_importance(self.x_test, self.y_test, self.rf_clf, self.feature_names, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
-            if self.meta_dict[MetaKeys.LEARNING_CURVE.value] in Options.PERFORM_FLAGS.value:
-                calc_learning_curve(self.x_y_df, self.clf_name, self.meta_dict[MetaKeys.LEARNING_CURVE_K_SPLITS.value], self.meta_dict[MetaKeys.LEARNING_CURVE_DATA_SPLITS.value], self.meta_dict[MetaKeys.TT_SIZE.value], self.rf_clf, self.model_dir_out, save_file_no=config_cnt)
-            if self.meta_dict[MetaKeys.PRECISION_RECALL.value] in Options.PERFORM_FLAGS.value:
+            if meta_dict[MetaKeys.LEARNING_CURVE.value] in Options.PERFORM_FLAGS.value:
+                calc_learning_curve(self.x_y_df, self.clf_name, meta_dict[MetaKeys.LEARNING_CURVE_K_SPLITS.value], meta_dict[MetaKeys.LEARNING_CURVE_DATA_SPLITS.value], meta_dict[MetaKeys.TT_SIZE.value], self.rf_clf, self.model_dir_out, save_file_no=config_cnt)
+            if meta_dict[MetaKeys.PRECISION_RECALL.value] in Options.PERFORM_FLAGS.value:
                 calc_pr_curve(self.rf_clf, self.x_test, self.y_test, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
-            if self.meta_dict[MetaKeys.EX_DECISION_TREE.value] in Options.PERFORM_FLAGS.value:
+            if meta_dict[MetaKeys.EX_DECISION_TREE.value] in Options.PERFORM_FLAGS.value:
                 create_example_dt(self.rf_clf, self.clf_name, self.feature_names, self.class_names, self.model_dir_out, save_file_no=config_cnt)
-            if self.meta_dict[MetaKeys.CLF_REPORT.value] in Options.PERFORM_FLAGS.value:
+            if meta_dict[MetaKeys.CLF_REPORT.value] in Options.PERFORM_FLAGS.value:
                 create_clf_report(self.rf_clf, self.x_test, self.y_test, self.class_names, self.model_dir_out, save_file_no=config_cnt)
-            if self.meta_dict[MetaKeys.IMPORTANCE_LOG.value] in Options.PERFORM_FLAGS.value:
+            if meta_dict[MetaKeys.IMPORTANCE_LOG.value] in Options.PERFORM_FLAGS.value:
                 create_x_importance_log(self.rf_clf, self.feature_names, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
-            if self.meta_dict[MetaKeys.IMPORTANCE_BAR_CHART.value] in Options.PERFORM_FLAGS.value:
-                create_x_importance_bar_chart(self.rf_clf, self.feature_names, self.clf_name, self.model_dir_out, self.meta_dict[MetaKeys.N_FEATURE_IMPORTANCE_BARS.value], save_file_no=config_cnt)
-            if MetaKeys.SHAP_SCORES.value in self.meta_dict.keys():
-                save_n = self.meta_dict[MetaKeys.SHAP_PRESENT.value] + self.meta_dict[MetaKeys.SHAP_ABSENT.value]
-                if MetaKeys.SHAP_SAVE_ITERATION.value in self.meta_dict.keys():
+            if meta_dict[MetaKeys.IMPORTANCE_BAR_CHART.value] in Options.PERFORM_FLAGS.value:
+                create_x_importance_bar_chart(self.rf_clf, self.feature_names, self.clf_name, self.model_dir_out, meta_dict[MetaKeys.N_FEATURE_IMPORTANCE_BARS.value], save_file_no=config_cnt)
+            if MetaKeys.SHAP_SCORES.value in meta_dict.keys():
+                save_n = meta_dict[MetaKeys.SHAP_PRESENT.value] + meta_dict[MetaKeys.SHAP_ABSENT.value]
+                if MetaKeys.SHAP_SAVE_ITERATION.value in meta_dict.keys():
                     try:
-                        save_n = int(self.meta_dict[MetaKeys.SHAP_SAVE_ITERATION.value])
+                        save_n = int(meta_dict[MetaKeys.SHAP_SAVE_ITERATION.value])
                     except ValueError:
-                        save_n = self.meta_dict[MetaKeys.SHAP_PRESENT.value] + self.meta_dict[MetaKeys.SHAP_ABSENT.value]
-                if self.meta_dict[MetaKeys.SHAP_SCORES.value] in Options.PERFORM_FLAGS.value:
-                    create_shap_log(self.ini_path, self.rf_clf, self.x_train, self.y_train, self.feature_names, self.clf_name, self.meta_dict[MetaKeys.SHAP_PRESENT.value], self.meta_dict[MetaKeys.SHAP_ABSENT.value], self.model_dir_out, save_it=save_n, save_file_no=config_cnt)
-            if MetaKeys.PARTIAL_DEPENDENCY.value in self.meta_dict.keys():
-                if self.meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value] in Options.PERFORM_FLAGS.value:
+                        save_n = meta_dict[MetaKeys.SHAP_PRESENT.value] + meta_dict[MetaKeys.SHAP_ABSENT.value]
+                if meta_dict[MetaKeys.SHAP_SCORES.value] in Options.PERFORM_FLAGS.value:
+                    create_shap_log(self.config_path, self.rf_clf, self.x_train, self.y_train, self.feature_names, self.clf_name, meta_dict[MetaKeys.SHAP_PRESENT.value], meta_dict[MetaKeys.SHAP_ABSENT.value], self.model_dir_out, save_it=save_n, save_file_no=config_cnt)
+            if MetaKeys.PARTIAL_DEPENDENCY.value in meta_dict.keys():
+                if meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value] in Options.PERFORM_FLAGS.value:
                     partial_dependence_calculator(clf=self.rf_clf, x_df=self.x_train, clf_name=self.clf_name, save_dir=self.model_dir_out)
-            create_meta_data_csv_training_multiple_models(self.meta_dict, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
+            create_meta_data_csv_training_multiple_models(meta_dict, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             save_rf_model(self.rf_clf, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             print('Classifier {} saved in models/validations/model_files directory ...'.format(str(self.clf_name + '_' + str(config_cnt))))
         stdout_success(msg='All models and evaluations complete. The models/evaluation files are in models/validations folders')
 
 # test = TrainMultipleModelsFromMeta(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini')
-# test.train_models_from_meta()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/SimBA.py` & `Simba-UW-tf-dev-1.57.2/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,15 +599,15 @@
         model_trainer = TrainSingleModel(config_path=config_path)
         model_trainer.perform_sampling()
         model_trainer.train_model()
         model_trainer.save_model()
 
     def train_multiple_models_from_meta(self, config_path=None):
         model_trainer = TrainMultipleModelsFromMeta(config_path=config_path)
-        model_trainer.train_models_from_meta()
+        model_trainer.run()
 
 
     def importBoris(self):
         ann_folder = askdirectory()
         boris_appender = BorisAppender(config_path=self.config_path, boris_folder=ann_folder)
         boris_appender.create_boris_master_file()
         boris_appender.run()
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.57.2/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/assets/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -484,274 +484,274 @@
 00001e30: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00001e40: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00001e50: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00001e60: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00001e70: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00001e80: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00001e90: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00001ea0: 01c5 22f4 c441 0000 0005 0069 0063 006f  .."..A.....i.c.o
-00001eb0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
-00001ec0: c1fc 2155 22f4 c441 0000 0005 0069 0063  ..!U"..A.....i.c
-00001ed0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
-00001ee0: 0000 0008 0000 0000 0005 0069 0063 006f  ...........i.c.o
-00001ef0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
-00001f00: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
-00001f10: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
-00001f20: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00001f30: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00001f40: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00001f50: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00001f60: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00001f70: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00001f80: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00001f90: 0809 0809 5f10 197b 7b33 3838 2c20 3231  ...._..{{388, 21
-00001fa0: 367d 2c20 7b31 3039 322c 2034 3232 7d7d  6}, {1092, 422}}
-00001fb0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-00001fc0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00001fd0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-00001fe0: 0000 0003 0069 006d 0067 6c67 3153 636f  .....i.m.glg1Sco
-00001ff0: 6d70 0000 0000 0011 10bf 0000 0003 0069  mp.............i
-00002000: 006d 0067 0000 0000 0000 0012 0000 0005  .m.g............
+00001ea0: 01c5 5522 f4c4 4100 0000 0500 6900 6300  ..U"..A.....i.c.
+00001eb0: 6f00 6e00 736d 6f64 4462 6c6f 6200 0000  o.n.smodDblob...
+00001ec0: 08c1 fc21 5522 f4c4 4100 0000 0500 6900  ...!U"..A.....i.
+00001ed0: 6300 6f00 6e00 7370 6831 5363 6f6d 7000  c.o.n.sph1Scomp.
+00001ee0: 0000 0000 0800 0000 0000 0500 6900 6300  ............i.c.
+00001ef0: 6f00 6e00 7376 5372 6e6c 6f6e 6700 0000  o.n.svSrnlong...
+00001f00: 0100 0000 0300 6900 6d00 6762 7773 7062  ......i.m.gbwspb
+00001f10: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
+00001f20: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
+00001f30: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+00001f40: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
+00001f50: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
+00001f60: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
+00001f70: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
+00001f80: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
+00001f90: 0808 0908 095f 1019 7b7b 3338 382c 2032  ....._..{{388, 2
+00001fa0: 3136 7d2c 207b 3130 3932 2c20 3432 327d  16}, {1092, 422}
+00001fb0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
+00001fc0: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
+00001fd0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
+00001fe0: 9b00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
+00001ff0: 6f6d 7000 0000 0000 1110 bf00 0000 0300  omp.............
+00002000: 6900 6d00 0000 0000 0000 0012 0000 0005  i.m.............
 00002010: 0069 0063 006f 006e 0073 6277 7370 626c  .i.c.o.n.sbwspbl
-00002020: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
+00002020: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00002030: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00002040: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002050: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00002060: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00002070: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00002080: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00002090: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000020a0: 0809 0809 5f10 187b 7b34 3134 2c20 3136  ...._..{{414, 16
-000020b0: 317d 2c20 7b37 3730 2c20 3433 367d 7d09  1}, {770, 436}}.
-000020c0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
-000020d0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-000020e0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
-000020f0: 0000 0500 6900 6300 6f00 6e00 736c 6731  ....i.c.o.n.slg1
-00002100: 5363 6f6d 7000 0000 0000 0598 d900 0000  Scomp...........
-00002110: 0500 6900 6300 6f00 6e00 736c 7376 4362  ..i.c.o.n.slsvCb
-00002120: 6c6f 6200 0002 af62 706c 6973 7430 30da  lob....bplist00.
-00002130: 0102 0304 0506 0708 090a 0b0c 0d1a 4849  ..............HI
-00002140: 484a 0c4c 5f10 1276 6965 774f 7074 696f  HJ.L_..viewOptio
-00002150: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-00002160: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00002170: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00002180: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-00002190: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-000021a0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-000021b0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
-000021c0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-000021d0: 6573 5869 636f 6e53 697a 6510 0109 ab0e  esXiconSize.....
-000021e0: 171c 2125 2a2f 3439 3e43 d40f 1011 1213  ..!%*/49>C......
-000021f0: 140c 0c5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
-00002200: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-00002210: 6973 6962 6c65 546e 616d 6510 ea09 09d4  isibleTname.....
-00002220: 0f10 1112 1819 1a1a 5875 6269 7175 6974  ........Xubiquit
-00002230: 7910 2308 08d4 0f10 1112 1d1e 1a0c 5c64  y.#...........\d
-00002240: 6174 654d 6f64 6966 6965 6410 b508 09d4  ateModified.....
-00002250: 0f10 1112 221e 1a1a 5b64 6174 6543 7265  ...."...[dateCre
-00002260: 6174 6564 0808 d40f 1011 1226 271a 0c54  ated.......&'..T
-00002270: 7369 7a65 1061 0809 d40f 1011 122b 2c0c  size.a.......+,.
-00002280: 0c54 6b69 6e64 1073 0909 d40f 1011 1230  .Tkind.s.......0
-00002290: 310c 1a55 6c61 6265 6c10 6409 08d4 0f10  1..Ulabel.d.....
-000022a0: 1112 3536 0c1a 5776 6572 7369 6f6e 104b  ..56..Wversion.K
-000022b0: 0908 d40f 1011 123a 3b0c 1a58 636f 6d6d  .......:;..Xcomm
-000022c0: 656e 7473 1101 2c09 08d4 0f10 1112 3f40  ents..,.......?@
-000022d0: 1a1a 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-000022e0: 6410 c808 08d4 0f10 1112 441e 1a1a 5964  d.........D...Yd
-000022f0: 6174 6541 6464 6564 0808 0823 0000 0000  ateAdded...#....
-00002300: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-00002310: 6d65 0923 4030 0000 0000 0000 0008 001d  me.#@0..........
-00002320: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
-00002330: 00ab 00b4 00b6 00b7 00c3 00cc 00d7 00dd  ................
-00002340: 00e7 00ef 00f4 00f6 00f7 00f8 0101 010a  ................
-00002350: 010c 010d 010e 0117 0124 0126 0127 0128  .........$.&.'.(
-00002360: 0131 013d 013e 013f 0148 014d 014f 0150  .1.=.>.?.H.M.O.P
-00002370: 0151 015a 015f 0161 0162 0163 016c 0172  .Q.Z._.a.b.c.l.r
-00002380: 0174 0175 0176 017f 0187 0189 018a 018b  .t.u.v..........
-00002390: 0194 019d 01a0 01a1 01a2 01ab 01ba 01bc  ................
-000023a0: 01bd 01be 01c7 01d1 01d2 01d3 01d4 01dd  ................
-000023b0: 01e6 01eb 01ec 0000 0000 0000 0201 0000  ................
-000023c0: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
-000023d0: 0000 0000 01f5 0000 0005 0069 0063 006f  ...........i.c.o
-000023e0: 006e 0073 6c73 7670 626c 6f62 0000 0294  .n.slsvpblob....
-000023f0: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00002400: 0809 0a0b 0c0d 1c47 4847 490c 4b5f 1012  .......GHGI.K_..
-00002410: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00002420: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00002430: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00002440: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00002450: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-00002460: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
-00002470: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
-00002480: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-00002490: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
-000024a0: 5369 7a65 1001 09d9 0e0f 1011 1213 1415  Size............
-000024b0: 1617 2025 292d 3237 3c41 5863 6f6d 6d65  .. %)-27<AXcomme
-000024c0: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
-000024d0: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
-000024e0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
-000024f0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
-00002500: 696f 6e54 6e61 6d65 d418 191a 1b1c 1d0c  ionTname........
-00002510: 1f57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
-00002520: 6173 6365 6e64 696e 6755 696e 6465 7808  ascendingUindex.
-00002530: 1101 2c09 1007 d418 191a 1b1c 221c 2408  ..,.........".$.
-00002540: 10c8 0810 08d4 1819 1a1b 0c27 1c0b 0910  ...........'....
-00002550: b508 d418 191a 1b1c 271c 2c08 0810 02d4  ........'.,.....
-00002560: 1819 1a1b 0c2f 1c31 0910 6108 1003 d418  ...../.1..a.....
-00002570: 191a 1b1c 340c 3608 1064 0910 05d4 1819  ....4.6..d......
-00002580: 1a1b 0c39 0c3b 0910 7309 1004 d418 191a  ...9.;..s.......
-00002590: 1b1c 3e0c 4008 104b 0910 06d4 1819 1a1b  ..>.@..K........
-000025a0: 0c43 0c45 0910 ea09 1000 0823 0000 0000  .C.E.......#....
-000025b0: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-000025c0: 6d65 0923 4030 0000 0000 0000 0008 001d  me.#@0..........
-000025d0: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
-000025e0: 00ab 00b4 00b6 00b7 00ca 00d3 00e2 00ef  ................
-000025f0: 00fb 0100 0106 010b 0113 0118 0121 0129  .............!.)
-00002600: 012f 0139 013f 0140 0143 0144 0146 014f  ./.9.?.@.C.D.F.O
-00002610: 0150 0152 0153 0155 015e 015f 0161 0162  .P.R.S.U.^._.a.b
-00002620: 016b 016c 016d 016f 0178 0179 017b 017c  .k.l.m.o.x.y.{.|
-00002630: 017e 0187 0188 018a 018b 018d 0196 0197  .~..............
-00002640: 0199 019a 019c 01a5 01a6 01a8 01a9 01ab  ................
-00002650: 01b4 01b5 01b7 01b8 01ba 01bb 01c4 01cd  ................
-00002660: 01d2 01d3 0000 0000 0000 0201 0000 0000  ................
-00002670: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
-00002680: 0000 01dc 0000 0005 0069 0063 006f 006e  .........i.c.o.n
-00002690: 0073 6d6f 4444 626c 6f62 0000 0008 c1fc  .smoDDblob......
-000026a0: 2155 22f4 c441 0000 0005 0069 0063 006f  !U"..A.....i.c.o
-000026b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
-000026c0: c1fc 2155 22f4 c441 0000 0005 0069 0063  ..!U"..A.....i.c
-000026d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
-000026e0: 0000 0008 0000 0000 0005 0069 0063 006f  ...........i.c.o
-000026f0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
-00002700: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
-00002710: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
-00002720: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00002730: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00002740: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00002750: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00002760: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00002770: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00002780: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00002790: 0809 0809 5f10 197b 7b33 3838 2c20 3231  ...._..{{388, 21
-000027a0: 367d 2c20 7b31 3039 322c 2034 3232 7d7d  6}, {1092, 422}}
-000027b0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-000027c0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-000027d0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-000027e0: 0000 0003 0069 006d 0067 6c67 3153 636f  .....i.m.glg1Sco
-000027f0: 6d70 0000 0000 0011 10bf 0000 0003 0069  mp.............i
-00002800: 006d 0067 6c73 7643 626c 6f62 0000 02b0  .m.glsvCblob....
-00002810: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00002820: 0809 0a0b 0c0d 1a48 4948 4a0c 4c5f 1012  .......HIHJ.L_..
-00002830: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00002840: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00002850: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00002860: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00002870: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-00002880: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
-00002890: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
-000028a0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-000028b0: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
-000028c0: 5369 7a65 1001 09ab 0e17 1c21 252a 2f34  Size.......!%*/4
-000028d0: 393e 43d4 0f10 1112 1314 0c0c 5a69 6465  9>C.........Zide
-000028e0: 6e74 6966 6965 7255 7769 6474 6859 6173  ntifierUwidthYas
-000028f0: 6365 6e64 696e 6757 7669 7369 626c 6554  cendingWvisibleT
-00002900: 6e61 6d65 1101 3709 09d4 0f10 1112 1819  name..7.........
-00002910: 1a1a 5875 6269 7175 6974 7910 2308 08d4  ..Xubiquity.#...
-00002920: 0f10 1112 1d1e 1a0c 5c64 6174 654d 6f64  ........\dateMod
-00002930: 6966 6965 6410 b508 09d4 0f10 1112 221e  ified.........".
-00002940: 1a1a 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
-00002950: d40f 1011 1226 271a 0c54 7369 7a65 1061  .....&'..Tsize.a
-00002960: 0809 d40f 1011 122b 2c0c 0c54 6b69 6e64  .......+,..Tkind
-00002970: 1073 0909 d40f 1011 1230 310c 1a55 6c61  .s.......01..Ula
-00002980: 6265 6c10 6409 08d4 0f10 1112 3536 0c1a  bel.d.......56..
-00002990: 5776 6572 7369 6f6e 104b 0908 d40f 1011  Wversion.K......
-000029a0: 123a 3b0c 1a58 636f 6d6d 656e 7473 1101  .:;..Xcomments..
-000029b0: 2c09 08d4 0f10 1112 3f40 1a1a 5e64 6174  ,.......?@..^dat
-000029c0: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
-000029d0: 0f10 1112 441e 1a1a 5964 6174 6541 6464  ....D...YdateAdd
-000029e0: 6564 0808 0823 0000 0000 0000 0000 2340  ed...#........#@
-000029f0: 2800 0000 0000 0054 6e61 6d65 0923 4030  (......Tname.#@0
-00002a00: 0000 0000 0000 0008 001d 0032 0044 004c  ...........2.D.L
-00002a10: 0060 0072 007b 008d 0098 00ab 00b4 00b6  .`.r.{..........
-00002a20: 00b7 00c3 00cc 00d7 00dd 00e7 00ef 00f4  ................
-00002a30: 00f7 00f8 00f9 0102 010b 010d 010e 010f  ................
-00002a40: 0118 0125 0127 0128 0129 0132 013e 013f  ...%.'.(.).2.>.?
-00002a50: 0140 0149 014e 0150 0151 0152 015b 0160  .@.I.N.P.Q.R.[.`
-00002a60: 0162 0163 0164 016d 0173 0175 0176 0177  .b.c.d.m.s.u.v.w
-00002a70: 0180 0188 018a 018b 018c 0195 019e 01a1  ................
-00002a80: 01a2 01a3 01ac 01bb 01bd 01be 01bf 01c8  ................
-00002a90: 01d2 01d3 01d4 01d5 01de 01e7 01ec 01ed  ................
-00002aa0: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
-00002ab0: 0000 0000 0000 0000 0000 0000 0000 01f6  ................
-00002ac0: 0000 0003 0069 006d 0067 6c73 7670 626c  .....i.m.glsvpbl
-00002ad0: 6f62 0000 0295 6270 6c69 7374 3030 da01  ob....bplist00..
-00002ae0: 0203 0405 0607 0809 0a0b 0c0d 1c47 4847  .............GHG
-00002af0: 490c 4b5f 1012 7669 6577 4f70 7469 6f6e  I.K_..viewOption
-00002b00: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00002b10: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00002b20: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00002b30: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
-00002b40: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
-00002b50: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
-00002b60: 6f6e 585a 736f 7274 436f 6c75 6d6e 5f10  onXZsortColumn_.
-00002b70: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-00002b80: 7358 6963 6f6e 5369 7a65 1001 09d9 0e0f  sXiconSize......
-00002b90: 1011 1213 1415 1617 2025 292d 3237 3c41  ........ %)-27<A
-00002ba0: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
-00002bb0: 7374 4f70 656e 6564 5c64 6174 654d 6f64  stOpened\dateMod
-00002bc0: 6966 6965 645b 6461 7465 4372 6561 7465  ified[dateCreate
-00002bd0: 6454 7369 7a65 556c 6162 656c 546b 696e  dTsizeUlabelTkin
-00002be0: 6457 7665 7273 696f 6e54 6e61 6d65 d418  dWversionTname..
-00002bf0: 191a 1b1c 1d0c 1f57 7669 7369 626c 6555  .......WvisibleU
-00002c00: 7769 6474 6859 6173 6365 6e64 696e 6755  widthYascendingU
-00002c10: 696e 6465 7808 1101 2c09 1007 d418 191a  index...,.......
-00002c20: 1b1c 221c 2408 10c8 0810 08d4 1819 1a1b  ..".$...........
-00002c30: 0c27 1c0b 0910 b508 d418 191a 1b1c 271c  .'............'.
-00002c40: 2c08 0810 02d4 1819 1a1b 0c2f 1c31 0910  ,........../.1..
-00002c50: 6108 1003 d418 191a 1b1c 340c 3608 1064  a.........4.6..d
-00002c60: 0910 05d4 1819 1a1b 0c39 0c3b 0910 7309  .........9.;..s.
-00002c70: 1004 d418 191a 1b1c 3e0c 4008 104b 0910  ........>.@..K..
-00002c80: 06d4 1819 1a1b 0c43 0c45 0911 0137 0910  .......C.E...7..
-00002c90: 0008 2300 0000 0000 0000 0023 4028 0000  ..#........#@(..
-00002ca0: 0000 0000 546e 616d 6509 2340 3000 0000  ....Tname.#@0...
-00002cb0: 0000 0000 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
-00002cc0: 7200 7b00 8d00 9800 ab00 b400 b600 b700  r.{.............
-00002cd0: ca00 d300 e200 ef00 fb01 0001 0601 0b01  ................
-00002ce0: 1301 1801 2101 2901 2f01 3901 3f01 4001  ....!.)./.9.?.@.
-00002cf0: 4301 4401 4601 4f01 5001 5201 5301 5501  C.D.F.O.P.R.S.U.
-00002d00: 5e01 5f01 6101 6201 6b01 6c01 6d01 6f01  ^._.a.b.k.l.m.o.
-00002d10: 7801 7901 7b01 7c01 7e01 8701 8801 8a01  x.y.{.|.~.......
-00002d20: 8b01 8d01 9601 9701 9901 9a01 9c01 a501  ................
-00002d30: a601 a801 a901 ab01 b401 b501 b801 b901  ................
-00002d40: bb01 bc01 c501 ce01 d301 d400 0000 0000  ................
-00002d50: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
-00002d60: 0000 0000 0000 0000 0001 dd00 0000 0300  ................
-00002d70: 6900 6d00 676d 6f44 4462 6c6f 6200 0000  i.m.gmoDDblob...
-00002d80: 0869 d309 0c67 f2c4 4100 0000 0300 6900  .i...g..A.....i.
-00002d90: 6d00 676d 6f64 4462 6c6f 6200 0000 0869  m.gmodDblob....i
-00002da0: d309 0c67 f2c4 4100 0000 0300 6900 6d00  ...g..A.....i.m.
-00002db0: 6770 6831 5363 6f6d 7000 0000 0000 1130  gph1Scomp......0
-00002dc0: 0000 0000 0300 6900 6d00 6776 5372 6e6c  ......i.m.gvSrnl
-00002dd0: 6f6e 6700 0000 0100 0000 0700 6c00 6f00  ong.........l.o.
-00002de0: 6f00 6b00 7500 7000 7362 7773 7062 6c6f  o.k.u.p.sbwspblo
-00002df0: 6200 0000 c862 706c 6973 7430 30d7 0102  b....bplist00...
-00002e00: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
-00002e10: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
-00002e20: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
-00002e30: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-00002e40: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-00002e50: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-00002e60: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-00002e70: 0908 095f 1017 7b7b 302c 2031 3136 7d2c  ..._..{{0, 116},
-00002e80: 207b 3132 3530 2c20 3736 317d 7d09 0817   {1250, 761}}...
-00002e90: 2531 3d49 606d 797a 7b7c 7d7e 9800 0000  %1=I`myz{|}~....
-00002ea0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00002eb0: 0000 0000 0000 0000 0000 0000 9900 0000  ................
-00002ec0: 0700 6c00 6f00 6f00 6b00 7500 7000 736c  ..l.o.o.k.u.p.sl
-00002ed0: 6731 5363 6f6d 7000 0000 0000 04b1 fb00  g1Scomp.........
+000020a0: 0809 0809 5f10 197b 7b31 3635 302c 2033  ...._..{{1650, 3
+000020b0: 3538 7d2c 207b 3737 302c 2034 3336 7d7d  58}, {770, 436}}
+000020c0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
+000020d0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+000020e0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
+000020f0: 0000 0005 0069 0063 006f 006e 0073 6c67  .....i.c.o.n.slg
+00002100: 3153 636f 6d70 0000 0000 0005 98d9 0000  1Scomp..........
+00002110: 0005 0069 0063 006f 006e 0073 6c73 7643  ...i.c.o.n.slsvC
+00002120: 626c 6f62 0000 02af 6270 6c69 7374 3030  blob....bplist00
+00002130: da01 0203 0405 0607 0809 0a0b 0c0d 1a48  ...............H
+00002140: 4948 4a0c 4c5f 1012 7669 6577 4f70 7469  IHJ.L_..viewOpti
+00002150: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
+00002160: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+00002170: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00002180: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
+00002190: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
+000021a0: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
+000021b0: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
+000021c0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+000021d0: 7465 7358 6963 6f6e 5369 7a65 1001 09ab  tesXiconSize....
+000021e0: 0e17 1c21 252a 2f34 393e 43d4 0f10 1112  ...!%*/49>C.....
+000021f0: 1314 0c0c 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
+00002200: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+00002210: 7669 7369 626c 6554 6e61 6d65 10ea 0909  visibleTname....
+00002220: d40f 1011 1218 191a 1a58 7562 6971 7569  .........Xubiqui
+00002230: 7479 1023 0808 d40f 1011 121d 1e1a 0c5c  ty.#...........\
+00002240: 6461 7465 4d6f 6469 6669 6564 10b5 0809  dateModified....
+00002250: d40f 1011 1222 1e1a 1a5b 6461 7465 4372  ....."...[dateCr
+00002260: 6561 7465 6408 08d4 0f10 1112 2627 1a0c  eated.......&'..
+00002270: 5473 697a 6510 6108 09d4 0f10 1112 2b2c  Tsize.a.......+,
+00002280: 0c0c 546b 696e 6410 7309 09d4 0f10 1112  ..Tkind.s.......
+00002290: 3031 0c1a 556c 6162 656c 1064 0908 d40f  01..Ulabel.d....
+000022a0: 1011 1235 360c 1a57 7665 7273 696f 6e10  ...56..Wversion.
+000022b0: 4b09 08d4 0f10 1112 3a3b 0c1a 5863 6f6d  K.......:;..Xcom
+000022c0: 6d65 6e74 7311 012c 0908 d40f 1011 123f  ments..,.......?
+000022d0: 401a 1a5e 6461 7465 4c61 7374 4f70 656e  @..^dateLastOpen
+000022e0: 6564 10c8 0808 d40f 1011 1244 1e1a 1a59  ed.........D...Y
+000022f0: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
+00002300: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
+00002310: 616d 6509 2340 3000 0000 0000 0000 0800  ame.#@0.........
+00002320: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
+00002330: 9800 ab00 b400 b600 b700 c300 cc00 d700  ................
+00002340: dd00 e700 ef00 f400 f600 f700 f801 0101  ................
+00002350: 0a01 0c01 0d01 0e01 1701 2401 2601 2701  ..........$.&.'.
+00002360: 2801 3101 3d01 3e01 3f01 4801 4d01 4f01  (.1.=.>.?.H.M.O.
+00002370: 5001 5101 5a01 5f01 6101 6201 6301 6c01  P.Q.Z._.a.b.c.l.
+00002380: 7201 7401 7501 7601 7f01 8701 8901 8a01  r.t.u.v.........
+00002390: 8b01 9401 9d01 a001 a101 a201 ab01 ba01  ................
+000023a0: bc01 bd01 be01 c701 d101 d201 d301 d401  ................
+000023b0: dd01 e601 eb01 ec00 0000 0000 0002 0100  ................
+000023c0: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
+000023d0: 0000 0000 0001 f500 0000 0500 6900 6300  ............i.c.
+000023e0: 6f00 6e00 736c 7376 7062 6c6f 6200 0002  o.n.slsvpblob...
+000023f0: 9462 706c 6973 7430 30da 0102 0304 0506  .bplist00.......
+00002400: 0708 090a 0b0c 0d1c 4748 4749 0c4b 5f10  ........GHGI.K_.
+00002410: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00002420: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
+00002430: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+00002440: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00002450: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
+00002460: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
+00002470: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
+00002480: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
+00002490: 656c 6174 6976 6544 6174 6573 5869 636f  elativeDatesXico
+000024a0: 6e53 697a 6510 0109 d90e 0f10 1112 1314  nSize...........
+000024b0: 1516 1720 2529 2d32 373c 4158 636f 6d6d  ... %)-27<AXcomm
+000024c0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
+000024d0: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
+000024e0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+000024f0: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
+00002500: 7369 6f6e 546e 616d 65d4 1819 1a1b 1c1d  sionTname.......
+00002510: 0c1f 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
+00002520: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
+00002530: 0811 012c 0910 07d4 1819 1a1b 1c22 1c24  ...,.........".$
+00002540: 0810 c808 1008 d418 191a 1b0c 271c 0b09  ............'...
+00002550: 10b5 08d4 1819 1a1b 1c27 1c2c 0808 1002  .........'.,....
+00002560: d418 191a 1b0c 2f1c 3109 1061 0810 03d4  ....../.1..a....
+00002570: 1819 1a1b 1c34 0c36 0810 6409 1005 d418  .....4.6..d.....
+00002580: 191a 1b0c 390c 3b09 1073 0910 04d4 1819  ....9.;..s......
+00002590: 1a1b 1c3e 0c40 0810 4b09 1006 d418 191a  ...>.@..K.......
+000025a0: 1b0c 430c 4509 10ea 0910 0008 2300 0000  ..C.E.......#...
+000025b0: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
+000025c0: 616d 6509 2340 3000 0000 0000 0000 0800  ame.#@0.........
+000025d0: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
+000025e0: 9800 ab00 b400 b600 b700 ca00 d300 e200  ................
+000025f0: ef00 fb01 0001 0601 0b01 1301 1801 2101  ..............!.
+00002600: 2901 2f01 3901 3f01 4001 4301 4401 4601  )./.9.?.@.C.D.F.
+00002610: 4f01 5001 5201 5301 5501 5e01 5f01 6101  O.P.R.S.U.^._.a.
+00002620: 6201 6b01 6c01 6d01 6f01 7801 7901 7b01  b.k.l.m.o.x.y.{.
+00002630: 7c01 7e01 8701 8801 8a01 8b01 8d01 9601  |.~.............
+00002640: 9701 9901 9a01 9c01 a501 a601 a801 a901  ................
+00002650: ab01 b401 b501 b701 b801 ba01 bb01 c401  ................
+00002660: cd01 d201 d300 0000 0000 0002 0100 0000  ................
+00002670: 0000 0000 4c00 0000 0000 0000 0000 0000  ....L...........
+00002680: 0000 0001 dc00 0000 0500 6900 6300 6f00  ..........i.c.o.
+00002690: 6e00 736d 6f44 4462 6c6f 6200 0000 08c1  n.smoDDblob.....
+000026a0: fc21 5522 f4c4 4100 0000 0500 6900 6300  .!U"..A.....i.c.
+000026b0: 6f00 6e00 736d 6f64 4462 6c6f 6200 0000  o.n.smodDblob...
+000026c0: 08c1 fc21 5522 f4c4 4100 0000 0500 6900  ...!U"..A.....i.
+000026d0: 6300 6f00 6e00 7370 6831 5363 6f6d 7000  c.o.n.sph1Scomp.
+000026e0: 0000 0000 0800 0000 0000 0500 6900 6300  ............i.c.
+000026f0: 6f00 6e00 7376 5372 6e6c 6f6e 6700 0000  o.n.svSrnlong...
+00002700: 0100 0000 0300 6900 6d00 6762 7773 7062  ......i.m.gbwspb
+00002710: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
+00002720: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
+00002730: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+00002740: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
+00002750: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
+00002760: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
+00002770: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
+00002780: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
+00002790: 0808 0908 095f 1019 7b7b 3338 382c 2032  ....._..{{388, 2
+000027a0: 3136 7d2c 207b 3130 3932 2c20 3432 327d  16}, {1092, 422}
+000027b0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
+000027c0: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
+000027d0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
+000027e0: 9b00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
+000027f0: 6f6d 7000 0000 0000 1110 bf00 0000 0300  omp.............
+00002800: 6900 6d00 676c 7376 4362 6c6f 6200 0002  i.m.glsvCblob...
+00002810: b062 706c 6973 7430 30da 0102 0304 0506  .bplist00.......
+00002820: 0708 090a 0b0c 0d1a 4849 484a 0c4c 5f10  ........HIHJ.L_.
+00002830: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00002840: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
+00002850: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+00002860: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00002870: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
+00002880: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
+00002890: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
+000028a0: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
+000028b0: 656c 6174 6976 6544 6174 6573 5869 636f  elativeDatesXico
+000028c0: 6e53 697a 6510 0109 ab0e 171c 2125 2a2f  nSize.......!%*/
+000028d0: 3439 3e43 d40f 1011 1213 140c 0c5a 6964  49>C.........Zid
+000028e0: 656e 7469 6669 6572 5577 6964 7468 5961  entifierUwidthYa
+000028f0: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
+00002900: 546e 616d 6511 0137 0909 d40f 1011 1218  Tname..7........
+00002910: 191a 1a58 7562 6971 7569 7479 1023 0808  ...Xubiquity.#..
+00002920: d40f 1011 121d 1e1a 0c5c 6461 7465 4d6f  .........\dateMo
+00002930: 6469 6669 6564 10b5 0809 d40f 1011 1222  dified........."
+00002940: 1e1a 1a5b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
+00002950: 08d4 0f10 1112 2627 1a0c 5473 697a 6510  ......&'..Tsize.
+00002960: 6108 09d4 0f10 1112 2b2c 0c0c 546b 696e  a.......+,..Tkin
+00002970: 6410 7309 09d4 0f10 1112 3031 0c1a 556c  d.s.......01..Ul
+00002980: 6162 656c 1064 0908 d40f 1011 1235 360c  abel.d.......56.
+00002990: 1a57 7665 7273 696f 6e10 4b09 08d4 0f10  .Wversion.K.....
+000029a0: 1112 3a3b 0c1a 5863 6f6d 6d65 6e74 7311  ..:;..Xcomments.
+000029b0: 012c 0908 d40f 1011 123f 401a 1a5e 6461  .,.......?@..^da
+000029c0: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
+000029d0: d40f 1011 1244 1e1a 1a59 6461 7465 4164  .....D...YdateAd
+000029e0: 6465 6408 0808 2300 0000 0000 0000 0023  ded...#........#
+000029f0: 4028 0000 0000 0000 546e 616d 6509 2340  @(......Tname.#@
+00002a00: 3000 0000 0000 0000 0800 1d00 3200 4400  0...........2.D.
+00002a10: 4c00 6000 7200 7b00 8d00 9800 ab00 b400  L.`.r.{.........
+00002a20: b600 b700 c300 cc00 d700 dd00 e700 ef00  ................
+00002a30: f400 f700 f800 f901 0201 0b01 0d01 0e01  ................
+00002a40: 0f01 1801 2501 2701 2801 2901 3201 3e01  ....%.'.(.).2.>.
+00002a50: 3f01 4001 4901 4e01 5001 5101 5201 5b01  ?.@.I.N.P.Q.R.[.
+00002a60: 6001 6201 6301 6401 6d01 7301 7501 7601  `.b.c.d.m.s.u.v.
+00002a70: 7701 8001 8801 8a01 8b01 8c01 9501 9e01  w...............
+00002a80: a101 a201 a301 ac01 bb01 bd01 be01 bf01  ................
+00002a90: c801 d201 d301 d401 d501 de01 e701 ec01  ................
+00002aa0: ed00 0000 0000 0002 0100 0000 0000 0000  ................
+00002ab0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
+00002ac0: f600 0000 0300 6900 6d00 676c 7376 7062  ......i.m.glsvpb
+00002ad0: 6c6f 6200 0002 9562 706c 6973 7430 30da  lob....bplist00.
+00002ae0: 0102 0304 0506 0708 090a 0b0c 0d1c 4748  ..............GH
+00002af0: 4749 0c4b 5f10 1276 6965 774f 7074 696f  GI.K_..viewOptio
+00002b00: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+00002b10: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00002b20: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00002b30: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
+00002b40: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
+00002b50: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
+00002b60: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
+00002b70: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00002b80: 6573 5869 636f 6e53 697a 6510 0109 d90e  esXiconSize.....
+00002b90: 0f10 1112 1314 1516 1720 2529 2d32 373c  ......... %)-27<
+00002ba0: 4158 636f 6d6d 656e 7473 5e64 6174 654c  AXcomments^dateL
+00002bb0: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
+00002bc0: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
+00002bd0: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
+00002be0: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
+00002bf0: 1819 1a1b 1c1d 0c1f 5776 6973 6962 6c65  ........Wvisible
+00002c00: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00002c10: 5569 6e64 6578 0811 012c 0910 07d4 1819  Uindex...,......
+00002c20: 1a1b 1c22 1c24 0810 c808 1008 d418 191a  ...".$..........
+00002c30: 1b0c 271c 0b09 10b5 08d4 1819 1a1b 1c27  ..'............'
+00002c40: 1c2c 0808 1002 d418 191a 1b0c 2f1c 3109  .,........../.1.
+00002c50: 1061 0810 03d4 1819 1a1b 1c34 0c36 0810  .a.........4.6..
+00002c60: 6409 1005 d418 191a 1b0c 390c 3b09 1073  d.........9.;..s
+00002c70: 0910 04d4 1819 1a1b 1c3e 0c40 0810 4b09  .........>.@..K.
+00002c80: 1006 d418 191a 1b0c 430c 4509 1101 3709  ........C.E...7.
+00002c90: 1000 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
+00002ca0: 0000 0000 0054 6e61 6d65 0923 4030 0000  .....Tname.#@0..
+00002cb0: 0000 0000 0008 001d 0032 0044 004c 0060  .........2.D.L.`
+00002cc0: 0072 007b 008d 0098 00ab 00b4 00b6 00b7  .r.{............
+00002cd0: 00ca 00d3 00e2 00ef 00fb 0100 0106 010b  ................
+00002ce0: 0113 0118 0121 0129 012f 0139 013f 0140  .....!.)./.9.?.@
+00002cf0: 0143 0144 0146 014f 0150 0152 0153 0155  .C.D.F.O.P.R.S.U
+00002d00: 015e 015f 0161 0162 016b 016c 016d 016f  .^._.a.b.k.l.m.o
+00002d10: 0178 0179 017b 017c 017e 0187 0188 018a  .x.y.{.|.~......
+00002d20: 018b 018d 0196 0197 0199 019a 019c 01a5  ................
+00002d30: 01a6 01a8 01a9 01ab 01b4 01b5 01b8 01b9  ................
+00002d40: 01bb 01bc 01c5 01ce 01d3 01d4 0000 0000  ................
+00002d50: 0000 0201 0000 0000 0000 004c 0000 0000  ...........L....
+00002d60: 0000 0000 0000 0000 0000 01dd 0000 0003  ................
+00002d70: 0069 006d 0067 6d6f 4444 626c 6f62 0000  .i.m.gmoDDblob..
+00002d80: 0008 69d3 090c 67f2 c441 0000 0003 0069  ..i...g..A.....i
+00002d90: 006d 0067 6d6f 6444 626c 6f62 0000 0008  .m.gmodDblob....
+00002da0: 69d3 090c 67f2 c441 0000 0003 0069 006d  i...g..A.....i.m
+00002db0: 0067 7068 3153 636f 6d70 0000 0000 0011  .gph1Scomp......
+00002dc0: 3000 0000 0003 0069 006d 0067 7653 726e  0......i.m.gvSrn
+00002dd0: 6c6f 6e67 0000 0001 0000 0007 006c 006f  long.........l.o
+00002de0: 006f 006b 0075 0070 0073 6277 7370 626c  .o.k.u.p.sbwspbl
+00002df0: 6f62 0000 00c8 6270 6c69 7374 3030 d701  ob....bplist00..
+00002e00: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
+00002e10: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00002e20: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00002e30: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00002e40: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00002e50: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00002e60: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00002e70: 0809 0809 5f10 177b 7b30 2c20 3131 367d  ...._..{{0, 116}
+00002e80: 2c20 7b31 3235 302c 2037 3631 7d7d 0908  , {1250, 761}}..
+00002e90: 1725 313d 4960 6d79 7a7b 7c7d 7e98 0000  .%1=I`myz{|}~...
+00002ea0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+00002eb0: 0000 0000 0000 0000 0000 0000 0099 0000  ................
+00002ec0: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
+00002ed0: 6c67 3153 636f 6d70 0000 0000 0004 b1fb  lg1Scomp........
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -868,37 +868,37 @@
 00003630: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00003640: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00003650: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00003660: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00003670: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00003680: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00003690: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-000036a0: 01c5 22f4 c441 0000 0005 0069 0063 006f  .."..A.....i.c.o
-000036b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
-000036c0: c1fc 2155 22f4 c441 0000 0005 0069 0063  ..!U"..A.....i.c
-000036d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
-000036e0: 0000 0008 0000 0000 0005 0069 0063 006f  ...........i.c.o
-000036f0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
-00003700: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
-00003710: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
-00003720: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00003730: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00003740: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00003750: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00003760: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00003770: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00003780: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00003790: 0809 0809 5f10 197b 7b33 3838 2c20 3231  ...._..{{388, 21
-000037a0: 367d 2c20 7b31 3039 322c 2034 3232 7d7d  6}, {1092, 422}}
-000037b0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-000037c0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-000037d0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-000037e0: 0000 0003 0069 006d 0067 6c67 3153 636f  .....i.m.glg1Sco
-000037f0: 6d70 0000 0000 0011 10bf 0000 0003 0069  mp.............i
-00003800: 006d 0067 0000 0006 0000 0000 0000 380b  .m.g..........8.
+000036a0: 01c5 5522 f4c4 4100 0000 0500 6900 6300  ..U"..A.....i.c.
+000036b0: 6f00 6e00 736d 6f64 4462 6c6f 6200 0000  o.n.smodDblob...
+000036c0: 08c1 fc21 5522 f4c4 4100 0000 0500 6900  ...!U"..A.....i.
+000036d0: 6300 6f00 6e00 7370 6831 5363 6f6d 7000  c.o.n.sph1Scomp.
+000036e0: 0000 0000 0800 0000 0000 0500 6900 6300  ............i.c.
+000036f0: 6f00 6e00 7376 5372 6e6c 6f6e 6700 0000  o.n.svSrnlong...
+00003700: 0100 0000 0300 6900 6d00 6762 7773 7062  ......i.m.gbwspb
+00003710: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
+00003720: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
+00003730: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+00003740: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
+00003750: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
+00003760: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
+00003770: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
+00003780: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
+00003790: 0808 0908 095f 1019 7b7b 3338 382c 2032  ....._..{{388, 2
+000037a0: 3136 7d2c 207b 3130 3932 2c20 3432 327d  16}, {1092, 422}
+000037b0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
+000037c0: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
+000037d0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
+000037e0: 9b00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
+000037f0: 6f6d 7000 0000 0000 1110 bf00 0000 0300  omp.............
+00003800: 6900 6d00 0000 0006 0000 0000 0000 380b  i.m...........8.
 00003810: 0000 0045 0000 100b 0000 300b 0000 200c  ...E......0... .
 00003820: 0000 180b 0000 0000 0000 0000 0000 0000  ................
 00003830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -996,30 +996,30 @@
 00003e30: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00003e40: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00003e50: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00003e60: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00003e70: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00003e80: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00003e90: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00003ea0: 01c5 22f4 c441 0000 0005 0069 0063 006f  .."..A.....i.c.o
-00003eb0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
-00003ec0: c1fc 2155 22f4 c441 0000 0005 0069 0063  ..!U"..A.....i.c
-00003ed0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
-00003ee0: 0000 0008 0000 0000 0005 0069 0063 006f  ...........i.c.o
-00003ef0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
-00003f00: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
-00003f10: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
-00003f20: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00003f30: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00003f40: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00003f50: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00003f60: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00003f70: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00003f80: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00003f90: 0809 0809 5f10 197b 7b33 3838 2c20 3231  ...._..{{388, 21
-00003fa0: 367d 2c20 7b31 3039 322c 2034 3232 7d7d  6}, {1092, 422}}
-00003fb0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-00003fc0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00003fd0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-00003fe0: 0000 0003 0069 006d 0067 6c67 3153 636f  .....i.m.glg1Sco
-00003ff0: 6d70 0000 0000 0011 10bf 0000 0003 0069  mp.............i
-00004000: 006d 0067                                .m.g
+00003ea0: 01c5 5522 f4c4 4100 0000 0500 6900 6300  ..U"..A.....i.c.
+00003eb0: 6f00 6e00 736d 6f64 4462 6c6f 6200 0000  o.n.smodDblob...
+00003ec0: 08c1 fc21 5522 f4c4 4100 0000 0500 6900  ...!U"..A.....i.
+00003ed0: 6300 6f00 6e00 7370 6831 5363 6f6d 7000  c.o.n.sph1Scomp.
+00003ee0: 0000 0000 0800 0000 0000 0500 6900 6300  ............i.c.
+00003ef0: 6f00 6e00 7376 5372 6e6c 6f6e 6700 0000  o.n.svSrnlong...
+00003f00: 0100 0000 0300 6900 6d00 6762 7773 7062  ......i.m.gbwspb
+00003f10: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
+00003f20: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
+00003f30: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+00003f40: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
+00003f50: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
+00003f60: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
+00003f70: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
+00003f80: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
+00003f90: 0808 0908 095f 1019 7b7b 3338 382c 2032  ....._..{{388, 2
+00003fa0: 3136 7d2c 207b 3130 3932 2c20 3432 327d  16}, {1092, 422}
+00003fb0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
+00003fc0: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
+00003fd0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
+00003fe0: 9b00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
+00003ff0: 6f6d 7000 0000 0000 1110 bf00 0000 0300  omp.............
+00004000: 6900 6d00                                i.m.
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.57.2/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.57.2/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.57.2/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.2/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.57.2/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.57.2/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.57.2/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.57.2/simba/drop_bp_cords.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.57.2/simba/read_config_unit_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,64 +14,116 @@
                                 FloatError,
                                 NotDirectoryError,
                                 MissingProjectConfigEntryError,
                                 CorruptedFileError,
                                 ColumnNotFoundError,
                                 CountError)
 
-def check_int(name, value, max_value=None, min_value=None):
+def check_int(name: str,
+              value: None,
+              max_value=None,
+              min_value=None,
+              raise_error: bool=True):
+    msg = ''
     try:
         t.Int().check(value)
     except t.DataError as e:
-        print(e)
-        raise IntegerError(msg=f'{name} should be an integer number in SimBA, but is set to {str(value)}')
+        msg=f'{name} should be an integer number in SimBA, but is set to {str(value)}'
+        if raise_error:
+            raise IntegerError(msg=msg)
+        else:
+            return False, msg
     if (min_value != None):
         if int(value) < min_value:
-            raise IntegerError(msg=f'{name} should be MORE THAN OR EQUAL to {str(min_value)}. It is set to {str(value)}')
+            msg = f'{name} should be MORE THAN OR EQUAL to {str(min_value)}. It is set to {str(value)}'
+            if raise_error:
+                raise IntegerError(msg=msg)
+            else:
+                return False, msg
     if (max_value != None):
         if int(value) > max_value:
-            raise IntegerError(msg=f'{name} should be LESS THAN OR EQUAL to {str(max_value)}. It is set to {str(value)}')
+            msg = f'{name} should be LESS THAN OR EQUAL to {str(max_value)}. It is set to {str(value)}'
+            if raise_error:
+                raise IntegerError(msg=msg)
+            else:
+                return False, msg
+    return True, msg
+
 
-def check_if_valid_input(name, input, options):
+def check_if_valid_input(name: str,
+                         input: str,
+                         options: list,
+                         raise_error: bool=True):
+    msg = ''
     if input not in options:
-        raise InvalidInputError(msg=f'{name} is set to {str(input)}, which is an invalid setting. OPTIONS {options}')
+        msg = f'{name} is set to {str(input)}, which is an invalid setting. OPTIONS {options}'
+        if raise_error:
+            raise InvalidInputError(msg=msg)
+        else:
+            return False, msg
     else:
-        pass
+        return True, msg
 
-def check_str(name, value, options=(), allow_blank=False):
+def check_str(name: str,
+              value: None,
+              options=(),
+              allow_blank=False,
+              raise_error: bool = True):
+    msg = ''
     try:
         t.String(allow_blank=allow_blank).check(value)
     except t.DataError as e:
-        print(e)
-        raise StringError(msg=f'{name} should be an string in SimBA, but is set to {str(value)}')
-
+        msg = f'{name} should be an string in SimBA, but is set to {str(value)}'
+        if raise_error:
+            raise StringError(msg=msg)
+        else:
+            return False, msg
     if len(options) > 0:
         if value not in options:
-            raise StringError(msg=f'{name} is set to {str(value)} in SimBA, but this is not a valid option: {options}')
+            msg = f'{name} is set to {str(value)} in SimBA, but this is not a valid option: {options}'
+            if raise_error:
+                raise StringError(msg=msg)
+            else:
+                return False, msg
         else:
-            pass
+            return True, msg
     else:
-        pass
+        return True, msg
 
 
 def check_float(name: str,
                 value=None,
                 max_value=None,
-                min_value=None):
+                min_value=None,
+                raise_error: bool=True):
+    msg = ''
     try:
         t.Float().check(value)
     except t.DataError as e:
-        print(e)
-        raise FloatError(msg=f'{name} should be a float number in SimBA, but is set to {str(value)}')
+        msg = f'{name} should be a float number in SimBA, but is set to {str(value)}'
+        if raise_error:
+            raise FloatError(msg=msg)
+        else:
+            return False, msg
     if (min_value != None):
         if float(value) < min_value:
-            raise FloatError(msg=f'{name} should be MORE THAN OR EQUAL to {str(min_value)}. It is set to {str(value)}')
+            msg = f'{name} should be MORE THAN OR EQUAL to {str(min_value)}. It is set to {str(value)}'
+            if raise_error:
+                raise FloatError(msg=msg)
+            else:
+                return False, msg
     if (max_value != None):
         if float(value) > max_value:
-            raise FloatError(msg=f'{name} should be LESS THAN OR EQUAL to {str(max_value)}. It is set to {str(value)}')
+            msg = f'{name} should be LESS THAN OR EQUAL to {str(max_value)}. It is set to {str(value)}'
+            if raise_error:
+                raise FloatError(msg=msg)
+            else:
+                return False, msg
+    return True, msg
+
 
 def read_config_entry(config: ConfigParser,
                       section: str,
                       option: str,
                       data_type: str,
                       default_value=None,
                       options=None):
```

### Comparing `Simba-UW-tf-dev-1.56.9/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.57.2/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.57.2/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/train_single_model.py` & `Simba-UW-tf-dev-1.57.2/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.57.2/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.57.2/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.57.2/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.57.2/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.9
+Version: 1.57.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -213,18 +213,20 @@
 simba/feature_extractors/misc/convex_hull_scratch_2.py
 simba/feature_extractors/misc/count_values_in_range.py
 simba/feature_extractors/misc/doctests.py
 simba/feature_extractors/misc/egocentrical_aligner.py
 simba/feature_extractors/misc/fish_feature_extractor_2022.py
 simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
 simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
 simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
+simba/feature_extractors/misc/peaks.py
 simba/feature_extractors/misc/read_in_mp.py
 simba/feature_extractors/misc/termite_rois.csv
 simba/feature_extractors/misc/video_color.py
 simba/feature_extractors/misc/video_rotator.py
 simba/feature_extractors/misc/video_rotator_mp.py
 simba/mixins/.DS_Store
 simba/mixins/config_reader.py
@@ -340,13 +342,12 @@
 simba/unsupervised/grid_search_visualizers.py
 simba/unsupervised/hdbscan_clusterer.py
 simba/unsupervised/pop_up_classes.py
 simba/unsupervised/tsne.py
 simba/unsupervised/ui.py
 simba/unsupervised/umap_embedder.py
 simba/unsupervised/unsupervised_ui.py
-simba/unsupervised/visualizers.py
 simba/utils/.DS_Store
 simba/utils/errors.py
 simba/utils/lookups.py
 simba/utils/printing.py
 simba/utils/warnings.py
```

### Comparing `Simba-UW-tf-dev-1.56.9/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 imgaug==0.4.0
 imutils==0.5.2
 matplotlib==3.0.3
 numpy==1.18.1
 opencv-python==3.4.5.20
 pandas==0.25.3
 scikit-image==0.14.2
-scipy==1.1.0
+scipy==1.5.4
 seaborn==0.9.0
 scikit-learn==0.22.2
 tabulate==0.8.3
 tqdm==4.30.0
 xgboost==0.90
 yellowbrick==0.9.1
 dash==1.14.0
```

### Comparing `Simba-UW-tf-dev-1.56.9/LICENSE.md` & `Simba-UW-tf-dev-1.57.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/README.md` & `Simba-UW-tf-dev-1.57.2/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.9/setup.py` & `Simba-UW-tf-dev-1.57.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.56.9",
+    version="1.57.2",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
-              'opencv-python == 3.4.5.20', 'pandas == 0.25.3','scikit-image == 0.14.2', 'scipy == 1.1.0','seaborn == 0.9.0',
+              'opencv-python == 3.4.5.20', 'pandas == 0.25.3','scikit-image == 0.14.2', 'scipy == 1.5.4','seaborn == 0.9.0',
               'scikit-learn == 0.22.2','tabulate == 0.8.3','tqdm == 4.30.0','xgboost == 0.90',
               'yellowbrick == 0.9.1', 'dash == 1.14.0', 'dash_color_picker == 0.0.1', 'dash_core_components == 1.10.2',
 			  'dash_colorscales == 0.0.4', 'dash_html_components == 1.0.3', 'h5py == 2.9.0', 'numba == 0.52.0', 'numexpr == 2.6.9',
 			  'plotly == 4.9.0', 'statsmodels == 0.9.0', 'cefpython3 == 66.0', "pyarrow == 6.0.1", "shap == 0.35.0","h5py==2.9.0",
 			  "tables==3.6.1", "xlrd==1.2.0", "trafaret==2.1.1"],
     license='GNU Lesser General Public License v3 (LGPLv3)',
     packages=setuptools.find_packages(),
```

