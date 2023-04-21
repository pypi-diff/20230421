# Comparing `tmp/aodhclient-3.2.0.tar.gz` & `tmp/aodhclient-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aodhclient-3.2.0.tar", last modified: Thu Mar  2 14:24:48 2023, max compression
+gzip compressed data, was "aodhclient-3.3.0.tar", last modified: Fri Apr 21 09:14:26 2023, max compression
```

## Comparing `aodhclient-3.2.0.tar` & `aodhclient-3.3.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.225567 aodhclient-3.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-03-02 14:24:24.000000 aodhclient-3.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-03-02 14:24:24.000000 aodhclient-3.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-03-02 14:24:24.000000 aodhclient-3.2.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2417 2023-03-02 14:24:48.000000 aodhclient-3.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-03-02 14:24:24.000000 aodhclient-3.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10510 2023-03-02 14:24:48.000000 aodhclient-3.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 14:24:24.000000 aodhclient-3.2.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-02 14:24:24.000000 aodhclient-3.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1673 2023-03-02 14:24:48.225567 aodhclient-3.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-03-02 14:24:24.000000 aodhclient-3.2.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.209564 aodhclient-3.2.0/aodhclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5287 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2567 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1844 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/osc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6879 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.213564 aodhclient-3.2.0/aodhclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.213564 aodhclient-3.2.0/aodhclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40002 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/functional/test_alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5294 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/functional/test_alarm_history.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/functional/test_capabilities.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.213564 aodhclient-3.2.0/aodhclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10470 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/unit/test_alarm_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1961 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/unit/test_alarm_history.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3418 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/unit/test_alarm_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1529 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/unit/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1417 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3219 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6980 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.217565 aodhclient-3.2.0/aodhclient/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8634 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27068 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/alarm_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/alarm_history.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2892 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/alarm_history_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1728 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/capabilities_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2282 2023-03-02 14:24:24.000000 aodhclient-3.2.0/aodhclient/v2/quota_cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.213564 aodhclient-3.2.0/aodhclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1673 2023-03-02 14:24:48.000000 aodhclient-3.2.0/aodhclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2023-03-02 14:24:48.000000 aodhclient-3.2.0/aodhclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 14:24:48.000000 aodhclient-3.2.0/aodhclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-03-02 14:24:48.000000 aodhclient-3.2.0/aodhclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 14:24:48.000000 aodhclient-3.2.0/aodhclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-02 14:24:48.000000 aodhclient-3.2.0/aodhclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-03-02 14:24:48.000000 aodhclient-3.2.0/aodhclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-03-02 14:24:48.000000 aodhclient-3.2.0/aodhclient.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-03-02 14:24:24.000000 aodhclient-3.2.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.217565 aodhclient-3.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-03-02 14:24:24.000000 aodhclient-3.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.217565 aodhclient-3.2.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-03-02 14:24:24.000000 aodhclient-3.2.0/doc/source/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4226 2023-03-02 14:24:24.000000 aodhclient-3.2.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-03-02 14:24:24.000000 aodhclient-3.2.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2023-03-02 14:24:24.000000 aodhclient-3.2.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-03-02 14:24:24.000000 aodhclient-3.2.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2023-03-02 14:24:24.000000 aodhclient-3.2.0/doc/source/shell.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.205563 aodhclient-3.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.221566 aodhclient-3.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/add-pagination-support-fcdf1cef0cfa5ca9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/drop-py-2-7-8f26d7e1e8dc83c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/drop-python-3-6-and-3-7-c70234384bc69b1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/merge-search-to-list-d44cd65ede348c3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/osc-support-9f9dae2d2203f307.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/remove-ceilometer-alarms-02049eef189c2812.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/split-alarm-query-and-list-5998020b88ddc9f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/support-get-set-state-interfaces-67419b925ffd6877.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/notes/ussuri-add-threshold-alarm-47e012620fd611ea.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.225567 aodhclient-3.2.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.225567 aodhclient-3.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:48.225567 aodhclient-3.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8462 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-02 14:24:24.000000 aodhclient-3.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2023-03-02 14:24:24.000000 aodhclient-3.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2023-03-02 14:24:48.225567 aodhclient-3.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-03-02 14:24:24.000000 aodhclient-3.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2023-03-02 14:24:24.000000 aodhclient-3.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.706300 aodhclient-3.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-04-21 09:14:01.000000 aodhclient-3.3.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-04-21 09:14:01.000000 aodhclient-3.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-04-21 09:14:01.000000 aodhclient-3.3.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2458 2023-04-21 09:14:26.000000 aodhclient-3.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-04-21 09:14:01.000000 aodhclient-3.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10594 2023-04-21 09:14:26.000000 aodhclient-3.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-21 09:14:01.000000 aodhclient-3.3.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-04-21 09:14:01.000000 aodhclient-3.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1673 2023-04-21 09:14:26.706300 aodhclient-3.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-04-21 09:14:01.000000 aodhclient-3.3.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.702300 aodhclient-3.3.0/aodhclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5287 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2567 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1844 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/osc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6879 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.702300 aodhclient-3.3.0/aodhclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.702300 aodhclient-3.3.0/aodhclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40002 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/functional/test_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5294 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/functional/test_alarm_history.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/functional/test_capabilities.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.702300 aodhclient-3.3.0/aodhclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10470 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/unit/test_alarm_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1961 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/unit/test_alarm_history.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3418 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/unit/test_alarm_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1529 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/unit/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1417 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3219 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6980 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.702300 aodhclient-3.3.0/aodhclient/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8634 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27068 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/alarm_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/alarm_history.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2892 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/alarm_history_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1728 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/capabilities_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2282 2023-04-21 09:14:01.000000 aodhclient-3.3.0/aodhclient/v2/quota_cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.702300 aodhclient-3.3.0/aodhclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1673 2023-04-21 09:14:26.000000 aodhclient-3.3.0/aodhclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2845 2023-04-21 09:14:26.000000 aodhclient-3.3.0/aodhclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-21 09:14:26.000000 aodhclient-3.3.0/aodhclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-04-21 09:14:26.000000 aodhclient-3.3.0/aodhclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-21 09:14:26.000000 aodhclient-3.3.0/aodhclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-21 09:14:26.000000 aodhclient-3.3.0/aodhclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-04-21 09:14:26.000000 aodhclient-3.3.0/aodhclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-04-21 09:14:26.000000 aodhclient-3.3.0/aodhclient.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-04-21 09:14:01.000000 aodhclient-3.3.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.702300 aodhclient-3.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-04-21 09:14:01.000000 aodhclient-3.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.706300 aodhclient-3.3.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-04-21 09:14:01.000000 aodhclient-3.3.0/doc/source/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4226 2023-04-21 09:14:01.000000 aodhclient-3.3.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-04-21 09:14:01.000000 aodhclient-3.3.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2023-04-21 09:14:01.000000 aodhclient-3.3.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-04-21 09:14:01.000000 aodhclient-3.3.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2023-04-21 09:14:01.000000 aodhclient-3.3.0/doc/source/shell.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.698300 aodhclient-3.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.706300 aodhclient-3.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/add-pagination-support-fcdf1cef0cfa5ca9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/drop-py-2-7-8f26d7e1e8dc83c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/drop-python-3-6-and-3-7-c70234384bc69b1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/merge-search-to-list-d44cd65ede348c3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/osc-support-9f9dae2d2203f307.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/remove-ceilometer-alarms-02049eef189c2812.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/split-alarm-query-and-list-5998020b88ddc9f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/support-get-set-state-interfaces-67419b925ffd6877.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/notes/ussuri-add-threshold-alarm-47e012620fd611ea.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.706300 aodhclient-3.3.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.706300 aodhclient-3.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:26.706300 aodhclient-3.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8462 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-04-21 09:14:01.000000 aodhclient-3.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-04-21 09:14:01.000000 aodhclient-3.3.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1988 2023-04-21 09:14:26.706300 aodhclient-3.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-04-21 09:14:01.000000 aodhclient-3.3.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2023-04-21 09:14:01.000000 aodhclient-3.3.0/tox.ini
```

### Comparing `aodhclient-3.2.0/AUTHORS` & `aodhclient-3.3.0/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 Nguyen Hai <nguyentrihai93@gmail.com>
 OpenStack Release Bot <infra-root@openstack.org>
 PanFengyun <fengyun.pan@easystack.cn>
 Pradeep Kilambi <pkilambi@redhat.com>
 Rui Yuan Dou <rydou@fiberhome.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Simon Merrick <simonmerrick@catalyst.net.nz>
+Stephen Finucane <stephenfin@redhat.com>
 Stéphane Albert <stephane.albert@objectif-libre.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Takashi Kajinami <tkajinam@redhat.com>
 Thomas Bechtold <tbechtold@suse.com>
 Tony Breeds <tony@bakeyournoodle.com>
 Tovin Seven <vinhnt@vn.fujitsu.com>
 Vieri <15050873171@163.com>
```

### Comparing `aodhclient-3.2.0/CONTRIBUTING.rst` & `aodhclient-3.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/ChangeLog` & `aodhclient-3.3.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+3.3.0
+-----
+
+* Move test requirements to tox.ini
+* Update master for stable/2023.1
+
 3.2.0
 -----
 
 * Fix CI jobs(py38, py310) and upload of wheels package to PyPi
 
 3.1.0
 -----
```

### Comparing `aodhclient-3.2.0/LICENSE` & `aodhclient-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/PKG-INFO` & `aodhclient-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aodhclient
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python client library for Aodh
 Home-page: https://docs.openstack.org/python-aodhclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         aodhclient
```

### Comparing `aodhclient-3.2.0/README.rst` & `aodhclient-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/__init__.py` & `aodhclient-3.3.0/aodhclient/__init__.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/client.py` & `aodhclient-3.3.0/aodhclient/client.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/exceptions.py` & `aodhclient-3.3.0/aodhclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/i18n.py` & `aodhclient-3.3.0/aodhclient/i18n.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/noauth.py` & `aodhclient-3.3.0/aodhclient/noauth.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/osc.py` & `aodhclient-3.3.0/aodhclient/osc.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/shell.py` & `aodhclient-3.3.0/aodhclient/shell.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/functional/base.py` & `aodhclient-3.3.0/aodhclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/functional/test_alarm.py` & `aodhclient-3.3.0/aodhclient/tests/functional/test_alarm.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/functional/test_alarm_history.py` & `aodhclient-3.3.0/aodhclient/tests/functional/test_alarm_history.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/functional/test_capabilities.py` & `aodhclient-3.3.0/aodhclient/tests/functional/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/unit/test_alarm_cli.py` & `aodhclient-3.3.0/aodhclient/tests/unit/test_alarm_cli.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/unit/test_alarm_history.py` & `aodhclient-3.3.0/aodhclient/tests/unit/test_alarm_history.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/unit/test_alarm_manager.py` & `aodhclient-3.3.0/aodhclient/tests/unit/test_alarm_manager.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/unit/test_exceptions.py` & `aodhclient-3.3.0/aodhclient/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/unit/test_quota.py` & `aodhclient-3.3.0/aodhclient/tests/unit/test_quota.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/unit/test_shell.py` & `aodhclient-3.3.0/aodhclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/tests/unit/test_utils.py` & `aodhclient-3.3.0/aodhclient/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/utils.py` & `aodhclient-3.3.0/aodhclient/utils.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/alarm.py` & `aodhclient-3.3.0/aodhclient/v2/alarm.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/alarm_cli.py` & `aodhclient-3.3.0/aodhclient/v2/alarm_cli.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/alarm_history.py` & `aodhclient-3.3.0/aodhclient/v2/alarm_history.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/alarm_history_cli.py` & `aodhclient-3.3.0/aodhclient/v2/alarm_history_cli.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/base.py` & `aodhclient-3.3.0/aodhclient/v2/base.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/capabilities.py` & `aodhclient-3.3.0/aodhclient/v2/capabilities.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/capabilities_cli.py` & `aodhclient-3.3.0/aodhclient/v2/capabilities_cli.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/client.py` & `aodhclient-3.3.0/aodhclient/v2/client.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/quota.py` & `aodhclient-3.3.0/aodhclient/v2/quota.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient/v2/quota_cli.py` & `aodhclient-3.3.0/aodhclient/v2/quota_cli.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/aodhclient.egg-info/PKG-INFO` & `aodhclient-3.3.0/aodhclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aodhclient
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python client library for Aodh
 Home-page: https://docs.openstack.org/python-aodhclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         aodhclient
```

### Comparing `aodhclient-3.2.0/aodhclient.egg-info/SOURCES.txt` & `aodhclient-3.3.0/aodhclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 releasenotes/notes/drop-python-3-6-and-3-7-c70234384bc69b1d.yaml
 releasenotes/notes/merge-search-to-list-d44cd65ede348c3e.yaml
 releasenotes/notes/osc-support-9f9dae2d2203f307.yaml
 releasenotes/notes/remove-ceilometer-alarms-02049eef189c2812.yaml
 releasenotes/notes/split-alarm-query-and-list-5998020b88ddc9f5.yaml
 releasenotes/notes/support-get-set-state-interfaces-67419b925ffd6877.yaml
 releasenotes/notes/ussuri-add-threshold-alarm-47e012620fd611ea.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
```

### Comparing `aodhclient-3.2.0/aodhclient.egg-info/entry_points.txt` & `aodhclient-3.3.0/aodhclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/doc/source/conf.py` & `aodhclient-3.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/doc/source/index.rst` & `aodhclient-3.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/doc/source/shell.rst` & `aodhclient-3.3.0/doc/source/shell.rst`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/releasenotes/source/conf.py` & `aodhclient-3.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/setup.cfg` & `aodhclient-3.3.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 	oslotest>=1.10.0 # Apache-2.0
 	reno>=1.6.2 # Apache2
 	tempest>=10
 	stestr>=2.0.0 # Apache-2.0
 	testtools>=1.4.0
 	pifpaf[gnocchi]>=0.23
 	gnocchi[postgresql,file]
+	SQLAlchemy-Utils<=0.38.3
+	sqlalchemy-migrate<=0.13.0
+	SQLAlchemy<=1.4.41
+	oslo.db<=12.3.1
 
 [entry_points]
 console_scripts = 
 	aodh = aodhclient.shell:main
 keystoneauth1.plugin = 
 	aodh-noauth = aodhclient.noauth:AodhNoAuthLoader
 openstack.cli.extension =
```

### Comparing `aodhclient-3.2.0/setup.py` & `aodhclient-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `aodhclient-3.2.0/tox.ini` & `aodhclient-3.3.0/tox.ini`

 * *Files identical despite different names*

