# Comparing `tmp/pydmt-0.1.78.tar.gz` & `tmp/pydmt-0.1.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmt-0.1.78.tar", last modified: Sun Oct 30 08:51:40 2022, max compression
+gzip compressed data, was "pydmt-0.1.79.tar", last modified: Fri Apr 21 14:50:53 2023, max compression
```

## Comparing `pydmt-0.1.78.tar` & `pydmt-0.1.79.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2022-10-30 08:51:24.000000 pydmt-0.1.78/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1360 2022-10-30 08:51:40.815088 pydmt-0.1.78/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      385 2022-10-30 08:51:20.000000 pydmt-0.1.78/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/pydmt/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/__init__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/pydmt/api/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/api/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/api/builder.py
--rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/api/copy.py
--rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/api/fail.py
--rw-r--r--   0 mark      (1000) mark      (1000)      613 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/api/feature.py
--rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/api/one_source_one_target.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/pydmt/builders/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/builders/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/builders/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      515 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/builders/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/builders/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/builders/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1390 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/builders/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/builders/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1716 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/builders/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1669 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/builders/venv_full.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:36:32.000000 pydmt-0.1.78/pydmt/builders/yaml.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2230 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/configs.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/pydmt/core/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/core/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/core/cache.py
--rw-r--r--   0 mark      (1000) mark      (1000)       50 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/core/graph.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/core/pydmt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      491 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/core/tempdir.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/pydmt/features/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/features/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1422 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)      392 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)      325 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/venv_full.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1010 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/features/yaml.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/pydmt/helpers/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      129 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/composites.py
--rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/deb.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/deb_python_package.py
--rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/files.py
--rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/general.py
--rw-r--r--   0 mark      (1000) mark      (1000)      313 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/helpers/git.py
--rw-r--r--   0 mark      (1000) mark      (1000)      465 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/github.py
--rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/messages.py
--rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/helpers/misc.py
--rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/pkgs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      218 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/project.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4899 2022-10-30 08:50:46.000000 pydmt-0.1.78/pydmt/helpers/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)      775 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/signature.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/helpers/snipplets.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1333 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/helpers/urls.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4961 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      175 2022-10-30 08:51:20.000000 pydmt-0.1.78/pydmt/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/pydmt/utils/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/utils/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-09-11 10:31:12.000000 pydmt-0.1.78/pydmt/utils/digest.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1044 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/utils/digester.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1244 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/utils/filesystem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/utils/logging.py
--rw-r--r--   0 mark      (1000) mark      (1000)      265 2022-06-13 04:33:28.000000 pydmt-0.1.78/pydmt/utils/php.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2822 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/utils/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1236 2022-10-18 09:50:26.000000 pydmt-0.1.78/pydmt/utils/subprocess.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-30 08:51:40.815088 pydmt-0.1.78/pydmt.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1360 2022-10-30 08:51:40.000000 pydmt-0.1.78/pydmt.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     1602 2022-10-30 08:51:40.000000 pydmt-0.1.78/pydmt.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-10-30 08:51:40.000000 pydmt-0.1.78/pydmt.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       43 2022-10-30 08:51:40.000000 pydmt-0.1.78/pydmt.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       77 2022-10-30 08:51:40.000000 pydmt-0.1.78/pydmt.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2022-10-30 08:51:40.000000 pydmt-0.1.78/pydmt.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2022-10-30 08:51:40.815088 pydmt-0.1.78/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2022-10-30 08:51:20.000000 pydmt-0.1.78/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.765725 pydmt-0.1.79/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-21 14:49:35.000000 pydmt-0.1.79/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-21 14:50:53.765725 pydmt-0.1.79/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      391 2023-04-21 14:49:35.000000 pydmt-0.1.79/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.760725 pydmt-0.1.79/pydmt/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/__init__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.761725 pydmt-0.1.79/pydmt/api/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/api/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.1.79/pydmt/api/builder.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.1.79/pydmt/api/copy.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.1.79/pydmt/api/fail.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      613 2020-09-20 14:25:08.000000 pydmt-0.1.79/pydmt/api/feature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.1.79/pydmt/api/one_source_one_target.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.762725 pydmt-0.1.79/pydmt/builders/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/builders/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.1.79/pydmt/builders/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      428 2023-04-21 14:45:52.000000 pydmt-0.1.79/pydmt/builders/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.1.79/pydmt/builders/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.1.79/pydmt/builders/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1390 2022-10-15 00:29:42.000000 pydmt-0.1.79/pydmt/builders/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.1.79/pydmt/builders/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1524 2023-04-21 14:45:15.000000 pydmt-0.1.79/pydmt/builders/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1584 2023-04-21 14:45:35.000000 pydmt-0.1.79/pydmt/builders/venv_full.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.1.79/pydmt/builders/yaml.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2230 2022-06-25 07:24:09.000000 pydmt-0.1.79/pydmt/configs.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.763725 pydmt-0.1.79/pydmt/core/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/core/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.1.79/pydmt/core/cache.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.1.79/pydmt/core/graph.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.1.79/pydmt/core/pydmt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/core/tempdir.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.763725 pydmt-0.1.79/pydmt/features/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/features/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.1.79/pydmt/features/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.1.79/pydmt/features/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1422 2022-05-04 08:25:10.000000 pydmt-0.1.79/pydmt/features/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.1.79/pydmt/features/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.1.79/pydmt/features/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.1.79/pydmt/features/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      392 2022-05-09 05:06:11.000000 pydmt-0.1.79/pydmt/features/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      325 2022-05-09 04:57:20.000000 pydmt-0.1.79/pydmt/features/venv_full.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1010 2022-05-04 08:23:35.000000 pydmt-0.1.79/pydmt/features/yaml.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.764725 pydmt-0.1.79/pydmt/helpers/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.1.79/pydmt/helpers/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.1.79/pydmt/helpers/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      129 2022-05-16 19:51:40.000000 pydmt-0.1.79/pydmt/helpers/composites.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.1.79/pydmt/helpers/deb.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.1.79/pydmt/helpers/deb_python_package.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.1.79/pydmt/helpers/files.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.1.79/pydmt/helpers/general.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      313 2022-06-25 06:56:24.000000 pydmt-0.1.79/pydmt/helpers/git.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      465 2022-05-19 21:23:46.000000 pydmt-0.1.79/pydmt/helpers/github.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.1.79/pydmt/helpers/messages.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.1.79/pydmt/helpers/misc.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.1.79/pydmt/helpers/pkgs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      218 2022-05-18 18:52:21.000000 pydmt-0.1.79/pydmt/helpers/project.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4895 2023-03-08 23:18:25.000000 pydmt-0.1.79/pydmt/helpers/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      775 2022-05-19 21:09:23.000000 pydmt-0.1.79/pydmt/helpers/signature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.1.79/pydmt/helpers/snipplets.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1333 2022-10-12 19:19:30.000000 pydmt-0.1.79/pydmt/helpers/urls.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4961 2022-10-14 23:14:11.000000 pydmt-0.1.79/pydmt/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      175 2023-04-21 14:49:47.000000 pydmt-0.1.79/pydmt/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.765725 pydmt-0.1.79/pydmt/utils/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.1.79/pydmt/utils/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.1.79/pydmt/utils/digest.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.1.79/pydmt/utils/digester.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.1.79/pydmt/utils/filesystem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.1.79/pydmt/utils/logging.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.1.79/pydmt/utils/php.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2822 2022-10-15 00:35:27.000000 pydmt-0.1.79/pydmt/utils/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1337 2023-04-21 14:48:53.000000 pydmt-0.1.79/pydmt/utils/subprocess.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-21 14:50:53.761725 pydmt-0.1.79/pydmt.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1364 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     1602 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       42 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       77 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2023-04-21 14:50:53.000000 pydmt-0.1.79/pydmt.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-21 14:50:53.765725 pydmt-0.1.79/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-21 14:49:47.000000 pydmt-0.1.79/setup.py
```

### Comparing `pydmt-0.1.78/LICENSE` & `pydmt-0.1.79/LICENSE`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/PKG-INFO` & `pydmt-0.1.79/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.1.78
+Version: 0.1.79
 Summary: python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
+Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pydmt
 Keywords: pydmt,cons,scons,software construction,make,cmake,maven,mvn
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -35,12 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.1.78
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022
-
+version: 0.1.79
 
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pydmt-0.1.78/pydmt/api/builder.py` & `pydmt-0.1.79/pydmt/api/builder.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/api/feature.py` & `pydmt-0.1.79/pydmt/api/feature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/api/one_source_one_target.py` & `pydmt-0.1.79/pydmt/api/one_source_one_target.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/builders/apt.py` & `pydmt-0.1.79/pydmt/builders/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/builders/mako.py` & `pydmt-0.1.79/pydmt/builders/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/builders/reqs.py` & `pydmt-0.1.79/pydmt/builders/reqs.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/builders/sphinx.py` & `pydmt-0.1.79/pydmt/builders/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/builders/venv.py` & `pydmt-0.1.79/pydmt/builders/venv.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 
 import os
 import shutil
 
 from pydmt.utils.filesystem import mkdir_touch
-from pydmt.utils.subprocess import check_call
+from pydmt.utils.subprocess import check_call, check_call_ve
 from pydmt.utils.python import collect_reqs, collect_bootstrap_reqs, get_install_args
 
 from pydmt.api.one_source_one_target import OneSourceOneTarget
 
 SOURCE_FILE = "config/python.py"
 TARGET_FOLDER = ".venv/default"
 
@@ -32,32 +32,21 @@
             shutil.rmtree(TARGET_FOLDER)
         # create new virtual env
         args = [
             "virtualenv",
             TARGET_FOLDER,
         ]
         check_call(args)
-        # now create bootstrap packages so that we could read config/*.py
-        args = [
-            "venv-run",
-            "--venv",
-            ".venv/default",
-            "--",
-        ]
-        args.extend(get_install_args())
+        # install bootstrap packages so that we could read config/* files
         packs = collect_bootstrap_reqs()
         if packs:
+            args = get_install_args()
             args.extend(packs)
-            check_call(args)
+            check_call_ve(args)
         # now install regular packages (we only run the install if there are packages to install)
-        args = [
-            "venv-run",
-            "--venv",
-            ".venv/default",
-            "--",
-        ]
-        args.extend(get_install_args())
         packs = collect_reqs()
         if packs:
             args.extend(packs)
-            check_call(args)
+            args = get_install_args()
+            args.extend(packs)
+            check_call_ve(args)
         mkdir_touch(self.target)
```

### Comparing `pydmt-0.1.78/pydmt/builders/venv_full.py` & `pydmt-0.1.79/pydmt/builders/venv_full.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import shutil
 from typing import Generator, Tuple, Sequence
 
 from pydmt.api.builder import Builder, Node, SourceFile, TargetFolder
 from pydmt.utils.filesystem import files_under_folder
 from pydmt.utils.digest import sha1_file
-from pydmt.utils.subprocess import check_call
+from pydmt.utils.subprocess import check_call, check_call_ve
 from pydmt.utils.python import collect_reqs, get_install_args
 
 SOURCE_FILE = "config/python.py"
 TARGET_FOLDER = ".venv/default"
 
 
 class BuilderVenvFull(Builder):
@@ -41,22 +41,17 @@
         if os.path.isdir(TARGET_FOLDER):
             shutil.rmtree(TARGET_FOLDER)
         args = [
             "virtualenv",
             TARGET_FOLDER,
         ]
         check_call(args)
-        args = [
-            "venv-run",
-            "--venv",
-            ".venv/default",
-            "--",
-        ]
-        args.extend(get_install_args())
+        # packages
         packs = collect_reqs()
         if packs:
+            args = get_install_args()
             args.extend(packs)
-            check_call(args)
+            check_call_ve(args)
 
     def yield_results(self) -> Generator[Tuple[str, str], None, None]:
         for x in files_under_folder(TARGET_FOLDER):
             yield sha1_file(x), x
```

### Comparing `pydmt-0.1.78/pydmt/builders/yaml.py` & `pydmt-0.1.79/pydmt/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/configs.py` & `pydmt-0.1.79/pydmt/configs.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/core/cache.py` & `pydmt-0.1.79/pydmt/core/cache.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/core/pydmt.py` & `pydmt-0.1.79/pydmt/core/pydmt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/features/apt.py` & `pydmt-0.1.79/pydmt/features/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/features/mako.py` & `pydmt-0.1.79/pydmt/features/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/features/yaml.py` & `pydmt-0.1.79/pydmt/features/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/helpers/apt.py` & `pydmt-0.1.79/pydmt/helpers/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/helpers/deb.py` & `pydmt-0.1.79/pydmt/helpers/deb.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/helpers/deb_python_package.py` & `pydmt-0.1.79/pydmt/helpers/deb_python_package.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/helpers/python.py` & `pydmt-0.1.79/pydmt/helpers/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     :param dictionary:
     :param quote_char:
     :param comma_after:
     :return:
     """
     out = "{\n"
     for k, v in dictionary.items():
-        spaces = (((level + 1) * 4) * " ")
+        spaces = ((level + 1) * 4) * " "
         out += f"{spaces}{quote_char}{k}{quote_char}: {v},\n"
-    spaces = ((level * 4) * " ")
+    spaces = (level * 4) * " "
     out += f"{spaces}}}"
     if comma_after:
         out += ","
     return out
 
 
 def find_packages(path: str) -> List[str]:
```

### Comparing `pydmt-0.1.78/pydmt/helpers/signature.py` & `pydmt-0.1.79/pydmt/helpers/signature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/helpers/snipplets.py` & `pydmt-0.1.79/pydmt/helpers/snipplets.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/helpers/urls.py` & `pydmt-0.1.79/pydmt/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/main.py` & `pydmt-0.1.79/pydmt/main.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/utils/digest.py` & `pydmt-0.1.79/pydmt/utils/digest.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/utils/digester.py` & `pydmt-0.1.79/pydmt/utils/digester.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/utils/filesystem.py` & `pydmt-0.1.79/pydmt/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/utils/python.py` & `pydmt-0.1.79/pydmt/utils/python.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/pydmt/utils/subprocess.py` & `pydmt-0.1.79/pydmt/utils/subprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import os.path
 import subprocess
 from typing import List
 
 from pydmt.configs import ConfigSubprocess
 
 
 def check_call(args: List[str]) -> None:
@@ -23,18 +24,19 @@
     if ConfigSubprocess.quiet:
         subprocess.check_call(args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
     else:
         subprocess.check_call(args)
 
 
 def check_call_ve(orig_args: List[str]) -> None:
+    # we cann venv-run with absolute path since it may change folder
     args = [
         "venv-run",
         "--venv",
-        ".venv/default",
+        os.path.abspath(".venv/default"),
         "--",
     ]
     args.extend(orig_args)
     if ConfigSubprocess.print_command:
         print(f"running {args}")
     if ConfigSubprocess.quiet:
         subprocess.check_call(args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```

### Comparing `pydmt-0.1.78/pydmt.egg-info/PKG-INFO` & `pydmt-0.1.79/pydmt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.1.78
+Version: 0.1.79
 Summary: python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
+Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pydmt
 Keywords: pydmt,cons,scons,software construction,make,cmake,maven,mvn
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -35,12 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.1.78
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022
-
+version: 0.1.79
 
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pydmt-0.1.78/pydmt.egg-info/SOURCES.txt` & `pydmt-0.1.79/pydmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydmt-0.1.78/setup.py` & `pydmt-0.1.79/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,69 +5,69 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pydmt",
-    version="0.1.78",
+    version="0.1.79",
     packages=[
-        'pydmt',
-        'pydmt.api',
-        'pydmt.builders',
-        'pydmt.core',
-        'pydmt.features',
-        'pydmt.helpers',
-        'pydmt.utils',
+        "pydmt",
+        "pydmt.api",
+        "pydmt.builders",
+        "pydmt.core",
+        "pydmt.features",
+        "pydmt.helpers",
+        "pydmt.utils",
     ],
     # from here all is optional
     description="python dependency management tool",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'pydmt',
-        'cons',
-        'scons',
-        'software construction',
-        'make',
-        'cmake',
-        'maven',
-        'mvn',
+        "pydmt",
+        "cons",
+        "scons",
+        "software construction",
+        "make",
+        "cmake",
+        "maven",
+        "mvn",
     ],
     url="https://veltzer.github.io/pydmt",
     download_url="https://github.com/veltzer/pydmt",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
     install_requires=[
-        'pyfakeuse',
-        'pylogconf',
-        'pytconf',
-        'mako',
-        'sphinx',
-        'pyyaml',
-        'jsonschema',
-        'venv-run',
-        'gitpython',
+        "pyfakeuse",
+        "pylogconf",
+        "pytconf",
+        "mako",
+        "sphinx",
+        "pyyaml",
+        "jsonschema",
+        "venv-run",
+        "gitpython",
     ],
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: MIT License',
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
     ],
     entry_points={"console_scripts": [
-        'pydmt=pydmt.main:main',
+        "pydmt=pydmt.main:main",
     ]},
 )
```

