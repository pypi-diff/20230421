# Comparing `tmp/discminer-0.2.0.tar.gz` & `tmp/discminer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.2.0.tar", last modified: Sat Apr 15 10:03:47 2023, max compression
+gzip compressed data, was "discminer-0.2.1.tar", last modified: Fri Apr 21 12:29:52 2023, max compression
```

## Comparing `discminer-0.2.0.tar` & `discminer-0.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.308641 discminer-0.2.0/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.0/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-15 10:03:47.308859 discminer-0.2.0/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.0/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.281924 discminer-0.2.0/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     4974 2023-04-15 07:21:20.000000 discminer-0.2.0/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.0/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.0/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.0/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.0/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.0/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.0/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.0/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.0/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.0/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.0/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000    10412 2023-04-13 16:23:21.000000 discminer-0.2.0/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.292228 discminer-0.2.0/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.0/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-15 10:00:30.000000 discminer-0.2.0/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.2.0/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.0/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8108 2023-03-26 15:14:30.000000 discminer-0.2.0/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74020 2023-04-04 09:57:01.000000 discminer-0.2.0/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    70761 2023-04-12 16:51:53.000000 discminer-0.2.0/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.0/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.302432 discminer-0.2.0/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.0/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.0/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.0/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    28759 2023-04-14 21:15:05.000000 discminer-0.2.0/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    35149 2023-04-12 16:32:43.000000 discminer-0.2.0/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.0/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.304561 discminer-0.2.0/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.0/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.0/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.0/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.0/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.294554 discminer-0.2.0/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.0/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-15 10:03:47.309448 discminer-0.2.0/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.0/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.307851 discminer-0.2.0/template/
--rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.0/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.0/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.0/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.0/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 12:29:52.880669 discminer-0.2.1/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.1/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-21 12:29:52.880832 discminer-0.2.1/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.1/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 12:29:52.861708 discminer-0.2.1/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.1/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.1/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.1/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.1/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.1/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.1/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.1/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.1/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.1/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.1/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.1/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.1/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 12:29:52.871730 discminer-0.2.1/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.1/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-21 12:24:45.000000 discminer-0.2.1/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.2.1/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.1/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8108 2023-03-26 15:14:30.000000 discminer-0.2.1/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74020 2023-04-04 09:57:01.000000 discminer-0.2.1/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    71217 2023-04-21 10:59:50.000000 discminer-0.2.1/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.1/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 12:29:52.875659 discminer-0.2.1/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.1/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.1/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.1/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.1/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.1/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.1/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.1/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.1/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    29567 2023-04-20 17:31:21.000000 discminer-0.2.1/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    35149 2023-04-12 16:32:43.000000 discminer-0.2.1/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.1/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 12:29:52.877158 discminer-0.2.1/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.1/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.1/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.1/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.1/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 12:29:52.873373 discminer-0.2.1/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-21 12:29:52.000000 discminer-0.2.1/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-21 12:29:52.000000 discminer-0.2.1/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-21 12:29:52.000000 discminer-0.2.1/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-21 12:29:52.000000 discminer-0.2.1/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-21 12:29:52.000000 discminer-0.2.1/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.1/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-21 12:29:52.881236 discminer-0.2.1/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.1/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-21 12:29:52.880040 discminer-0.2.1/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.1/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.1/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.1/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.1/template/prepare_data.py
```

### Comparing `discminer-0.2.0/LICENSE` & `discminer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/PKG-INFO` & `discminer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.0 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.1 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.0/README.md` & `discminer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/make_channels.py` & `discminer-0.2.1/_mining/make_channels.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 #****************************
 model = General2d(datacube, Rmax, Rmin=0, prototype=True)
 
 model.z_upper_func = cart.z_upper_exp_tapered
 model.z_lower_func = cart.z_lower_exp_tapered
 model.velocity_func = model.keplerian_vertical # vrot = sqrt(GM/r**3)*R
 model.line_profile = model.line_profile_bell
+model.line_uplow = model.line_uplow_mask
 
 if 'I2pwl' in meta['kind']:
     model.intensity_func = cart.intensity_powerlaw_rbreak
 elif 'I2pwlnosurf' in meta['kind']:
     model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
 else:
     model.intensity_func = cart.intensity_powerlaw_rout
```

### Comparing `discminer-0.2.0/_mining/make_parfile.py` & `discminer-0.2.1/_mining/make_parfile.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/make_single_moments.py` & `discminer-0.2.1/_mining/make_single_moments.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/plot_attributes_model.py` & `discminer-0.2.1/_mining/plot_attributes_model.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/plot_azimuthal_profiles.py` & `discminer-0.2.1/_mining/plot_azimuthal_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/plot_moment+offset.py` & `discminer-0.2.1/_mining/plot_moment+offset.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/plot_moment+residuals.py` & `discminer-0.2.1/_mining/plot_moment+residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/plot_peak_residuals.py` & `discminer-0.2.1/_mining/plot_peak_residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/plot_radial_profiles.py` & `discminer-0.2.1/_mining/plot_radial_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/plot_residuals+all.py` & `discminer-0.2.1/_mining/plot_residuals+all.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/plot_residuals+deproj.py` & `discminer-0.2.1/_mining/plot_residuals+deproj.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/_mining/utils.py` & `discminer-0.2.1/_mining/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         Rmax = Rmax*Rout*u.au
         model = Model(datacube, Rmax=Rmax, Rmin=Rmin, prototype=True)
         
         model.z_upper_func = cart.z_upper_exp_tapered
         model.z_lower_func = cart.z_lower_exp_tapered
         model.velocity_func = model.keplerian_vertical # vrot = sqrt(GM/r**3)*R
         model.line_profile = model.line_profile_bell
+        model.line_uplow = model.line_uplow_mask
     
         if 'I2pwl' in meta['kind']:
             model.intensity_func = cart.intensity_powerlaw_rbreak
         elif 'I2pwlnosurf' in meta['kind']:
             model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
         else:
             model.intensity_func = cart.intensity_powerlaw_rout
```

### Comparing `discminer-0.2.0/discminer/cart.py` & `discminer-0.2.1/discminer/cart.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/core.py` & `discminer-0.2.1/discminer/core.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/cube.py` & `discminer-0.2.1/discminer/cube.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/disc2d.py` & `discminer-0.2.1/discminer/disc2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,15 +502,29 @@
         print('Setting line profile function to', profile) 
         self._line_profile = profile
 
     @line_profile.deleter 
     def line_profile(self): 
         print('Deleting intensity function') 
         del self._line_profile
-    
+
+    @property
+    def line_uplow(self): 
+        return self._line_uplow
+          
+    @line_uplow.setter 
+    def line_uplow(self, uplow): 
+        print('Setting composite upper+lower line profile function to', uplow) 
+        self._line_uplow = uplow
+
+    @line_uplow.deleter 
+    def line_uplow(self): 
+        print('Deleting intensity function') 
+        del self._line_uplow
+        
     @property
     def intensity_func(self): 
         return self._intensity_func
           
     @intensity_func.setter 
     def intensity_func(self, intensity): 
         print('Setting intensity function to', intensity) 
@@ -605,14 +619,23 @@
         dvsub = vsub[1]-vsub[0]
         J = 0
         for vs in vsub:
             J += 1/(1+np.abs((v-vs)/v_sigma)**(2*b_slope))
         J = J * dvsub/channel_width
         return J
 
+    @staticmethod
+    def line_uplow_sum(Iup, Ilow):
+        return Iup + Ilow
+    
+    @staticmethod
+    def line_uplow_mask(Iup, Ilow):
+        #velocity nans might differ from Int nans when a z surf is zero and SG is active, nanmax must be used
+        return np.nanmax([Iup, Ilow], axis=0)
+    
     def get_line_profile(self, v_chan, vel2d, linew2d, lineb2d, **kwargs):
         if self.subpixels:
             v_near, v_far = [], []
             for i in range(self.subpixels_sq):
                 v_near.append(self.line_profile(v_chan, vel2d[i]['upper'], linew2d['upper'], lineb2d['upper'], **kwargs))
                 v_far.append(self.line_profile(v_chan, vel2d[i]['lower'], linew2d['lower'], lineb2d['lower'], **kwargs))
 
@@ -632,41 +655,45 @@
         else: int2d = intensity2d
         if isinstance(linewidth2d, numbers.Number): linew2d['upper'] = linew2d['lower'] = linewidth2d
         else: linew2d = linewidth2d
         if isinstance(lineslope2d, numbers.Number): lineb2d['upper'] = lineb2d['lower'] = lineslope2d
         else: lineb2d = lineslope2d
     
         v_near, v_far = self.get_line_profile(v_chan, vel2d, linew2d, lineb2d, **kwargs)
-        int2d_full = np.nanmax([int2d_near, int2d_far], axis=0)
+        int2d_full = self.line_uplow(int2d_near, int2d_far)
         
         if self.beam_kernel:
             inf_mask = np.isnan(int2d_full)
             int2d_full = np.where(inf_mask, 0.0, int2d_full) # Use np.nan_to_num instead
             int2d_full = self.beam_area*convolve(int2d_full, self.beam_kernel, preserve_nan=False)
 
         return int2d_full
 
     def get_cube(self, vchannels, velocity2d, intensity2d, linewidth2d, lineslope2d, make_convolve=True,
-                 nchan=None, rms=None, tb={'nu': False, 'beam': False, 'full': True}, return_data_only=False, header=None, dpc=None, **kwargs_line):
+                 rms=None, tb={'nu': False, 'beam': False, 'full': True}, return_data_only=False, header=None, dpc=None, **kwargs_line):
         
         vel2d, int2d, linew2d, lineb2d = velocity2d, {}, {}, {}
-        line_profile = self.line_profile
-        if nchan is None: nchan=len(vchannels)
         int2d_shape = np.shape(velocity2d['upper'])
         
-        if isinstance(intensity2d, numbers.Number): int2d['upper'] = int2d['lower'] = intensity2d
-        else: int2d = intensity2d
-        if isinstance(linewidth2d, numbers.Number): linew2d['upper'] = linew2d['lower'] = linewidth2d
-        else: linew2d = linewidth2d
-        if isinstance(lineslope2d, numbers.Number): lineb2d['upper'] = lineb2d['lower'] = lineslope2d
-        else: lineb2d = lineslope2d
+        if isinstance(intensity2d, numbers.Number):
+            int2d['upper'] = int2d['lower'] = intensity2d
+        else:
+            int2d = intensity2d
+
+        if isinstance(linewidth2d, numbers.Number):
+            linew2d['upper'] = linew2d['lower'] = linewidth2d
+        else:
+            linew2d = linewidth2d
+
+        if isinstance(lineslope2d, numbers.Number):
+            lineb2d['upper'] = lineb2d['lower'] = lineslope2d
+        else:
+            lineb2d = lineslope2d
 
         """
-        int2d_near_nan = np.isnan(int2d['upper']) #~int2d['upper'].mask
-        int2d_far_nan = np.isnan(int2d['lower']) #~int2d['lower'].mask
         if self.subpixels:
             vel2d_near_nan = np.isnan(vel2d[self.sub_centre_id]['upper'])
             vel2d_far_nan = np.isnan(vel2d[self.sub_centre_id]['lower'])
         else:
             vel2d_near_nan = np.isnan(vel2d['upper']) #~vel2d['upper'].mask
             vel2d_far_nan = np.isnan(vel2d['lower']) #~vel2d['lower'].mask
         """
@@ -674,16 +701,16 @@
         cube = []
         noise = 0.0
         #for _ in itertools.repeat(None, nchan):
         for vchan in vchannels:
             v_near, v_far = self.get_line_profile(vchan, vel2d, linew2d, lineb2d, **kwargs_line)
             int2d_near = int2d['upper'] * v_near
             int2d_far = int2d['lower'] * v_far
-            #vel nans might differ from Int nans when a z surf is zero and SG is active, then nanmax must be used: 
-            int2d_full = np.nanmax([int2d_near, int2d_far], axis=0) 
+            int2d_full = self.line_uplow(int2d_near, int2d_far) 
+            
             if rms is not None:
                 noise = np.random.normal(scale=rms, size=int2d_shape)
                 int2d_full += noise
 
             if self.beam_kernel is not None:
                 if make_convolve:
                     int2d_full[np.isnan(int2d_full)] = noise
@@ -904,14 +931,15 @@
         self._z_upper_func = Model.z_cone
         self._z_lower_func = Model.z_cone_neg
         self._velocity_func = Model.keplerian
         self._intensity_func = Model.intensity_powerlaw
         self._linewidth_func = Model.linewidth_powerlaw
         self._lineslope_func = Model.lineslope_powerlaw
         self._line_profile = Model.line_profile_bell
+        self._line_uplow = Model.line_uplow_mask
         self._use_temperature = False
         self._use_full_channel = False
  
         x_true, y_true = grid['x'], grid['y']
         self.x_true, self.y_true = x_true, y_true
         self.phi_true = grid['phi'] #From 0 to 2pi, old sf3d version: -pi, pi
         self.R_true = grid['R']
```

### Comparing `discminer-0.2.0/discminer/grid.py` & `discminer-0.2.1/discminer/grid.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/icons/button_box.png` & `discminer-0.2.1/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/icons/button_cursor.jpeg` & `discminer-0.2.1/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/icons/button_path.png` & `discminer-0.2.1/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/icons/button_return.png` & `discminer-0.2.1/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/icons/button_surface.png` & `discminer-0.2.1/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/icons/button_trash.jpg` & `discminer-0.2.1/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/pick.py` & `discminer-0.2.1/discminer/pick.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/plottools.py` & `discminer-0.2.1/discminer/plottools.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,15 +513,15 @@
 
 
 def make_polar_map(
         map2d, levels, R, PHI, Rout,
         Rin = 0.0,
         fig=None, ax=None, 
         cmap=get_discminer_cmap('velocity'),
-        fmt='%5.2f', clabel=None, 
+        fmt='%5.2f', clabel=None, gradient=0, 
         #,filaments=[],                            
 ):
     from scipy.interpolate import griddata
 
     #SOME DEFINITIONS
     if fig is None:
         fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(12, 3))
@@ -532,25 +532,52 @@
         Rin = Rin
 
     #GRID AND PLOT
     phi_nonan_deg = np.nan_to_num(PHI, nan=10*np.nanmax(PHI)).to('deg').value
     R_nonan_au = np.nan_to_num(R).to('au').value
 
     dR = int((Rout-Rin)/50)
-    PP, RR = np.meshgrid(np.linspace(-180, 180, 10000),
-                         np.arange(Rin, Rout+dR, dR),
-                         indexing='xy')
+    R1d = np.arange(Rin, Rout+dR, dR)
+    phi1d = np.linspace(-180, 180, 1000)
+    dP = phi1d[1] - phi1d[0]
+
+    PP, RR = np.meshgrid(phi1d, R1d, indexing='xy')
     
     pmap2d = griddata((phi_nonan_deg.flatten(), R_nonan_au.flatten()), map2d.flatten(), (PP, RR), method='linear')
-
-    im=ax.contourf(pmap2d, cmap=cmap,
-                   extent=[PP.min(), PP.max(), RR.min(), RR.max()],
-                   levels=levels,
-                   extend='both', origin='lower')
-
+    
+    make_plot = lambda map2d: ax.contourf(map2d, cmap=cmap,
+                                          extent=[PP.min(), PP.max(), RR.min(), RR.max()],
+                                          levels=levels,
+                                          extend='both', origin='lower')
+    
+    if not gradient:
+        im = make_plot(pmap2d)
+        map2d = pmap2d
+        
+    else:
+        dr, dphi = np.gradient(pmap2d) #in pix-1 units
+        dr /= dR # in au-1 units
+        dphi *= 1/np.radians(dP) * 1/RR # in au-1 rad-1 units 
+        dmax = np.sqrt(dphi**2 + dr**2)
+        
+        if gradient=='phi':
+            im = make_plot(dphi)
+            map2d = dphi
+        elif gradient=='r':
+            im = make_plot(dr)
+            map2d = dr
+        elif gradient=='peak':
+            im = make_plot(dmax)
+            map2d = dmax
+        else:
+            raise InputError(
+                kind, "kind must be 'attribute' or 'residuals'"
+            )
+   
+        
     """
     kw_fil = dict(s=20, lw=1, marker='+')
     for i,filament in enumerate(filaments):
         if i==0 and filament is not None:
             kw_fil.update(dict(fc='red', ec='firebrick'))
         elif i==1 and filament is not None:
             kw_fil.update(dict(fc='blue', ec='navy'))
```

### Comparing `discminer-0.2.0/discminer/rail.py` & `discminer-0.2.1/discminer/rail.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/testyapf.py` & `discminer-0.2.1/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/tools/discminer.mplstyle` & `discminer-0.2.1/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/tools/fit_kernel.py` & `discminer-0.2.1/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer/tools/utils.py` & `discminer-0.2.1/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/discminer.egg-info/PKG-INFO` & `discminer-0.2.1/discminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.0 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.1 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.0/discminer.egg-info/SOURCES.txt` & `discminer-0.2.1/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/setup.py` & `discminer-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/template/README.rst` & `discminer-0.2.1/template/README.rst`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/template/download_MAPS.sh` & `discminer-0.2.1/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.2.1/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.0/template/prepare_data.py` & `discminer-0.2.1/template/prepare_data.py`

 * *Files identical despite different names*

