# Comparing `tmp/ops-scenario-2.1.3.4.tar.gz` & `tmp/ops-scenario-2.1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-scenario-2.1.3.4.tar", last modified: Wed Apr  5 09:11:16 2023, max compression
+gzip compressed data, was "ops-scenario-2.1.3.5.tar", last modified: Fri Apr 21 13:19:18 2023, max compression
```

## Comparing `ops-scenario-2.1.3.4.tar` & `ops-scenario-2.1.3.5.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.122798 ops-scenario-2.1.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.114798 ops-scenario-2.1.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.118798 ops-scenario-2.1.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-04-05 09:11:16.122798 ops-scenario-2.1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28953 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.118798 ops-scenario-2.1.3.4/ops_scenario.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-04-05 09:11:15.000000 ops-scenario-2.1.3.4/ops_scenario.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-05 09:11:16.000000 ops-scenario-2.1.3.4/ops_scenario.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:11:15.000000 ops-scenario-2.1.3.4/ops_scenario.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-05 09:11:15.000000 ops-scenario-2.1.3.4/ops_scenario.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-05 09:11:15.000000 ops-scenario-2.1.3.4/ops_scenario.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 09:11:15.000000 ops-scenario-2.1.3.4/ops_scenario.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.118798 ops-scenario-2.1.3.4/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/resources/state-transition-model.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.118798 ops-scenario-2.1.3.4/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/capture_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/fs_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/ops_main_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.118798 ops-scenario-2.1.3.4/scenario/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29186 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/scripts/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    38426 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/scenario/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:11:16.122798 ops-scenario-2.1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.118798 ops-scenario-2.1.3.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.122798 ops-scenario-2.1.3.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/resources/demo_decorate_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_consistency_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:11:16.122798 ops-scenario-2.1.3.4/tests/test_e2e/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_builtin_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_custom_event_triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_deferred.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_juju_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_play_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_rubbish_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_stored_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_e2e/test_vroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_emitted_events_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-05 09:11:02.000000 ops-scenario-2.1.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.320035 ops-scenario-2.1.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.312034 ops-scenario-2.1.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-04-21 13:19:18.320035 ops-scenario-2.1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28953 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/ops_scenario.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/resources/state-transition-model.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/capture_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/fs_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/ops_main_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/scenario/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29386 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38623 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:19:18.320035 ops-scenario-2.1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/resources/demo_decorate_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_consistency_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.320035 ops-scenario-2.1.3.5/tests/test_e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_builtin_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_custom_event_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_deferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_juju_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_play_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_rubbish_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_stored_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_vroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_emitted_events_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tox.ini
```

### Comparing `ops-scenario-2.1.3.4/.github/workflows/build_wheels.yaml` & `ops-scenario-2.1.3.5/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/.github/workflows/quality_checks.yaml` & `ops-scenario-2.1.3.5/.github/workflows/quality_checks.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/LICENSE.txt` & `ops-scenario-2.1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/PKG-INFO` & `ops-scenario-2.1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 2.1.3.4
+Version: 2.1.3.5
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/PietroPasotti/ops-scenario
 Project-URL: Bug Tracker, https://github.com/PietroPasotti/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ops-scenario-2.1.3.4/README.md` & `ops-scenario-2.1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/ops_scenario.egg-info/PKG-INFO` & `ops-scenario-2.1.3.5/ops_scenario.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 2.1.3.4
+Version: 2.1.3.5
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/PietroPasotti/ops-scenario
 Project-URL: Bug Tracker, https://github.com/PietroPasotti/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ops-scenario-2.1.3.4/ops_scenario.egg-info/SOURCES.txt` & `ops-scenario-2.1.3.5/ops_scenario.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,19 @@
 scenario/fs_mocks.py
 scenario/logger.py
 scenario/mocking.py
 scenario/ops_main_mock.py
 scenario/runtime.py
 scenario/sequences.py
 scenario/state.py
+scenario/scripts/errors.py
+scenario/scripts/logger.py
 scenario/scripts/main.py
 scenario/scripts/snapshot.py
+scenario/scripts/utils.py
 tests/test_consistency_checker.py
 tests/test_emitted_events_util.py
 tests/test_runtime.py
 tests/resources/__init__.py
 tests/resources/demo_decorate_class.py
 tests/test_e2e/test_builtin_scenes.py
 tests/test_e2e/test_config.py
```

### Comparing `ops-scenario-2.1.3.4/pyproject.toml` & `ops-scenario-2.1.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools_scm >= 2.0.0, <3"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ops-scenario"
 
-version = "2.1.3.4"
+version = "2.1.3.5"
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" }
 ]
 description = "Python library providing a Scenario-based testing API for Operator Framework charms."
 license.text = "Apache-2.0"
 keywords = ["juju", "test"]
```

### Comparing `ops-scenario-2.1.3.4/resources/state-transition-model.png` & `ops-scenario-2.1.3.5/resources/state-transition-model.png`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/scenario/capture_events.py` & `ops-scenario-2.1.3.5/scenario/capture_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/scenario/consistency_checker.py` & `ops-scenario-2.1.3.5/scenario/consistency_checker.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/scenario/fs_mocks.py` & `ops-scenario-2.1.3.5/scenario/fs_mocks.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/scenario/mocking.py` & `ops-scenario-2.1.3.5/scenario/mocking.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/scenario/ops_main_mock.py` & `ops-scenario-2.1.3.5/scenario/ops_main_mock.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/scenario/runtime.py` & `ops-scenario-2.1.3.5/scenario/runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/scenario/scripts/snapshot.py` & `ops-scenario-2.1.3.5/scenario/scripts/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,84 +1,57 @@
 #!/usr/bin/env python3
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
+
 import datetime
 import json
-import logging
 import os
 import re
 import shlex
 import sys
 import tempfile
 from dataclasses import asdict
 from enum import Enum
 from itertools import chain
 from pathlib import Path
 from subprocess import run
-from textwrap import dedent
 from typing import Any, BinaryIO, Dict, Iterable, List, Optional, TextIO, Tuple, Union
 
 import ops.pebble
 import typer
 import yaml
 from ops.storage import SQLiteStorage
 
 from scenario.runtime import UnitStateDB
+from scenario.scripts.errors import InvalidTargetModelName, InvalidTargetUnitName
+from scenario.scripts.logger import logger as root_scripts_logger
+from scenario.scripts.utils import JujuUnitName
 from scenario.state import (
     Address,
     BindAddress,
     Container,
     Model,
     Mount,
     Network,
     Relation,
     Secret,
     State,
     Status,
     _EntityStatus,
 )
 
-logger = logging.getLogger("snapshot")
+logger = root_scripts_logger.getChild(__file__)
 
 JUJU_RELATION_KEYS = frozenset({"egress-subnets", "ingress-address", "private-address"})
 JUJU_CONFIG_KEYS = frozenset({})
 
 SNAPSHOT_OUTPUT_DIR = (Path(os.getcwd()).parent / "snapshot_storage").absolute()
 CHARM_SUBCLASS_REGEX = re.compile(r"class (\D+)\(CharmBase\):")
 
 
-class SnapshotError(RuntimeError):
-    """Base class for errors raised by snapshot."""
-
-
-class InvalidTargetUnitName(SnapshotError):
-    """Raised if the unit name passed to snapshot is invalid."""
-
-
-class InvalidTargetModelName(SnapshotError):
-    """Raised if the model name passed to snapshot is invalid."""
-
-
-class JujuUnitName(str):
-    """This class represents the name of a juju unit that can be snapshotted."""
-
-    def __init__(self, unit_name: str):
-        super().__init__()
-        app_name, _, unit_id = unit_name.rpartition("/")
-        if not app_name or not unit_id:
-            raise InvalidTargetUnitName(f"invalid unit name: {unit_name!r}")
-        self.unit_name = unit_name
-        self.app_name = app_name
-        self.unit_id = int(unit_id)
-        self.normalized = f"{app_name}-{unit_id}"
-        self.remote_charm_root = Path(
-            f"/var/lib/juju/agents/unit-{self.normalized}/charm"
-        )
-
-
 def _try_format(string: str):
     try:
         import black
 
         try:
             return black.format_str(string, mode=black.Mode())
         except black.parsing.InvalidInput as e:
@@ -86,50 +59,51 @@
             return string
     except ModuleNotFoundError:
         logger.warning("install black for formatting")
         return string
 
 
 def format_state(state: State):
-    """Pretty-print this State as-is."""
+    """Stringify this State as nicely as possible."""
     return _try_format(repr(state))
 
 
+PYTEST_TEST_TEMPLATE = """
+from scenario.state import *
+from charm import {ct}
+
+def test_case():
+    # Arrange: prepare the state
+    state = {state}
+    
+    #Act: trigger an event on the state 
+    out = state.trigger(
+        {en}
+        {ct}
+        juju_version="{jv}"
+        )
+        
+    # Assert: verify that the output state is the way you want it to be
+    # TODO: add assertions
+"""
+
+
 def format_test_case(
     state: State,
     charm_type_name: str = None,
     event_name: str = None,
     juju_version: str = None,
 ):
     """Format this State as a pytest test case."""
     ct = charm_type_name or "CHARM_TYPE,  # TODO: replace with charm type name"
     en = event_name or "EVENT_NAME,  # TODO: replace with event name"
     jv = juju_version or "3.0,  # TODO: check juju version is correct"
+    state_fmt = repr(state)
     return _try_format(
-        dedent(
-            f"""
-            from scenario.state import *
-            from charm import {ct}
-            
-            def test_case():
-                # Arrange: prepare the state
-                state = {state}
-                
-                #Act: trigger an event on the state 
-                out = state.trigger(
-                    {en}
-                    {ct}
-                    juju_version="{jv}"
-                    )
-                    
-                # Assert: verify that the output state is the way you want it to be
-                # TODO: add assertions
-            
-            """
-        )
+        PYTEST_TEST_TEMPLATE.format(state=state_fmt, ct=ct, en=en, jv=jv)
     )
 
 
 def _juju_run(cmd: str, model=None) -> Dict[str, Any]:
     """Execute juju {command} in a given model."""
     _model = f" -m {model}" if model else ""
     cmd = f"juju {cmd}{_model} --format json"
@@ -213,16 +187,15 @@
     model: Optional[str],
     metadata: Dict,
     include_dead: bool = False,
     relations: Tuple[str, ...] = (),
 ) -> List[Network]:
     """Get all Networks from this unit."""
     logger.info("getting networks...")
-    networks = []
-    networks.append(get_network(target, model, "juju-info"))
+    networks = [get_network(target, model, "juju-info")]
 
     endpoints = relations  # only alive relations
     if include_dead:
         endpoints = chain(
             metadata.get("provides", ()),
             metadata.get("requires", ()),
             metadata.get("peers", ()),
@@ -247,18 +220,14 @@
     )
     return yaml.safe_load(raw_meta)
 
 
 class RemotePebbleClient:
     """Clever little class that wraps calls to a remote pebble client."""
 
-    # TODO: there is a .pebble.state in kubernetes containers at
-    #  /var/lib/pebble/default/.pebble.state
-    #  figure out what it's for.
-
     def __init__(
         self, container: str, target: JujuUnitName, model: Optional[str] = None
     ):
         self.socket_path = f"/charm/containers/{container}/pebble.socket"
         self.container = container
         self.target = target
         self.model = model
@@ -469,15 +438,18 @@
         app_version=app_version,
     )
 
 
 def get_endpoints(juju_status: Dict, target: JujuUnitName) -> Tuple[str, ...]:
     """Parse `juju status` to get the relation names owned by the target."""
     app = juju_status["applications"][target.app_name]
-    relations = tuple(app["relations"].keys())
+    relations_raw = app.get("relations", None)
+    if not relations_raw:
+        return ()
+    relations = tuple(relations_raw.keys())
     return relations
 
 
 def get_config(
     target: JujuUnitName, model: Optional[str]
 ) -> Dict[str, Union[str, int, float, bool]]:
     """Get config dict from target."""
@@ -571,14 +543,19 @@
             target,
             model,
             f"relation-get -r {relation_id} - {target} --format json --app",
         )
         local_app_data = json.loads(local_app_data_raw)
 
         some_remote_unit_id = JujuUnitName(next(iter(related_units)))
+
+        # fixme: at the moment the juju CLI offers no way to see what type of relation this is;
+        #  if it's a peer relation or a subordinate, we should use the corresponding
+        #  scenario.state types instead of a regular Relation.
+
         relations.append(
             Relation(
                 endpoint=raw_relation["endpoint"],
                 interface=_get_interface_from_metadata(
                     raw_relation["endpoint"], metadata
                 ),
                 relation_id=relation_id,
@@ -642,14 +619,28 @@
 
 
 def get_juju_version(juju_status: Dict) -> str:
     """Get juju agent version from juju status output."""
     return juju_status["model"]["version"]
 
 
+def get_charm_version(target: JujuUnitName, juju_status: Dict) -> str:
+    """Get charm version info from juju status output."""
+    app_info = juju_status["applications"][target.app_name]
+    channel = app_info["charm-channel"]
+    charm_name = app_info["charm-name"]
+    app_version = app_info["version"]
+    charm_rev = app_info["charm-rev"]
+    charm_origin = app_info["charm-origin"]
+    return (
+        f"charm {charm_name!r} ({channel}/{charm_rev}); "
+        f"origin := {charm_origin}; app version := {app_version}."
+    )
+
+
 class RemoteUnitStateDB(UnitStateDB):
     """Represents a remote unit's state db."""
 
     def __init__(self, model: Optional[str], target: JujuUnitName):
         self._tempfile = tempfile.NamedTemporaryFile()
         super().__init__(self._tempfile.name)
 
@@ -696,18 +687,18 @@
             f"invalid target: {target!r} is not a valid unit name. Should be formatted like so:"
             f"`foo/1`, or `database/0`, or `myapp-foo-bar/42`."
         )
         sys.exit(1)
 
     logger.info(f'beginning snapshot of {target} in model {model or "<current>"}...')
 
-    def if_include(key, get_value, null_value):
+    def if_include(key, fn, default):
         if include is None or key in include:
-            return get_value()
-        return null_value
+            return fn()
+        return default
 
     try:
         state_model = get_model(model)
     except InvalidTargetModelName:
         logger.critical(f"unable to get Model from name {model}.", exc_info=True)
         sys.exit(1)
 
@@ -757,15 +748,15 @@
                     metadata,
                     include_dead=include_dead_relation_networks,
                     relations=endpoints,
                 ),
                 [],
             ),
             secrets=if_include(
-                "s",
+                "S",
                 lambda: get_secrets(
                     target,
                     model,
                     metadata,
                     relations=endpoints,
                 ),
                 [],
@@ -790,32 +781,36 @@
     except InvalidTargetModelName:
         logger.critical(f"invalid model: {model!r} not found.")
         sys.exit(1)
 
     logger.info(f"snapshot done.")
 
     if pprint:
+        charm_version = get_charm_version(target, juju_status)
         juju_version = get_juju_version(juju_status)
         if format == FormatOption.pytest:
             charm_type_name = try_guess_charm_type_name()
             txt = format_test_case(
                 state, charm_type_name=charm_type_name, juju_version=juju_version
             )
         elif format == FormatOption.state:
             txt = format_state(state)
         elif format == FormatOption.json:
             txt = json.dumps(asdict(state), indent=2)
         else:
             raise ValueError(f"unknown format {format}")
 
-        timestamp = datetime.datetime.now().strftime("%m/%d/%Y, %H:%M:%S")
+        controller_timestamp = juju_status["controller"]["timestamp"]
+        local_timestamp = datetime.datetime.now().strftime("%m/%d/%Y, %H:%M:%S")
         print(
             f"# Generated by scenario.snapshot. \n"
-            f"# Snapshot of {state_model.name}:{target.unit_name} at {timestamp}. \n"
+            f"# Snapshot of {state_model.name}:{target.unit_name} at {local_timestamp}. \n"
+            f"# Controller timestamp := {controller_timestamp}. \n"
             f"# Juju version := {juju_version} \n"
+            f"# Charm fingerprint := {charm_version} \n"
         )
         print(txt)
 
     return state
 
 
 def snapshot(
@@ -825,26 +820,27 @@
     ),
     format: FormatOption = typer.Option(
         "state",
         "-f",
         "--format",
         help="How to format the output. "
         "``state``: Outputs a black-formatted repr() of the State object (if black is installed! "
-        "else it will be ugly but valid python code). "
+        "else it will be ugly but valid python code). All you need to do then is import the necessary "
+        "objects from scenario.state, and you should have a valid State object."
         "``json``: Outputs a Jsonified State object. Perfect for storage. "
         "``pytest``: Outputs a full-blown pytest scenario test based on this State. "
         "Pipe it to a file and fill in the blanks.",
     ),
     include: str = typer.Option(
         "rckndt",
         "--include",
         "-i",
         help="What data to include in the state. "
         "``r``: relation, ``c``: config, ``k``: containers, "
-        "``n``: networks, ``s``: secrets(!), "
+        "``n``: networks, ``S``: secrets(!), "
         "``d``: deferred events, ``t``: stored state.",
     ),
     include_dead_relation_networks: bool = typer.Option(
         False,
         "--include-dead-relation-networks",
         help="Whether to gather networks of inactive relation endpoints.",
         is_flag=True,
@@ -896,17 +892,17 @@
 _snapshot.__doc__ = snapshot.__doc__
 
 if __name__ == "__main__":
     # print(_snapshot("zookeeper/0", model="foo", format=FormatOption.pytest))
 
     print(
         _snapshot(
-            "prom/0",
-            format=FormatOption.pytest,
-            include="t",
+            "traefik/0",
+            format=FormatOption.state,
+            include="r",
             # fetch_files={
             #     "traefik": [
             #         Path("/opt/traefik/juju/certificates.yaml"),
             #         Path("/opt/traefik/juju/certificate.cert"),
             #         Path("/opt/traefik/juju/certificate.key"),
             #         Path("/etc/traefik/traefik.yaml"),
             #     ]
```

### Comparing `ops-scenario-2.1.3.4/scenario/sequences.py` & `ops-scenario-2.1.3.5/scenario/sequences.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/scenario/state.py` & `ops-scenario-2.1.3.5/scenario/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -656,15 +656,15 @@
 
 @dataclasses.dataclass
 class _EntityStatus(_DCBase):
     """This class represents StatusBase and should not be interacted with directly."""
 
     # Why not use StatusBase directly? Because that's not json-serializable.
 
-    name: str
+    name: Literal["waiting", "blocked", "active", "unknown", "error", "maintenance"]
     message: str = ""
 
     def __eq__(self, other):
         if isinstance(other, Tuple):
             logger.warning(
                 "Comparing Status with Tuples is deprecated and will be removed soon."
             )
@@ -676,14 +676,18 @@
             f"Please compare with StatusBase directly."
         )
         return super().__eq__(other)
 
     def __iter__(self):
         return iter([self.name, self.message])
 
+    def __repr__(self):
+        status_type_name = self.name.title() + "Status"
+        return f"{status_type_name}('{self.message}')"
+
 
 def _status_to_entitystatus(obj: StatusBase) -> _EntityStatus:
     """Convert StatusBase to _EntityStatus."""
     return _EntityStatus(obj.name, obj.message)
 
 
 @dataclasses.dataclass
@@ -1083,16 +1087,14 @@
 
 @dataclasses.dataclass
 class Inject(_DCBase):
     """Base class for injectors: special placeholders used to tell harness_ctx
     to inject instances that can't be retrieved in advance in event args or kwargs.
     """
 
-    pass
-
 
 @dataclasses.dataclass
 class InjectRelation(Inject):
     relation_name: str
     relation_id: Optional[int] = None
```

### Comparing `ops-scenario-2.1.3.4/tests/test_consistency_checker.py` & `ops-scenario-2.1.3.5/tests/test_consistency_checker.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_builtin_scenes.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_builtin_scenes.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_config.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_config.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_custom_event_triggers.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_custom_event_triggers.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,32 @@
 
     class MyCharmEvents(CharmEvents):
         foo = EventSource(FooEvent)
 
     class MyCharm(CharmBase):
         META = {"name": "mycharm"}
         on = MyCharmEvents()
-        _foo_called = False
+        _foo_called = 0
 
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self.framework.observe(self.on.foo, self._on_foo)
+            self.framework.observe(self.on.start, self._on_start)
 
         def _on_foo(self, e):
-            MyCharm._foo_called = True
+            MyCharm._foo_called += 1
+
+        def _on_start(self, e):
+            self.on.foo.emit()
 
     State().trigger("foo", MyCharm, meta=MyCharm.META)
-    assert MyCharm._foo_called
+    assert MyCharm._foo_called == 1
+
+    State().trigger("start", MyCharm, meta=MyCharm.META)
+    assert MyCharm._foo_called == 2
 
 
 def test_funky_named_event_emitted():
     class FooRelationChangedEvent(EventBase):
         pass
 
     class MyCharmEvents(CharmEvents):
```

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_deferred.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_deferred.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_juju_log.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_juju_log.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_network.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_network.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_observers.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_observers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_pebble.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_pebble.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_play_assertions.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_play_assertions.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_relations.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_relations.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_rubbish_events.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_rubbish_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_secrets.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_secrets.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_state.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_status.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_status.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_stored_state.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_stored_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_e2e/test_vroot.py` & `ops-scenario-2.1.3.5/tests/test_e2e/test_vroot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_emitted_events_util.py` & `ops-scenario-2.1.3.5/tests/test_emitted_events_util.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tests/test_runtime.py` & `ops-scenario-2.1.3.5/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.4/tox.ini` & `ops-scenario-2.1.3.5/tox.ini`

 * *Files identical despite different names*

