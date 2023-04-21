# Comparing `tmp/pose_format-0.2.1.tar.gz` & `tmp/pose_format-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pose_format-0.2.1.tar", last modified: Tue Mar 28 10:56:35 2023, max compression
+gzip compressed data, was "pose_format-0.2.2.tar", last modified: Fri Apr 21 15:22:42 2023, max compression
```

## Comparing `pose_format-0.2.1.tar` & `pose_format-0.2.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.984309 pose_format-0.2.1/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      255 2023-03-28 10:56:35.984118 pose_format-0.2.1/PKG-INFO
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.973731 pose_format-0.2.1/pose_format/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      124 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/__init__.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.974863 pose_format-0.2.1/pose_format/numpy/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)       37 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/numpy/__init__.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     9748 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/numpy/pose_body.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.975389 pose_format-0.2.1/pose_format/numpy/representation/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/numpy/representation/__init__.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      677 2023-03-21 14:34:24.000000 pose_format-0.2.1/pose_format/numpy/representation/distance.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      866 2023-03-21 14:34:24.000000 pose_format-0.2.1/pose_format/numpy/representation/distance_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     6387 2023-03-18 14:40:30.000000 pose_format-0.2.1/pose_format/pose.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     8763 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/pose_body.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     5009 2023-03-21 14:34:24.000000 pose_format-0.2.1/pose_format/pose_header.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     3722 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/pose_representation.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     7789 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/pose_visualizer.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.976287 pose_format-0.2.1/pose_format/tensorflow/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/__init__.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.977308 pose_format-0.2.1/pose_format/tensorflow/masked/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      132 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/masked/__init__.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     5752 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/masked/tensor.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1099 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/masked/tensor_graph_mode_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     4022 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/masked/tensor_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1923 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/masked/tensorflow.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     2170 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/masked/tensorflow_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     4228 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/pose_body.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      727 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/pose_body_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      677 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/pose_representation.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1702 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/pose_representation_test.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.978714 pose_format-0.2.1/pose_format/tensorflow/representation/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/__init__.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      699 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/angle.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      566 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/angle_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      678 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/distance.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      595 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/distance_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1156 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/inner_angle.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      662 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/inner_angle_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1115 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/point_line_distance.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      704 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/tensorflow/representation/point_line_distance_test.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.978869 pose_format-0.2.1/pose_format/testing/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/testing/__init__.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.979234 pose_format-0.2.1/pose_format/torch/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/__init__.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.980044 pose_format-0.2.1/pose_format/torch/masked/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      112 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/masked/__init__.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     4084 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/masked/tensor.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     2063 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/masked/torch.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1937 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/masked/torch_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     2120 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/pose_body.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1272 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/pose_representation.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.982024 pose_format-0.2.1/pose_format/torch/representation/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/__init__.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      993 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/angle.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      954 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/angle_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      801 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/distance.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      989 2023-03-21 14:34:24.000000 pose_format-0.2.1/pose_format/torch/representation/distance_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1344 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/inner_angle.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1148 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/inner_angle_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1302 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/point_line_distance.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1196 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/point_line_distance_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      558 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/torch/representation/points.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.983890 pose_format-0.2.1/pose_format/utils/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/__init__.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      120 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/fast_math.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     5696 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/holistic.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     2719 2023-03-21 14:34:24.000000 pose_format-0.2.1/pose_format/utils/normalization_3d.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)    10965 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/openpose.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     6946 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/openpose_135.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)    15245 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/openpose_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      452 2023-03-21 14:34:24.000000 pose_format-0.2.1/pose_format/utils/optical_flow.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     4925 2023-03-21 14:34:24.000000 pose_format-0.2.1/pose_format/utils/pose_converter.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     2115 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/reader.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     2693 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/reader_test.py
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     6405 2023-03-18 13:29:49.000000 pose_format-0.2.1/pose_format/utils/siren.py
-drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-03-28 10:56:35.974571 pose_format-0.2.1/pose_format.egg-info/
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      255 2023-03-28 10:56:35.000000 pose_format-0.2.1/pose_format.egg-info/PKG-INFO
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     2683 2023-03-28 10:56:35.000000 pose_format-0.2.1/pose_format.egg-info/SOURCES.txt
--rw-r--r--   0 amitmoryossef   (501) staff       (20)        1 2023-03-28 10:56:35.000000 pose_format-0.2.1/pose_format.egg-info/dependency_links.txt
--rw-r--r--   0 amitmoryossef   (501) staff       (20)      108 2023-03-28 10:56:35.000000 pose_format-0.2.1/pose_format.egg-info/requires.txt
--rw-r--r--   0 amitmoryossef   (501) staff       (20)       12 2023-03-28 10:56:35.000000 pose_format-0.2.1/pose_format.egg-info/top_level.txt
--rw-r--r--   0 amitmoryossef   (501) staff       (20)     1103 2023-03-28 10:43:42.000000 pose_format-0.2.1/pyproject.toml
--rw-r--r--   0 amitmoryossef   (501) staff       (20)       38 2023-03-28 10:56:35.984357 pose_format-0.2.1/setup.cfg
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.539852 pose_format-0.2.2/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      255 2023-04-21 15:22:42.539662 pose_format-0.2.2/PKG-INFO
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.529072 pose_format-0.2.2/pose_format/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      124 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/__init__.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.530179 pose_format-0.2.2/pose_format/numpy/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)       37 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/numpy/__init__.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     9748 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/numpy/pose_body.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.530896 pose_format-0.2.2/pose_format/numpy/representation/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/numpy/representation/__init__.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      677 2023-03-21 14:34:24.000000 pose_format-0.2.2/pose_format/numpy/representation/distance.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      866 2023-03-21 14:34:24.000000 pose_format-0.2.2/pose_format/numpy/representation/distance_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     6387 2023-03-18 14:40:30.000000 pose_format-0.2.2/pose_format/pose.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     8763 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/pose_body.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     5430 2023-04-21 15:09:47.000000 pose_format-0.2.2/pose_format/pose_header.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     3722 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/pose_representation.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     8078 2023-04-21 15:18:25.000000 pose_format-0.2.2/pose_format/pose_visualizer.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.531869 pose_format-0.2.2/pose_format/tensorflow/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/__init__.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.533010 pose_format-0.2.2/pose_format/tensorflow/masked/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      132 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/masked/__init__.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     5752 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/masked/tensor.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1099 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/masked/tensor_graph_mode_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     4022 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/masked/tensor_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1923 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/masked/tensorflow.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     2170 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/masked/tensorflow_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     4228 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/pose_body.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      727 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/pose_body_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      677 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/pose_representation.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1702 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/pose_representation_test.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.534526 pose_format-0.2.2/pose_format/tensorflow/representation/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/__init__.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      699 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/angle.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      566 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/angle_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      678 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/distance.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      595 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/distance_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1156 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/inner_angle.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      662 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/inner_angle_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1115 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/point_line_distance.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      704 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/tensorflow/representation/point_line_distance_test.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.534690 pose_format-0.2.2/pose_format/testing/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/testing/__init__.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.535095 pose_format-0.2.2/pose_format/torch/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/__init__.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.535833 pose_format-0.2.2/pose_format/torch/masked/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      112 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/masked/__init__.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     4084 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/masked/tensor.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     2063 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/masked/torch.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1937 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/masked/torch_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     2120 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/pose_body.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1272 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/pose_representation.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.537512 pose_format-0.2.2/pose_format/torch/representation/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/__init__.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      993 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/angle.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      954 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/angle_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      801 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/distance.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      989 2023-03-21 14:34:24.000000 pose_format-0.2.2/pose_format/torch/representation/distance_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1344 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/inner_angle.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1148 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/inner_angle_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1302 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/point_line_distance.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1196 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/point_line_distance_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      558 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/torch/representation/points.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.539444 pose_format-0.2.2/pose_format/utils/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)        0 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/__init__.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      120 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/fast_math.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     5696 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/holistic.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     3191 2023-04-21 14:37:01.000000 pose_format-0.2.2/pose_format/utils/normalization_3d.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)    10965 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/openpose.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     6946 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/openpose_135.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)    15245 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/openpose_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      452 2023-03-21 14:34:24.000000 pose_format-0.2.2/pose_format/utils/optical_flow.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     4925 2023-03-21 14:34:24.000000 pose_format-0.2.2/pose_format/utils/pose_converter.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     2115 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/reader.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     2693 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/reader_test.py
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     6405 2023-03-18 13:29:49.000000 pose_format-0.2.2/pose_format/utils/siren.py
+drwxr-xr-x   0 amitmoryossef   (501) staff       (20)        0 2023-04-21 15:22:42.529834 pose_format-0.2.2/pose_format.egg-info/
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      255 2023-04-21 15:22:42.000000 pose_format-0.2.2/pose_format.egg-info/PKG-INFO
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     2683 2023-04-21 15:22:42.000000 pose_format-0.2.2/pose_format.egg-info/SOURCES.txt
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)        1 2023-04-21 15:22:42.000000 pose_format-0.2.2/pose_format.egg-info/dependency_links.txt
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)      108 2023-04-21 15:22:42.000000 pose_format-0.2.2/pose_format.egg-info/requires.txt
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)       12 2023-04-21 15:22:42.000000 pose_format-0.2.2/pose_format.egg-info/top_level.txt
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)     1103 2023-04-21 15:18:50.000000 pose_format-0.2.2/pyproject.toml
+-rw-r--r--   0 amitmoryossef   (501) staff       (20)       38 2023-04-21 15:22:42.539903 pose_format-0.2.2/setup.cfg
```

### Comparing `pose_format-0.2.1/pose_format/numpy/pose_body.py` & `pose_format-0.2.2/pose_format/numpy/pose_body.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/numpy/representation/distance.py` & `pose_format-0.2.2/pose_format/numpy/representation/distance.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/numpy/representation/distance_test.py` & `pose_format-0.2.2/pose_format/numpy/representation/distance_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/pose.py` & `pose_format-0.2.2/pose_format/pose.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/pose_body.py` & `pose_format-0.2.2/pose_format/pose_body.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/pose_header.py` & `pose_format-0.2.2/pose_format/pose_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,21 @@
 
     @staticmethod
     def read(version: float, reader: BufferReader):
         width, height, depth = reader.unpack(ConstStructs.triple_ushort)
         return PoseHeaderDimensions(width, height, depth)
 
     def write(self, buffer: BinaryIO):
+        if not (0 <= self.width <= (0x7fff * 2 + 1)):
+            raise ValueError(f"Width must be between 0 and 65535. Got {self.width}")
+        if not (0 <= self.height <= (0x7fff * 2 + 1)):
+            raise ValueError(f"Height must be between 0 and 65535. Got {self.height}")
+        if not (0 <= self.depth <= (0x7fff * 2 + 1)):
+            raise ValueError(f"Depth must be between 0 and 65535. Got {self.depth}")
+
         buffer.write(ConstStructs.triple_ushort.pack(self.width, self.height, self.depth))
 
 
 class PoseHeader:
     def __init__(self,
                  version: float,
                  dimensions: PoseHeaderDimensions,
```

### Comparing `pose_format-0.2.1/pose_format/pose_representation.py` & `pose_format-0.2.2/pose_format/pose_representation.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/pose_visualizer.py` & `pose_format-0.2.2/pose_format/pose_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import itertools
+import logging
 import math
 from functools import lru_cache
 from typing import Tuple, Iterable
 
 import numpy as np
 import numpy.ma as ma
 from tqdm import tqdm
@@ -140,24 +141,28 @@
 
         # image_size = (self.pose.header.dimensions.width, self.pose.header.dimensions.height)
 
         output_params = {
             "-vcodec": "libx264",
             "-preset": "fast",
             "-input_framerate": self.pose.body.fps,
-            "-pix_fmt": "yuv420p",
         }
 
-        # Define writer with defined parameters and suitable output filename for e.g. `Output.mp4`
-        out = WriteGear(output=f_name, logging=False, custom_ffmpeg=custom_ffmpeg, **output_params)
-        # out = cv2.VideoWriter(f_name, cv2.VideoWriter_fourcc(*'MP4V'), self.pose.body.fps, image_size)
+        writer = None  # Define writer with defined parameters and suitable output filename for e.g. `Output.mp4`
         for frame in tqdm(frames):
-            out.write(frame)
+            if writer is None:  # Create writer on first frame
+                if frame.shape[0] % 2 == 0 and frame.shape[1] % 2 == 0:
+                    output_params["-pix_fmt"] = "yuv420p"  # H.264
+                else:
+                    logging.warning(
+                        "Video shape is not divisible by 2. Can not use H.264. Consider resizing to a divisible shape.")
+                writer = WriteGear(output=f_name, logging=False, custom_ffmpeg=custom_ffmpeg, **output_params)
+            writer.write(frame)
 
-        out.close()
+        writer.close()
 
 
 class FastAndUglyPoseVisualizer(PoseVisualizer):
     """
     This class draws all frames as grayscale, without opacity based on confidence
     """
```

### Comparing `pose_format-0.2.1/pose_format/tensorflow/masked/tensor.py` & `pose_format-0.2.2/pose_format/tensorflow/masked/tensor.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/masked/tensor_graph_mode_test.py` & `pose_format-0.2.2/pose_format/tensorflow/masked/tensor_graph_mode_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/masked/tensor_test.py` & `pose_format-0.2.2/pose_format/tensorflow/masked/tensor_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/masked/tensorflow.py` & `pose_format-0.2.2/pose_format/tensorflow/masked/tensorflow.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/masked/tensorflow_test.py` & `pose_format-0.2.2/pose_format/tensorflow/masked/tensorflow_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/pose_body.py` & `pose_format-0.2.2/pose_format/tensorflow/pose_body.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/pose_body_test.py` & `pose_format-0.2.2/pose_format/tensorflow/pose_body_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/pose_representation.py` & `pose_format-0.2.2/pose_format/tensorflow/pose_representation.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/pose_representation_test.py` & `pose_format-0.2.2/pose_format/tensorflow/pose_representation_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/representation/angle.py` & `pose_format-0.2.2/pose_format/tensorflow/representation/angle.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/representation/angle_test.py` & `pose_format-0.2.2/pose_format/tensorflow/representation/angle_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/representation/distance.py` & `pose_format-0.2.2/pose_format/tensorflow/representation/distance.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/representation/distance_test.py` & `pose_format-0.2.2/pose_format/tensorflow/representation/distance_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/representation/inner_angle.py` & `pose_format-0.2.2/pose_format/tensorflow/representation/inner_angle.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/representation/inner_angle_test.py` & `pose_format-0.2.2/pose_format/tensorflow/representation/inner_angle_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/representation/point_line_distance.py` & `pose_format-0.2.2/pose_format/tensorflow/representation/point_line_distance.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/tensorflow/representation/point_line_distance_test.py` & `pose_format-0.2.2/pose_format/tensorflow/representation/point_line_distance_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/masked/tensor.py` & `pose_format-0.2.2/pose_format/torch/masked/tensor.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/masked/torch.py` & `pose_format-0.2.2/pose_format/torch/masked/torch.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/masked/torch_test.py` & `pose_format-0.2.2/pose_format/torch/masked/torch_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/pose_body.py` & `pose_format-0.2.2/pose_format/torch/pose_body.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/pose_representation.py` & `pose_format-0.2.2/pose_format/torch/pose_representation.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/angle.py` & `pose_format-0.2.2/pose_format/torch/representation/angle.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/angle_test.py` & `pose_format-0.2.2/pose_format/torch/representation/angle_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/distance.py` & `pose_format-0.2.2/pose_format/torch/representation/distance.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/distance_test.py` & `pose_format-0.2.2/pose_format/torch/representation/distance_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/inner_angle.py` & `pose_format-0.2.2/pose_format/torch/representation/inner_angle.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/inner_angle_test.py` & `pose_format-0.2.2/pose_format/torch/representation/inner_angle_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/point_line_distance.py` & `pose_format-0.2.2/pose_format/torch/representation/point_line_distance.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/point_line_distance_test.py` & `pose_format-0.2.2/pose_format/torch/representation/point_line_distance_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/torch/representation/points.py` & `pose_format-0.2.2/pose_format/torch/representation/points.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/utils/holistic.py` & `pose_format-0.2.2/pose_format/utils/holistic.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/utils/normalization_3d.py` & `pose_format-0.2.2/pose_format/utils/normalization_3d.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import math
 from typing import Tuple
 
 import numpy as np
 import numpy.ma as ma
 from pose_format.pose_header import PoseNormalizationInfo
 from scipy.spatial.transform import Rotation
 
@@ -12,70 +11,77 @@
                  plane: PoseNormalizationInfo,
                  line: PoseNormalizationInfo,
                  size: float = 1):
         self.size = size
         self.plane = plane
         self.line = line
 
-    def rotate_to_normal(self, pose: np.ndarray, normal: np.ndarray, around: np.ndarray):
-        # Let's rotate the points such that the normal is the new Z axis
-        # Following https://stackoverflow.com/questions/1023948/rotate-normal-vector-onto-axis-plane
+    def rotate_to_normal(self, pose: ma.masked_array, normal: ma.masked_array, around: ma.masked_array):
+        # Move pose to origin
+        pose = pose - around[:, np.newaxis]
+
         old_x_axis = np.array([1, 0, 0])
 
         z_axis = normal
-        y_axis = np.cross(old_x_axis, z_axis)
-        x_axis = np.cross(z_axis, y_axis)
+        y_axis = np.cross(old_x_axis, z_axis, axis=-1)
+        x_axis = np.cross(z_axis, y_axis, axis=-1)
 
-        axis = np.stack([x_axis, y_axis, z_axis])
+        axis = np.stack([x_axis, y_axis, z_axis], axis=1)
 
-        return np.dot(pose - around, axis.T)
+        rotated = np.einsum('...ij,...kj->...ik', pose, axis)
+        return ma.masked_array(rotated, pose.mask)
 
-    def get_normal(self, pose: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-        triangle = pose[[self.plane.p1, self.plane.p2, self.plane.p3]]
+    def get_normal(self, pose: ma.masked_array) -> Tuple[ma.masked_array, ma.masked_array]:
+        triangle = pose[:, [self.plane.p1, self.plane.p2, self.plane.p3]]
 
-        v1 = triangle[1] - triangle[0]
-        v2 = triangle[2] - triangle[0]
+        v1 = triangle[:, 1] - triangle[:, 0]
+        v2 = triangle[:, 2] - triangle[:, 0]
 
-        normal = np.cross(v1, v2)
-        normal /= np.linalg.norm(normal)
+        normal = np.cross(v1, v2, axisa=-1)
+        normal /= np.linalg.norm(normal, axis=-1, keepdims=True)
 
-        return normal, triangle[0]
+        normal = ma.masked_array(normal, pose[:, 0].mask)
+        return normal, triangle[:, 0]
 
-    def get_rotation_angle(self, pose: ma.masked_array) -> float:
-        p1 = pose[self.line.p1]
-        p2 = pose[self.line.p2]
+    def get_rotation_angle(self, pose: ma.masked_array) -> ma.masked_array:
+        p1 = pose[:, self.line.p1]
+        p2 = pose[:, self.line.p2]
         vec = p2 - p1
 
-        return 90 + math.degrees(math.atan2(vec[1], vec[0]))
+        return 90 + np.degrees(np.arctan2(vec[..., 1], vec[..., 0]))
 
-    def rotate(self, pose: ma.masked_array, angle: float) -> ma.masked_array:
-        r = Rotation.from_euler('z', angle, degrees=True)
-        return ma.dot(pose, r.as_matrix())
+    def rotate(self, pose: ma.masked_array, angle: np.ndarray) -> ma.masked_array:
+        r = Rotation.from_euler('z', -angle[..., np.newaxis], degrees=True)  # Clockwise rotation
+        rotated = np.einsum('...ij,...kj->...ik', pose, r.as_matrix()).reshape(pose.shape)
+        return ma.masked_array(rotated, pose.mask)
 
     def scale(self, pose: ma.masked_array) -> ma.masked_array:
-        p1 = pose[self.line.p1]
-        p2 = pose[self.line.p2]
-        current_size = np.sqrt(np.power(p2 - p1, 2).sum())
-
-        pose *= self.size / current_size
-        pose -= pose[self.line.p1]  # move to first point of the line
+        p1 = pose[:, self.line.p1]
+        p2 = pose[:, self.line.p2]
+        current_size = ma.sqrt(ma.power(p2 - p1, 2).sum(axis=-1))
+        scale = self.size / current_size
+        pose *= scale.reshape(-1, 1, 1)
+        pose -= pose[:, [self.line.p1]]  # move to first point of the line
         return pose
 
     def normalize_pose(self, pose: ma.masked_array) -> ma.masked_array:
-        if ma.all(pose == 0):
-            return pose
-
         # First rotate to normal
         normal, base = self.get_normal(pose)
         pose = self.rotate_to_normal(pose, normal, base)
 
         # Then rotate on the X-Y plane such that the line is on the Y axis
-        angle = self.get_rotation_angle(pose.data)
-        pose = self.rotate(pose.data, angle)
+        angle = self.get_rotation_angle(pose)
+        pose = self.rotate(pose, angle)
 
         # Scale pose such that the line is of size self.size
         pose = self.scale(pose)
 
+        # Filled with zeros
+        pose = ma.array(pose.filled(0), mask=pose.mask)
+
         return pose
 
     def __call__(self, poses: ma.masked_array) -> ma.masked_array:
-        return ma.array([[self.normalize_pose(p) for p in ps] for ps in poses], mask=poses.mask)
+        frames, people, joints, dims = poses.shape
+        poses = poses.reshape(-1, joints, dims)
+        poses = self.normalize_pose(poses)
+        return poses.reshape(frames, people, joints, dims)
```

### Comparing `pose_format-0.2.1/pose_format/utils/openpose.py` & `pose_format-0.2.2/pose_format/utils/openpose.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/utils/openpose_135.py` & `pose_format-0.2.2/pose_format/utils/openpose_135.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/utils/openpose_test.py` & `pose_format-0.2.2/pose_format/utils/openpose_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/utils/pose_converter.py` & `pose_format-0.2.2/pose_format/utils/pose_converter.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/utils/reader.py` & `pose_format-0.2.2/pose_format/utils/reader.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/utils/reader_test.py` & `pose_format-0.2.2/pose_format/utils/reader_test.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format/utils/siren.py` & `pose_format-0.2.2/pose_format/utils/siren.py`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pose_format.egg-info/SOURCES.txt` & `pose_format-0.2.2/pose_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pose_format-0.2.1/pyproject.toml` & `pose_format-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pose_format"
 description = "Library for viewing, augmenting, and handling .pose files"
-version = "0.2.1"
+version = "0.2.2"
 keywords = ["Pose Files", "Pose Interpolation", "Pose Augmentation"]
 authors = [
     { name = "Amit Moryossef", email = "amitmoryossef@gmail.com" }
 ]
 dependencies = [
     "numpy",
     "scipy",
```

