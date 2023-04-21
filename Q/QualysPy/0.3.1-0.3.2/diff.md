# Comparing `tmp/qualyspy-0.3.1.tar.gz` & `tmp/qualyspy-0.3.2.tar.gz`

## Comparing `qualyspy-0.3.1.tar` & `qualyspy-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.1/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.1/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.1/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/remove_cookies.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qualyspy-0.3.1/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.1/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/__init__.py
--rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/qutils.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/urls.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/api_input.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    15586 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.1/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.1/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.1/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.1/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.1/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.2/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.2/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.2/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.2/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.2/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.2/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.2/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.2/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.2/debug/remove_cookies.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 qualyspy-0.3.2/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.2/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/__init__.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/urls.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/asset_mgmt_tagging/api_input.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/asset_mgmt_tagging/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.2/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.2/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.2/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.2/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.2/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.2/PKG-INFO
```

### Comparing `qualyspy-0.3.1/.vscode/launch.json` & `qualyspy-0.3.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/debug/dtd.txt` & `qualyspy-0.3.2/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/debug/output.txt` & `qualyspy-0.3.2/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/debug/parse_dtd.py` & `qualyspy-0.3.2/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/debug/quickscan.py` & `qualyspy-0.3.2/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/debug/remove_cookies.py` & `qualyspy-0.3.2/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/docs/Makefile` & `qualyspy-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/docs/make.bat` & `qualyspy-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/docs/source/conf.py` & `qualyspy-0.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/qualysapi.py` & `qualyspy-0.3.2/qualyspy/qualysapi.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/qutils.py` & `qualyspy-0.3.2/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/urls.json` & `qualyspy-0.3.2/qualyspy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/api_input.py` & `qualyspy-0.3.2/qualyspy/asset_mgmt_tagging/api_input.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.3.2/qualyspy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/asset_mgmt_tagging/tag.py` & `qualyspy-0.3.2/qualyspy/asset_mgmt_tagging/tag.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/assets/host_list.py` & `qualyspy-0.3.2/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/assets/host_list_detection.py` & `qualyspy-0.3.2/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/qualyspy/certview/certificate.py` & `qualyspy-0.3.2/qualyspy/certview/certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
     id: int
     uuid: str
     netbios_name: str
     name: str
     operating_system: str | None
     host_instances: list[Host_Instance]
     asset_interfaces: list[Asset_Interface] | None
-    primary_ip: pyd.IPvAnyAddress
+    primary_ip: pyd.IPvAnyAddress | None
 
     class Config:
         alias_generator = qutils.to_lower_camel
         orm_mode = True
         allow_population_by_field_name = True
 
 
@@ -271,15 +271,15 @@
     )
 
     certificate_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("certificate.id"))
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
         back_populates="assets", uselist=False
     )
     primary_ip: orm.Mapped[
-        ipaddress.IPv4Address | ipaddress.IPv6Address
+        ipaddress.IPv4Address | ipaddress.IPv6Address | None
     ] = orm.mapped_column("primary_ip", sa_pg.INET)
 
 
 ####################################################################################################
 # Certificate
 
 
@@ -375,22 +375,22 @@
 
 ####################################################################################################
 
 ####################################################################################################
 # Function input
 
 
-class Field_Value_Operator(pyd.BaseModel):
+class Field_Operator_Value(pyd.BaseModel):
     field: str
-    value: str
     operator: str
+    value: str
 
 
 class Filter(pyd.BaseModel):
-    filters: list[Field_Value_Operator]
+    filters: list[Field_Operator_Value]
     operation: str = "AND"
 
 
 class List_CertView_Certificates_V2_Input(pyd.BaseModel):
     filter: Filter | None = None
     page_number: int = 0
     page_size: int | None = None
@@ -429,25 +429,24 @@
                 c = Certificate.parse_obj(cert)
 
                 # subject.name somtimes includes null characters "\x00", even though the GUI doesn't
                 # show these.  I've opened a ticket with Qualys about it.  In the meanwhile, this
                 # will replace them with something PostgreSQL is happy with.
                 # Also other fields, apparently...
                 #
-                # Qualys claim to have fixed this, so commenting it out for now.
-                # c.subject.name = c.subject.name.replace("\x00", "\uFFFD")
-                # c.subject.locality = c.subject.locality.replace("\x00", "\uFFFD")
-                # c.subject.state = c.subject.state.replace("\x00", "\uFFFD")
+                c.subject.name = c.subject.name.replace("\x00", "\uFFFD")
+                c.subject.locality = c.subject.locality.replace("\x00", "\uFFFD")
+                c.subject.state = c.subject.state.replace("\x00", "\uFFFD")
 
                 certificates.append(c)
             return certificates
         else:
             return None
 
-    def call(
+    def __call__(
         self,
         params: List_CertView_Certificates_V2_Input = List_CertView_Certificates_V2_Input(),
     ) -> list[Certificate]:
         certificates: list[Certificate] = []
 
         while (new_certs := self.__call_once(params)) is not None:
             certificates.extend(new_certs)
```

### Comparing `qualyspy-0.3.1/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.3.2/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/.gitignore` & `qualyspy-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/LICENSE` & `qualyspy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.1/pyproject.toml` & `qualyspy-0.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.3.1/PKG-INFO` & `qualyspy-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

