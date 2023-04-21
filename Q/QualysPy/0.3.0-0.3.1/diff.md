# Comparing `tmp/qualyspy-0.3.0.tar.gz` & `tmp/qualyspy-0.3.1.tar.gz`

## Comparing `qualyspy-0.3.0.tar` & `qualyspy-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.0/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.0/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/remove_cookies.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/__init__.py
--rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/qutils.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/urls.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/api_input.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    15601 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.0/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.0/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.0/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.0/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.1/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.1/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/remove_cookies.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/__init__.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/urls.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/api_input.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    15586 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.1/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.1/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.1/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.1/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.1/PKG-INFO
```

### Comparing `qualyspy-0.3.0/.vscode/launch.json` & `qualyspy-0.3.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/debug/dtd.txt` & `qualyspy-0.3.1/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/debug/output.txt` & `qualyspy-0.3.1/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/debug/parse_dtd.py` & `qualyspy-0.3.1/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/debug/quickscan.py` & `qualyspy-0.3.1/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/debug/remove_cookies.py` & `qualyspy-0.3.1/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/docs/Makefile` & `qualyspy-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/docs/make.bat` & `qualyspy-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/docs/source/conf.py` & `qualyspy-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/qualysapi.py` & `qualyspy-0.3.1/qualyspy/qualysapi.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/qutils.py` & `qualyspy-0.3.1/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/urls.json` & `qualyspy-0.3.1/qualyspy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/api_input.py` & `qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/api_input.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/tag.py` & `qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/tag.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/assets/host_list.py` & `qualyspy-0.3.1/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/assets/host_list_detection.py` & `qualyspy-0.3.1/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/qualyspy/certview/certificate.py` & `qualyspy-0.3.1/qualyspy/certview/certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 
     certificate_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("certificate.id"))
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
         back_populates="assets", uselist=False
     )
     primary_ip: orm.Mapped[
         ipaddress.IPv4Address | ipaddress.IPv6Address
-    ] = orm.mapped_column("address", sa_pg.INET, primary_key=True)
+    ] = orm.mapped_column("primary_ip", sa_pg.INET)
 
 
 ####################################################################################################
 # Certificate
 
 
 class Certificate(pyd.BaseModel):
```

### Comparing `qualyspy-0.3.0/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.3.1/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/.gitignore` & `qualyspy-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/LICENSE` & `qualyspy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.0/pyproject.toml` & `qualyspy-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.3.0/PKG-INFO` & `qualyspy-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

