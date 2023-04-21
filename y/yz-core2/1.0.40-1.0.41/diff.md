# Comparing `tmp/yz-core2-1.0.40.tar.gz` & `tmp/yz-core2-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yz-core2-1.0.40.tar", last modified: Thu Apr  6 03:52:27 2023, max compression
+gzip compressed data, was "yz-core2-1.0.41.tar", last modified: Thu Apr 20 09:41:40 2023, max compression
```

## Comparing `yz-core2-1.0.40.tar` & `yz-core2-1.0.41.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.340987 yz-core2-1.0.40/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2022-08-11 09:11:57.000000 yz-core2-1.0.40/LICENSE
--rw-r--r--   0 zhouwei    (501) staff       (20)     3072 2023-04-06 03:52:27.340860 yz-core2-1.0.40/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-04 03:40:14.000000 yz-core2-1.0.40/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-04-06 03:52:27.341026 yz-core2-1.0.40/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)     1714 2023-04-06 03:38:32.000000 yz-core2-1.0.40/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.327628 yz-core2-1.0.40/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       94 2022-08-11 09:11:57.000000 yz-core2-1.0.40/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      965 2022-08-11 09:11:57.000000 yz-core2-1.0.40/tests/test_setting_reload.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2022-08-11 09:11:57.000000 yz-core2-1.0.40/tests/test_uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.328486 yz-core2-1.0.40/yz_core2.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)     3072 2023-04-06 03:52:27.000000 yz-core2-1.0.40/yz_core2.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     3279 2023-04-06 03:52:27.000000 yz-core2-1.0.40/yz_core2.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-04-06 03:52:27.000000 yz-core2-1.0.40/yz_core2.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-04-06 03:52:27.000000 yz-core2-1.0.40/yz_core2.egg-info/entry_points.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)      184 2023-04-06 03:52:27.000000 yz-core2-1.0.40/yz_core2.egg-info/requires.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-04-06 03:52:27.000000 yz-core2-1.0.40/yz_core2.egg-info/top_level.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.329334 yz-core2-1.0.40/yzcore/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      440 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/__main__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.330393 yz-core2-1.0.40/yzcore/core/
--rw-r--r--   0 zhouwei    (501) staff       (20)       95 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      301 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      466 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/data_hash.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/datastructures.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/encoders.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.330839 yz-core2-1.0.40/yzcore/core/management/
--rw-r--r--   0 zhouwei    (501) staff       (20)      614 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/management/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      122 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/management/base.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.331238 yz-core2-1.0.40/yzcore/core/management/commands/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/management/commands/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      594 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/management/commands/startapp.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      783 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/management/commands/startproject.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/core/management/templates.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     6841 2023-04-06 03:36:37.000000 yz-core2-1.0.40/yzcore/core/storage.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.331746 yz-core2-1.0.40/yzcore/db/
--rw-r--r--   0 zhouwei    (501) staff       (20)       92 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/db/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/db/db_session.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/db/pymongo_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/db/sqlalchemy_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/decorators.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-04-04 08:45:55.000000 yz-core2-1.0.40/yzcore/default_settings.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2248 2022-09-21 06:34:23.000000 yz-core2-1.0.40/yzcore/exceptions.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.332116 yz-core2-1.0.40/yzcore/extensions/
--rw-r--r--   0 zhouwei    (501) staff       (20)       93 2022-08-17 11:17:37.000000 yz-core2-1.0.40/yzcore/extensions/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.332812 yz-core2-1.0.40/yzcore/extensions/storage/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1121 2023-04-06 03:20:10.000000 yz-core2-1.0.40/yzcore/extensions/storage/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10986 2023-04-06 03:19:34.000000 yz-core2-1.0.40/yzcore/extensions/storage/base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      452 2022-11-22 10:08:14.000000 yz-core2-1.0.40/yzcore/extensions/storage/const.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.332989 yz-core2-1.0.40/yzcore/extensions/storage/minio/
--rw-r--r--   0 zhouwei    (501) staff       (20)     7559 2023-03-10 03:21:32.000000 yz-core2-1.0.40/yzcore/extensions/storage/minio/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.333860 yz-core2-1.0.40/yzcore/extensions/storage/obs/
--rw-r--r--   0 zhouwei    (501) staff       (20)     7845 2023-04-06 03:40:37.000000 yz-core2-1.0.40/yzcore/extensions/storage/obs/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2022-11-25 06:30:07.000000 yz-core2-1.0.40/yzcore/extensions/storage/obs/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2948 2022-11-15 03:37:12.000000 yz-core2-1.0.40/yzcore/extensions/storage/obs/obs_inherit.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      402 2022-11-21 09:30:20.000000 yz-core2-1.0.40/yzcore/extensions/storage/obs/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.334401 yz-core2-1.0.40/yzcore/extensions/storage/oss/
--rw-r--r--   0 zhouwei    (501) staff       (20)    13169 2023-04-06 03:13:38.000000 yz-core2-1.0.40/yzcore/extensions/storage/oss/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      762 2022-11-25 06:19:55.000000 yz-core2-1.0.40/yzcore/extensions/storage/oss/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-06 03:27:35.000000 yz-core2-1.0.40/yzcore/extensions/storage/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/extensions/uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.335017 yz-core2-1.0.40/yzcore/logger/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/logger/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/logger/config.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/logger/filters.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/logger/handlers.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.335272 yz-core2-1.0.40/yzcore/request/
--rw-r--r--   0 zhouwei    (501) staff       (20)      133 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/request/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/request/aio_http.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.335651 yz-core2-1.0.40/yzcore/response/
--rw-r--r--   0 zhouwei    (501) staff       (20)      188 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/response/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/response/response.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/response/response_code.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.335858 yz-core2-1.0.40/yzcore/templates/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.336587 yz-core2-1.0.40/yzcore/templates/app_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/app_template/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      945 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/app_template/controllers.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      421 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/app_template/models.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      907 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/app_template/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/app_template/tests.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/app_template/views.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.337015 yz-core2-1.0.40/yzcore/templates/project_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/.gitignore
--rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/README.md
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.337317 yz-core2-1.0.40/yzcore/templates/project_template/docs/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/docs/install_explain.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      922 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/docs/supervisor.ini
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.337483 yz-core2-1.0.40/yzcore/templates/project_template/migrations/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/migrations/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      453 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/requirements.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.338055 yz-core2-1.0.40/yzcore/templates/project_template/src/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.338188 yz-core2-1.0.40/yzcore/templates/project_template/src/apps/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/apps/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.338874 yz-core2-1.0.40/yzcore/templates/project_template/src/conf/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/conf/config_dev.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/conf/config_dev.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/conf/config_production.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/conf/config_production.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/conf/config_testing.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/conf/config_testing.yaml
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.339243 yz-core2-1.0.40/yzcore/templates/project_template/src/const/
--rw-r--r--   0 zhouwei    (501) staff       (20)      157 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/const/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      409 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/const/_job.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      418 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/const/_task.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      843 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/main.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      807 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/settings.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.339539 yz-core2-1.0.40/yzcore/templates/project_template/src/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      840 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/tests/test_xxx.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.339676 yz-core2-1.0.40/yzcore/templates/project_template/src/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/templates/project_template/src/utils/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-06 03:52:27.340646 yz-core2-1.0.40/yzcore/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)      386 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      231 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/utils/check_path.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/utils/check_sys.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/utils/crypto.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/utils/encoding.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/utils/nacos.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1473 2022-08-11 09:11:57.000000 yz-core2-1.0.40/yzcore/utils/time_utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.772494 yz-core2-1.0.41/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2022-08-11 09:11:57.000000 yz-core2-1.0.41/LICENSE
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3095 2023-04-20 09:41:40.772298 yz-core2-1.0.41/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-04 03:40:14.000000 yz-core2-1.0.41/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-04-20 09:41:40.772534 yz-core2-1.0.41/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1765 2023-04-20 09:38:13.000000 yz-core2-1.0.41/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.757064 yz-core2-1.0.41/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       94 2022-08-11 09:11:57.000000 yz-core2-1.0.41/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      965 2022-08-11 09:11:57.000000 yz-core2-1.0.41/tests/test_setting_reload.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2022-08-11 09:11:57.000000 yz-core2-1.0.41/tests/test_uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.757836 yz-core2-1.0.41/yz_core2.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3095 2023-04-20 09:41:40.000000 yz-core2-1.0.41/yz_core2.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3279 2023-04-20 09:41:40.000000 yz-core2-1.0.41/yz_core2.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-04-20 09:41:40.000000 yz-core2-1.0.41/yz_core2.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-04-20 09:41:40.000000 yz-core2-1.0.41/yz_core2.egg-info/entry_points.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)      222 2023-04-20 09:41:40.000000 yz-core2-1.0.41/yz_core2.egg-info/requires.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-04-20 09:41:40.000000 yz-core2-1.0.41/yz_core2.egg-info/top_level.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.758794 yz-core2-1.0.41/yzcore/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      440 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/__main__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.759798 yz-core2-1.0.41/yzcore/core/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       95 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      301 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      466 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/data_hash.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/datastructures.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/encoders.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.760584 yz-core2-1.0.41/yzcore/core/management/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      614 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/management/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      122 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/management/base.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.761050 yz-core2-1.0.41/yzcore/core/management/commands/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/management/commands/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      594 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/management/commands/startapp.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      783 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/management/commands/startproject.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/core/management/templates.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6825 2023-04-20 09:32:33.000000 yz-core2-1.0.41/yzcore/core/storage.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.761641 yz-core2-1.0.41/yzcore/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       92 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/db/db_session.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/db/pymongo_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/db/sqlalchemy_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/decorators.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-04-04 08:45:55.000000 yz-core2-1.0.41/yzcore/default_settings.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2248 2022-09-21 06:34:23.000000 yz-core2-1.0.41/yzcore/exceptions.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.762016 yz-core2-1.0.41/yzcore/extensions/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       93 2022-08-17 11:17:37.000000 yz-core2-1.0.41/yzcore/extensions/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.762912 yz-core2-1.0.41/yzcore/extensions/storage/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1121 2023-04-20 09:34:50.000000 yz-core2-1.0.41/yzcore/extensions/storage/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10986 2023-04-20 09:35:03.000000 yz-core2-1.0.41/yzcore/extensions/storage/base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      452 2023-04-20 09:35:12.000000 yz-core2-1.0.41/yzcore/extensions/storage/const.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.763121 yz-core2-1.0.41/yzcore/extensions/storage/minio/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7559 2023-04-20 09:35:25.000000 yz-core2-1.0.41/yzcore/extensions/storage/minio/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.764124 yz-core2-1.0.41/yzcore/extensions/storage/obs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7845 2023-04-20 09:35:28.000000 yz-core2-1.0.41/yzcore/extensions/storage/obs/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2022-11-25 06:30:07.000000 yz-core2-1.0.41/yzcore/extensions/storage/obs/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2948 2022-11-15 03:37:12.000000 yz-core2-1.0.41/yzcore/extensions/storage/obs/obs_inherit.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      402 2022-11-21 09:30:20.000000 yz-core2-1.0.41/yzcore/extensions/storage/obs/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.764773 yz-core2-1.0.41/yzcore/extensions/storage/oss/
+-rw-r--r--   0 zhouwei    (501) staff       (20)    13169 2023-04-20 09:35:34.000000 yz-core2-1.0.41/yzcore/extensions/storage/oss/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      762 2022-11-25 06:19:55.000000 yz-core2-1.0.41/yzcore/extensions/storage/oss/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-06 03:27:35.000000 yz-core2-1.0.41/yzcore/extensions/storage/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/extensions/uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.765694 yz-core2-1.0.41/yzcore/logger/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/logger/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/logger/config.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/logger/filters.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/logger/handlers.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.766092 yz-core2-1.0.41/yzcore/request/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      133 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/request/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/request/aio_http.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.766593 yz-core2-1.0.41/yzcore/response/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      188 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/response/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/response/response.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/response/response_code.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.766867 yz-core2-1.0.41/yzcore/templates/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.767899 yz-core2-1.0.41/yzcore/templates/app_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/app_template/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      945 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/app_template/controllers.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      421 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/app_template/models.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      907 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/app_template/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/app_template/tests.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/app_template/views.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.768576 yz-core2-1.0.41/yzcore/templates/project_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/.gitignore
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/README.md
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.768803 yz-core2-1.0.41/yzcore/templates/project_template/docs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/docs/install_explain.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      922 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/docs/supervisor.ini
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.768933 yz-core2-1.0.41/yzcore/templates/project_template/migrations/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/migrations/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      453 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/requirements.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.769299 yz-core2-1.0.41/yzcore/templates/project_template/src/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.769428 yz-core2-1.0.41/yzcore/templates/project_template/src/apps/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/apps/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.770014 yz-core2-1.0.41/yzcore/templates/project_template/src/conf/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/conf/config_dev.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/conf/config_dev.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/conf/config_production.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/conf/config_production.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/conf/config_testing.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/conf/config_testing.yaml
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.770388 yz-core2-1.0.41/yzcore/templates/project_template/src/const/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      157 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/const/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      409 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/const/_job.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      418 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/const/_task.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      843 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/main.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      807 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/settings.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.770703 yz-core2-1.0.41/yzcore/templates/project_template/src/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      840 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/tests/test_xxx.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.770853 yz-core2-1.0.41/yzcore/templates/project_template/src/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/templates/project_template/src/utils/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-04-20 09:41:40.771864 yz-core2-1.0.41/yzcore/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      386 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      231 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/utils/check_path.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/utils/check_sys.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/utils/crypto.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/utils/encoding.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2022-08-11 09:11:57.000000 yz-core2-1.0.41/yzcore/utils/nacos.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1473 2023-04-20 09:36:02.000000 yz-core2-1.0.41/yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.40/LICENSE` & `yz-core2-1.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/PKG-INFO` & `yz-core2-1.0.41/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.40
+Version: 1.0.41
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
 Provides-Extra: rpc
 Provides-Extra: oss-aliyun
-Provides-Extra: oss-huawei
+Provides-Extra: obs-huawei
 Provides-Extra: oss-aws
-Provides-Extra: oss-minio
+Provides-Extra: minio
+Provides-Extra: azure-blob
 License-File: LICENSE
 
 # readme-template
 
 --------------
 
 ## Introduction
```

### Comparing `yz-core2-1.0.40/README.md` & `yz-core2-1.0.41/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/setup.py` & `yz-core2-1.0.41/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yz-core2",  # Replace with your own username
-    version="1.0.40",
+    version="1.0.41",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     description="An ID generator for distributed microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhouwe1/yz-core.git",
     packages=setuptools.find_packages(),
@@ -42,12 +42,13 @@
         'console_scripts': [
             'yzcore=yzcore.__main__:main'
         ],
     },
     extras_require={
         'rpc': ['yzrpc>=0.1'],
         'oss-aliyun': ['oss2>=2.13.1, !=3.0.0'],
-        'oss-huawei': ['esdk-obs-python>=3.22.2'],
+        'obs-huawei': ['esdk-obs-python==3.22.2'],
         'oss-aws': ['boto3==1.17.27'],
-        'oss-minio': ['minio==7.1.12'],
+        'minio': ['minio==7.1.12'],
+        'azure-blob': ['azure-storage-blob==12.16.0'],
     }
 )
```

### Comparing `yz-core2-1.0.40/tests/test_setting_reload.py` & `yz-core2-1.0.41/tests/test_setting_reload.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/tests/test_uid.py` & `yz-core2-1.0.41/tests/test_uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yz_core2.egg-info/PKG-INFO` & `yz-core2-1.0.41/yz_core2.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.40
+Version: 1.0.41
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
 Provides-Extra: rpc
 Provides-Extra: oss-aliyun
-Provides-Extra: oss-huawei
+Provides-Extra: obs-huawei
 Provides-Extra: oss-aws
-Provides-Extra: oss-minio
+Provides-Extra: minio
+Provides-Extra: azure-blob
 License-File: LICENSE
 
 # readme-template
 
 --------------
 
 ## Introduction
```

### Comparing `yz-core2-1.0.40/yz_core2.egg-info/SOURCES.txt` & `yz-core2-1.0.41/yz_core2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/core/datastructures.py` & `yz-core2-1.0.41/yzcore/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/core/encoders.py` & `yz-core2-1.0.41/yzcore/core/encoders.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/core/management/__init__.py` & `yz-core2-1.0.41/yzcore/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/core/management/commands/startapp.py` & `yz-core2-1.0.41/yzcore/core/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/core/management/commands/startproject.py` & `yz-core2-1.0.41/yzcore/core/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/core/management/templates.py` & `yz-core2-1.0.41/yzcore/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/core/storage.py` & `yz-core2-1.0.41/yzcore/core/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     组织自定义对象存储
     >>> storage_ctrl = await StorageController.init(organiz_id='organiz_id')
     >>> storage_ctrl.organiz_storage_conf  # 组织自定义对象存储配置，未配置则为空字典
     >>> storage_ctrl.storage_conf  # 组织自定义对象存储配置或全局配置
     >>> storage_ctrl.public_storage_manage  # 非加密存储控制器
     >>> storage_ctrl.private_storage_manage  # 加密存储控制器
     全局对象存储
-    >>> global_storage_manage = StorageController.sync_init()
-    >>> global_storage_manage.public_storage_manage  # 全局非加密存储控制器
-    >>> global_storage_manage.private_storage_manage  # 全局加密存储控制器
+    >>> global_storage_ctrl = StorageController.sync_init()
+    >>> global_storage_ctrl.public_storage_manage  # 全局非加密存储控制器
+    >>> global_storage_ctrl.private_storage_manage  # 全局加密存储控制器
     """
 
     global_storage_conf = settings.STORAGE_CONF  # 全局对象存储配置
 
-    def __init__(self, organiz_id):
+    def __init__(self, organiz_id: str = ''):
         """
-        不可直接使用，请在 StorageManage.init 初始化
+        不可直接使用，请使用 StorageController.init() / StorageController.sync_init() 初始化
         """
         self.organiz_id = organiz_id
         self.organiz_storage_conf = dict()  # 组织自定义对象存储
         self.storage_conf = dict()  # 对象存储实际使用的配置
         self.storage_mode = ''
 
     @classmethod
@@ -98,23 +98,23 @@
             access_key_secret: str
             endpoint: str
             public_bucket_name: str             # 非加密桶使用
             private_bucket_name: Optional[str]  # 加密桶使用
             image_domain: Optional[str]         # 非加密桶使用，可选
             asset_domain: Optional[str]         # 非加密桶使用，可选
             private_domain: Optional[str]       # 加密桶使用，可选
-            private_cname: Optional[str]        # 加密桶使用，可选
 
         :return: _StorageManage实例，即 ObsManager 或 OssManager
         """
         return StorageManage(
             mode=storage_conf['mode'],
             access_key_id=storage_conf['access_key_id'],
             access_key_secret=storage_conf['access_key_secret'],
             endpoint=storage_conf['endpoint'],
+            internal_endpoint=storage_conf.get('internal_endpoint'),
             bucket_name=storage_conf['public_bucket_name'],  # 注意区分加密/非加密存储桶
             image_domain=storage_conf['image_domain'],
             asset_domain=storage_conf['asset_domain'],
             scheme=storage_conf.get('scheme', 'https'),
             cache_path=cls.global_storage_conf['cache_path'],  # 来自全局配置
             policy_expire_time=cls.global_storage_conf['policy_expire_time'],  # 来自全局配置
             private_expire_time=cls.global_storage_conf['private_expire_time'],  # 来自全局配置
@@ -131,25 +131,24 @@
             access_key_secret: str
             endpoint: str
             public_bucket_name: Optional[str]   # 非加密桶使用
             private_bucket_name: str            # 加密桶使用
             image_domain: Optional[str]         # 非加密桶使用，可选
             asset_domain: Optional[str]         # 非加密桶使用，可选
             private_domain: Optional[str]       # 加密桶使用，可选
-            private_cname: Optional[str]        # 加密桶使用，可选
 
         :return: _StorageManage实例，即 ObsManager 或 OssManager
         """
         return StorageManage(
             mode=storage_conf['mode'],
             access_key_id=storage_conf['access_key_id'],
             access_key_secret=storage_conf['access_key_secret'],
             endpoint=storage_conf['endpoint'],
+            internal_endpoint=storage_conf.get('internal_endpoint'),
             bucket_name=storage_conf['private_bucket_name'],  # 注意区分加密/非加密存储桶
             image_domain=storage_conf['private_domain'],
             asset_domain=storage_conf['private_domain'],
-            cname=storage_conf['private_cname'],
             scheme=storage_conf.get('scheme', 'https'),
             cache_path=cls.global_storage_conf['cache_path'],  # 来自全局配置
             policy_expire_time=cls.global_storage_conf['policy_expire_time'],  # 来自全局配置
             private_expire_time=cls.global_storage_conf['private_expire_time'],  # 来自全局配置
         )
```

### Comparing `yz-core2-1.0.40/yzcore/db/db_session.py` & `yz-core2-1.0.41/yzcore/db/db_session.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/db/pymongo_crud_base.py` & `yz-core2-1.0.41/yzcore/db/pymongo_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/db/sqlalchemy_crud_base.py` & `yz-core2-1.0.41/yzcore/db/sqlalchemy_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/decorators.py` & `yz-core2-1.0.41/yzcore/decorators.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/default_settings.py` & `yz-core2-1.0.41/yzcore/default_settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/exceptions.py` & `yz-core2-1.0.41/yzcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/storage/__init__.py` & `yz-core2-1.0.41/yzcore/extensions/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/storage/base.py` & `yz-core2-1.0.41/yzcore/extensions/storage/base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/storage/minio/__init__.py` & `yz-core2-1.0.41/yzcore/extensions/storage/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/storage/obs/__init__.py` & `yz-core2-1.0.41/yzcore/extensions/storage/obs/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/storage/obs/const.py` & `yz-core2-1.0.41/yzcore/extensions/storage/obs/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/storage/obs/obs_inherit.py` & `yz-core2-1.0.41/yzcore/extensions/storage/obs/obs_inherit.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/storage/oss/__init__.py` & `yz-core2-1.0.41/yzcore/extensions/storage/oss/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/storage/oss/const.py` & `yz-core2-1.0.41/yzcore/extensions/storage/oss/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/extensions/uid.py` & `yz-core2-1.0.41/yzcore/extensions/uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/logger/__init__.py` & `yz-core2-1.0.41/yzcore/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/logger/config.py` & `yz-core2-1.0.41/yzcore/logger/config.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/logger/filters.py` & `yz-core2-1.0.41/yzcore/logger/filters.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/logger/handlers.py` & `yz-core2-1.0.41/yzcore/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/request/aio_http.py` & `yz-core2-1.0.41/yzcore/request/aio_http.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/response/response.py` & `yz-core2-1.0.41/yzcore/response/response.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/response/response_code.py` & `yz-core2-1.0.41/yzcore/response/response_code.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/app_template/controllers.py` & `yz-core2-1.0.41/yzcore/templates/app_template/controllers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/app_template/schemas.py` & `yz-core2-1.0.41/yzcore/templates/app_template/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/app_template/views.py` & `yz-core2-1.0.41/yzcore/templates/app_template/views.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/project_template/.gitignore` & `yz-core2-1.0.41/yzcore/templates/project_template/.gitignore`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/project_template/README.md` & `yz-core2-1.0.41/yzcore/templates/project_template/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/project_template/docs/supervisor.ini` & `yz-core2-1.0.41/yzcore/templates/project_template/docs/supervisor.ini`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/project_template/src/main.py` & `yz-core2-1.0.41/yzcore/templates/project_template/src/main.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/project_template/src/settings.py` & `yz-core2-1.0.41/yzcore/templates/project_template/src/settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/templates/project_template/src/tests/test_xxx.py` & `yz-core2-1.0.41/yzcore/templates/project_template/src/tests/test_xxx.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/utils/check_sys.py` & `yz-core2-1.0.41/yzcore/utils/check_sys.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/utils/crypto.py` & `yz-core2-1.0.41/yzcore/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/utils/encoding.py` & `yz-core2-1.0.41/yzcore/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/utils/nacos.py` & `yz-core2-1.0.41/yzcore/utils/nacos.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.40/yzcore/utils/time_utils.py` & `yz-core2-1.0.41/yzcore/utils/time_utils.py`

 * *Files identical despite different names*

