# Comparing `tmp/snews_pt-1.3.1.dev1.tar.gz` & `tmp/snews_pt-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snews_pt-1.3.1.dev1.tar", last modified: Mon Feb  6 13:14:24 2023, max compression
+gzip compressed data, was "/mnt/c/Users/bj7780/Desktop/Kara/GitHub/SNEWS/SNEWS_Publishing_Tools/dist/.tmp-kc52we8s/snews_pt-1.3.2.tar", last modified: Fri Apr 21 11:57:32 2023, max compression
```

## Comparing `snews_pt-1.3.1.dev1.tar` & `snews_pt-1.3.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:24.156827 snews_pt-1.3.1.dev1/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:22.233404 snews_pt-1.3.1.dev1/.github/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:22.603517 snews_pt-1.3.1.dev1/.github/workflows/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/.github/workflows/mac10-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/.github/workflows/mac10-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1877 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/.github/workflows/mac11-py310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/.github/workflows/mac11-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/.github/workflows/mac11-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1817 2022-07-29 18:24:09.000000 snews_pt-1.3.1.dev1/.github/workflows/mac11-py39.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2367 2023-02-06 12:44:04.000000 snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2135 2023-02-06 12:44:04.000000 snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py37-310.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py37.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py38.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2090 2023-02-06 12:44:04.000000 snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py39.yml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      178 2022-05-20 14:39:26.000000 snews_pt-1.3.1.dev1/.readthedocs.yaml
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      436 2023-02-06 13:14:19.000000 snews_pt-1.3.1.dev1/AUTHORS
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    16208 2023-02-06 13:14:18.000000 snews_pt-1.3.1.dev1/ChangeLog
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10042 2023-02-06 13:14:24.156827 snews_pt-1.3.1.dev1/PKG-INFO
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9034 2022-09-27 15:09:46.000000 snews_pt-1.3.1.dev1/README.md
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:22.760373 snews_pt-1.3.1.dev1/docs/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      623 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/docs/Makefile
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      205 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/docs/README.md
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:22.240923 snews_pt-1.3.1.dev1/docs/_static/
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:22.793148 snews_pt-1.3.1.dev1/docs/_static/css/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      616 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/docs/_static/css/my_theme.css
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:22.807661 snews_pt-1.3.1.dev1/docs/_templates/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       60 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/docs/_templates/layout.html
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:22.964502 snews_pt-1.3.1.dev1/docs/api/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      148 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/docs/api/api.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      129 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/docs/api/message_schema.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      123 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/docs/api/snews_pt_utils.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      111 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/docs/api/snews_pub.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      114 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/docs/api/snews_sub.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6080 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/docs/cli_docs.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      535 2022-05-20 12:43:48.000000 snews_pt-1.3.1.dev1/docs/cli_help.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4472 2022-09-27 15:04:20.000000 snews_pt-1.3.1.dev1/docs/conf.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   139863 2022-04-28 07:02:44.000000 snews_pt-1.3.1.dev1/docs/custom_logo.png
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      408 2022-09-27 15:01:02.000000 snews_pt-1.3.1.dev1/docs/index.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    17706 2022-05-20 12:43:49.000000 snews_pt-1.3.1.dev1/docs/snews_logo.png
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1107 2022-05-20 12:43:49.000000 snews_pt-1.3.1.dev1/docs/subscribed_messages.json
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:23.152827 snews_pt-1.3.1.dev1/docs/user/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      258 2022-05-20 12:43:49.000000 snews_pt-1.3.1.dev1/docs/user/architecture.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5119 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/docs/user/command_line_interface.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4242 2022-09-29 07:36:14.000000 snews_pt-1.3.1.dev1/docs/user/firedrills.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      840 2022-05-20 12:43:49.000000 snews_pt-1.3.1.dev1/docs/user/installation.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1603 2023-02-06 12:44:04.000000 snews_pt-1.3.1.dev1/docs/user/message_schema.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1259 2022-05-20 12:43:49.000000 snews_pt-1.3.1.dev1/docs/user/protocol.rst
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1258 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/docs/user/publishing_protocols.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     8746 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/docs/user/quickstart.md
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4786 2022-12-01 10:17:24.000000 snews_pt-1.3.1.dev1/examples.ipynb
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    19290 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/firedrill.ipynb
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   108013 2022-05-20 12:43:49.000000 snews_pt-1.3.1.dev1/img.png
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:23.185084 snews_pt-1.3.1.dev1/logs/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        2 2022-08-01 20:52:31.000000 snews_pt-1.3.1.dev1/logs/.gitignore
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      440 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/requirements.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      169 2023-02-06 13:14:24.172454 snews_pt-1.3.1.dev1/setup.cfg
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2419 2023-02-06 13:05:49.000000 snews_pt-1.3.1.dev1/setup.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:23.419453 snews_pt-1.3.1.dev1/snews_pt/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      747 2022-09-27 12:03:30.000000 snews_pt-1.3.1.dev1/snews_pt/__init__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9762 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/__main__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       19 2022-11-18 16:58:48.000000 snews_pt-1.3.1.dev1/snews_pt/_version.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:23.748945 snews_pt-1.3.1.dev1/snews_pt/auxiliary/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1523 2022-05-20 13:27:18.000000 snews_pt-1.3.1.dev1/snews_pt/auxiliary/custom_script.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1565 2022-11-18 16:58:48.000000 snews_pt-1.3.1.dev1/snews_pt/auxiliary/detector_properties.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2431 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/auxiliary/make_scenarios.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3539 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/auxiliary/scenarios.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      528 2023-02-06 09:56:27.000000 snews_pt-1.3.1.dev1/snews_pt/auxiliary/test-config.env
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2099 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/auxiliary/try_scenarios.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:23.796217 snews_pt-1.3.1.dev1/snews_pt/core/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2022-09-27 12:03:31.000000 snews_pt-1.3.1.dev1/snews_pt/core/__init__.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1314 2022-09-27 12:03:31.000000 snews_pt-1.3.1.dev1/snews_pt/core/logging.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4067 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/message_schema.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5750 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/remote_commands.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9163 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/snews_format_checker.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    12129 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/snews_pt_utils.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9097 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/snews_pub.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4736 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/snews_sub.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:24.125581 snews_pt-1.3.1.dev1/snews_pt/test/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      272 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/test/example_coincidence_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      483 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/test/example_combined_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      182 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/test/example_heartbeat_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      318 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/test/example_significance_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      328 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/test/example_timing_tier_message.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1161 2022-05-20 13:27:19.000000 snews_pt-1.3.1.dev1/snews_pt/test/random_plugin.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1709 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/test/test_coincidence_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      239 2022-05-20 13:27:19.000000 snews_pt-1.3.1.dev1/snews_pt/test/test_install.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1705 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/test/test_old_crashes.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      842 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/test/test_plugin.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1288 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/test/test_retraction.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2437 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/test/test_significance_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      643 2022-11-18 16:58:49.000000 snews_pt-1.3.1.dev1/snews_pt/test/test_subscribe.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1840 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/test/test_timing_tier.py
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3894 2023-02-06 12:44:05.000000 snews_pt-1.3.1.dev1/snews_pt/tier_decider.py
-drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-02-06 13:14:23.607892 snews_pt-1.3.1.dev1/snews_pt.egg-info/
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10042 2023-02-06 13:14:19.000000 snews_pt-1.3.1.dev1/snews_pt.egg-info/PKG-INFO
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2398 2023-02-06 13:14:22.000000 snews_pt-1.3.1.dev1/snews_pt.egg-info/SOURCES.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2023-02-06 13:14:19.000000 snews_pt-1.3.1.dev1/snews_pt.egg-info/dependency_links.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       52 2023-02-06 13:14:19.000000 snews_pt-1.3.1.dev1/snews_pt.egg-info/entry_points.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2022-05-20 13:36:30.000000 snews_pt-1.3.1.dev1/snews_pt.egg-info/not-zip-safe
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       47 2023-02-06 13:14:19.000000 snews_pt-1.3.1.dev1/snews_pt.egg-info/pbr.json
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      417 2023-02-06 13:14:19.000000 snews_pt-1.3.1.dev1/snews_pt.egg-info/requires.txt
--rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        9 2023-02-06 13:14:19.000000 snews_pt-1.3.1.dev1/snews_pt.egg-info/top_level.txt
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:32.000000 snews_pt-1.3.2/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:30.000000 snews_pt-1.3.2/.github/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:30.000000 snews_pt-1.3.2/.github/workflows/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac10-py37.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1878 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac10-py38.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1877 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac11-py310.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac11-py37.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1875 2022-05-20 12:43:48.000000 snews_pt-1.3.2/.github/workflows/mac11-py38.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1817 2022-07-29 18:24:09.000000 snews_pt-1.3.2/.github/workflows/mac11-py39.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2367 2023-02-06 12:44:04.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py310.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2135 2023-02-06 12:44:04.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py37-310.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py37.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2378 2022-05-20 13:27:18.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py38.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2090 2023-02-06 12:44:04.000000 snews_pt-1.3.2/.github/workflows/ubuntu20-py39.yml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      178 2022-05-20 14:39:26.000000 snews_pt-1.3.2/.readthedocs.yaml
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      436 2023-04-21 11:57:26.000000 snews_pt-1.3.2/AUTHORS
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    16863 2023-04-21 11:57:25.000000 snews_pt-1.3.2/ChangeLog
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10037 2023-04-21 11:57:32.000000 snews_pt-1.3.2/PKG-INFO
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9034 2022-09-27 15:09:46.000000 snews_pt-1.3.2/README.md
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:30.000000 snews_pt-1.3.2/docs/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      623 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/Makefile
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      205 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/README.md
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:30.000000 snews_pt-1.3.2/docs/_static/
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/docs/_static/css/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      616 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/_static/css/my_theme.css
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/docs/_templates/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       60 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/_templates/layout.html
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/docs/api/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      148 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/api/api.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      129 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/api/message_schema.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      123 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/api/snews_pt_utils.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      111 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/api/snews_pub.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      114 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/api/snews_sub.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6080 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/cli_docs.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      535 2022-05-20 12:43:48.000000 snews_pt-1.3.2/docs/cli_help.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4472 2022-09-27 15:04:20.000000 snews_pt-1.3.2/docs/conf.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   139863 2022-04-28 07:02:44.000000 snews_pt-1.3.2/docs/custom_logo.png
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      408 2022-09-27 15:01:02.000000 snews_pt-1.3.2/docs/index.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    17706 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/snews_logo.png
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1107 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/subscribed_messages.json
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/docs/user/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      258 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/user/architecture.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5119 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/user/command_line_interface.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4242 2022-09-29 07:36:14.000000 snews_pt-1.3.2/docs/user/firedrills.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      840 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/user/installation.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1603 2023-03-30 14:38:00.000000 snews_pt-1.3.2/docs/user/message_schema.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1259 2022-05-20 12:43:49.000000 snews_pt-1.3.2/docs/user/protocol.rst
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1258 2023-03-30 14:38:00.000000 snews_pt-1.3.2/docs/user/publishing_protocols.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     8746 2022-05-20 13:27:18.000000 snews_pt-1.3.2/docs/user/quickstart.md
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4786 2022-12-01 10:17:24.000000 snews_pt-1.3.2/examples.ipynb
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    19290 2023-03-30 14:38:00.000000 snews_pt-1.3.2/firedrill.ipynb
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)   108013 2022-05-20 12:43:49.000000 snews_pt-1.3.2/img.png
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/logs/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        2 2022-08-01 20:52:31.000000 snews_pt-1.3.2/logs/.gitignore
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      440 2023-04-21 11:47:54.000000 snews_pt-1.3.2/requirements.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      169 2023-04-21 11:57:32.000000 snews_pt-1.3.2/setup.cfg
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2419 2023-03-30 14:38:00.000000 snews_pt-1.3.2/setup.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/snews_pt/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      747 2022-09-27 12:03:30.000000 snews_pt-1.3.2/snews_pt/__init__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9762 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/__main__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       19 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/_version.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:32.000000 snews_pt-1.3.2/snews_pt/auxiliary/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1523 2022-05-20 13:27:18.000000 snews_pt-1.3.2/snews_pt/auxiliary/custom_script.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1565 2022-11-18 16:58:48.000000 snews_pt-1.3.2/snews_pt/auxiliary/detector_properties.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2435 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/auxiliary/make_scenarios.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3543 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/auxiliary/scenarios.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      616 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/auxiliary/test-config.env
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2267 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/auxiliary/try_scenarios.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:32.000000 snews_pt-1.3.2/snews_pt/core/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2022-09-27 12:03:31.000000 snews_pt-1.3.2/snews_pt/core/__init__.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1314 2022-09-27 12:03:31.000000 snews_pt-1.3.2/snews_pt/core/logging.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     4011 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/message_schema.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     6196 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/remote_commands.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9366 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/snews_format_checker.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    11921 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/snews_pt_utils.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     9081 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/snews_pub.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     5042 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/snews_sub.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:32.000000 snews_pt-1.3.2/snews_pt/test/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      272 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_coincidence_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      483 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_combined_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      182 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_heartbeat_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      318 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_significance_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      328 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/example_timing_tier_message.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1161 2022-05-20 13:27:19.000000 snews_pt-1.3.2/snews_pt/test/random_plugin.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1689 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/test/test_coincidence_tier.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      239 2022-05-20 13:27:19.000000 snews_pt-1.3.2/snews_pt/test/test_install.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1705 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/test_old_crashes.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      842 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/test_plugin.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1288 2023-03-30 14:38:00.000000 snews_pt-1.3.2/snews_pt/test/test_retraction.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2384 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/test/test_significance_tier.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      643 2022-11-18 16:58:49.000000 snews_pt-1.3.2/snews_pt/test/test_subscribe.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     1820 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/test/test_timing_tier.py
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     3880 2023-04-21 11:47:54.000000 snews_pt-1.3.2/snews_pt/tier_decider.py
+drwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        0 2023-04-21 11:57:31.000000 snews_pt-1.3.2/snews_pt.egg-info/
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)    10037 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/PKG-INFO
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)     2398 2023-04-21 11:57:30.000000 snews_pt-1.3.2/snews_pt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       52 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/entry_points.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        1 2022-05-20 13:36:30.000000 snews_pt-1.3.2/snews_pt.egg-info/not-zip-safe
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)       47 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/pbr.json
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)      417 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/requires.txt
+-rwxrwxrwx   0 kara-unix  (1000) kara-unix  (1000)        9 2023-04-21 11:57:27.000000 snews_pt-1.3.2/snews_pt.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/mac10-py37.yml` & `snews_pt-1.3.2/.github/workflows/mac10-py37.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/mac10-py38.yml` & `snews_pt-1.3.2/.github/workflows/mac10-py38.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/mac11-py310.yml` & `snews_pt-1.3.2/.github/workflows/mac11-py310.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/mac11-py37.yml` & `snews_pt-1.3.2/.github/workflows/mac11-py37.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/mac11-py38.yml` & `snews_pt-1.3.2/.github/workflows/mac11-py38.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/mac11-py39.yml` & `snews_pt-1.3.2/.github/workflows/mac11-py39.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py310.yml` & `snews_pt-1.3.2/.github/workflows/ubuntu20-py310.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py37-310.yml` & `snews_pt-1.3.2/.github/workflows/ubuntu20-py37-310.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py37.yml` & `snews_pt-1.3.2/.github/workflows/ubuntu20-py37.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py38.yml` & `snews_pt-1.3.2/.github/workflows/ubuntu20-py38.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/.github/workflows/ubuntu20-py39.yml` & `snews_pt-1.3.2/.github/workflows/ubuntu20-py39.yml`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/ChangeLog` & `snews_pt-1.3.2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,35 @@
 CHANGES
 =======
 
+v1.3.2
+------
+
+* Update snews\_sub.py
+* add correct topic
+* add correct topic
+* add write hb logs command
+* raise error if not hop0.8.0
+* add connection topic
+* remove redundant whcih tier
+* remove redundant whcih tier
+* change requirements to hop-client v0.8.0
+* change version for hop-client 0.8.0
+* change messaging to hop-client v0.8.0 syntax only
+* put JSONBlob import in try/except, add hop8 flag
+* replace try/except with if isinstance(JSONBlob)
+* add try, except blocks for hop-0.8.0 messages
+* update requirements for new hop-client version
+* write messages to stream as JSONBlob, hop>=0.6.0
+* fix test-connection
+* testing fixes
+
+v1.3.1
+------
+
 * stamp time before sending
 
 v1.3.0
 ------
 
 * stamp time before sending
 * check if detector name valid
```

### Comparing `snews_pt-1.3.1.dev1/PKG-INFO` & `snews_pt-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snews_pt
-Version: 1.3.1.dev1
+Version: 1.3.2
 Summary: An alert application for observing supernovas.
 Home-page: https://github.com/SNEWS2/SNEWS_Publishing_Tools
 Author: Sebastian Torres-Lara, Melih Kara
 Author-email: sebastiantorreslara17@gmail.com, karamel.itu@gmail.com
 License: BSD 3-Clause
 Keywords: setup,distutils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `snews_pt-1.3.1.dev1/README.md` & `snews_pt-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/Makefile` & `snews_pt-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/_static/css/my_theme.css` & `snews_pt-1.3.2/docs/_static/css/my_theme.css`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/cli_docs.md` & `snews_pt-1.3.2/docs/cli_docs.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/cli_help.txt` & `snews_pt-1.3.2/docs/cli_help.txt`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/conf.py` & `snews_pt-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/custom_logo.png` & `snews_pt-1.3.2/docs/custom_logo.png`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/snews_logo.png` & `snews_pt-1.3.2/docs/snews_logo.png`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/subscribed_messages.json` & `snews_pt-1.3.2/docs/subscribed_messages.json`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/user/command_line_interface.md` & `snews_pt-1.3.2/docs/user/command_line_interface.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/user/firedrills.md` & `snews_pt-1.3.2/docs/user/firedrills.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/user/installation.rst` & `snews_pt-1.3.2/docs/user/installation.rst`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/user/message_schema.md` & `snews_pt-1.3.2/docs/user/message_schema.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/user/protocol.rst` & `snews_pt-1.3.2/docs/user/protocol.rst`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/user/publishing_protocols.md` & `snews_pt-1.3.2/docs/user/publishing_protocols.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/docs/user/quickstart.md` & `snews_pt-1.3.2/docs/user/quickstart.md`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/examples.ipynb` & `snews_pt-1.3.2/examples.ipynb`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/firedrill.ipynb` & `snews_pt-1.3.2/firedrill.ipynb`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/img.png` & `snews_pt-1.3.2/img.png`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/setup.py` & `snews_pt-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/__init__.py` & `snews_pt-1.3.2/snews_pt/__init__.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/__main__.py` & `snews_pt-1.3.2/snews_pt/__main__.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/auxiliary/custom_script.py` & `snews_pt-1.3.2/snews_pt/auxiliary/custom_script.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/auxiliary/detector_properties.json` & `snews_pt-1.3.2/snews_pt/auxiliary/detector_properties.json`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/auxiliary/make_scenarios.py` & `snews_pt-1.3.2/snews_pt/auxiliary/make_scenarios.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 ####
 msg7 = {"detector_name": "Borexino",
         "neutrino_time": "2030-01-01T12:30:10.678999",
         "p_val": 0.98,
         "is_test":True}
 
-msg8 = {"detector_name": "ICE",
+msg8 = {"detector_name": "IceCube",
         "neutrino_time": "2030-01-01T12:30:19.678999",
         "p_val": 0.98,
         "is_test":True}
 
 msg9 = {"detector_name": "NOvA",
         "neutrino_time": "2030-01-01T12:30:21.678999",
         "p_val": 0.98,
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/auxiliary/scenarios.json` & `snews_pt-1.3.2/snews_pt/auxiliary/scenarios.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987244897959184%*

 * *Differences: {"'msgs at 10, 19, 21, 22, 20, 29, 18 seconds'": "{1: {'detector_name': 'IceCube'}}"}*

```diff
@@ -37,15 +37,15 @@
         {
             "detector_name": "Borexino",
             "is_test": true,
             "neutrino_time": "2030-01-01T12:30:10.678999",
             "p_val": 0.98
         },
         {
-            "detector_name": "ICE",
+            "detector_name": "IceCube",
             "is_test": true,
             "neutrino_time": "2030-01-01T12:30:19.678999",
             "p_val": 0.98
         },
         {
             "detector_name": "NOvA",
             "is_test": true,
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/auxiliary/test-config.env` & `snews_pt-1.3.2/snews_pt/auxiliary/test-config.env`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-DETECTOR_NAME='XENONnT'
-HAS_NAME_CHANGED='1'
-ADMIN_PASS='very1secret2password'
-
-DATABASE_SERVER=""
-LOCAL_SERVER="mongodb://localhost:27017"
-ALERT_OUTPUT="SNEWS_ALERTS/"
-
-NEW_DATABASE=0
-COINCIDENCE_THRESHOLD=10
-MSG_EXPIRATION=120
-
-HOP_BROKER="kafka.scimma.org"
-
-OBSERVATION_TOPIC="kafka://${HOP_BROKER}/snews.experiments-test"
-ALERT_TOPIC="kafka://${HOP_BROKER}/snews.alert-test"
-
-FIREDRILL_OBSERVATION_TOPIC="kafka://${HOP_BROKER}/snews.experiments-firedrill"
-FIREDRILL_ALERT_TOPIC="kafka://${HOP_BROKER}/snews.alert-firedrill"
+DETECTOR_NAME='TEST'
+HAS_NAME_CHANGED='0'
+ADMIN_PASS='very1secret2password'
+
+DATABASE_SERVER=""
+LOCAL_SERVER="mongodb://localhost:27017"
+ALERT_OUTPUT="SNEWS_ALERTS/"
+
+NEW_DATABASE=0
+COINCIDENCE_THRESHOLD=10
+MSG_EXPIRATION=120
+
+HOP_BROKER="kafka.scimma.org"
+
+OBSERVATION_TOPIC="kafka://${HOP_BROKER}/snews.experiments-test"
+ALERT_TOPIC="kafka://${HOP_BROKER}/snews.alert-test"
+
+FIREDRILL_OBSERVATION_TOPIC="kafka://${HOP_BROKER}/snews.experiments-firedrill"
+FIREDRILL_ALERT_TOPIC="kafka://${HOP_BROKER}/snews.alert-firedrill"
+CONNECTION_TEST_TOPIC="kafka://${HOP_BROKER}/snews.connection-testing"
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/auxiliary/try_scenarios.py` & `snews_pt-1.3.2/snews_pt/auxiliary/try_scenarios.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,64 +69,74 @@
 00000440: 7465 7374 2d62 726f 6b65 7220 2f20 7465  test-broker / te
 00000450: 7374 2d63 6163 6865 0d0a 2020 2020 2020  st-cache..      
 00000460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000470: 2020 7075 622e 7365 6e64 285b 7b27 5f69    pub.send([{'_i
 00000480: 6427 3a20 2730 5f68 6172 642d 7265 7365  d': '0_hard-rese
 00000490: 745f 272c 2027 7061 7373 273a 2027 7665  t_', 'pass': 've
 000004a0: 7279 3173 6563 7265 7432 7061 7373 776f  ry1secret2passwo
-000004b0: 7264 277d 5d29 0d0a 2020 2020 2020 2020  rd'}])..        
-000004c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004d0: 7072 696e 7428 273e 2043 6163 6865 2063  print('> Cache c
-000004e0: 6c65 616e 6564 5c6e 2729 0d0a 2020 2020  leaned\n')..    
-000004f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00000500: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000510: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-00000520: 686f 2866 225c 6e3e 3e3e 2054 6573 7469  ho(f"\n>>> Testi
-00000530: 6e67 207b 7363 656e 6172 696f 7d22 2c20  ng {scenario}", 
-00000540: 6667 3d27 7965 6c6c 6f77 272c 2062 6f6c  fg='yellow', bol
-00000550: 643d 5472 7565 290d 0a20 2020 2020 2020  d=True)..       
-00000560: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00000570: 7361 6765 7320 3d20 6461 7461 5b73 6365  sages = data[sce
-00000580: 6e61 7269 6f5d 0d0a 2020 2020 2020 2020  nario]..        
-00000590: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000005a0: 6d73 6720 696e 206d 6573 7361 6765 733a  msg in messages:
-000005b0: 2023 2073 656e 6420 6f6e 6520 6279 206f   # send one by o
-000005c0: 6e65 2061 6e64 2073 6c65 6570 2069 6e20  ne and sleep in 
-000005d0: 6265 7477 6565 6e0d 0a20 2020 2020 2020  between..       
-000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005f0: 2053 4e45 5753 5469 6572 7350 7562 6c69   SNEWSTiersPubli
-00000600: 7368 6572 282a 2a6d 7367 2c20 6669 7265  sher(**msg, fire
-00000610: 6472 696c 6c5f 6d6f 6465 3d66 645f 6d6f  drill_mode=fd_mo
-00000620: 6465 292e 7365 6e64 5f74 6f5f 736e 6577  de).send_to_snew
-00000630: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
-00000640: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00000650: 652e 736c 6565 7028 3129 0d0a 2020 2020  e.sleep(1)..    
-00000660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000670: 2020 2020 2320 636c 6561 7220 6361 6368      # clear cach
-00000680: 6520 6166 7465 7220 6561 6368 2073 6365  e after each sce
-00000690: 6e61 7269 6f0d 0a20 2020 2020 2020 2020  nario..         
-000006a0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-000006b0: 5075 626c 6973 6865 7228 6669 7265 6472  Publisher(firedr
-000006c0: 696c 6c5f 6d6f 6465 3d66 645f 6d6f 6465  ill_mode=fd_mode
-000006d0: 2c20 7665 7262 6f73 653d 4661 6c73 6529  , verbose=False)
-000006e0: 2061 7320 7075 623a 0d0a 2020 2020 2020   as pub:..      
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2020 7075 622e 7365 6e64 285b 7b27 5f69    pub.send([{'_i
-00000710: 6427 3a20 2730 5f68 6172 642d 7265 7365  d': '0_hard-rese
-00000720: 745f 272c 2027 7061 7373 273a 2776 6572  t_', 'pass':'ver
-00000730: 7931 7365 6372 6574 3270 6173 7377 6f72  y1secret2passwor
-00000740: 6427 2c20 2764 6574 6563 746f 725f 6e61  d', 'detector_na
-00000750: 6d65 273a 2754 4553 5427 7d5d 290d 0a20  me':'TEST'}]).. 
+000004b0: 7264 272c 2027 6465 7465 6374 6f72 5f6e  rd', 'detector_n
+000004c0: 616d 6527 3a27 5845 4e4f 4e6e 5427 2c0d  ame':'XENONnT',.
+000004d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004f0: 2020 2020 276d 6574 6127 3a7b 7d7d 5d29      'meta':{}}])
+00000500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000510: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00000520: 273e 2043 6163 6865 2063 6c65 616e 6564  '> Cache cleaned
+00000530: 5c6e 2729 0d0a 2020 2020 2020 2020 2020  \n')..          
+00000540: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000560: 2063 6c69 636b 2e73 6563 686f 2866 225c   click.secho(f"\
+00000570: 6e3e 3e3e 2054 6573 7469 6e67 207b 7363  n>>> Testing {sc
+00000580: 656e 6172 696f 7d22 2c20 6667 3d27 7965  enario}", fg='ye
+00000590: 6c6c 6f77 272c 2062 6f6c 643d 5472 7565  llow', bold=True
+000005a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000005b0: 2020 2020 2020 206d 6573 7361 6765 7320         messages 
+000005c0: 3d20 6461 7461 5b73 6365 6e61 7269 6f5d  = data[scenario]
+000005d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000005e0: 2020 2020 2020 666f 7220 6d73 6720 696e        for msg in
+000005f0: 206d 6573 7361 6765 733a 2023 2073 656e   messages: # sen
+00000600: 6420 6f6e 6520 6279 206f 6e65 2061 6e64  d one by one and
+00000610: 2073 6c65 6570 2069 6e20 6265 7477 6565   sleep in betwee
+00000620: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00000630: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00000640: 286d 7367 2c20 225c 6e5c 6e22 290d 0a20  (msg, "\n\n").. 
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 2020 2020 2053 4e45 5753 5469 6572         SNEWSTier
+00000670: 7350 7562 6c69 7368 6572 282a 2a6d 7367  sPublisher(**msg
+00000680: 2c20 6669 7265 6472 696c 6c5f 6d6f 6465  , firedrill_mode
+00000690: 3d66 645f 6d6f 6465 292e 7365 6e64 5f74  =fd_mode).send_t
+000006a0: 6f5f 736e 6577 7328 290d 0a20 2020 2020  o_snews()..     
+000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006c0: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
+000006d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000006e0: 2020 2020 2020 2020 2020 2320 636c 6561            # clea
+000006f0: 7220 6361 6368 6520 6166 7465 7220 6561  r cache after ea
+00000700: 6368 2073 6365 6e61 7269 6f0d 0a20 2020  ch scenario..   
+00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000720: 2077 6974 6820 5075 626c 6973 6865 7228   with Publisher(
+00000730: 6669 7265 6472 696c 6c5f 6d6f 6465 3d66  firedrill_mode=f
+00000740: 645f 6d6f 6465 2c20 7665 7262 6f73 653d  d_mode, verbose=
+00000750: 4661 6c73 6529 2061 7320 7075 623a 0d0a  False) as pub:..
 00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000770: 2020 2020 2020 2070 7269 6e74 2827 3e20         print('> 
-00000780: 4361 6368 6520 636c 6561 6e65 645c 6e27  Cache cleaned\n'
-00000790: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
-000007a0: 7420 4b65 7962 6f61 7264 496e 7465 7272  t KeyboardInterr
-000007b0: 7570 743a 0d0a 2020 2020 2020 2020 2020  upt:..          
-000007c0: 2020 6272 6561 6b0d 0a65 7863 6570 7420    break..except 
-000007d0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-000007e0: 0a20 2020 2070 7269 6e74 2822 536f 6d65  .    print("Some
-000007f0: 7468 696e 6720 7765 6e74 2077 726f 6e67  thing went wrong
-00000800: 5c6e 222c 2065 2c20 225c 6e54 7279 206d  \n", e, "\nTry m
-00000810: 616e 7561 6c6c 7920 7375 626d 6974 7469  anually submitti
-00000820: 6e67 206d 6573 7361 6765 7320 3a2f 2229  ng messages :/")
-00000830: 0d0a 23                                  ..#
+00000770: 2020 2020 2020 2020 7075 622e 7365 6e64          pub.send
+00000780: 285b 7b27 5f69 6427 3a20 2730 5f68 6172  ([{'_id': '0_har
+00000790: 642d 7265 7365 745f 272c 2027 7061 7373  d-reset_', 'pass
+000007a0: 273a 2776 6572 7931 7365 6372 6574 3270  ':'very1secret2p
+000007b0: 6173 7377 6f72 6427 2c20 2764 6574 6563  assword', 'detec
+000007c0: 746f 725f 6e61 6d65 273a 2758 454e 4f4e  tor_name':'XENON
+000007d0: 6e54 272c 0d0a 2020 2020 2020 2020 2020  nT',..          
+000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007f0: 2020 2020 2020 2020 2027 6d65 7461 273a           'meta':
+00000800: 7b7d 7d5d 290d 0a20 2020 2020 2020 2020  {}}])..         
+00000810: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00000820: 7269 6e74 2827 3e20 4361 6368 6520 636c  rint('> Cache cl
+00000830: 6561 6e65 645c 6e27 290d 0a20 2020 2020  eaned\n')..     
+00000840: 2020 2065 7863 6570 7420 4b65 7962 6f61     except Keyboa
+00000850: 7264 496e 7465 7272 7570 743a 0d0a 2020  rdInterrupt:..  
+00000860: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
+00000870: 0a65 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
+00000880: 6e20 6173 2065 3a0d 0a20 2020 2070 7269  n as e:..    pri
+00000890: 6e74 2822 536f 6d65 7468 696e 6720 7765  nt("Something we
+000008a0: 6e74 2077 726f 6e67 5c6e 222c 2065 2c20  nt wrong\n", e, 
+000008b0: 225c 6e54 7279 206d 616e 7561 6c6c 7920  "\nTry manually 
+000008c0: 7375 626d 6974 7469 6e67 206d 6573 7361  submitting messa
+000008d0: 6765 7320 3a2f 2229 0d0a 23              ges :/")..#
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/core/logging.py` & `snews_pt-1.3.2/snews_pt/core/logging.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/message_schema.py` & `snews_pt-1.3.2/snews_pt/message_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,14 @@
 
         if tier == 'CoincidenceTier':
             message['neutrino_time'] = data['neutrino_time']
             message['p_val'] = data['p_val']
             message['meta'] = data['meta']
 
         if tier == 'Retraction':
-            message['which_tier'] = data['which_tier']
             message['retract_latest'] = data['retract_latest']
             message['retraction_reason'] = data['retraction_reason']
             message['meta'] = data['meta']
 
         # if len(data.keys()) > len(message.keys()):
         #     for key in data.keys():
         #         if key not in message.keys():
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/remote_commands.py` & `snews_pt-1.3.2/snews_pt/remote_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,31 +13,37 @@
     """ test the server connection
         It should prompt your whether the
         coincidence script is running in the server
         :param start_at: `negative int` the last N number of msg to check
         :param wait: `int` seconds to wait before terminating the check
     """
     detector_name = detector_name or os.getenv("DETECTOR_NAME")
+    default_connection_topic = "kafka://kafka.scimma.org/snews.connection-testing"
+    connection_broker = os.getenv("CONNECTION_TEST_TOPIC", default_connection_topic)
     stamp_time = datetime.utcnow().isoformat()
     message = {'_id': '0_test-connection',
                'detector_name': detector_name,
                'time': stamp_time,
                'status': 'sending',
                'meta':{}}
     if firedrill:
         topic = os.getenv("FIREDRILL_OBSERVATION_TOPIC")
     else:
         topic = os.getenv("OBSERVATION_TOPIC")
-    substream = Stream(until_eos=False, auth=True, start_at=start_at)
+
+    # substream = Stream(until_eos=False, auth=True, start_at=start_at) # when False, while loop doesn't break
+    substream = Stream(until_eos=True, auth=True, start_at=start_at)
     pubstream = Stream(until_eos=True, auth=True)
-    click.secho(f"\n> Testing your connection to {topic}. \n> Should take ~{wait} seconds...\n")
+    click.secho(f"\n> Testing your connection.\n> Sending to {topic}\n"
+                f"> Expecting from {connection_broker}. \n> Should take ~{wait} seconds...\n")
 
     start_time = datetime.utcnow()
     confirmed = False
-    with pubstream.open(topic, "w") as ps, substream.open(topic, "r") as ss:
+    # with pubstream.open(topic, "w") as ps, substream.open(topic, "r") as ss:
+    with pubstream.open(topic, "w") as ps, substream.open(connection_broker, "r") as ss:
         ps.write(message)
         while (datetime.utcnow() - start_time) < timedelta(seconds=wait):
             for read in ss:
                 message_expected = message.copy()
                 message_expected["status"] = "received"
                 if read == message_expected:
                     read_name = click.style(read['detector_name'], fg='green', bold=True)
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/snews_format_checker.py` & `snews_pt-1.3.2/snews_pt/snews_format_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             self.log.debug("*" * 40 + " END OF lOGS\n")
             return False
 
     def check_if_test(self):
         if "meta" in self.message_keys:
             if "is_test" in self.message['meta'].keys():
                 return self.message["meta"]["is_test"]
+        return False
 
     def check_id(self):
         """ check if the format is correct
             snews_pt sends messages in mongodb format
             which HAS TO contain an _id field
         """
         self.log.debug(f"\t> Checking _id ..")
@@ -115,14 +116,18 @@
         elif 'Heartbeat' in self.message['_id']:
             self.log.debug("\t> Heartbeat Passed. Checking time and status.")
             if not self.check_detector_status(): # if detector_status does not exist, return False
                 self.log.error("\t> Heartbeat not valid!")
                 return False
             self.bypass = True
 
+        elif "display-heartbeats" in self.message['_id']:
+            self.log.debug(f"\t> display-heartbeat is passed. Skipping format check.")
+            self.bypass = True
+
         elif [i in self.message['_id'] for i in ['TimeTier', 'SigTier', 'CoincidenceTier']]:
             self.log.debug(f"\t> Tier message Passed. Checking times.")
 
         else:
             self.log.error(f"\t> Unknown id Passed : {self.message['_id']}.")
             return False
         self.log.info(f"\t> Message type : {self.message['_id']} valid.")
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/snews_pt_utils.py` & `snews_pt-1.3.2/snews_pt/snews_pt_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,24 +184,21 @@
     keys = ['machine_time', 'neutrino_time', 'timing_series', 'p_val', 'meta']
     values = [machine_time, neutrino_time, timing_series, p_val, meta]
     zip_iterator = zip(keys, values)
     time_tier_dict = dict(zip_iterator)
     return time_tier_dict
 
 
-def retraction_data(machine_time=None, which_tier=None,
-                    retract_latest=0, retraction_reason=None, meta=None):
+def retraction_data(machine_time=None, retract_latest=0, retraction_reason=None, meta=None):
     """ Formats data for Retraction as dict object
 
         Parameters
         ----------
         machine_time : `str`
             The machine time at the time of execution of command
-        which_tier : 'str'
-            OBS type of false message ['CoincidenceTier', 'SigTier', 'TimeTier, 'ALL']
         retract_latest: 'int' or 'str'
             Tells retraction methods to look for N  latest message sent by a detector. can also pass 'ALL'
             to retract all messages in a OBS tier.
         retraction_reason: 'str"
             Reason for message(s) retraction
        meta : `dict`
             Any other key-value pair desired to be published.
@@ -209,18 +206,16 @@
 
         Returns
         -------
             retraction_dict : `dict`
                 dictionary of the retraction data
 
     """
-    keys = ['machine_time',
-            'retract_latest', 'which_tier', 'retraction_reason', 'meta']
-    values = [machine_time, retract_latest,
-              which_tier, retraction_reason, meta]
+    keys = ['machine_time', 'retract_latest', 'retraction_reason', 'meta']
+    values = [machine_time, retract_latest, retraction_reason, meta]
     zip_iterator = zip(keys, values)
     retraction_dict = dict(zip_iterator)
     return retraction_dict
 
 
 def heartbeat_data(machine_time=None, detector_status=None, meta=None):
     """ Formats data for Heartbeat as dict object
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/snews_pub.py` & `snews_pt-1.3.2/snews_pt/snews_pub.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from datetime import datetime
 try:
     fromisoformat = datetime.fromisoformat
 except AttributeError:
     from dateutil.parser import isoparse as fromisoformat
 import os, click
 from hop import Stream
+try:
+    from hop.models import JSONBlob
+except ImportError:
+    raise ImportError(f"SNEWS Publishing Tools and Coincidence System requires hop version>=0.8.0\n"
+                      f"Please upgrade your `pip install -U hop-client`")
 from . import snews_pt_utils
 from .snews_format_checker import SnewsFormat
 from .snews_pt_utils import prettyprint_dictionary
 from .tier_decider import TierDecider
 
 def homogenise_time_field(message):
     """ Make sure all messages follow the same
@@ -95,15 +100,15 @@
             # None of the messages passed the format checker!
             raise UserWarning("No valid message exists!")
 
         if type(messages) == dict:
             messages = list(messages)
         for message in messages:
             message["sent_time"] = datetime.utcnow().isoformat()
-            self.stream.write(message)
+            self.stream.write(JSONBlob(message))
             self.display_message(message)
 
             
     def display_message(self, message):
         if self.verbose:
             tier = message['_id'].split('_')[1]
             click.secho(f'{"-" * 64}', fg='bright_blue')
@@ -119,15 +124,14 @@
                  detector_name='TEST',
                  machine_time=None,
                  neutrino_time=None,
                  p_val=None,
                  p_values=None,
                  t_bin_width=None,
                  timing_series=None,
-                 which_tier=None,
                  retract_latest=None,
                  retraction_reason=None,
                  detector_status=None,
                  is_pre_sn=False,
                  firedrill_mode=True,
                  is_test=False,
                  **kwargs):
@@ -153,17 +157,14 @@
         p_values: `list`
             p values of possible neutrino observation(s),defaults to None.
             list of floats
         t_bin_width: `float`
             width of time window [sec] ,defaults to None.
         timing_series: `list`,
             defaults to None, list of strings following ISO format
-        which_tier: `str`
-            which tier are you trying to retract from, defaults to None.
-            Options: 'CoincidenceTier' / 'SigTier' / 'TimingTier' / 'ALL'
         retract_latest: `int`
             how many of your last messages do you want to retract, defaults to None
         retraction_reason: `str`
             (optional) share with SNEWS what caused your false observation, defaults to None.
             We won't judge you :)
         detector_status: `str`
             tell SNEWS if your detector is ON or OFF, defaults to None.
@@ -182,15 +183,14 @@
         self.message_data = {'detector_name': detector_name,
                              'machine_time': machine_time,
                              'neutrino_time': neutrino_time,
                              'p_val': p_val,
                              'p_values': p_values,
                              't_bin_width': t_bin_width,
                              'timing_series': timing_series,
-                             'which_tier': which_tier,
                              'retract_latest': retract_latest,
                              'retraction_reason': retraction_reason,
                              'detector_status': detector_status,
                              'is_pre_sn': is_pre_sn,
                              'is_test':is_test}
         self.meta = dict(**kwargs)
         self.message_data = {**self.message_data, ** self.meta}
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/snews_sub.py` & `snews_pt-1.3.2/snews_pt/snews_sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 def save_message(message, outputfolder, return_file=False):
     """ Save messages to a json file.
 
     """
     file = make_file(outputfolder)
     with open(file, 'w') as outfile:
         json.dump(message, outfile, indent=4, sort_keys=True)
+
     if return_file:
         return file
 
 def display(message):
     """ Function to format output messages
     """
     click.echo(click.style('ALERT MESSAGE'.center(65, '_'), bg='red', bold=True))
+
     for k, v in message.items():
         key_type = type(v)
         if key_type == type(None):
             v = 'None'
 
         if key_type in [int, float, str]:
             if k=='alert_type':
@@ -48,14 +50,15 @@
         elif key_type == list:
             v = [str(item) for item in v]
             items = '\t'.join(v)
             if k == 'detector_names':
                 click.echo(f'{k:<20s}' + click.style(f':{items:<45}', bg='blue'))
             else:
                 click.echo(f'{k:<20s}:{items:<45}')
+
     click.secho('_'.center(65, '_'), bg='bright_red')
 
 
 class Subscriber:
     """ Class to subscribe ALERT message stream
 
     Parameters
@@ -96,14 +99,17 @@
                    click.style(f'{ self.alert_topic}', bg='green'))
 
         # Initiate hop_stream
         stream = Stream(until_eos=False, auth=auth)
         try:
             with stream.open(self.alert_topic, "r") as s:
                 for message in s:
+                    # Access message dictionary from JSOBlob
+                    message = message.content
+                    # Save and display
                     save_message(message, outputfolder)
                     snews_pt_utils.display_gif()
                     display(message)
         except KeyboardInterrupt:
             click.secho('Done', fg='green')
 
 
@@ -116,13 +122,16 @@
                    click.style(f'{ self.alert_topic}', bg='green'))
 
         # Initiate hop_stream
         stream = Stream(until_eos=False, auth=auth)
         try:
             with stream.open(self.alert_topic, "r") as s:
                 for message in s:
+                    # Access message dictionary from JSONBlobg
+                    message = message.content
+                    # Save and display
                     file = save_message(message, outputfolder, return_file=True)
                     snews_pt_utils.display_gif()
                     display(message)
                     yield file
         except KeyboardInterrupt:
             click.secho('Done', fg='green')
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/test/random_plugin.py` & `snews_pt-1.3.2/snews_pt/test/random_plugin.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/test/test_coincidence_tier.py` & `snews_pt-1.3.2/snews_pt/test/test_coincidence_tier.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # Check that message has expected structure.
     assert list(coin.tiernames) == ['CoincidenceTier']
     assert len(coin.messages) == 1, f"Expected 1 CoincidenceTier Message got {len(coin.messages)}!"
 
     assert coin.message_data == {'detector_name': 'KamLAND', 'machine_time': None,
                                  'neutrino_time': '2012-06-09T15:31:08.891011',
                                  'p_val': None, 'p_values': None, 't_bin_width': None, 'timing_series': None,
-                                 'which_tier': None, 'retract_latest': None, 'retraction_reason': None,
+                                 'retract_latest': None, 'retraction_reason': None,
                                  'detector_status': None, 'is_pre_sn': False, 'is_test':True}
 
     # the SNEWSTierPublisher already checks this in creation, but we can double check
     for message in coin.messages:
         format_checker = SnewsFormat(message)
         assert format_checker() is True, "Message is not in the snews format"
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/test/test_old_crashes.py` & `snews_pt-1.3.2/snews_pt/test/test_old_crashes.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/test/test_plugin.py` & `snews_pt-1.3.2/snews_pt/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/test/test_retraction.py` & `snews_pt-1.3.2/snews_pt/test/test_retraction.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/test/test_significance_tier.py` & `snews_pt-1.3.2/snews_pt/test/test_significance_tier.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     assert sign.message_data == {'detector_name': 'DS-20K',
                                 'machine_time': None,
                                 'neutrino_time': '2012-06-09T15:31:08.109876',
                                 'p_val': None,
                                 'p_values': [0.4, 0.5],
                                 't_bin_width': 0.8,
                                 'timing_series': None,
-                                'which_tier': None,
                                 'retract_latest': None,
                                 'retraction_reason': None,
                                 'detector_status': None,
                                 'is_pre_sn': False,
                                 'neutrino_times': ['2012-06-09T15:31:08.109876',
                                                    '2012-06-09T15:33:07.891098'],
                                 'is_test':True}
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/test/test_subscribe.py` & `snews_pt-1.3.2/snews_pt/test/test_subscribe.py`

 * *Files identical despite different names*

### Comparing `snews_pt-1.3.1.dev1/snews_pt/test/test_timing_tier.py` & `snews_pt-1.3.2/snews_pt/test/test_timing_tier.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     # Check that message has expected structure.
     assert list(tims.tiernames) == ['CoincidenceTier', 'TimeTier']
     assert tims.message_data == {'detector_name': 'XENONnT',  'machine_time': None,
                                  'neutrino_time': '2012-06-09T15:31:08.109876',  'p_val': None,
                                  'p_values': None,  't_bin_width': None,
                                  'timing_series': ['2012-06-09T15:31:08.109876', '2012-06-09T15:33:07.891011'],
-                                 'which_tier': None, 'retract_latest': None, 'retraction_reason': None,
+                                 'retract_latest': None, 'retraction_reason': None,
                                  'detector_status': None, 'is_pre_sn': False, 'is_test':True}
     assert tims.env_file == None
 
     # the SNEWSTierPublisher already checks this in creation, but we can double check
     for message in tims.messages:
         format_checker = SnewsFormat(message)
         assert format_checker() is True, "Message is not in the snews format"
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt/tier_decider.py` & `snews_pt-1.3.2/snews_pt/tier_decider.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from inspect import signature
 from .snews_pt_utils import set_env
 from .snews_pt_utils import coincidence_tier_data, sig_tier_data, time_tier_data, heartbeat_data, retraction_data
 from .message_schema import Message_Schema
 from datetime import datetime
 import os, sys
 
-valid_keys = ["detector_name", "machine_time", "neutrino_time", "p_val", "p_values", "timing_series", "which_tier",
+valid_keys = ["detector_name", "machine_time", "neutrino_time", "p_val", "p_values", "timing_series",
               "retract_latest", "retraction_reason", "detector_status", "is_pre_sn", 't_bin_width']
 
 class TierDecider:
     def __init__(self, data, env_file=None):
         set_env(env_file)
         self.data = data
         self.meta_data = {}
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt.egg-info/PKG-INFO` & `snews_pt-1.3.2/snews_pt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snews-pt
-Version: 1.3.1.dev1
+Version: 1.3.2
 Summary: An alert application for observing supernovas.
 Home-page: https://github.com/SNEWS2/SNEWS_Publishing_Tools
 Author: Sebastian Torres-Lara, Melih Kara
 Author-email: sebastiantorreslara17@gmail.com, karamel.itu@gmail.com
 License: BSD 3-Clause
 Keywords: setup,distutils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `snews_pt-1.3.1.dev1/snews_pt.egg-info/SOURCES.txt` & `snews_pt-1.3.2/snews_pt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

