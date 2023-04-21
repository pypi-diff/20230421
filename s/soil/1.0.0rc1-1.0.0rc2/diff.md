# Comparing `tmp/soil-1.0.0rc1.tar.gz` & `tmp/soil-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soil-1.0.0rc1.tar", last modified: Thu Apr 20 16:05:38 2023, max compression
+gzip compressed data, was "soil-1.0.0rc2.tar", last modified: Fri Apr 21 11:42:16 2023, max compression
```

## Comparing `soil-1.0.0rc1.tar` & `soil-1.0.0rc2.tar`

### file list

```diff
@@ -1,98 +1,95 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/
--rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc1/LICENSE
--rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc1/MANIFEST.in
--rw-rw-r--   0 j         (1000) j         (1000)     5741 2023-04-20 16:05:38.760715 soil-1.0.0rc1/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)     4660 2023-04-20 15:35:04.000000 soil-1.0.0rc1/README.md
--rw-rw-r--   0 j         (1000) j         (1000)      166 2023-04-14 21:22:05.000000 soil-1.0.0rc1/requirements.txt
--rw-r--r--   0 j         (1000) j         (1000)      191 2023-04-20 16:05:38.760715 soil-1.0.0rc1/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)     2188 2023-04-20 16:05:16.000000 soil-1.0.0rc1/setup.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/
--rw-rw-r--   0 j         (1000) j         (1000)      365 2023-03-23 13:48:55.000000 soil-1.0.0rc1/soil/.VERSION.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc1/soil/.__init__.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc1/soil/.analysis.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    14451 2023-04-14 21:44:41.000000 soil-1.0.0rc1/soil/.environment.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc1/soil/.exporters.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc1/soil/.serialization.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc1/soil/.simulation.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc1/soil/.stats.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)    19083 2023-04-16 21:07:22.000000 soil-1.0.0rc1/soil/.time.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      330 2023-04-14 19:49:37.000000 soil-1.0.0rc1/soil/.utils.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc1/soil/.visualization.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)        8 2023-04-20 16:02:50.000000 soil-1.0.0rc1/soil/VERSION
--rw-rw-r--   0 j         (1000) j         (1000)     7923 2023-04-19 23:43:19.000000 soil-1.0.0rc1/soil/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-14 18:17:58.000000 soil-1.0.0rc1/soil/__main__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/agents/
--rw-rw-r--   0 j         (1000) j         (1000)     1422 2023-04-16 20:19:36.000000 soil-1.0.0rc1/soil/agents/.__init__.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)     5970 2023-04-14 19:52:27.000000 soil-1.0.0rc1/soil/agents/.fsm.py.~undo-tree~
--rw-rw-r--   0 j         (1000) j         (1000)      734 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/agents/BassModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-14 18:19:58.000000 soil-1.0.0rc1/soil/agents/CounterModel.py
--rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-17 13:43:11.000000 soil-1.0.0rc1/soil/agents/Geo.py
--rw-rw-r--   0 j         (1000) j         (1000)      766 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/agents/IndependentCascadeModel.py
--rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/agents/SISaModel.py
--rw-rw-r--   0 j         (1000) j         (1000)    19495 2023-04-17 13:33:41.000000 soil-1.0.0rc1/soil/agents/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     2365 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/agents/evented.py
--rw-rw-r--   0 j         (1000) j         (1000)     4493 2023-04-17 14:27:57.000000 soil-1.0.0rc1/soil/agents/fsm.py
--rw-rw-r--   0 j         (1000) j         (1000)     3409 2023-04-17 13:51:14.000000 soil-1.0.0rc1/soil/agents/network_agents.py
--rw-rw-r--   0 j         (1000) j         (1000)     2196 2023-04-20 11:27:08.000000 soil-1.0.0rc1/soil/analysis.py
--rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-13 16:06:35.000000 soil-1.0.0rc1/soil/config.py
--rw-rw-r--   0 j         (1000) j         (1000)      843 2023-04-18 16:33:54.000000 soil-1.0.0rc1/soil/datacollection.py
--rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-14 15:59:02.000000 soil-1.0.0rc1/soil/debugging.py
--rw-rw-r--   0 j         (1000) j         (1000)      168 2023-04-14 11:40:15.000000 soil-1.0.0rc1/soil/decorators.py
--rw-rw-r--   0 j         (1000) j         (1000)    15254 2023-04-20 09:19:00.000000 soil-1.0.0rc1/soil/environment.py
--rw-rw-r--   0 j         (1000) j         (1000)     1092 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/events.py
--rw-rw-r--   0 j         (1000) j         (1000)     9141 2023-04-20 11:22:12.000000 soil-1.0.0rc1/soil/exporters.py
--rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-09 02:16:08.000000 soil-1.0.0rc1/soil/network.py
--rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-08 22:41:17.000000 soil-1.0.0rc1/soil/parameters.py
--rw-rw-r--   0 j         (1000) j         (1000)     7687 2023-04-14 21:29:51.000000 soil-1.0.0rc1/soil/serialization.py
--rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc1/soil/settings.py
--rw-rw-r--   0 j         (1000) j         (1000)    13830 2023-04-20 14:51:30.000000 soil-1.0.0rc1/soil/simulation.py
--rw-rw-r--   0 j         (1000) j         (1000)     6099 2023-04-17 22:07:07.000000 soil-1.0.0rc1/soil/time.py
--rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-17 21:29:17.000000 soil-1.0.0rc1/soil/utils.py
--rw-rw-r--   0 j         (1000) j         (1000)      476 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/version.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/web/
--rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/.gitignore
--rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/README.md
--rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/web/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)       59 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/web/__main__.py
--rw-rw-r--   0 j         (1000) j         (1000)      575 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/web/config.yml
--rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-03-23 16:42:54.000000 soil-1.0.0rc1/soil/web/run.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.740715 soil-1.0.0rc1/soil/web/static/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/web/static/css/
--rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/static/css/main.css
--rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/static/css/timeline.css
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil/web/static/img/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.752715 soil-1.0.0rc1/soil/web/static/img/background/
--rw-r--r--   0 j         (1000) j         (1000)  1167302 2018-12-08 17:08:24.000000 soil-1.0.0rc1/soil/web/static/img/background/map.png
--rw-r--r--   0 j         (1000) j         (1000)  8340070 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/background/map_4800x2860.jpg
--rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/logo_gsi.svg
--rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/logo_soil.png
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/soil/web/static/img/svg/
--rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/home.svg
--rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/person.svg
--rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/plus.svg
--rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/target.svg
--rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/img/svg/time.svg
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/soil/web/static/js/
--rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/js/socket.js
--rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/js/template.js
--rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/js/timeline.js
--rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/static/js/visualization.js
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/soil/web/templates/
--rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc1/soil/web/templates/index.html
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.748715 soil-1.0.0rc1/soil.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)     5741 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     2046 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       78 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/entry_points.txt
--rw-r--r--   0 j         (1000) j         (1000)      257 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        5 2023-04-20 16:05:38.000000 soil-1.0.0rc1/soil.egg-info/top_level.txt
--rw-rw-r--   0 j         (1000) j         (1000)       43 2023-03-23 16:42:54.000000 soil-1.0.0rc1/test-requirements.txt
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-20 16:05:38.760715 soil-1.0.0rc1/tests/
--rw-rw-r--   0 j         (1000) j         (1000)     5920 2023-04-17 17:50:01.000000 soil-1.0.0rc1/tests/test_agents.py
--rw-rw-r--   0 j         (1000) j         (1000)     2336 2023-04-19 17:02:06.000000 soil-1.0.0rc1/tests/test_config.py
--rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-19 17:02:06.000000 soil-1.0.0rc1/tests/test_examples.py
--rw-rw-r--   0 j         (1000) j         (1000)     3756 2023-04-20 11:00:16.000000 soil-1.0.0rc1/tests/test_exporters.py
--rw-rw-r--   0 j         (1000) j         (1000)     7709 2023-04-19 22:29:46.000000 soil-1.0.0rc1/tests/test_main.py
--rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-03-23 16:42:54.000000 soil-1.0.0rc1/tests/test_mesa.py
--rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-14 11:36:16.000000 soil-1.0.0rc1/tests/test_network.py
--rw-rw-r--   0 j         (1000) j         (1000)     2092 2023-04-17 17:32:50.000000 soil-1.0.0rc1/tests/test_time.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.635202 soil-1.0.0rc2/
+-rw-r--r--   0 j         (1000) j         (1000)    11412 2018-12-07 19:26:39.000000 soil-1.0.0rc2/LICENSE
+-rw-r--r--   0 j         (1000) j         (1000)      163 2020-03-11 15:11:50.000000 soil-1.0.0rc2/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)     5740 2023-04-21 11:42:16.635202 soil-1.0.0rc2/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     4659 2023-04-21 11:40:49.000000 soil-1.0.0rc2/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)      166 2023-04-21 11:40:49.000000 soil-1.0.0rc2/requirements.txt
+-rw-rw-r--   0 j         (1000) j         (1000)      191 2023-04-21 11:42:16.635202 soil-1.0.0rc2/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     2188 2023-04-21 11:40:49.000000 soil-1.0.0rc2/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.627202 soil-1.0.0rc2/soil/
+-rw-rw-r--   0 j         (1000) j         (1000)      365 2023-03-23 13:48:55.000000 soil-1.0.0rc2/soil/.VERSION.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-14 19:48:55.000000 soil-1.0.0rc2/soil/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    13297 2023-03-23 13:34:51.000000 soil-1.0.0rc2/soil/.analysis.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    14451 2023-04-14 21:44:41.000000 soil-1.0.0rc2/soil/.environment.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     2588 2023-04-14 20:43:29.000000 soil-1.0.0rc2/soil/.exporters.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     1110 2023-04-14 21:29:51.000000 soil-1.0.0rc2/soil/.serialization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    15937 2023-04-16 19:59:22.000000 soil-1.0.0rc2/soil/.simulation.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5011 2023-03-23 13:48:01.000000 soil-1.0.0rc2/soil/.stats.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)    19083 2023-04-16 21:07:22.000000 soil-1.0.0rc2/soil/.time.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      330 2023-04-14 19:49:37.000000 soil-1.0.0rc2/soil/.utils.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      139 2023-04-04 13:46:42.000000 soil-1.0.0rc2/soil/.visualization.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)        8 2023-04-21 11:40:57.000000 soil-1.0.0rc2/soil/VERSION
+-rw-rw-r--   0 j         (1000) j         (1000)     7923 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      107 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/__main__.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.631202 soil-1.0.0rc2/soil/agents/
+-rw-rw-r--   0 j         (1000) j         (1000)     1422 2023-04-16 20:19:36.000000 soil-1.0.0rc2/soil/agents/.__init__.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)     5970 2023-04-14 19:52:27.000000 soil-1.0.0rc2/soil/agents/.fsm.py.~undo-tree~
+-rw-rw-r--   0 j         (1000) j         (1000)      734 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/agents/BassModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1171 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/agents/CounterModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)      731 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/agents/Geo.py
+-rw-rw-r--   0 j         (1000) j         (1000)      766 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/agents/IndependentCascadeModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3385 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/agents/SISaModel.py
+-rw-rw-r--   0 j         (1000) j         (1000)    19469 2023-04-21 11:41:58.000000 soil-1.0.0rc2/soil/agents/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2365 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/agents/evented.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4493 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/agents/fsm.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3409 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/agents/network_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2196 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/analysis.py
+-rw-rw-r--   0 j         (1000) j         (1000)       36 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/config.py
+-rw-rw-r--   0 j         (1000) j         (1000)      843 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/datacollection.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7217 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/debugging.py
+-rw-rw-r--   0 j         (1000) j         (1000)      168 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/decorators.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15254 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/environment.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1092 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/events.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9141 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2149 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/network.py
+-rw-rw-r--   0 j         (1000) j         (1000)      739 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/parameters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7687 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/serialization.py
+-rw-r--r--   0 j         (1000) j         (1000)       24 2018-12-07 19:26:39.000000 soil-1.0.0rc2/soil/settings.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13830 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/simulation.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6099 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/time.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/utils.py
+-rw-rw-r--   0 j         (1000) j         (1000)      476 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/version.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.631202 soil-1.0.0rc2/soil/web/
+-rw-r--r--   0 j         (1000) j         (1000)       41 2018-12-08 17:08:24.000000 soil-1.0.0rc2/soil/web/.gitignore
+-rw-r--r--   0 j         (1000) j         (1000)     2984 2018-12-08 17:08:24.000000 soil-1.0.0rc2/soil/web/README.md
+-rw-rw-r--   0 j         (1000) j         (1000)    11272 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/web/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)       59 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/web/__main__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      575 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/web/config.yml
+-rw-rw-r--   0 j         (1000) j         (1000)     1073 2023-04-21 11:40:49.000000 soil-1.0.0rc2/soil/web/run.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.623202 soil-1.0.0rc2/soil/web/static/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.631202 soil-1.0.0rc2/soil/web/static/css/
+-rw-r--r--   0 j         (1000) j         (1000)     7157 2018-12-08 17:08:24.000000 soil-1.0.0rc2/soil/web/static/css/main.css
+-rw-r--r--   0 j         (1000) j         (1000)     1107 2018-12-08 17:08:24.000000 soil-1.0.0rc2/soil/web/static/css/timeline.css
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.631202 soil-1.0.0rc2/soil/web/static/img/
+-rw-r--r--   0 j         (1000) j         (1000)    18053 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/img/logo_gsi.svg
+-rw-r--r--   0 j         (1000) j         (1000)   103744 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/img/logo_soil.png
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.631202 soil-1.0.0rc2/soil/web/static/img/svg/
+-rw-r--r--   0 j         (1000) j         (1000)      462 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/img/svg/home.svg
+-rw-r--r--   0 j         (1000) j         (1000)      812 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/img/svg/person.svg
+-rw-r--r--   0 j         (1000) j         (1000)      697 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/img/svg/plus.svg
+-rw-r--r--   0 j         (1000) j         (1000)      992 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/img/svg/target.svg
+-rw-r--r--   0 j         (1000) j         (1000)     1561 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/img/svg/time.svg
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.631202 soil-1.0.0rc2/soil/web/static/js/
+-rwxr-xr-x   0 j         (1000) j         (1000)    16528 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/js/socket.js
+-rw-r--r--   0 j         (1000) j         (1000)     5040 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/js/template.js
+-rw-r--r--   0 j         (1000) j         (1000)    12269 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/js/timeline.js
+-rw-r--r--   0 j         (1000) j         (1000)    21818 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/static/js/visualization.js
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.635202 soil-1.0.0rc2/soil/web/templates/
+-rw-r--r--   0 j         (1000) j         (1000)    16450 2018-12-08 17:08:25.000000 soil-1.0.0rc2/soil/web/templates/index.html
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.631202 soil-1.0.0rc2/soil.egg-info/
+-rw-r--r--   0 j         (1000) j         (1000)     5740 2023-04-21 11:42:16.000000 soil-1.0.0rc2/soil.egg-info/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1958 2023-04-21 11:42:16.000000 soil-1.0.0rc2/soil.egg-info/SOURCES.txt
+-rw-r--r--   0 j         (1000) j         (1000)        1 2023-04-21 11:42:16.000000 soil-1.0.0rc2/soil.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       78 2023-04-21 11:42:16.000000 soil-1.0.0rc2/soil.egg-info/entry_points.txt
+-rw-r--r--   0 j         (1000) j         (1000)      257 2023-04-21 11:42:16.000000 soil-1.0.0rc2/soil.egg-info/requires.txt
+-rw-r--r--   0 j         (1000) j         (1000)        5 2023-04-21 11:42:16.000000 soil-1.0.0rc2/soil.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       43 2023-04-21 11:40:49.000000 soil-1.0.0rc2/test-requirements.txt
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-04-21 11:42:16.635202 soil-1.0.0rc2/tests/
+-rw-rw-r--   0 j         (1000) j         (1000)     5920 2023-04-21 11:40:49.000000 soil-1.0.0rc2/tests/test_agents.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2336 2023-04-21 11:40:49.000000 soil-1.0.0rc2/tests/test_config.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2450 2023-04-21 11:40:49.000000 soil-1.0.0rc2/tests/test_examples.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3756 2023-04-21 11:40:49.000000 soil-1.0.0rc2/tests/test_exporters.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7709 2023-04-21 11:40:49.000000 soil-1.0.0rc2/tests/test_main.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1940 2023-04-21 11:40:49.000000 soil-1.0.0rc2/tests/test_mesa.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3133 2023-04-21 11:40:49.000000 soil-1.0.0rc2/tests/test_network.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2092 2023-04-21 11:40:49.000000 soil-1.0.0rc2/tests/test_time.py
```

### Comparing `soil-1.0.0rc1/LICENSE` & `soil-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/PKG-INFO` & `soil-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soil
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: An Agent-Based Social Simulator for Social Networks
 Home-page: https://github.com/gsi-upm/soil
-Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc1.tar.gz
+Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc2.tar.gz
 Author: J. Fernando Sanchez
 Author-email: jf.sanchez@upm.es
 Keywords: agent,social,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
@@ -61,15 +61,14 @@
 * A simulation runner (`soil.Simulation`) that can:
   * Run models in parallel
   * Save results to different formats
 * Simulation configuration files 
 * A command line interface (`soil`), to quickly run simulations with different parameters
 * An integrated debugger (`soil --debug`) with custom functions to print agent states and break at specific states
 
-
 ## Mesa compatibility
 
 SOIL has been redesigned to integrate well with [Mesa](https://github.com/projectmesa/mesa).
 For instance, it should be possible to run a `mesa.Model` models using a `soil.Simulation` and the `soil` CLI, or to integrate the `soil.TimedActivation` scheduler on a `mesa.Model`.
 
 Note that some combinations of `mesa` and `soil` components, while technically possible, are much less useful or might yield surprising results.
 For instance, you may add any `soil.agent` agent on a regular `mesa.Model` with a vanilla scheduler from `mesa.time`.
```

### Comparing `soil-1.0.0rc1/README.md` & `soil-1.0.0rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 * A simulation runner (`soil.Simulation`) that can:
   * Run models in parallel
   * Save results to different formats
 * Simulation configuration files 
 * A command line interface (`soil`), to quickly run simulations with different parameters
 * An integrated debugger (`soil --debug`) with custom functions to print agent states and break at specific states
 
-
 ## Mesa compatibility
 
 SOIL has been redesigned to integrate well with [Mesa](https://github.com/projectmesa/mesa).
 For instance, it should be possible to run a `mesa.Model` models using a `soil.Simulation` and the `soil` CLI, or to integrate the `soil.TimedActivation` scheduler on a `mesa.Model`.
 
 Note that some combinations of `mesa` and `soil` components, while technically possible, are much less useful or might yield surprising results.
 For instance, you may add any `soil.agent` agent on a regular `mesa.Model` with a vanilla scheduler from `mesa.time`.
```

### Comparing `soil-1.0.0rc1/setup.py` & `soil-1.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/.analysis.py.~undo-tree~` & `soil-1.0.0rc2/soil/.analysis.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/.environment.py.~undo-tree~` & `soil-1.0.0rc2/soil/.environment.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/.exporters.py.~undo-tree~` & `soil-1.0.0rc2/soil/.exporters.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/.serialization.py.~undo-tree~` & `soil-1.0.0rc2/soil/.serialization.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/.simulation.py.~undo-tree~` & `soil-1.0.0rc2/soil/.simulation.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/.stats.py.~undo-tree~` & `soil-1.0.0rc2/soil/.stats.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/.time.py.~undo-tree~` & `soil-1.0.0rc2/soil/.time.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/__init__.py` & `soil-1.0.0rc2/soil/__init__.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/.__init__.py.~undo-tree~` & `soil-1.0.0rc2/soil/agents/.__init__.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/.fsm.py.~undo-tree~` & `soil-1.0.0rc2/soil/agents/.fsm.py.~undo-tree~`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/BassModel.py` & `soil-1.0.0rc2/soil/agents/BassModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/CounterModel.py` & `soil-1.0.0rc2/soil/agents/CounterModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/Geo.py` & `soil-1.0.0rc2/soil/agents/Geo.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/IndependentCascadeModel.py` & `soil-1.0.0rc2/soil/agents/IndependentCascadeModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/SISaModel.py` & `soil-1.0.0rc2/soil/agents/SISaModel.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/__init__.py` & `soil-1.0.0rc2/soil/agents/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             ):
                 new_nmspc[attr] = func
             elif attr == "defaults":
                 defaults.update(func)
             else:
                 defaults[attr] = copy(func)
 
-        return super().__new__(mcls=mcls, name=name, bases=bases, namespace=new_nmspc)
+        return super().__new__(mcls, name, bases, new_nmspc)
 
 
 class BaseAgent(MesaAgent, MutableMapping, metaclass=MetaAgent):
     """
     A special type of Mesa Agent that:
 
     * Can be used as a dictionary to access its state.
```

### Comparing `soil-1.0.0rc1/soil/agents/evented.py` & `soil-1.0.0rc2/soil/agents/evented.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/fsm.py` & `soil-1.0.0rc2/soil/agents/fsm.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/agents/network_agents.py` & `soil-1.0.0rc2/soil/agents/network_agents.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/analysis.py` & `soil-1.0.0rc2/soil/analysis.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/datacollection.py` & `soil-1.0.0rc2/soil/datacollection.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/debugging.py` & `soil-1.0.0rc2/soil/debugging.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/environment.py` & `soil-1.0.0rc2/soil/environment.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/events.py` & `soil-1.0.0rc2/soil/events.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/exporters.py` & `soil-1.0.0rc2/soil/exporters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/network.py` & `soil-1.0.0rc2/soil/network.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/parameters.py` & `soil-1.0.0rc2/soil/parameters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/serialization.py` & `soil-1.0.0rc2/soil/serialization.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/simulation.py` & `soil-1.0.0rc2/soil/simulation.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/time.py` & `soil-1.0.0rc2/soil/time.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/utils.py` & `soil-1.0.0rc2/soil/utils.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/README.md` & `soil-1.0.0rc2/soil/web/README.md`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/__init__.py` & `soil-1.0.0rc2/soil/web/__init__.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/config.yml` & `soil-1.0.0rc2/soil/web/config.yml`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/run.py` & `soil-1.0.0rc2/soil/web/run.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/css/main.css` & `soil-1.0.0rc2/soil/web/static/css/main.css`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/css/timeline.css` & `soil-1.0.0rc2/soil/web/static/css/timeline.css`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/img/logo_gsi.svg` & `soil-1.0.0rc2/soil/web/static/img/logo_gsi.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/img/logo_soil.png` & `soil-1.0.0rc2/soil/web/static/img/logo_soil.png`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/img/svg/person.svg` & `soil-1.0.0rc2/soil/web/static/img/svg/person.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/img/svg/plus.svg` & `soil-1.0.0rc2/soil/web/static/img/svg/plus.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/img/svg/target.svg` & `soil-1.0.0rc2/soil/web/static/img/svg/target.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/img/svg/time.svg` & `soil-1.0.0rc2/soil/web/static/img/svg/time.svg`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/js/socket.js` & `soil-1.0.0rc2/soil/web/static/js/socket.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/js/template.js` & `soil-1.0.0rc2/soil/web/static/js/template.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/js/timeline.js` & `soil-1.0.0rc2/soil/web/static/js/timeline.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/static/js/visualization.js` & `soil-1.0.0rc2/soil/web/static/js/visualization.js`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil/web/templates/index.html` & `soil-1.0.0rc2/soil/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/soil.egg-info/PKG-INFO` & `soil-1.0.0rc2/soil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soil
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: An Agent-Based Social Simulator for Social Networks
 Home-page: https://github.com/gsi-upm/soil
-Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc1.tar.gz
+Download-URL: https://github.com/gsi-upm/soil/archive/1.0.0rc2.tar.gz
 Author: J. Fernando Sanchez
 Author-email: jf.sanchez@upm.es
 Keywords: agent,social,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
@@ -61,15 +61,14 @@
 * A simulation runner (`soil.Simulation`) that can:
   * Run models in parallel
   * Save results to different formats
 * Simulation configuration files 
 * A command line interface (`soil`), to quickly run simulations with different parameters
 * An integrated debugger (`soil --debug`) with custom functions to print agent states and break at specific states
 
-
 ## Mesa compatibility
 
 SOIL has been redesigned to integrate well with [Mesa](https://github.com/projectmesa/mesa).
 For instance, it should be possible to run a `mesa.Model` models using a `soil.Simulation` and the `soil` CLI, or to integrate the `soil.TimedActivation` scheduler on a `mesa.Model`.
 
 Note that some combinations of `mesa` and `soil` components, while technically possible, are much less useful or might yield surprising results.
 For instance, you may add any `soil.agent` agent on a regular `mesa.Model` with a vanilla scheduler from `mesa.time`.
```

### Comparing `soil-1.0.0rc1/soil.egg-info/SOURCES.txt` & `soil-1.0.0rc2/soil.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -58,16 +58,14 @@
 soil/web/__main__.py
 soil/web/config.yml
 soil/web/run.py
 soil/web/static/css/main.css
 soil/web/static/css/timeline.css
 soil/web/static/img/logo_gsi.svg
 soil/web/static/img/logo_soil.png
-soil/web/static/img/background/map.png
-soil/web/static/img/background/map_4800x2860.jpg
 soil/web/static/img/svg/home.svg
 soil/web/static/img/svg/person.svg
 soil/web/static/img/svg/plus.svg
 soil/web/static/img/svg/target.svg
 soil/web/static/img/svg/time.svg
 soil/web/static/js/socket.js
 soil/web/static/js/template.js
```

### Comparing `soil-1.0.0rc1/tests/test_agents.py` & `soil-1.0.0rc2/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/tests/test_config.py` & `soil-1.0.0rc2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/tests/test_examples.py` & `soil-1.0.0rc2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/tests/test_exporters.py` & `soil-1.0.0rc2/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/tests/test_main.py` & `soil-1.0.0rc2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/tests/test_mesa.py` & `soil-1.0.0rc2/tests/test_mesa.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/tests/test_network.py` & `soil-1.0.0rc2/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `soil-1.0.0rc1/tests/test_time.py` & `soil-1.0.0rc2/tests/test_time.py`

 * *Files identical despite different names*

