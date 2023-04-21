# Comparing `tmp/aiokatcp-1.6.2.tar.gz` & `tmp/aiokatcp-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bmerry/work/sdp/git/aiokatcp/dist/.tmp-erg890qe/aiokatcp-1.6.2.tar", last modified: Wed Mar 15 09:30:49 2023, max compression
+gzip compressed data, was "/home/bmerry/work/sdp/git/aiokatcp/dist/.tmp-u_iimfkm/aiokatcp-1.7.0.tar", last modified: Fri Apr 21 09:47:11 2023, max compression
```

## Comparing `aiokatcp-1.6.2.tar` & `aiokatcp-1.7.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       53 2022-04-14 06:11:41.000000 aiokatcp-1.6.2/.flake8
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/.github/
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/.github/workflows/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1343 2022-11-14 14:15:32.000000 aiokatcp-1.6.2/.github/workflows/test.yml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       91 2021-07-26 11:03:08.000000 aiokatcp-1.6.2/.gitignore
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1285 2023-03-15 08:34:40.000000 aiokatcp-1.6.2/.pre-commit-config.yaml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      118 2022-04-14 06:11:41.000000 aiokatcp-1.6.2/.readthedocs.yml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1486 2022-04-14 06:11:41.000000 aiokatcp-1.6.2/LICENSE.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1932 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/PKG-INFO
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1144 2022-04-14 06:11:41.000000 aiokatcp-1.6.2/README.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      480 2022-04-19 12:05:31.000000 aiokatcp-1.6.2/TODO
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/doc/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        7 2017-09-27 07:56:58.000000 aiokatcp-1.6.2/doc/.gitignore
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      670 2018-01-11 09:16:27.000000 aiokatcp-1.6.2/doc/Makefile
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/doc/_static/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2018-01-11 09:16:27.000000 aiokatcp-1.6.2/doc/_static/.keep
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1205 2022-12-08 13:25:04.000000 aiokatcp-1.6.2/doc/aiokatcp.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      346 2022-12-08 13:25:04.000000 aiokatcp-1.6.2/doc/aiokatcp.tools.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5272 2023-03-15 09:30:00.000000 aiokatcp-1.6.2/doc/changelog.rst
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/doc/client/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2371 2018-01-11 09:16:27.000000 aiokatcp-1.6.2/doc/client/reconnect.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1658 2019-06-03 08:19:32.000000 aiokatcp-1.6.2/doc/client/sensor_watcher.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4288 2019-06-03 08:19:32.000000 aiokatcp-1.6.2/doc/client/tutorial.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      152 2019-06-03 08:19:32.000000 aiokatcp-1.6.2/doc/client.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5979 2022-12-08 13:42:27.000000 aiokatcp-1.6.2/doc/conf.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      499 2018-01-11 09:16:27.000000 aiokatcp-1.6.2/doc/index.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      741 2019-11-11 08:33:27.000000 aiokatcp-1.6.2/doc/intro.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3196 2019-06-03 08:19:32.000000 aiokatcp-1.6.2/doc/migration.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       61 2022-12-06 15:10:53.000000 aiokatcp-1.6.2/doc/modules.rst
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/doc/server/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1892 2022-07-18 10:37:55.000000 aiokatcp-1.6.2/doc/server/logging.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1647 2022-04-19 12:04:15.000000 aiokatcp-1.6.2/doc/server/service_tasks.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14674 2022-11-15 06:01:07.000000 aiokatcp-1.6.2/doc/server/tutorial.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      149 2022-04-19 12:04:15.000000 aiokatcp-1.6.2/doc/server.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1654 2017-11-06 19:05:40.000000 aiokatcp-1.6.2/doc/unicode.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      122 2018-01-11 09:16:27.000000 aiokatcp-1.6.2/doc/user.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       34 2022-04-14 06:11:41.000000 aiokatcp-1.6.2/doc-requirements.txt
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/examples/
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     2161 2022-11-15 08:24:36.000000 aiokatcp-1.6.2/examples/example_client.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     5130 2022-11-15 08:24:36.000000 aiokatcp-1.6.2/examples/example_server.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     3551 2022-10-24 06:29:45.000000 aiokatcp-1.6.2/examples/mirror_sensors.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      173 2022-04-13 12:58:23.000000 aiokatcp-1.6.2/mypy.ini
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      164 2022-10-24 06:29:45.000000 aiokatcp-1.6.2/pyproject.toml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      129 2022-04-19 07:10:17.000000 aiokatcp-1.6.2/pytest.ini
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      124 2022-11-13 09:09:04.000000 aiokatcp-1.6.2/requirements.in
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1806 2023-03-15 08:34:40.000000 aiokatcp-1.6.2/requirements.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1143 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/setup.cfg
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1592 2022-04-14 06:11:41.000000 aiokatcp-1.6.2/setup.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2405 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4143 2022-12-08 13:25:04.000000 aiokatcp-1.6.2/src/aiokatcp/adjtimex.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    39419 2022-11-15 08:24:36.000000 aiokatcp-1.6.2/src/aiokatcp/client.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    12958 2022-11-16 09:51:48.000000 aiokatcp-1.6.2/src/aiokatcp/connection.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    20966 2022-12-08 13:25:04.000000 aiokatcp-1.6.2/src/aiokatcp/core.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2021-07-26 11:03:08.000000 aiokatcp-1.6.2/src/aiokatcp/py.typed
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    35508 2022-11-15 08:24:36.000000 aiokatcp-1.6.2/src/aiokatcp/sensor.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    41616 2022-11-15 08:24:36.000000 aiokatcp-1.6.2/src/aiokatcp/server.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3564 2022-12-10 12:01:04.000000 aiokatcp-1.6.2/src/aiokatcp/time_sync.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp/tools/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       59 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp/tools/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4105 2022-11-15 08:24:36.000000 aiokatcp-1.6.2/src/aiokatcp/tools/katcpcmd.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp.egg-info/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1932 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp.egg-info/PKG-INFO
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1356 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp.egg-info/SOURCES.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp.egg-info/dependency_links.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       58 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp.egg-info/entry_points.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2022-04-13 14:35:48.000000 aiokatcp-1.6.2/src/aiokatcp.egg-info/not-zip-safe
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      136 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp.egg-info/requires.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        9 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/src/aiokatcp.egg-info/top_level.txt
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-03-15 09:30:49.000000 aiokatcp-1.6.2/tests/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    33887 2022-10-24 06:29:45.000000 aiokatcp-1.6.2/tests/test_client.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     8972 2022-10-24 06:29:45.000000 aiokatcp-1.6.2/tests/test_connection.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14597 2022-11-16 09:51:48.000000 aiokatcp-1.6.2/tests/test_core.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    18939 2022-11-15 08:24:36.000000 aiokatcp-1.6.2/tests/test_sensor.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    39408 2022-10-24 06:29:45.000000 aiokatcp-1.6.2/tests/test_server.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3834 2022-12-08 13:25:04.000000 aiokatcp-1.6.2/tests/test_time_sync.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       53 2022-04-14 06:11:41.000000 aiokatcp-1.7.0/.flake8
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/.github/
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/.github/workflows/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1343 2022-11-14 14:15:32.000000 aiokatcp-1.7.0/.github/workflows/test.yml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       91 2021-07-26 11:03:08.000000 aiokatcp-1.7.0/.gitignore
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1285 2023-03-15 08:34:40.000000 aiokatcp-1.7.0/.pre-commit-config.yaml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      118 2022-04-14 06:11:41.000000 aiokatcp-1.7.0/.readthedocs.yml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1486 2022-04-14 06:11:41.000000 aiokatcp-1.7.0/LICENSE.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1932 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/PKG-INFO
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1144 2022-04-14 06:11:41.000000 aiokatcp-1.7.0/README.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      480 2022-04-19 12:05:31.000000 aiokatcp-1.7.0/TODO
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/doc/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        7 2017-09-27 07:56:58.000000 aiokatcp-1.7.0/doc/.gitignore
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      670 2018-01-11 09:16:27.000000 aiokatcp-1.7.0/doc/Makefile
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/doc/_static/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2018-01-11 09:16:27.000000 aiokatcp-1.7.0/doc/_static/.keep
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1205 2022-12-08 13:25:04.000000 aiokatcp-1.7.0/doc/aiokatcp.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      346 2022-12-08 13:25:04.000000 aiokatcp-1.7.0/doc/aiokatcp.tools.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5455 2023-04-21 09:46:13.000000 aiokatcp-1.7.0/doc/changelog.rst
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/doc/client/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2371 2018-01-11 09:16:27.000000 aiokatcp-1.7.0/doc/client/reconnect.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1658 2019-06-03 08:19:32.000000 aiokatcp-1.7.0/doc/client/sensor_watcher.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4288 2019-06-03 08:19:32.000000 aiokatcp-1.7.0/doc/client/tutorial.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      152 2019-06-03 08:19:32.000000 aiokatcp-1.7.0/doc/client.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5979 2022-12-08 13:42:27.000000 aiokatcp-1.7.0/doc/conf.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      499 2018-01-11 09:16:27.000000 aiokatcp-1.7.0/doc/index.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      741 2019-11-11 08:33:27.000000 aiokatcp-1.7.0/doc/intro.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3196 2019-06-03 08:19:32.000000 aiokatcp-1.7.0/doc/migration.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       61 2022-12-06 15:10:53.000000 aiokatcp-1.7.0/doc/modules.rst
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/doc/server/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1892 2022-07-18 10:37:55.000000 aiokatcp-1.7.0/doc/server/logging.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1647 2022-04-19 12:04:15.000000 aiokatcp-1.7.0/doc/server/service_tasks.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14674 2022-11-15 06:01:07.000000 aiokatcp-1.7.0/doc/server/tutorial.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      149 2022-04-19 12:04:15.000000 aiokatcp-1.7.0/doc/server.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1654 2017-11-06 19:05:40.000000 aiokatcp-1.7.0/doc/unicode.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      122 2018-01-11 09:16:27.000000 aiokatcp-1.7.0/doc/user.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       34 2022-04-14 06:11:41.000000 aiokatcp-1.7.0/doc-requirements.txt
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/examples/
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     2161 2022-11-15 08:24:36.000000 aiokatcp-1.7.0/examples/example_client.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     5130 2022-11-15 08:24:36.000000 aiokatcp-1.7.0/examples/example_server.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     3551 2022-10-24 06:29:45.000000 aiokatcp-1.7.0/examples/mirror_sensors.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      173 2022-04-13 12:58:23.000000 aiokatcp-1.7.0/mypy.ini
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      164 2022-10-24 06:29:45.000000 aiokatcp-1.7.0/pyproject.toml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      129 2022-04-19 07:10:17.000000 aiokatcp-1.7.0/pytest.ini
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      124 2022-11-13 09:09:04.000000 aiokatcp-1.7.0/requirements.in
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1806 2023-03-15 08:34:40.000000 aiokatcp-1.7.0/requirements.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1143 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/setup.cfg
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1592 2022-04-14 06:11:41.000000 aiokatcp-1.7.0/setup.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2405 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4143 2022-12-08 13:25:04.000000 aiokatcp-1.7.0/src/aiokatcp/adjtimex.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    39972 2023-04-21 09:45:43.000000 aiokatcp-1.7.0/src/aiokatcp/client.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    12958 2022-11-16 09:51:48.000000 aiokatcp-1.7.0/src/aiokatcp/connection.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    20966 2022-12-08 13:25:04.000000 aiokatcp-1.7.0/src/aiokatcp/core.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2021-07-26 11:03:08.000000 aiokatcp-1.7.0/src/aiokatcp/py.typed
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    35508 2022-11-15 08:24:36.000000 aiokatcp-1.7.0/src/aiokatcp/sensor.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    41631 2023-04-21 09:45:43.000000 aiokatcp-1.7.0/src/aiokatcp/server.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3564 2022-12-10 12:01:04.000000 aiokatcp-1.7.0/src/aiokatcp/time_sync.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp/tools/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       59 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp/tools/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4105 2022-11-15 08:24:36.000000 aiokatcp-1.7.0/src/aiokatcp/tools/katcpcmd.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp.egg-info/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1932 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp.egg-info/PKG-INFO
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1356 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp.egg-info/SOURCES.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp.egg-info/dependency_links.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       58 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp.egg-info/entry_points.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2022-04-13 14:35:48.000000 aiokatcp-1.7.0/src/aiokatcp.egg-info/not-zip-safe
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      136 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp.egg-info/requires.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        9 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/src/aiokatcp.egg-info/top_level.txt
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-04-21 09:47:11.000000 aiokatcp-1.7.0/tests/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    34810 2023-04-21 09:45:43.000000 aiokatcp-1.7.0/tests/test_client.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     8972 2022-10-24 06:29:45.000000 aiokatcp-1.7.0/tests/test_connection.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14597 2022-11-16 09:51:48.000000 aiokatcp-1.7.0/tests/test_core.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    18939 2022-11-15 08:24:36.000000 aiokatcp-1.7.0/tests/test_sensor.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    39408 2022-10-24 06:29:45.000000 aiokatcp-1.7.0/tests/test_server.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3834 2022-12-08 13:25:04.000000 aiokatcp-1.7.0/tests/test_time_sync.py
```

### Comparing `aiokatcp-1.6.2/.github/workflows/test.yml` & `aiokatcp-1.7.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/.pre-commit-config.yaml` & `aiokatcp-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/LICENSE.txt` & `aiokatcp-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/PKG-INFO` & `aiokatcp-1.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokatcp
-Version: 1.6.2
+Version: 1.7.0
 Summary: Asynchronous I/O implementation of the katcp protocol
 Home-page: https://github.com/ska-sa/aiokatcp
 Author: Bruce Merry
 Author-email: bmerry@sarao.ac.za
 License: BSD
 Keywords: asyncio,katcp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiokatcp-1.6.2/README.rst` & `aiokatcp-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/Makefile` & `aiokatcp-1.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/aiokatcp.rst` & `aiokatcp-1.7.0/doc/aiokatcp.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/changelog.rst` & `aiokatcp-1.7.0/doc/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+.. rubric:: Version 1.7.0
+
+- Extend :class:`.SensorWatcher` to allow incoming sensors to be replicated
+  under multiple names.
+- Log exception traceback when a service task crashes.
+
 .. rubric:: Version 1.6.2
 
 - Make things work on MacOS again.
 - CI: Update certifi to a newer version.
 - Add a type annotation to prevent an internal error in old versions of mypy.
 
 .. rubric:: Version 1.6.1
```

### Comparing `aiokatcp-1.6.2/doc/client/reconnect.rst` & `aiokatcp-1.7.0/doc/client/reconnect.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/client/sensor_watcher.rst` & `aiokatcp-1.7.0/doc/client/sensor_watcher.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/client/tutorial.rst` & `aiokatcp-1.7.0/doc/client/tutorial.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/conf.py` & `aiokatcp-1.7.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/intro.rst` & `aiokatcp-1.7.0/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/migration.rst` & `aiokatcp-1.7.0/doc/migration.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/server/logging.rst` & `aiokatcp-1.7.0/doc/server/logging.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/server/service_tasks.rst` & `aiokatcp-1.7.0/doc/server/service_tasks.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/server/tutorial.rst` & `aiokatcp-1.7.0/doc/server/tutorial.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/doc/unicode.rst` & `aiokatcp-1.7.0/doc/unicode.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/examples/example_client.py` & `aiokatcp-1.7.0/examples/example_client.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/examples/example_server.py` & `aiokatcp-1.7.0/examples/example_server.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/examples/mirror_sensors.py` & `aiokatcp-1.7.0/examples/mirror_sensors.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/requirements.txt` & `aiokatcp-1.7.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/setup.cfg` & `aiokatcp-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/setup.py` & `aiokatcp-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/src/aiokatcp/__init__.py` & `aiokatcp-1.7.0/src/aiokatcp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 # Automatically added by katversion
-__version__ = '1.6.2'
+__version__ = '1.7.0'
 
 import sys
 
 from .client import (  # noqa: F401
     AbstractSensorWatcher,
     Client,
     ProtocolError,
```

### Comparing `aiokatcp-1.6.2/src/aiokatcp/adjtimex.py` & `aiokatcp-1.7.0/src/aiokatcp/adjtimex.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/src/aiokatcp/client.py` & `aiokatcp-1.7.0/src/aiokatcp/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -733,21 +733,30 @@
         self.sensors = sensor.SensorSet()
         # Synthesized enum types for discrete sensors
         self._enum_cache: Dict[Tuple[bytes, ...], Type[enum.Enum]] = {}
         for enum_type in enum_types:
             key = tuple(core.encode(value) for value in enum_type.__members__.values())
             self._enum_cache[key] = enum_type
 
-    def rewrite_name(self, name: str) -> str:
+    def rewrite_name(self, name: str) -> Union[str, Sequence[str]]:
         """Convert name of incoming sensor to name to use in the sensor set.
 
-        This defaults to the identity, but can be overridden to provide name mangling.
+        This defaults to the identity, but can be overridden to provide name
+        mangling. It may also return a sequence of names, in which case the
+        original sensor is replicated under each of those names.
         """
         return name
 
+    def _rewritten_names(self, name: str) -> Sequence[str]:
+        names = self.rewrite_name(name)
+        if isinstance(names, str):
+            return [names]
+        else:
+            return names
+
     def make_type(self, type_name: str, parameters: Sequence[bytes]) -> type:
         """Get the sensor type for a given type name"""
         if type_name == "discrete":
             values = tuple(parameters)
             if values in self._enum_cache:
                 return self._enum_cache[values]
             else:
@@ -765,42 +774,45 @@
     def sensor_added(
         self, name: str, description: str, units: str, type_name: str, *args: bytes
     ) -> None:
         if type_name not in self.SENSOR_TYPES:
             self.logger.warning("Type %s is not recognised, skipping sensor %s", type_name, name)
             return
         stype = self.make_type(type_name, args)
-        s: sensor.Sensor = sensor.Sensor(stype, self.rewrite_name(name), description, units)
-        self.sensors.add(s)
+        for new_name in self._rewritten_names(name):
+            s: sensor.Sensor = sensor.Sensor(stype, new_name, description, units)
+            self.sensors.add(s)
 
     def sensor_removed(self, name: str) -> None:
-        self.sensors.pop(self.rewrite_name(name), None)
+        for new_name in self._rewritten_names(name):
+            self.sensors.pop(new_name, None)
 
     def sensor_updated(
         self, name: str, value: bytes, status: sensor.Sensor.Status, timestamp: float
     ) -> None:
-        try:
-            sensor = self.sensors[self.rewrite_name(name)]
-        except KeyError:
-            self.logger.warning("Received update for unknown sensor %s", name)
-            return
-
-        try:
-            decoded = core.decode(sensor.stype, value)
-        except ValueError as exc:
-            self.logger.warning(
-                "Sensor %s: value %r does not match type %s: %s",
-                name,
-                value,
-                sensor.type_name,
-                exc,
-            )
-            return
+        for new_name in self._rewritten_names(name):
+            try:
+                sensor = self.sensors[new_name]
+            except KeyError:
+                self.logger.warning("Received update for unknown sensor %s", name)
+                continue
+
+            try:
+                decoded = core.decode(sensor.stype, value)
+            except ValueError as exc:
+                self.logger.warning(
+                    "Sensor %s: value %r does not match type %s: %s",
+                    name,
+                    value,
+                    sensor.type_name,
+                    exc,
+                )
+                continue
 
-        sensor.set_value(decoded, status=status, timestamp=timestamp)
+            sensor.set_value(decoded, status=status, timestamp=timestamp)
 
     def state_updated(self, state: SyncState) -> None:
         if state == SyncState.DISCONNECTED:
             now = time.time()
             for s in self.sensors.values():
                 s.set_value(s.value, status=sensor.Sensor.Status.UNREACHABLE, timestamp=now)
```

### Comparing `aiokatcp-1.6.2/src/aiokatcp/connection.py` & `aiokatcp-1.7.0/src/aiokatcp/connection.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/src/aiokatcp/core.py` & `aiokatcp-1.7.0/src/aiokatcp/core.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/src/aiokatcp/sensor.py` & `aiokatcp-1.7.0/src/aiokatcp/sensor.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/src/aiokatcp/server.py` & `aiokatcp-1.7.0/src/aiokatcp/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,15 @@
             remove = True
         except BaseException as exc:
             try:
                 name = f"task {task.get_name()!r}"  # type: ignore
             except AttributeError:
                 # Python 3.7 does not have task names
                 name = "a task"
-            logger.warning("Halting the server because %s raised %s", name, exc)
+            logger.warning("Halting the server because %s raised %s", name, exc, exc_info=True)
             self.halt()
         if remove:
             # No exception to report during shutdown, so clean it up
             try:
                 self._service_tasks.remove(task)
             except ValueError:  # Can happen during shutdown
                 pass
```

### Comparing `aiokatcp-1.6.2/src/aiokatcp/time_sync.py` & `aiokatcp-1.7.0/src/aiokatcp/time_sync.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/src/aiokatcp/tools/katcpcmd.py` & `aiokatcp-1.7.0/src/aiokatcp/tools/katcpcmd.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/src/aiokatcp.egg-info/PKG-INFO` & `aiokatcp-1.7.0/src/aiokatcp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokatcp
-Version: 1.6.2
+Version: 1.7.0
 Summary: Asynchronous I/O implementation of the katcp protocol
 Home-page: https://github.com/ska-sa/aiokatcp
 Author: Bruce Merry
 Author-email: bmerry@sarao.ac.za
 License: BSD
 Keywords: asyncio,katcp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiokatcp-1.6.2/src/aiokatcp.egg-info/SOURCES.txt` & `aiokatcp-1.7.0/src/aiokatcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/tests/test_client.py` & `aiokatcp-1.7.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import asyncio.base_events
 import enum
 import gc
 import logging
 import re
 import unittest
 import unittest.mock
-from typing import AsyncGenerator, Tuple, Type, Union, cast
+from typing import AsyncGenerator, Sequence, Tuple, Type, Union, cast
 from unittest.mock import call
 
 import async_solipsism
 import pytest
 
 from aiokatcp import (
     AbstractSensorWatcher,
@@ -625,15 +625,17 @@
             call.sensor_updated("device-status", b"ok", Sensor.Status.NOMINAL, 123456789.0),
             call.batch_stop(),
             call.state_updated(SyncState.SYNCED),
         ]
 
 
 class DummySensorWatcher(SensorWatcher):
-    def rewrite_name(self, name: str) -> str:
+    def rewrite_name(self, name: str) -> Union[str, Sequence[str]]:
+        if name == "bar":
+            return ["test_bar1", "test_bar2"]
         return "test_" + name
 
 
 class DummyEnum(enum.Enum):
     THING_ONE = 1
     THING_TWO = 2
 
@@ -654,22 +656,30 @@
     def test_construct(self, watcher: DummySensorWatcher) -> None:
         assert len(watcher.sensors) == 0
         assert not watcher.synced.is_set()
 
     def test_sensor_added(self, watcher: DummySensorWatcher) -> None:
         watcher.batch_start()
         watcher.sensor_added("foo", "A sensor", "F", "float")
+        watcher.sensor_added("bar", "A duplicated sensor", "s", "integer")
         watcher.batch_stop()
-        assert len(watcher.sensors) == 1
+        assert len(watcher.sensors) == 3
         sensor = watcher.sensors["test_foo"]
         assert sensor.name == "test_foo"
         assert sensor.description == "A sensor"
         assert sensor.units == "F"
         assert sensor.stype == float
         assert sensor.status == Sensor.Status.UNKNOWN
+        for name in ["test_bar1", "test_bar2"]:
+            sensor = watcher.sensors[name]
+            assert sensor.name == name
+            assert sensor.description == "A duplicated sensor"
+            assert sensor.units == "s"
+            assert sensor.stype == int
+            assert sensor.status == Sensor.Status.UNKNOWN
 
     def test_sensor_added_discrete(self, watcher: DummySensorWatcher) -> None:
         watcher.batch_start()
         watcher.sensor_added("disc", "Discrete sensor", "", "discrete", b"abc", b"def-xyz")
         watcher.sensor_added("disc2", "Discrete sensor 2", "", "discrete", b"abc", b"def-xyz")
         watcher.batch_stop()
         assert len(watcher.sensors) == 2
@@ -708,27 +718,34 @@
         )
 
     def test_sensor_removed(self, watcher: DummySensorWatcher) -> None:
         self.test_sensor_added(watcher)
 
         watcher.batch_start()
         watcher.sensor_removed("foo")
+        watcher.sensor_removed("bar")
         watcher.batch_stop()
         assert len(watcher.sensors) == 0
 
     def test_sensor_updated(self, watcher: DummySensorWatcher) -> None:
         self.test_sensor_added(watcher)
 
         watcher.batch_start()
         watcher.sensor_updated("foo", b"12.5", Sensor.Status.WARN, 1234567890.0)
+        watcher.sensor_updated("bar", b"42", Sensor.Status.ERROR, 1234567891.5)
         watcher.batch_stop()
         sensor = watcher.sensors["test_foo"]
         assert sensor.value == 12.5
         assert sensor.status == Sensor.Status.WARN
         assert sensor.timestamp == 1234567890.0
+        for name in ["test_bar1", "test_bar2"]:
+            sensor = watcher.sensors[name]
+            assert sensor.value == 42
+            assert sensor.status == Sensor.Status.ERROR
+            assert sensor.timestamp == 1234567891.5
 
     def test_sensor_updated_bad_value(self, watcher: DummySensorWatcher) -> None:
         self.test_sensor_added(watcher)
 
         watcher.batch_start()
         watcher.sensor_updated("foo", b"not a float", Sensor.Status.WARN, 1234567890.0)
         watcher.batch_stop()
@@ -740,37 +757,38 @@
             unittest.mock.ANY,
         )
 
     def test_sensor_updated_unknown_sensor(self, watcher: DummySensorWatcher) -> None:
         self.test_sensor_added(watcher)
 
         watcher.batch_start()
-        watcher.sensor_updated("bar", b"123.0", Sensor.Status.WARN, 1234567890.0)
+        watcher.sensor_updated("spam", b"123.0", Sensor.Status.WARN, 1234567890.0)
         watcher.batch_stop()
         watcher.logger.warning.assert_called_once_with(  # type: ignore
-            "Received update for unknown sensor %s", "bar"
+            "Received update for unknown sensor %s", "spam"
         )
 
     def test_state_updated(self, watcher: DummySensorWatcher) -> None:
         self.test_sensor_added(watcher)
 
         watcher.state_updated(SyncState.SYNCING)
         assert not watcher.synced.is_set()
-        assert len(watcher.sensors) == 1
+        assert len(watcher.sensors) == 3
         assert watcher.sensors["test_foo"].status == Sensor.Status.UNKNOWN
 
         watcher.state_updated(SyncState.SYNCED)
         assert watcher.synced.is_set()
-        assert len(watcher.sensors) == 1
+        assert len(watcher.sensors) == 3
         assert watcher.sensors["test_foo"].status == Sensor.Status.UNKNOWN
 
         watcher.state_updated(SyncState.DISCONNECTED)
         assert not watcher.synced.is_set()
         # Disconnecting should set all sensors to UNREACHABLE
-        assert watcher.sensors["test_foo"].status == Sensor.Status.UNREACHABLE
+        for name in ["test_foo", "test_bar1", "test_bar2"]:
+            assert watcher.sensors[name].status == Sensor.Status.UNREACHABLE
 
 
 @pytest.mark.channel_args(auto_reconnect=False)
 class TestClientNoReconnect:
     async def test_unparsable_protocol(self, channel) -> None:
         channel.writer.write(b"#version-connect katcp-protocol notvalid\n")
         assert await channel.reader.read() == b""
```

### Comparing `aiokatcp-1.6.2/tests/test_connection.py` & `aiokatcp-1.7.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/tests/test_core.py` & `aiokatcp-1.7.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/tests/test_sensor.py` & `aiokatcp-1.7.0/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/tests/test_server.py` & `aiokatcp-1.7.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.6.2/tests/test_time_sync.py` & `aiokatcp-1.7.0/tests/test_time_sync.py`

 * *Files identical despite different names*

