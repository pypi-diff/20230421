# Comparing `tmp/NbRisk-0.3.0.tar.gz` & `tmp/NbRisk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NbRisk-0.3.0.tar", last modified: Sun Apr  2 19:52:30 2023, max compression
+gzip compressed data, was "NbRisk-0.3.1.tar", last modified: Fri Apr 21 00:08:24 2023, max compression
```

## Comparing `NbRisk-0.3.0.tar` & `NbRisk-0.3.1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-02 19:52:30.292258 NbRisk-0.3.0/
--rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-0.3.0/LICENSE
--rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-0.3.0/MANIFEST.in
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-02 19:52:30.188285 NbRisk-0.3.0/NbRisk.egg-info/
--rw-rw-r--   0 renato    (1000) renato    (1000)     3017 2023-04-02 19:52:30.000000 NbRisk-0.3.0/NbRisk.egg-info/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     1367 2023-04-02 19:52:30.000000 NbRisk-0.3.0/NbRisk.egg-info/SOURCES.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-04-02 19:52:30.000000 NbRisk-0.3.0/NbRisk.egg-info/dependency_links.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-04-02 19:52:30.000000 NbRisk-0.3.0/NbRisk.egg-info/top_level.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)     3017 2023-04-02 19:52:30.292258 NbRisk-0.3.0/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2589 2023-04-02 18:56:28.000000 NbRisk-0.3.0/README.md
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-02 19:52:30.228275 NbRisk-0.3.0/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-0.3.0/nb_risk/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-0.3.0/nb_risk/admin.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-02 19:52:30.244270 NbRisk-0.3.0/nb_risk/api/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.3.0/nb_risk/api/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      538 2023-03-31 22:00:38.000000 NbRisk-0.3.0/nb_risk/api/nested_serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4539 2023-03-31 22:00:43.000000 NbRisk-0.3.0/nb_risk/api/serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      440 2023-01-25 20:20:26.000000 NbRisk-0.3.0/nb_risk/api/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1019 2023-01-25 20:20:19.000000 NbRisk-0.3.0/nb_risk/api/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2991 2023-04-02 19:37:23.000000 NbRisk-0.3.0/nb_risk/choices.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1469 2023-04-02 19:37:23.000000 NbRisk-0.3.0/nb_risk/columns.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3392 2023-04-02 19:37:24.000000 NbRisk-0.3.0/nb_risk/cve.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1380 2023-04-02 19:39:18.000000 NbRisk-0.3.0/nb_risk/filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3799 2023-03-13 03:34:58.000000 NbRisk-0.3.0/nb_risk/forms.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.3.0/nb_risk/middleware.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-02 19:52:30.268264 NbRisk-0.3.0/nb_risk/migrations/
--rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-0.3.0/nb_risk/migrations/0001_initial.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1510 2023-03-13 03:36:44.000000 NbRisk-0.3.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)      439 2023-03-13 03:54:37.000000 NbRisk-0.3.0/nb_risk/migrations/0003_alter_vulnerability_cvssbasescore.py
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-0.3.0/nb_risk/migrations/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     7789 2023-04-02 19:37:24.000000 NbRisk-0.3.0/nb_risk/models.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3228 2023-04-02 19:37:24.000000 NbRisk-0.3.0/nb_risk/navigation.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.3.0/nb_risk/signals.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3197 2023-04-02 19:37:24.000000 NbRisk-0.3.0/nb_risk/tables.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-0.3.0/nb_risk/template_content.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-02 19:52:30.180287 NbRisk-0.3.0/nb_risk/templates/
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-02 19:52:30.292258 NbRisk-0.3.0/nb_risk/templates/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/generic_vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/risk.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2211 2023-01-25 20:53:20.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/threatevent.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      505 2023-01-25 20:53:31.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/threatsource.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2837 2023-04-02 19:18:33.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/vulnerability.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      609 2023-04-02 19:20:45.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-0.3.0/nb_risk/templates/nb_risk/vulnerability_search.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     4544 2023-04-02 19:37:24.000000 NbRisk-0.3.0/nb_risk/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       22 2023-04-02 19:03:46.000000 NbRisk-0.3.0/nb_risk/version.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     7432 2023-04-02 19:37:24.000000 NbRisk-0.3.0/nb_risk/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-04-02 19:52:30.292258 NbRisk-0.3.0/setup.cfg
--rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-0.3.0/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-21 00:08:24.053626 NbRisk-0.3.1/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-0.3.1/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-0.3.1/MANIFEST.in
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-21 00:08:23.881596 NbRisk-0.3.1/NbRisk.egg-info/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3017 2023-04-21 00:08:23.000000 NbRisk-0.3.1/NbRisk.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1306 2023-04-21 00:08:23.000000 NbRisk-0.3.1/NbRisk.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-04-21 00:08:23.000000 NbRisk-0.3.1/NbRisk.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-04-21 00:08:23.000000 NbRisk-0.3.1/NbRisk.egg-info/top_level.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3017 2023-04-21 00:08:24.049626 NbRisk-0.3.1/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2589 2023-04-02 18:56:28.000000 NbRisk-0.3.1/README.md
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-21 00:08:23.889597 NbRisk-0.3.1/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-0.3.1/nb_risk/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-0.3.1/nb_risk/admin.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-21 00:08:23.917602 NbRisk-0.3.1/nb_risk/api/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.3.1/nb_risk/api/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      538 2023-03-31 22:00:38.000000 NbRisk-0.3.1/nb_risk/api/nested_serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4539 2023-03-31 22:00:43.000000 NbRisk-0.3.1/nb_risk/api/serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      440 2023-01-25 20:20:26.000000 NbRisk-0.3.1/nb_risk/api/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1019 2023-01-25 20:20:19.000000 NbRisk-0.3.1/nb_risk/api/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2991 2023-04-02 19:37:23.000000 NbRisk-0.3.1/nb_risk/choices.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1469 2023-04-02 19:37:23.000000 NbRisk-0.3.1/nb_risk/columns.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3392 2023-04-02 19:37:24.000000 NbRisk-0.3.1/nb_risk/cve.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1380 2023-04-02 19:39:18.000000 NbRisk-0.3.1/nb_risk/filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3799 2023-03-13 03:34:58.000000 NbRisk-0.3.1/nb_risk/forms.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.3.1/nb_risk/middleware.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-21 00:08:23.933605 NbRisk-0.3.1/nb_risk/migrations/
+-rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-0.3.1/nb_risk/migrations/0001_initial.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-0.3.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-0.3.1/nb_risk/migrations/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     7789 2023-04-02 19:37:24.000000 NbRisk-0.3.1/nb_risk/models.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3228 2023-04-02 19:37:24.000000 NbRisk-0.3.1/nb_risk/navigation.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.3.1/nb_risk/signals.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3197 2023-04-02 19:37:24.000000 NbRisk-0.3.1/nb_risk/tables.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-0.3.1/nb_risk/template_content.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-21 00:08:23.853591 NbRisk-0.3.1/nb_risk/templates/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-21 00:08:24.041624 NbRisk-0.3.1/nb_risk/templates/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/generic_vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/risk.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2211 2023-01-25 20:53:20.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/threatevent.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      505 2023-01-25 20:53:31.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/threatsource.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2837 2023-04-02 19:18:33.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/vulnerability.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      609 2023-04-02 19:20:45.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-0.3.1/nb_risk/templates/nb_risk/vulnerability_search.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4544 2023-04-02 19:37:24.000000 NbRisk-0.3.1/nb_risk/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       22 2023-04-21 00:07:32.000000 NbRisk-0.3.1/nb_risk/version.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     7432 2023-04-02 19:37:24.000000 NbRisk-0.3.1/nb_risk/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-04-21 00:08:24.053626 NbRisk-0.3.1/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-0.3.1/setup.py
```

### Comparing `NbRisk-0.3.0/LICENSE` & `NbRisk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/NbRisk.egg-info/PKG-INFO` & `NbRisk-0.3.1/NbRisk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 0.3.0
+Version: 0.3.1
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-0.3.0/NbRisk.egg-info/SOURCES.txt` & `NbRisk-0.3.1/NbRisk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 nb_risk/api/__init__.py
 nb_risk/api/nested_serializers.py
 nb_risk/api/serializers.py
 nb_risk/api/urls.py
 nb_risk/api/views.py
 nb_risk/migrations/0001_initial.py
 nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
-nb_risk/migrations/0003_alter_vulnerability_cvssbasescore.py
 nb_risk/migrations/__init__.py
 nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
 nb_risk/templates/nb_risk/generic_vulnerability_list.html
 nb_risk/templates/nb_risk/risk.html
 nb_risk/templates/nb_risk/threatevent.html
 nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
 nb_risk/templates/nb_risk/threatsource.html
```

### Comparing `NbRisk-0.3.0/PKG-INFO` & `NbRisk-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 0.3.0
+Version: 0.3.1
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-0.3.0/README.md` & `NbRisk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/__init__.py` & `NbRisk-0.3.1/nb_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/api/nested_serializers.py` & `NbRisk-0.3.1/nb_risk/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/api/serializers.py` & `NbRisk-0.3.1/nb_risk/api/serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/api/views.py` & `NbRisk-0.3.1/nb_risk/api/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/choices.py` & `NbRisk-0.3.1/nb_risk/choices.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/columns.py` & `NbRisk-0.3.1/nb_risk/columns.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/cve.py` & `NbRisk-0.3.1/nb_risk/cve.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/filters.py` & `NbRisk-0.3.1/nb_risk/filters.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/forms.py` & `NbRisk-0.3.1/nb_risk/forms.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/migrations/0001_initial.py` & `NbRisk-0.3.1/nb_risk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py` & `NbRisk-0.3.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.5 on 2023-03-13 03:36
+# Generated by Django 4.1.5 on 2023-04-21 00:03
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
@@ -29,15 +29,16 @@
             model_name='vulnerability',
             name='cvssavailabilityImpact',
             field=models.CharField(blank=True, max_length=100),
         ),
         migrations.AddField(
             model_name='vulnerability',
             name='cvssbaseScore',
-            field=models.CharField(blank=True, max_length=100),
+            field=models.FloatField(blank=True, default=0, max_length=100),
+            preserve_default=False,
         ),
         migrations.AddField(
             model_name='vulnerability',
             name='cvssconfidentialityImpact',
             field=models.CharField(blank=True, max_length=100),
         ),
         migrations.AddField(
```

### Comparing `NbRisk-0.3.0/nb_risk/models.py` & `NbRisk-0.3.1/nb_risk/models.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/navigation.py` & `NbRisk-0.3.1/nb_risk/navigation.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/tables.py` & `NbRisk-0.3.1/nb_risk/tables.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/template_content.py` & `NbRisk-0.3.1/nb_risk/template_content.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html` & `NbRisk-0.3.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/templates/nb_risk/risk.html` & `NbRisk-0.3.1/nb_risk/templates/nb_risk/risk.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/templates/nb_risk/threatevent.html` & `NbRisk-0.3.1/nb_risk/templates/nb_risk/threatevent.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/templates/nb_risk/threatsource.html` & `NbRisk-0.3.1/nb_risk/templates/nb_risk/threatsource.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/templates/nb_risk/vulnerability.html` & `NbRisk-0.3.1/nb_risk/templates/nb_risk/vulnerability.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html` & `NbRisk-0.3.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/templates/nb_risk/vulnerability_search.html` & `NbRisk-0.3.1/nb_risk/templates/nb_risk/vulnerability_search.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/urls.py` & `NbRisk-0.3.1/nb_risk/urls.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/nb_risk/views.py` & `NbRisk-0.3.1/nb_risk/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.3.0/setup.py` & `NbRisk-0.3.1/setup.py`

 * *Files identical despite different names*

