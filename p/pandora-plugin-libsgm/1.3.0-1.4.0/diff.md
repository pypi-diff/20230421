# Comparing `tmp/pandora_plugin_libsgm-1.3.0.tar.gz` & `tmp/pandora_plugin_libsgm-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Pandora_plugin_libSGM/Pandora_plugin_libSGM/dist/.tmp-90vt7ywx/pandora_plugin_libsgm-1.3.0.tar", last modified: Tue Mar 28 09:35:53 2023, max compression
+gzip compressed data, was "/home/runner/work/Pandora_plugin_libSGM/Pandora_plugin_libSGM/dist/.tmp-7c_of7w1/pandora_plugin_libsgm-1.4.0.tar", last modified: Fri Apr 21 17:23:29 2023, max compression
```

## Comparing `pandora_plugin_libsgm-1.3.0.tar` & `pandora_plugin_libsgm-1.4.0.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/.github/workflows/pandora_plugin_libsgm_ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/.gitlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/.gitlab/issue_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/.gitlab/issue_templates/Bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/.gitlab/issue_templates/Proposition.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/.gitlab/merge_request_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/.gitlab/merge_request_templates/MR.md
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_rose.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_rose_large.png
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_rose_medium.png
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_rose_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo_large.png
--rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo_medium.png
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo_very_small.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/doc/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/doc/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/_static/css/my_custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/doc/source/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/developer_guide/penalty_and_invalid_value.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/abstract_sgm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/lib_3sgm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/lib_sgm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/penalty.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/penalty_mc_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/penalty_sgm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/tests/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/conf/3sgm.json
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/conf/sgm.json
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/conf/sgm_python.json
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/conf/sgm_python_parall.json
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/conf/sgm_zncc.json
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/conf/sgm_zncc_python.json
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/conf/sgm_zncc_python_parall.json
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/disable_test_plugin_python_parall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/tests/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/inputs/data_description.md
--rw-r--r--   0 runner    (1001) docker     (123)   169076 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/inputs/left.png
--rw-r--r--   0 runner    (1001) docker     (123)  2027662 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/inputs/left_rgb.tif
--rw-r--r--   0 runner    (1001) docker     (123)   169076 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/inputs/right.png
--rw-r--r--   0 runner    (1001) docker     (123)  2027662 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/inputs/right_rgb.tif
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/inputs/white_band_mask.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:35:53.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/data_description.md
--rw-r--r--   0 runner    (1001) docker     (123)   675898 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/disp_left.tif
--rw-r--r--   0 runner    (1001) docker     (123)   675898 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/disp_left_zncc.tif
--rw-r--r--   0 runner    (1001) docker     (123)   675898 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/disp_right.tif
--rw-r--r--   0 runner    (1001) docker     (123)   675898 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/disp_right_zncc.tif
--rw-r--r--   0 runner    (1001) docker     (123)   675710 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/left_disparity_3sgm.tif
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/occl.png
--rw-r--r--   0 runner    (1001) docker     (123)   675710 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/outputs/right_disparity_3sgm.tif
--rw-r--r--   0 runner    (1001) docker     (123)    19933 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/test_lib3sgm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25939 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/test_libsgm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/test_penality_sgm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/test_penalty_mc_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-03-28 09:10:46.000000 pandora_plugin_libsgm-1.3.0/tests/test_plugin_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/.github/workflows/pandora_plugin_libsgm_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/.gitlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/.gitlab/issue_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/.gitlab/issue_templates/Bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/.gitlab/issue_templates/Proposition.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/.gitlab/merge_request_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/.gitlab/merge_request_templates/MR.md
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_rose.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_rose_large.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_rose_medium.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_rose_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo_large.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo_medium.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo_very_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/doc/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/doc/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/_static/css/my_custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/doc/source/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/developer_guide/penalty_and_invalid_value.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17930 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/abstract_sgm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/lib_3sgm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/lib_sgm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/penalty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/penalty_mc_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/penalty_sgm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/tests/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/conf/3sgm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/conf/sgm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/conf/sgm_python.json
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/conf/sgm_python_parall.json
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/conf/sgm_zncc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/conf/sgm_zncc_python.json
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/conf/sgm_zncc_python_parall.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/disable_test_plugin_python_parall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/data_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)   169076 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/left.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2027826 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/left_classif.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  2027662 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/left_rgb.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   169076 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/right.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2027826 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/right_classif.tif
+-rw-r--r--   0 runner    (1001) docker     (123)  2027662 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/right_rgb.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/inputs/white_band_mask.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:23:29.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/data_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)   675898 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/disp_left.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   675898 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/disp_left_zncc.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   675898 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/disp_right.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   675898 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/disp_right_zncc.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   675710 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/left_disparity_3sgm.tif
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/occl.png
+-rw-r--r--   0 runner    (1001) docker     (123)   675710 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/outputs/right_disparity_3sgm.tif
+-rw-r--r--   0 runner    (1001) docker     (123)    52471 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/test_lib3sgm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/test_libsgm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/test_penality_sgm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/test_penalty_mc_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-21 17:02:03.000000 pandora_plugin_libsgm-1.4.0/tests/test_plugin_python.py
```

### Comparing `pandora_plugin_libsgm-1.3.0/.github/workflows/pandora_plugin_libsgm_ci.yml` & `pandora_plugin_libsgm-1.4.0/.github/workflows/pandora_plugin_libsgm_ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     - name: Set up Python 3.x
       uses: actions/setup-python@v2
       with:
         python-version: '3.7'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install codecov
         pip freeze
     - name: Install Pandora plugin libSGM
       run: |
         pip install .[dev]
         pip freeze
     - name: Clone Pandora submodule
       run: |
```

### Comparing `pandora_plugin_libsgm-1.3.0/.gitlab/merge_request_templates/MR.md` & `pandora_plugin_libsgm-1.4.0/.gitlab/merge_request_templates/MR.md`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/.pre-commit-config.yaml` & `pandora_plugin_libsgm-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/.pylintrc` & `pandora_plugin_libsgm-1.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/AUTHORS.md` & `pandora_plugin_libsgm-1.4.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/CHANGELOG.md` & `pandora_plugin_libsgm-1.4.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
-## Unreleased
+## 1.4.0 (April 2023)
 
-### Added
+### Added 
+
+- Update warnings mentioning semantic_segmentation step in pipeline. 
+- Adapt tests to new check conf pandora's format. [#77]
+- Add multiband classifications. [#76]
+
+### Fixed
 
-### Changed
+- Deletion of the pip install codecov of githubAction CI.
 
 ## 1.3.0 (March 2023)
 
 ### Added
 
 - Multiband images compatibility. [#72]
```

### Comparing `pandora_plugin_libsgm-1.3.0/LICENSE` & `pandora_plugin_libsgm-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/NOTICE` & `pandora_plugin_libsgm-1.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/PKG-INFO` & `pandora_plugin_libsgm-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandora_plugin_libsgm
-Version: 1.3.0
+Version: 1.4.0
 Summary: Pandora plugin to optimize the cost volume with the LibSGM library
 Home-page: https://github.com/CNES/Pandora_plugin_libsgm
 Author: CNES
 Author-email: myriam.cournet@cnes.fr
 License: Apache License 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pandora_plugin_libsgm Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: pandora_plugin_libsgm Version: 1.4.0 Summary:
 Pandora plugin to optimize the cost volume with the LibSGM library Home-page:
 https://github.com/CNES/Pandora_plugin_libsgm Author: CNES Author-email:
 myriam.cournet@cnes.fr License: Apache License 2.0 Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
 docs License-File: LICENSE
                       ****** Pandora plugin libSGM ******
             *** Semi-Global Matching algorithm plugin for [https://
```

### Comparing `pandora_plugin_libsgm-1.3.0/README.md` & `pandora_plugin_libsgm-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/Makefile` & `pandora_plugin_libsgm-1.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/make.bat` & `pandora_plugin_libsgm-1.4.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_rose.svg` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_rose.svg`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_rose_large.png` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_rose_large.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_rose_medium.png` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_rose_medium.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_rose_small.png` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_rose_small.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo.svg` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo.svg`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo_large.png` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo_large.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo_medium.png` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo_medium.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo_small.png` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo_small.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/Images/logo/logo_typo_very_small.png` & `pandora_plugin_libsgm-1.4.0/doc/source/Images/logo/logo_typo_very_small.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/_static/css/my_custom.css` & `pandora_plugin_libsgm-1.4.0/doc/source/_static/css/my_custom.css`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/conf.py` & `pandora_plugin_libsgm-1.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/developer_guide/penalty_and_invalid_value.rst` & `pandora_plugin_libsgm-1.4.0/doc/source/developer_guide/penalty_and_invalid_value.rst`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/getting_started.rst` & `pandora_plugin_libsgm-1.4.0/doc/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/doc/source/index.rst` & `pandora_plugin_libsgm-1.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/mypy.ini` & `pandora_plugin_libsgm-1.4.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/__init__.py` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/__init__.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/abstract_sgm.py` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/abstract_sgm.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,17 +105,15 @@
         schema = {
             "sgm_version": And(str, lambda x: is_method(x, ["c++", "python_libsgm", "python_libsgm_parall"])),
             "optimization_method": And(str, lambda x: is_method(x, ["sgm", "3sgm"])),
             "overcounting": bool,
             "min_cost_paths": bool,
             "use_confidence": bool,
             "penalty": dict,
-            OptionalKey("geometric_prior"): And(
-                dict, lambda x: cfg["geometric_prior"]["source"] in ["internal", "classif", "segm"]  # type: ignore
-            ),
+            OptionalKey("geometric_prior"): dict,
         }
 
         checker = Checker(schema)
         checker.validate(cfg)
         return cfg
 
     def optimize_cv(self, cv: xr.Dataset, img_left: xr.Dataset, img_right: xr.Dataset) -> xr.Dataset:
```

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/lib_3sgm.py` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/lib_3sgm.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import logging
 import sys
 from typing import Union, Tuple
 
 import numpy as np
 import xarray as xr
-
+from pandora.img_tools import fuse_classification_bands
 from . import abstract_sgm
 
 
 @abstract_sgm.AbstractSGM.register_subclass("3sgm")
 class SEGSEMSGM(abstract_sgm.AbstractSGM):
     """
 
@@ -52,30 +52,56 @@
         :param cfg: optional configuration, {}
         :type cfg: dict
         :return: None
         """
         super().__init__(**cfg)
         self.cfg = self.check_geometric_prior(cfg)
         self._geometric_prior = self.cfg["geometric_prior"]
+        if self._geometric_prior["source"] == "classif":  # type: ignore
+            self._classes = self._geometric_prior["classes"]  # type: ignore
 
     def check_geometric_prior(self, cfg: dict) -> dict:
         """
         Verify geometric_prior parameter for 3sgm classification
         :param cfg:
         :type cfg: dict
         :return cfg: optimization configuration updated
         :rtype cfg: dict
         """
 
+        # Geometric prior is internal if not mentioned
         if "geometric_prior" not in cfg:
             cfg["geometric_prior"] = self._GEOMETRIC_PRIOR
         elif isinstance(cfg["geometric_prior"], dict):
             if not cfg["geometric_prior"]["source"] in self._AVAILABLE_GEOMETRIC_PRIOR:
                 logging.error("%s is not available as a geometric prior", cfg["geometric_prior"]["source"])
 
+        # Must be classif, segm or internal
+        if cfg["geometric_prior"]["source"] not in self._AVAILABLE_GEOMETRIC_PRIOR:
+            logging.error("%s is not available as a geometric prior source", cfg["geometric_prior"]["source"])
+            sys.exit(1)
+
+        # If source is classif, classes must be instantiated
+        if cfg["geometric_prior"]["source"] == "classif":
+            if "classes" not in cfg["geometric_prior"]:
+                logging.error("Classes must be instantiated if source is classif")
+                sys.exit(1)
+            else:
+                # If source is classif, classes must be instantiated as a list of string
+                if not isinstance(cfg["geometric_prior"]["classes"], list) and not all(
+                    isinstance(item, str) for item in cfg["geometric_prior"]["classes"]
+                ):
+                    logging.error("Classes must be a list of string")
+                    sys.exit(1)
+
+        if cfg["geometric_prior"]["source"] == "segm":
+            if "classes" in cfg["geometric_prior"]:
+                logging.error("Classes can't be instantiated if source is segm")
+                sys.exit(1)
+
         return cfg
 
     def desc(self):
         """
         Describes the optimization method
         """
         print("Optimization with 3SGM")
@@ -104,37 +130,42 @@
         # internal (from cv), segm or classif (from image)
         mode = self._geometric_prior["source"]  # type: ignore
 
         if mode in ["segm", "classif"]:
             # if geometric_prior comes from the image (segm or classif)
             if mode in img_left:
                 geometric_prior_array = img_left[mode].data
+                if mode == "classif":
+                    geometric_prior_array = fuse_classification_bands(img_left, self._classes)
             else:
                 logging.warning("%s not in image dataset.", mode)
                 sys.exit(1)
         # if user wants to use another type of geometric prior
         else:
             geometric_prior_array = np.ones(img_shape)
             if mode != "internal":
                 logging.warning(
                     "User wants to use a mode not in image dataset. \n "
                     "Default is used : no optimization with 3sgm will be performed."
                 )
             else:
-                # if layer not computed we add a default one
-                logging.warning("For now, 3SGM doesn't compute piecewise layer from internal mode.")
                 if "internal" not in cv:
+                    # if layer not computed we add a default one
                     prior_array = xr.DataArray(
                         data=geometric_prior_array,
                         coords=[("row", np.arange(img_shape[0])), ("col", np.arange(img_shape[1]))],
                     )
                     logging.warning(
                         "User wants to use a mode not in cost volume. \n "
                         "Default is used : no optimization with 3sgm will be performed."
                     )
+                    logging.warning(
+                        "If semantic_segmentation is present in the pipeline, \n "
+                        "it should be placed before the 3SGM optimization step."
+                    )
                     # Apply geometric prior to cost volume
                     cv["internal"] = prior_array
                 else:
                     geometric_prior_array = cv["internal"].data
 
         geometric_prior_array = geometric_prior_array.astype(np.float32)
         geometric_prior_array[np.isnan(geometric_prior_array)] = -9999
```

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/lib_sgm.py` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/lib_sgm.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/__init__.py` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/__init__.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/penalty.py` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/penalty.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/penalty_mc_cnn.py` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/penalty_mc_cnn.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm/penalty/penalty_sgm.py` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm/penalty/penalty_sgm.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/PKG-INFO` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandora-plugin-libsgm
-Version: 1.3.0
+Version: 1.4.0
 Summary: Pandora plugin to optimize the cost volume with the LibSGM library
 Home-page: https://github.com/CNES/Pandora_plugin_libsgm
 Author: CNES
 Author-email: myriam.cournet@cnes.fr
 License: Apache License 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pandora-plugin-libsgm Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: pandora-plugin-libsgm Version: 1.4.0 Summary:
 Pandora plugin to optimize the cost volume with the LibSGM library Home-page:
 https://github.com/CNES/Pandora_plugin_libsgm Author: CNES Author-email:
 myriam.cournet@cnes.fr License: Apache License 2.0 Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
 docs License-File: LICENSE
                       ****** Pandora plugin libSGM ******
             *** Semi-Global Matching algorithm plugin for [https://
```

### Comparing `pandora_plugin_libsgm-1.3.0/pandora_plugin_libsgm.egg-info/SOURCES.txt` & `pandora_plugin_libsgm-1.4.0/pandora_plugin_libsgm.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -62,16 +62,18 @@
 tests/conf/sgm_python.json
 tests/conf/sgm_python_parall.json
 tests/conf/sgm_zncc.json
 tests/conf/sgm_zncc_python.json
 tests/conf/sgm_zncc_python_parall.json
 tests/inputs/data_description.md
 tests/inputs/left.png
+tests/inputs/left_classif.tif
 tests/inputs/left_rgb.tif
 tests/inputs/right.png
+tests/inputs/right_classif.tif
 tests/inputs/right_rgb.tif
 tests/inputs/white_band_mask.png
 tests/outputs/data_description.md
 tests/outputs/disp_left.tif
 tests/outputs/disp_left_zncc.tif
 tests/outputs/disp_right.tif
 tests/outputs/disp_right_zncc.tif
```

### Comparing `pandora_plugin_libsgm-1.3.0/setup.cfg` & `pandora_plugin_libsgm-1.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 python_requires = >=3.7
 setup_requires = 
 	setuptools_scm # Following https://pypi.org/project/setuptools-scm/
 install_requires = 
 	numpy
 	rasterio
 	libsgm==0.4.*
-	pandora>=1.4.0
+	pandora>=1.5.0
 	xarray
 	json-checker
 package_dir = 
 	. = plugin_libsgm
 packages = find:
 
 [options.extras_require]
```

### Comparing `pandora_plugin_libsgm-1.3.0/setup.py` & `pandora_plugin_libsgm-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/sonar-project.properties` & `pandora_plugin_libsgm-1.4.0/sonar-project.properties`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/common.py` & `pandora_plugin_libsgm-1.4.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/conf/3sgm.json` & `pandora_plugin_libsgm-1.4.0/tests/conf/3sgm.json`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/conf/sgm.json` & `pandora_plugin_libsgm-1.4.0/tests/conf/sgm.json`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/conf/sgm_python.json` & `pandora_plugin_libsgm-1.4.0/tests/conf/sgm_python.json`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/conf/sgm_python_parall.json` & `pandora_plugin_libsgm-1.4.0/tests/conf/sgm_python_parall.json`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/conf/sgm_zncc.json` & `pandora_plugin_libsgm-1.4.0/tests/conf/sgm_zncc.json`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/conf/sgm_zncc_python.json` & `pandora_plugin_libsgm-1.4.0/tests/conf/sgm_zncc_python.json`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/conf/sgm_zncc_python_parall.json` & `pandora_plugin_libsgm-1.4.0/tests/conf/sgm_zncc_python_parall.json`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/disable_test_plugin_python_parall.py` & `pandora_plugin_libsgm-1.4.0/tests/disable_test_plugin_python_parall.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/inputs/data_description.md` & `pandora_plugin_libsgm-1.4.0/tests/inputs/data_description.md`

 * *Files 25% similar despite different names*

```diff
@@ -4,8 +4,11 @@
 
 * **left.png and right.png :**  
 Our data test sample is based on the 2003 Middleburry dataset (D. Scharstein & R. Szeliski, 2003).
 (D. Scharstein & R. Szeliski, 2002). Scharstein, D., & Szeliski, R. (2002). A taxonomy and evaluation of dense two-frame stereo correspondence algorithms. International journal of computer vision, 47(1-3), 7-42.
 (D. Scharstein & R. Szeliski, 2003). Scharstein, D., & Szeliski, R. (2003, June). High-accuracy stereo depth maps using structured light. In 2003 IEEE Computer Society Conference on Computer Vision and Pattern Recognition, 2003. Proceedings. (Vol. 1, pp. I-I). IEEE.
 
 * **white_band_mask.png** 
-Manually computed binary mask with strides for segmentation and classification for 3sgm optimization method tests. 
+Manually computed binary mask with strides for segmentation and classification for 3sgm optimization method tests. 
+
+* **left_classif.tif and right_classif.tif** 
+Manually computed 3 dimensions binary classification for 3sgm classification method tests.
```

### Comparing `pandora_plugin_libsgm-1.3.0/tests/inputs/left.png` & `pandora_plugin_libsgm-1.4.0/tests/inputs/left.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/inputs/left_rgb.tif` & `pandora_plugin_libsgm-1.4.0/tests/inputs/left_rgb.tif`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/inputs/right.png` & `pandora_plugin_libsgm-1.4.0/tests/inputs/right.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/inputs/right_rgb.tif` & `pandora_plugin_libsgm-1.4.0/tests/inputs/right_rgb.tif`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/outputs/data_description.md` & `pandora_plugin_libsgm-1.4.0/tests/outputs/data_description.md`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/outputs/disp_left.tif` & `pandora_plugin_libsgm-1.4.0/tests/outputs/disp_left.tif`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/outputs/disp_left_zncc.tif` & `pandora_plugin_libsgm-1.4.0/tests/outputs/disp_left_zncc.tif`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/outputs/disp_right.tif` & `pandora_plugin_libsgm-1.4.0/tests/outputs/disp_right.tif`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/outputs/disp_right_zncc.tif` & `pandora_plugin_libsgm-1.4.0/tests/outputs/disp_right_zncc.tif`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/outputs/left_disparity_3sgm.tif` & `pandora_plugin_libsgm-1.4.0/tests/outputs/left_disparity_3sgm.tif`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/outputs/occl.png` & `pandora_plugin_libsgm-1.4.0/tests/outputs/occl.png`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/outputs/right_disparity_3sgm.tif` & `pandora_plugin_libsgm-1.4.0/tests/outputs/right_disparity_3sgm.tif`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/test_libsgm.py` & `pandora_plugin_libsgm-1.4.0/tests/test_libsgm.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         # Import pandora plugins
         pandora.import_plugin()
 
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
         # Run the pandora pipeline
-        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, 0, user_cfg["pipeline"])
+        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, 0, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the percentage of pixel errors is > 0.20, raise an error
         if common.error(left["disparity_map"].data, self.disp_left, 1, flag_inverse_value=False) > 0.20:
             raise AssertionError
 
         # Compares the calculated left disparity map with the ground truth
@@ -164,15 +164,15 @@
         # Import pandora plugins
         pandora.import_plugin()
 
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
         # Run the pandora pipeline
-        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, -1, user_cfg["pipeline"])
+        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, -1, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the percentage of pixel errors is > 0.20, raise an error
         if common.error(left["disparity_map"].data, self.disp_left, 1, flag_inverse_value=False) > 0.20:
             raise AssertionError
 
         # Compares the calculated left disparity map with the ground truth
@@ -208,15 +208,15 @@
 
         # Import pandora plugins
         pandora.import_plugin()
 
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
-        right, left = pandora.run(pandora_machine, self.right_cones, self.left_cones, 1, 60, user_cfg["pipeline"])
+        right, left = pandora.run(pandora_machine, self.right_cones, self.left_cones, 1, 60, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the percentage of pixel errors is > 0.20, raise an error
         if common.error(left["disparity_map"].data, self.disp_left, 1, flag_inverse_value=False) > 0.20:
             raise AssertionError
 
         # Compares the calculated left disparity map with the ground truth
@@ -245,15 +245,15 @@
         # Import pandora plugins
         pandora.import_plugin()
 
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
         # Run the pandora pipeline
-        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, 0, user_cfg["pipeline"])
+        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, 0, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the disparity maps are not equal, raise an error
 
         if common.strict_error(left["disparity_map"].data[61:-61, 61:-61], self.disp_left_zncc[61:-61, 61:-61]) > 0:
             raise AssertionError
 
@@ -570,15 +570,15 @@
         pandora.import_plugin()
 
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
         # Pandora pipeline should fail
         with pytest.raises(SystemExit):
-            _, _ = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, -1, user_cfg["pipeline"])
+            _, _ = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, -1, user_cfg)
 
     def test_optimization_layer_with_multiband(self):
         """
         Test the optimization layer function with multiband input images
         """
         # Read input rgb images
         left_rgb = pandora.read_img("tests/inputs/left_rgb.tif", no_data=np.nan, mask=None)
```

### Comparing `pandora_plugin_libsgm-1.3.0/tests/test_penality_sgm.py` & `pandora_plugin_libsgm-1.4.0/tests/test_penality_sgm.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/test_penalty_mc_cnn.py` & `pandora_plugin_libsgm-1.4.0/tests/test_penalty_mc_cnn.py`

 * *Files identical despite different names*

### Comparing `pandora_plugin_libsgm-1.3.0/tests/test_plugin_python.py` & `pandora_plugin_libsgm-1.4.0/tests/test_plugin_python.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
         # Import pandora plugins
         pandora.import_plugin()
 
         # Run the pandora pipeline
-        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, 0, user_cfg["pipeline"])
+        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, 0, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the percentage of pixel errors is > 0.20, raise an error
         if common.error(left["disparity_map"].data, self.disp_left, 1, flag_inverse_value=False) > 0.20:
             raise AssertionError
 
         # Compares the calculated left disparity map with the ground truth
@@ -109,15 +109,15 @@
         # Import pandora plugins
         pandora.import_plugin()
 
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
         # Run the pandora pipeline
-        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, -1, user_cfg["pipeline"])
+        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, -1, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the percentage of pixel errors is > 0.20, raise an error
         if common.error(left["disparity_map"].data, self.disp_left, 1, flag_inverse_value=False) > 0.20:
             raise AssertionError
 
         # Compares the calculated left disparity map with the ground truth
@@ -153,15 +153,15 @@
 
         # Import pandora plugins
         pandora.import_plugin()
 
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
-        right, left = pandora.run(pandora_machine, self.right_cones, self.left_cones, 1, 60, user_cfg["pipeline"])
+        right, left = pandora.run(pandora_machine, self.right_cones, self.left_cones, 1, 60, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the percentage of pixel errors is > 0.20, raise an error
         if common.error(left["disparity_map"].data, self.disp_left, 1, flag_inverse_value=False) > 0.20:
             raise AssertionError
 
         # Compares the calculated left disparity map with the ground truth
@@ -190,15 +190,15 @@
         # Import pandora plugins
         pandora.import_plugin()
 
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
         # Run the pandora pipeline
-        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, 0, user_cfg["pipeline"])
+        left, right = pandora.run(pandora_machine, self.left_cones, self.right_cones, -60, 0, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the disparity maps are not equal, raise an error
         np.testing.assert_allclose(left["disparity_map"].data, self.disp_left_zncc, rtol=1e-04)
 
         # Compares the calculated right disparity map with the ground truth
         # If the disparity maps are not equal, raise an error
@@ -222,15 +222,15 @@
         # Instantiate machine
         pandora_machine = PandoraMachine()
 
         # Import pandora plugins
         pandora.import_plugin()
 
         # Run the pandora pipeline
-        left, right = pandora.run(pandora_machine, left_rgb, right_rgb, -60, 0, user_cfg["pipeline"])
+        left, right = pandora.run(pandora_machine, left_rgb, right_rgb, -60, 0, user_cfg)
 
         # Compares the calculated left disparity map with the ground truth
         # If the percentage of pixel errors is > 0.20, raise an error
         if common.error(left["disparity_map"].data, self.disp_left, 1, flag_inverse_value=False) > 0.20:
             raise AssertionError
 
         # Compares the calculated left disparity map with the ground truth
```

