# Comparing `tmp/perceval_puppet-0.2.8rc1.tar.gz` & `tmp/perceval_puppet-0.2.8rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_puppet-0.2.8rc1.tar", max compression
+gzip compressed data, was "perceval_puppet-0.2.8rc2.tar", max compression
```

## Comparing `perceval_puppet-0.2.8rc1.tar` & `perceval_puppet-0.2.8rc2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       50 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/LICENSE
--rw-r--r--   0        0        0      798 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/NEWS
--rw-r--r--   0        0        0     2197 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/README.md
--rw-r--r--   0        0        0        0 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/perceval/backends/puppet/__init__.py
--rw-r--r--   0        0        0       91 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/perceval/backends/puppet/_version.py
--rw-r--r--   0        0        0    10849 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/perceval/backends/puppet/puppetforge.py
--rw-r--r--   0        0        0     1402 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/__init__.py
--rw-r--r--   0        0        0     1888 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/base.py
--rw-r--r--   0        0        0      192 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_empty.json
--rw-r--r--   0        0        0    15963 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_modules.json
--rw-r--r--   0        0        0     1028 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_modules_next.json
--rw-r--r--   0        0        0    22968 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_releases_ceph.json
--rw-r--r--   0        0        0     1810 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_releases_nomad.json
--rw-r--r--   0        0        0      318 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_user_norisnetwork.json
--rw-r--r--   0        0        0      302 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_user_sshuyskiy.json
--rwxr-xr-x   0        0        0     1017 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/run_tests.py
--rw-r--r--   0        0        0    18656 2023-04-20 15:35:36.632819 perceval_puppet-0.2.8rc1/tests/test_puppetforge.py
--rw-r--r--   0        0        0     3423 1970-01-01 00:00:00.000000 perceval_puppet-0.2.8rc1/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-04-21 09:54:23.696463 perceval_puppet-0.2.8rc2/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-21 09:54:23.696463 perceval_puppet-0.2.8rc2/LICENSE
+-rw-r--r--   0        0        0      798 2023-04-21 09:54:23.696463 perceval_puppet-0.2.8rc2/NEWS
+-rw-r--r--   0        0        0     2197 2023-04-21 09:54:23.696463 perceval_puppet-0.2.8rc2/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 09:54:23.696463 perceval_puppet-0.2.8rc2/perceval/backends/puppet/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-21 09:54:23.696463 perceval_puppet-0.2.8rc2/perceval/backends/puppet/_version.py
+-rw-r--r--   0        0        0    10849 2023-04-21 09:54:23.696463 perceval_puppet-0.2.8rc2/perceval/backends/puppet/puppetforge.py
+-rw-r--r--   0        0        0     1402 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/__init__.py
+-rw-r--r--   0        0        0     1888 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/base.py
+-rw-r--r--   0        0        0      192 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_empty.json
+-rw-r--r--   0        0        0    15963 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_modules.json
+-rw-r--r--   0        0        0     1028 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_modules_next.json
+-rw-r--r--   0        0        0    22968 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_releases_ceph.json
+-rw-r--r--   0        0        0     1810 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_releases_nomad.json
+-rw-r--r--   0        0        0      318 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_user_norisnetwork.json
+-rw-r--r--   0        0        0      302 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_user_sshuyskiy.json
+-rwxr-xr-x   0        0        0     1017 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/run_tests.py
+-rw-r--r--   0        0        0    18656 2023-04-21 09:54:23.700463 perceval_puppet-0.2.8rc2/tests/test_puppetforge.py
+-rw-r--r--   0        0        0     3423 1970-01-01 00:00:00.000000 perceval_puppet-0.2.8rc2/PKG-INFO
```

### Comparing `perceval_puppet-0.2.8rc1/LICENSE` & `perceval_puppet-0.2.8rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/NEWS` & `perceval_puppet-0.2.8rc2/NEWS`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/README.md` & `perceval_puppet-0.2.8rc2/README.md`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/perceval/backends/puppet/puppetforge.py` & `perceval_puppet-0.2.8rc2/perceval/backends/puppet/puppetforge.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/pyproject.toml` & `perceval_puppet-0.2.8rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-puppet"
-version = "0.2.8-rc.1"
+version = "0.2.8-rc.2"
 description = "Bundle of Perceval backends for Puppet, Inc. ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_puppet-0.2.8rc1/tests/base.py` & `perceval_puppet-0.2.8rc2/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_modules.json` & `perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_modules.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_modules_next.json` & `perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_modules_next.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_releases_ceph.json` & `perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_releases_ceph.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_releases_nomad.json` & `perceval_puppet-0.2.8rc2/tests/data/puppetforge/puppetforge_releases_nomad.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/tests/run_tests.py` & `perceval_puppet-0.2.8rc2/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/tests/test_puppetforge.py` & `perceval_puppet-0.2.8rc2/tests/test_puppetforge.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.8rc1/PKG-INFO` & `perceval_puppet-0.2.8rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-puppet
-Version: 0.2.8rc1
+Version: 0.2.8rc2
 Summary: Bundle of Perceval backends for Puppet, Inc. ecosystem.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

