# Comparing `tmp/scanoss-1.5.0.tar.gz` & `tmp/scanoss-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanoss-1.5.0.tar", last modified: Tue Mar 21 09:48:32 2023, max compression
+gzip compressed data, was "scanoss-1.5.1.tar", last modified: Fri Apr 21 12:28:02 2023, max compression
```

## Comparing `scanoss-1.5.0.tar` & `scanoss-1.5.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.359836 scanoss-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-21 09:48:09.000000 scanoss-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-03-21 09:48:09.000000 scanoss-1.5.0/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-21 09:48:32.359836 scanoss-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-03-21 09:48:09.000000 scanoss-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-21 09:48:09.000000 scanoss-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-21 09:48:32.359836 scanoss-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.351836 scanoss-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/common/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/common/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/common/v2/scanoss_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/components/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/components/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/components/v2/scanoss_components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.351836 scanoss-1.5.0/src/scanoss/api/cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/cryptography/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/dependencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/dependencies/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/dependencies/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss/api/scanning/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/scanning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.359836 scanoss-1.5.0/src/scanoss/api/scanning/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/scanning/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.359836 scanoss-1.5.0/src/scanoss/api/vulnerabilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/vulnerabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.359836 scanoss-1.5.0/src/scanoss/api/vulnerabilities/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/vulnerabilities/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32906 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/csvoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/cyclonedx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.359836 scanoss-1.5.0/src/scanoss/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-21 09:48:20.000000 scanoss-1.5.0/src/scanoss/data/build_date.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/data/spdx-exceptions.json
--rw-r--r--   0 runner    (1001) docker     (123)   228794 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/data/spdx-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/filecount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/scancodedeps.py
--rw-r--r--   0 runner    (1001) docker     (123)    38969 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/scanossapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/scanossbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/scanossgrpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/spdxlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/threadeddependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/threadedscanning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-03-21 09:48:09.000000 scanoss-1.5.0/src/scanoss/winnowing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 09:48:32.355836 scanoss-1.5.0/src/scanoss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-21 09:48:32.000000 scanoss-1.5.0/src/scanoss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-21 09:48:32.000000 scanoss-1.5.0/src/scanoss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 09:48:32.000000 scanoss-1.5.0/src/scanoss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-21 09:48:32.000000 scanoss-1.5.0/src/scanoss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-21 09:48:32.000000 scanoss-1.5.0/src/scanoss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-21 09:48:32.000000 scanoss-1.5.0/src/scanoss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-21 12:27:38.000000 scanoss-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-21 12:27:38.000000 scanoss-1.5.1/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-21 12:28:02.444543 scanoss-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-21 12:27:38.000000 scanoss-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-21 12:27:38.000000 scanoss-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-21 12:28:02.444543 scanoss-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.436543 scanoss-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.440543 scanoss-1.5.1/src/scanoss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.440543 scanoss-1.5.1/src/scanoss/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/common/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/common/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/common/v2/scanoss_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/components/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/components/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/components/v2/scanoss_components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.436543 scanoss-1.5.1/src/scanoss/api/cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/cryptography/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/dependencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/dependencies/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/dependencies/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/scanning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/scanning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/scanning/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/scanning/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/vulnerabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/vulnerabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33773 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/csvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/cyclonedx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 12:27:51.000000 scanoss-1.5.1/src/scanoss/data/build_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/data/spdx-exceptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   228794 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/data/spdx-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/filecount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scancodedeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41124 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scanossapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scanossbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scanossgrpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/spdxlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/threadeddependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/threadedscanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/winnowing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.440543 scanoss-1.5.1/src/scanoss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/top_level.txt
```

### Comparing `scanoss-1.5.0/LICENSE` & `scanoss-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/PACKAGE.md` & `scanoss-1.5.1/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/PKG-INFO` & `scanoss-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.5.0
+Version: 1.5.1
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.5.0/README.md` & `scanoss-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/setup.cfg` & `scanoss-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/__init__.py` & `scanoss-1.5.1/src/scanoss/api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,9 +17,7 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
-
-__version__ = '1.5.0'
```

### Comparing `scanoss-1.5.0/src/scanoss/api/__init__.py` & `scanoss-1.5.1/src/scanoss/api/common/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/common/__init__.py` & `scanoss-1.5.1/src/scanoss/api/common/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/common/v2/__init__.py` & `scanoss-1.5.1/src/scanoss/api/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/common/v2/scanoss_common_pb2.py` & `scanoss-1.5.1/src/scanoss/api/common/v2/scanoss_common_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/components/__init__.py` & `scanoss-1.5.1/src/scanoss/api/components/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/components/v2/__init__.py` & `scanoss-1.5.1/src/scanoss/api/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/components/v2/scanoss_components_pb2.py` & `scanoss-1.5.1/src/scanoss/api/components/v2/scanoss_components_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py` & `scanoss-1.5.1/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py` & `scanoss-1.5.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py` & `scanoss-1.5.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/dependencies/__init__.py` & `scanoss-1.5.1/src/scanoss/api/dependencies/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/dependencies/v2/__init__.py` & `scanoss-1.5.1/src/scanoss/api/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py` & `scanoss-1.5.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py` & `scanoss-1.5.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/scanning/__init__.py` & `scanoss-1.5.1/src/scanoss/api/scanning/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/scanning/v2/__init__.py` & `scanoss-1.5.1/src/scanoss/api/vulnerabilities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2021, SCANOSS
+   Copyright (c) 2022, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
```

### Comparing `scanoss-1.5.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py` & `scanoss-1.5.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py` & `scanoss-1.5.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/vulnerabilities/__init__.py` & `scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/vulnerabilities/v2/__init__.py` & `scanoss-1.5.1/src/scanoss/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2022, SCANOSS
+   Copyright (c) 2021, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
@@ -17,7 +17,9 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
+
+__version__ = '1.5.1'
```

### Comparing `scanoss-1.5.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py` & `scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py` & `scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/cli.py` & `scanoss-1.5.1/src/scanoss/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,17 @@
     p_scan.add_argument('scan_dir', metavar='FILE/DIR', type=str, nargs='?', help='A file or folder to scan')
     p_scan.add_argument('--wfp', '-w',  type=str,
                         help='Scan a WFP File instead of a folder (optional)'
                         )
     p_scan.add_argument('--dep', '-p',  type=str,
                         help='Use a dependency file instead of a folder (optional)'
                         )
+    p_scan.add_argument('--stdin', '-s', metavar='STDIN-FILENAME',  type=str,
+                        help='Scan the file contents supplied via STDIN (optional)'
+                        )
     p_scan.add_argument('--identify', '-i', type=str, help='Scan and identify components in SBOM file')
     p_scan.add_argument('--ignore',   '-n', type=str, help='Ignore components specified in the SBOM file')
     p_scan.add_argument('--output',   '-o', type=str, help='Output result file name (optional - default stdout).')
     p_scan.add_argument('--format',   '-f', type=str, choices=['plain', 'cyclonedx', 'spdxlite', 'csv'],
                         help='Result output format (optional - default: plain)'
                         )
     p_scan.add_argument('--threads', '-T', type=int, default=10,
@@ -113,14 +116,17 @@
     # Sub-command: fingerprint
     p_wfp = subparsers.add_parser('fingerprint', aliases=['fp', 'wfp'],
                                   description=f'Fingerprint the given source base: {__version__}',
                                   help='Fingerprint source code')
     p_wfp.set_defaults(func=wfp)
     p_wfp.add_argument('scan_dir', metavar='FILE/DIR', type=str, nargs='?',
                        help='A file or folder to scan')
+    p_wfp.add_argument('--stdin', '-s', metavar='STDIN-FILENAME',  type=str,
+                        help='Fingerprint the file contents supplied via STDIN (optional)'
+                        )
     p_wfp.add_argument('--output', '-o', type=str, help='Output result file name (optional - default stdout).')
     p_wfp.add_argument('--obfuscate', action='store_true', help='Obfuscate fingerprints')
     p_wfp.add_argument('--skip-snippets', '-S', action='store_true', help='Skip the generation of snippets')
     p_wfp.add_argument('--all-extensions', action='store_true', help='Fingerprint all file extensions')
     p_wfp.add_argument('--all-folders', action='store_true', help='Fingerprint all folders')
     p_wfp.add_argument('--all-hidden', action='store_true', help='Fingerprint all hidden files/folders')
 
@@ -324,37 +330,44 @@
     Parameters
     ----------
         parser: ArgumentParser
             command line parser object
         args: Namespace
             Parsed arguments
     """
-    if not args.scan_dir:
-        print_stderr('Please specify a file/folder')
+    if not args.scan_dir and not args.stdin:
+        print_stderr('Please specify a file/folder or STDIN (--stdin)')
         parser.parse_args([args.subparser, '-h'])
         exit(1)
     scan_output: str = None
     if args.output:
         scan_output = args.output
         open(scan_output, 'w').close()
 
     scan_options = 0 if args.skip_snippets else ScanType.SCAN_SNIPPETS.value  # Skip snippet generation or not
     scanner = Scanner(debug=args.debug, trace=args.trace, quiet=args.quiet, obfuscate=args.obfuscate,
                       scan_options=scan_options, all_extensions=args.all_extensions,
                       all_folders=args.all_folders, hidden_files_folders=args.all_hidden)
 
-    if not os.path.exists(args.scan_dir):
-        print_stderr(f'Error: File or folder specified does not exist: {args.scan_dir}.')
-        exit(1)
-    if os.path.isdir(args.scan_dir):
-        scanner.wfp_folder(args.scan_dir, scan_output)
-    elif os.path.isfile(args.scan_dir):
-        scanner.wfp_file(args.scan_dir, scan_output)
+    if args.stdin:
+        contents = sys.stdin.buffer.read()
+        scanner.wfp_contents(args.stdin, contents, scan_output)
+    elif args.scan_dir:
+        if not os.path.exists(args.scan_dir):
+            print_stderr(f'Error: File or folder specified does not exist: {args.scan_dir}.')
+            exit(1)
+        if os.path.isdir(args.scan_dir):
+            scanner.wfp_folder(args.scan_dir, scan_output)
+        elif os.path.isfile(args.scan_dir):
+            scanner.wfp_file(args.scan_dir, scan_output)
+        else:
+            print_stderr(f'Error: Path specified is neither a file or a folder: {args.scan_dir}.')
+            exit(1)
     else:
-        print_stderr(f'Error: Path specified is neither a file or a folder: {args.scan_dir}.')
+        print_stderr('No action found to process')
         exit(1)
 
 
 def get_scan_options(args):
     """
     Parse the scanning options to determine the correct scan settings
     :param args: cmd args
@@ -392,16 +405,16 @@
     Parameters
     ----------
         parser: ArgumentParser
             command line parser object
         args: Namespace
             Parsed arguments
     """
-    if not args.scan_dir and not args.wfp:
-        print_stderr('Please specify a file/folder or fingerprint (--wfp)')
+    if not args.scan_dir and not args.wfp and not args.stdin:
+        print_stderr('Please specify a file/folder, fingerprint (--wfp) or STDIN (--stdin)')
         parser.parse_args([args.subparser, '-h'])
         exit(1)
     if args.pac and args.proxy:
         print_stderr('Please specify one of --proxy or --pac, not both')
         parser.parse_args([args.subparser, '-h'])
         exit(1)
     scan_type: str = None
@@ -489,14 +502,18 @@
         if not scanner.is_file_or_snippet_scan():
             print_stderr(f'Error: Cannot specify WFP scanning if file/snippet options are disabled ({scan_options})')
             exit(1)
         if args.threads > 1:
             scanner.scan_wfp_file_threaded(args.wfp)
         else:
             scanner.scan_wfp_file(args.wfp)
+    elif args.stdin:
+        contents = sys.stdin.buffer.read()
+        if not scanner.scan_contents(args.stdin, contents):
+            exit(1)
     elif args.scan_dir:
         if not os.path.exists(args.scan_dir):
             print_stderr(f'Error: File or folder specified does not exist: {args.scan_dir}.')
             exit(1)
         if os.path.isdir(args.scan_dir):
             if not scanner.scan_folder_with_options(args.scan_dir, scanner.winnowing.file_map):
                 exit(1)
```

### Comparing `scanoss-1.5.0/src/scanoss/components.py` & `scanoss-1.5.1/src/scanoss/components.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/csvoutput.py` & `scanoss-1.5.1/src/scanoss/csvoutput.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/cyclonedx.py` & `scanoss-1.5.1/src/scanoss/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/data/spdx-exceptions.json` & `scanoss-1.5.1/src/scanoss/data/spdx-exceptions.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/data/spdx-licenses.json` & `scanoss-1.5.1/src/scanoss/data/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/filecount.py` & `scanoss-1.5.1/src/scanoss/filecount.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/scancodedeps.py` & `scanoss-1.5.1/src/scanoss/scancodedeps.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/scanner.py` & `scanoss-1.5.1/src/scanoss/scanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -583,14 +583,43 @@
             self.print_debug(f'Scanning {file}...')
             if self.threaded_scan:
                 success = self.__run_scan_threaded(False, 1)
         else:
             success = False
         return success
 
+    def scan_contents(self, filename: str, contents: bytes) -> bool:
+        """
+        Scan the given contents as a file
+
+        :param filename: filename to associate with the contents
+        :param contents: file contents
+        :return: True if successful, False otherwise
+        """
+        success = True
+        if not filename:
+            raise Exception(f"ERROR: Please specify a filename to scan")
+        if not contents:
+            raise Exception(f"ERROR: Please specify a file contents to scan")
+
+        self.print_debug(f'Fingerprinting {filename}...')
+        wfp = self.winnowing.wfp_for_contents(filename, False, contents)
+        if wfp is not None and wfp != '':
+            if self.threaded_scan:
+                self.threaded_scan.queue_add(wfp)  # Submit the WFP for scanning
+            self.print_debug(f'Scanning {filename}...')
+            if self.threaded_scan:
+                success = self.__run_scan_threaded(False, 1)
+        else:
+            success = False
+        if self.threaded_scan:
+            if not self.__finish_scan_threaded():
+                success = False
+        return success
+
     def scan_wfp_file(self, file: str = None) -> bool:
         """
         Scan the contents of the specified WFP file (in the current process)
         :param file: Scan the contents of the specified WFP file (in the current process)
         :return: True if successful, False otherwise
         """
         success = True
@@ -773,14 +802,40 @@
             csvo.produce_from_str(raw_output)
         else:
             self.print_stderr(f'ERROR: Unknown output format: {self.output_format}')
             success = False
 
         return success
 
+    def wfp_contents(self, filename: str, contents: bytes, wfp_file: str = None):
+        """
+        Fingerprint the specified contents as a file
+
+        :param filename: filename to associate with the contents
+        :param contents: file contents
+        :param wfp_file: WFP to write results to (optional)
+        :return:
+        """
+        if not filename:
+            raise Exception(f"ERROR: Please specify a filename to scan")
+        if not contents:
+            raise Exception(f"ERROR: Please specify a file contents to scan")
+
+        self.print_debug(f'Fingerprinting {filename}...')
+        wfp = self.winnowing.wfp_for_contents(filename, False, contents)
+        if wfp:
+            if wfp_file:
+                self.print_stderr(f'Writing fingerprints to {wfp_file}')
+                with open(wfp_file, 'w') as f:
+                    f.write(wfp)
+            else:
+                print(wfp)
+        else:
+            Scanner.print_stderr(f'Warning: No fingerprints generated for: {scan_file}')
+
     def wfp_file(self, scan_file: str, wfp_file: str = None):
         """
         Fingerprint the specified file
         """
         if not scan_file:
             raise Exception(f"ERROR: Please specify a file to fingerprint")
         if not os.path.exists(scan_file) or not os.path.isfile(scan_file):
```

### Comparing `scanoss-1.5.0/src/scanoss/scanossapi.py` & `scanoss-1.5.1/src/scanoss/scanossapi.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/scanossbase.py` & `scanoss-1.5.1/src/scanoss/scanossbase.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/scanossgrpc.py` & `scanoss-1.5.1/src/scanoss/scanossgrpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/scantype.py` & `scanoss-1.5.1/src/scanoss/scantype.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/spdxlite.py` & `scanoss-1.5.1/src/scanoss/spdxlite.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/threadeddependencies.py` & `scanoss-1.5.1/src/scanoss/threadeddependencies.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/threadedscanning.py` & `scanoss-1.5.1/src/scanoss/threadedscanning.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss/winnowing.py` & `scanoss-1.5.1/src/scanoss/winnowing.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.0/src/scanoss.egg-info/PKG-INFO` & `scanoss-1.5.1/src/scanoss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.5.0
+Version: 1.5.1
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.5.0/src/scanoss.egg-info/SOURCES.txt` & `scanoss-1.5.1/src/scanoss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

