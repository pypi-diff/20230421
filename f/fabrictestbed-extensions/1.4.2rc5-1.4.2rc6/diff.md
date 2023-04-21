# Comparing `tmp/fabrictestbed-extensions-1.4.2rc5.tar.gz` & `tmp/fabrictestbed-extensions-1.4.2rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.4.2rc5.tar", last modified: Mon Apr 17 16:00:46 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.4.2rc6.tar", last modified: Thu Apr 20 18:03:41 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.4.2rc5.tar` & `fabrictestbed-extensions-1.4.2rc6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-04-02 13:36:30.329332 fabrictestbed-extensions-1.4.2rc5/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-04-10 21:57:28.666104 fabrictestbed-extensions-1.4.2rc5/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-04-10 21:57:28.666104 fabrictestbed-extensions-1.4.2rc5/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc5/.gitignore
--rw-r--r--   0        0        0      666 2023-04-02 13:36:30.329332 fabrictestbed-extensions-1.4.2rc5/.readthedocs.yaml
--rw-r--r--   0        0        0     2326 2023-04-17 15:58:37.151208 fabrictestbed-extensions-1.4.2rc5/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc5/LICENSE
--rw-r--r--   0        0        0     4054 2023-04-10 21:57:28.670104 fabrictestbed-extensions-1.4.2rc5/README.md
--rw-r--r--   0        0        0      638 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc5/docs/Makefile
--rw-r--r--   0        0        0      799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc5/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc5/docs/source/conf.py
--rw-r--r--   0        0        0     8869 2023-02-17 15:17:40.022255 fabrictestbed-extensions-1.4.2rc5/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-04-10 21:57:28.670104 fabrictestbed-extensions-1.4.2rc5/docs/source/index.rst
--rw-r--r--   0        0        0      151 2023-04-17 15:58:37.151208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    20922 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    76799 2023-04-17 15:58:37.151208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5807 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    25679 2023-04-17 15:58:37.155208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    38588 2023-04-17 15:50:56.020260 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    94720 2023-04-17 15:58:37.155208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    34672 2023-04-10 21:57:48.078249 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81254 2023-04-17 15:58:37.159208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34231 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-04-02 13:36:30.333332 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-04-10 21:57:28.682104 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1304 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/pyproject.toml
--rwxr-xr-x   0        0        0      122 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc5/sphinx.sh
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc5/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-02-13 18:31:49.552350 fabrictestbed-extensions-1.4.2rc6/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-04-06 16:18:57.453917 fabrictestbed-extensions-1.4.2rc6/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-04-06 16:18:57.454239 fabrictestbed-extensions-1.4.2rc6/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1799 2022-08-18 16:55:06.303125 fabrictestbed-extensions-1.4.2rc6/.gitignore
+-rw-r--r--   0        0        0      666 2023-02-13 18:31:49.552528 fabrictestbed-extensions-1.4.2rc6/.readthedocs.yaml
+-rw-r--r--   0        0        0     2395 2023-04-20 18:01:14.627945 fabrictestbed-extensions-1.4.2rc6/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2022-08-18 16:55:06.303384 fabrictestbed-extensions-1.4.2rc6/LICENSE
+-rw-r--r--   0        0        0     4054 2023-04-06 16:18:57.455050 fabrictestbed-extensions-1.4.2rc6/README.md
+-rw-r--r--   0        0        0      638 2022-08-18 16:55:06.303668 fabrictestbed-extensions-1.4.2rc6/docs/Makefile
+-rw-r--r--   0        0        0      799 2022-08-18 16:55:06.303743 fabrictestbed-extensions-1.4.2rc6/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-02-13 18:31:49.552781 fabrictestbed-extensions-1.4.2rc6/docs/source/conf.py
+-rw-r--r--   0        0        0     8869 2022-10-28 15:15:07.136211 fabrictestbed-extensions-1.4.2rc6/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-04-06 16:18:57.455278 fabrictestbed-extensions-1.4.2rc6/docs/source/index.rst
+-rw-r--r--   0        0        0      151 2023-04-20 18:01:14.628067 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-02-13 18:31:49.553082 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-02-13 18:31:49.553270 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-02-13 18:31:49.553528 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-02-13 18:31:49.553650 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2022-08-18 16:55:06.304986 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-02-13 18:31:49.553839 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    21062 2023-04-20 18:01:14.628314 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    76799 2023-04-20 18:01:14.628593 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5807 2023-02-13 18:31:49.554628 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    25825 2023-04-20 18:01:14.628746 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    39140 2023-04-20 18:01:14.628864 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    95917 2023-04-20 18:01:14.629267 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    34672 2023-04-20 18:01:14.629639 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81904 2023-04-20 18:01:14.629937 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-02-13 18:31:49.555813 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2022-08-18 16:55:06.307676 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2022-08-18 16:55:06.307757 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2022-08-18 16:55:06.307862 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-02-13 18:31:49.555903 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-02-13 18:31:49.556039 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34231 2023-02-13 18:31:49.556263 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-02-13 18:31:49.556325 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-02-13 18:31:49.556445 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-02-13 18:31:49.556551 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-02-13 18:31:49.556711 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-02-13 18:31:49.556814 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-02-13 18:31:49.557045 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-02-13 18:31:49.557127 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-04-06 16:18:57.459146 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-02-13 18:31:49.557261 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-02-13 18:31:49.557349 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-02-13 18:31:49.557428 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-02-13 18:31:49.557517 fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1318 2023-04-20 18:01:14.630443 fabrictestbed-extensions-1.4.2rc6/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2022-08-18 16:55:06.309489 fabrictestbed-extensions-1.4.2rc6/sphinx.sh
+-rw-r--r--   0        0        0     5267 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc6/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.4.2rc5/.github/workflows/build.yml` & `fabrictestbed-extensions-1.4.2rc6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.4.2rc6/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/.github/workflows/test.yml` & `fabrictestbed-extensions-1.4.2rc6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/.gitignore` & `fabrictestbed-extensions-1.4.2rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/.readthedocs.yaml` & `fabrictestbed-extensions-1.4.2rc6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/CHANGELOG.md` & `fabrictestbed-extensions-1.4.2rc6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 - Support for post-boot configuration.  Files or directories can be
   uploaded post-boot, and commands can be submitted to be run
   post-boot.
 - A way to define layer-2 networks.
 - A way to query link and facility port information
 - Added function to make IP address of node publicly routable with external networking. `make_ip_publicly_routable`
 - Streamlined polling after a submit to reduce load on the control framework
+- Added easy, one-line "add_fabnet" functionality simple L3 networks
 
 ### Changed
 
 - Fablib now uses pyproject.toml for specifying packaging metadata
   instead of setup.py and friends (issue
   [#74](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/74)).
 - Make configure_nvme() more generic (PR
```

### Comparing `fabrictestbed-extensions-1.4.2rc5/LICENSE` & `fabrictestbed-extensions-1.4.2rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/README.md` & `fabrictestbed-extensions-1.4.2rc6/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/docs/Makefile` & `fabrictestbed-extensions-1.4.2rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/docs/make.bat` & `fabrictestbed-extensions-1.4.2rc6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/docs/source/conf.py` & `fabrictestbed-extensions-1.4.2rc6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/docs/source/fablib.rst` & `fabrictestbed-extensions-1.4.2rc6/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/docs/source/index.rst` & `fabrictestbed-extensions-1.4.2rc6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,30 +314,34 @@
         :type node: Node
         :param fim_component: the FIM component this object represents
         :type fim_component: FIMComponent
         """
         super().__init__()
         self.fim_component = fim_component
         self.node = node
+        self.interfaces = None
 
     def get_interfaces(self) -> List[Interface]:
         """
         Gets the interfaces attached to this fablib component's FABRIC component.
 
         :return: a list of the interfaces on this component.
         :rtype: List[Interface]
         """
 
         from fabrictestbed_extensions.fablib.interface import Interface
 
-        ifaces = []
-        for fim_interface in self.get_fim_component().interface_list:
-            ifaces.append(Interface(component=self, fim_interface=fim_interface))
+        if not self.interfaces:
+            self.interfaces = []
+            for fim_interface in self.get_fim_component().interface_list:
+                self.interfaces.append(
+                    Interface(component=self, fim_interface=fim_interface)
+                )
 
-        return ifaces
+        return self.interfaces
 
     def get_fim_component(self) -> FimComponent:
         """
         Not recommended for most users.
 
         GGets the FABRIC component this fablib component represents. This method
         is used to access data at a lower level than FABlib.
```

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         :param fim_interface: the FABRIC information model interface to set on this fablib interface
         :type fim_interface: FimInterface
         """
         super().__init__()
         self.fim_interface = fim_interface
         self.component = component
         self.network = None
+        self.dev = None
 
     def get_fablib_manager(self):
         return self.get_slice().get_fablib_manager()
 
     def __str__(self):
         """
         Creates a tabulated string describing the properties of the interface.
@@ -334,20 +335,24 @@
         """
         Gets json output of 'ip addr list' for the interface.
 
         :return: device description
         :rtype: Dict
         """
 
-        ip_addr_list_json = self.get_node().ip_addr_list(output="json")
+        if not self.dev:
+            ip_addr_list_json = self.get_node().ip_addr_list(output="json")
 
-        mac = self.get_mac()
-        for dev in ip_addr_list_json:
-            if str(dev["address"].upper()) == str(mac.upper()):
-                return dev
+            mac = self.get_mac()
+            for dev in ip_addr_list_json:
+                if str(dev["address"].upper()) == str(mac.upper()):
+                    self.dev = dev
+                    return dev
+        else:
+            return self.dev
 
         return None
 
     def get_physical_os_interface(self):
         """
         Not intended for API use
         """
```

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/network_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author: Paul Ruth (pruth@renci.org)
 from __future__ import annotations
+
 import logging
 
 from tabulate import tabulate
 from typing import List
 
 from typing import TYPE_CHECKING
 
@@ -494,18 +495,25 @@
         :param fim_network_service: the FIM network service to set as instance state
         :type fim_network_service: FIMNetworkService
         """
         super().__init__()
         self.fim_network_service = fim_network_service
         self.slice = slice
 
+        self.interfaces = None
+
         try:
-            self.sliver = slice.get_sliver(reservation_id=self.get_reservation_id())
+            if self.slice.isStable():
+                self.sliver = self.slice.get_sliver(
+                    reservation_id=self.get_reservation_id()
+                )
         except:
-            self.sliver = None
+            pass
+
+        self.sliver = None
 
     def __str__(self):
         """
         Creates a tabulated string describing the properties of the network service.
 
         Intended for printing network service information.
 
@@ -684,14 +692,18 @@
             return self.get_fim().get_property(pname="type")
             # return self.get_sliver().fim_sliver.resource_type
         except Exception as e:
             logging.warning(f"Failed to get type: {e}")
             return None
 
     def get_sliver(self) -> OrchestratorSliver:
+        if not self.sliver and self.slice.isStable():
+            self.sliver = self.slice.get_sliver(
+                reservation_id=self.get_reservation_id()
+            )
         return self.sliver
 
     def get_fim_network_service(self) -> FimNetworkService:
         """
         Not recommended for most users.
 
         Gets the FABRIC network service this instance represents.
@@ -854,20 +866,23 @@
     def get_interfaces(self) -> List[Interface]:
         """
         Gets the interfaces on this network service.
 
         :return: the interfaces on this network service
         :rtype: List[Interfaces]
         """
-        interfaces = []
-        for interface in self.get_fim_network_service().interface_list:
-            logging.debug(f"interface: {interface}")
-            interfaces.append(self.get_slice().get_interface(name=interface.name))
+        if not self.interfaces:
+            self.interfaces = []
+            for interface in self.get_fim_network_service().interface_list:
+                logging.debug(f"interface: {interface}")
+                self.interfaces.append(
+                    self.get_slice().get_interface(name=interface.name)
+                )
 
-        return interfaces
+        return self.interfaces
 
     def get_interface(self, name: str = None) -> Interface or None:
         """
         Gets a particular interface on this network service.
 
         :param name: the name of the interface to search for
         :type name: str
@@ -933,14 +948,16 @@
         new_interfaces.append(interface)
 
         curr_nstype = self.get_type()
         if self.get_layer() == NSLayer.L2:
             new_nstype = NetworkService.calculate_l2_nstype(interfaces=new_interfaces)
             if curr_nstype != new_nstype:
                 self.__replace_network_service(new_nstype)
+            else:
+                self.get_fim().connect_interface(interface=interface.get_fim())
         elif self.get_layer() == NSLayer.L3 and self.is_instantiated():
             if interface.get_site() != self.get_site():
                 raise Exception("L3 networks can only include nodes from one site")
 
         if "addr" in iface_fablib_data:
             addr = iface_fablib_data["addr"]
         else:
@@ -955,15 +972,16 @@
             if addr:
                 iface_fablib_data["addr"] = str(self.allocate_ip(addr))
             elif auto:
                 iface_fablib_data["addr"] = str(self.allocate_ip())
 
         interface.set_fablib_data(iface_fablib_data)
 
-        self.get_fim().connect_interface(interface=interface.get_fim())
+        if self.get_layer() == NSLayer.L3:
+            self.get_fim().connect_interface(interface=interface.get_fim())
 
     def remove_interface(self, interface: Interface):
         iface_fablib_data = interface.get_fablib_data()
 
         self.free_ip(interface.get_ip_addr())
 
         interfaces = self.get_interfaces()
```

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,20 @@
         # Try to set the username.
         try:
             self.set_username()
         except:
             self.username = None
 
         try:
-            self.sliver = slice.get_sliver(reservation_id=self.get_reservation_id())
+            if slice.isStable():
+                self.sliver = slice.get_sliver(reservation_id=self.get_reservation_id())
         except:
-            self.sliver = None
+            pass
+
+        self.sliver = None
 
         logging.getLogger("paramiko").setLevel(logging.WARNING)
 
     def get_fablib_manager(self):
         return self.slice.get_fablib_manager()
 
     def __str__(self):
@@ -1171,15 +1174,16 @@
         :return: a tuple of  (stdout[Sting],stderr[String])
         :rtype: Tuple
         :raise Exception: if management IP is invalid
         """
         import logging
 
         logging.debug(
-            f"execute node: {self.get_name()}, management_ip: {self.get_management_ip()}, command: {command}"
+            f"execute node: {self.get_name()}, management_ip: {self.get_management_ip()}, command: {command}",
+            stack_info=True,
         )
 
         if not self.get_reservation_state() == "Active":
             logging.debug(
                 f"Execute failed. Node {self.get_name()} in state {self.get_reservation_state()}"
             )
 
@@ -2668,7 +2672,40 @@
             self.set_instantiated(True)
             self.run_post_boot_tasks()
 
         if self.run_update_commands():
             self.run_post_update_commands()
 
         return "Done"
+
+    def add_fabnet(
+        self, name="FABNET", net_type="IPv4", nic_type="NIC_Basic", routes=None
+    ):
+        site = self.get_site()
+
+        net_name = f"{name}_{net_type}_{site}"
+
+        net = self.get_slice().get_network(net_name)
+        if not net:
+            net = self.get_slice().add_l3network(name=net_name, type=net_type)
+
+        # Add ccontrol plane network to node1
+        iface = self.add_component(
+            model=nic_type, name=f"{net_name}_nic"
+        ).get_interfaces()[0]
+        net.add_interface(iface)
+        iface.set_mode("auto")
+
+        if routes:
+            for route in routes:
+                self.add_route(subnet=route, next_hop=net.get_gateway())
+        else:
+            if net_type == "IPv4":
+                self.add_route(
+                    subnet=self.get_fablib_manager().FABNETV4_SUBNET,
+                    next_hop=net.get_gateway(),
+                )
+            elif net_type == "IPv6":
+                self.add_route(
+                    subnet=self.get_fablib_manager().FABNETV6_SUBNET,
+                    next_hop=net.get_gateway(),
+                )
```

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/fablib/slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
         self.slice_name = name
         self.sm_slice = None
         self.slice_id = None
         self.topology = None
         self.slivers = []
         self.fablib_manager = fablib_manager
 
+        self.nodes = None
+        self.interfaces = None
+
         self.slice_key = fablib_manager.get_default_slice_key()
 
         self.update_topology_count = 0
         self.update_slivers_count = 0
         self.update_slice_count = 0
         self.update_count = 0
 
@@ -630,14 +633,15 @@
     def get_sliver(self, reservation_id: str) -> OrchestratorSliver:
         slivers = self.get_slivers()
         sliver = list(filter(lambda x: x.sliver_id == reservation_id, slivers))[0]
         return sliver
 
     def get_slivers(self) -> List[OrchestratorSliver]:
         if not self.slivers:
+            logging.debug(f"get_slivers", stack_info=False)
             self.update_slivers()
 
         return self.slivers
 
     def update(self):
         """
         (re)Query the FABRIC services for updated information about this slice.
@@ -653,14 +657,16 @@
             logging.warning(f"slice.update_slice failed: {e}")
 
         try:
             self.update_slivers()
         except Exception as e:
             logging.warning(f"slice.update_slivers failed: {e}")
 
+        self.nodes = None
+        self.interfaces = None
         self.update_topology()
 
         if self.get_state() == "ModifyOK":
             self.modify_accept()
 
     def get_private_key_passphrase(self) -> str:
         """
@@ -876,14 +882,17 @@
         :param interfaces: a list of interfaces to build the network with
         :type interfaces: List[Interface]
         :param type: optional L2 network type "L2Bridge", "L2STS", or "L2PTP"
         :type type: String
         :return: a new L2 network service
         :rtype: NetworkService
         """
+        self.nodes = None
+        self.interfaces = None
+
         network_service = NetworkService.new_l2network(
             slice=self, name=name, interfaces=interfaces, type=type, user_data=user_data
         )
         if subnet:
             network_service.set_subnet(subnet)
 
         if gateway:
@@ -934,14 +943,17 @@
         :param interfaces: a list of interfaces to build the network with
         :type interfaces: List[Interface]
         :param type: L3 network type "IPv4" or "IPv6"
         :type type: String
         :return: a new L3 network service
         :rtype: NetworkService
         """
+        self.nodes = None
+        self.interfaces = None
+
         return NetworkService.new_l3network(
             slice=self,
             name=name,
             interfaces=interfaces,
             type=type,
             user_data=user_data,
         )
@@ -1022,14 +1034,17 @@
 
         if image:
             node.set_image(image)
 
         if host:
             node.set_host(host)
 
+        self.nodes = None
+        self.interfaces = None
+
         return node
 
     def get_object_by_reservation(
         self, reservation_id: str
     ) -> Union[Node, NetworkService, Interface, None]:
         """
         Gets an object associated with this slice by its reservation ID.
@@ -1129,25 +1144,26 @@
     def get_nodes(self) -> List[Node]:
         """
         Gets a list of all nodes in this slice.
 
         :return: a list of fablib nodes
         :rtype: List[Node]
         """
-        return_nodes = []
 
-        # fails for topology that does not have nodes
-        try:
-            for node_name, node in self.get_fim_topology().nodes.items():
-                return_nodes.append(Node.get_node(self, node))
-        except Exception as e:
-            logging.info(f"get_nodes: exception {e}")
-            # traceback.print_exc()
-            pass
-        return return_nodes
+        if not self.nodes:
+            self.nodes = []
+            # fails for topology that does not have nodes
+            try:
+                for node_name, node in self.get_fim_topology().nodes.items():
+                    self.nodes.append(Node.get_node(self, node))
+            except Exception as e:
+                logging.info(f"get_nodes: exception {e}")
+                pass
+
+        return self.nodes
 
     def get_node(self, name: str) -> Node:
         """
         Gets a node from the slice by name.
 
         :param name: Name of the node
         :type name: String
@@ -1163,23 +1179,24 @@
     def get_interfaces(self) -> List[Interface]:
         """
         Gets all interfaces in this slice.
 
         :return: a list of interfaces on this slice
         :rtype: List[Interface]
         """
-        interfaces = []
-        for node in self.get_nodes():
-            logging.debug(f"Getting interfaces for node {node.get_name()}")
-            for interface in node.get_interfaces():
-                logging.debug(
-                    f"Getting interface {interface.get_name()} for node {node.get_name()}: \n{interface}"
-                )
-                interfaces.append(interface)
-        return interfaces
+        if not self.interfaces:
+            self.interfaces = []
+            for node in self.get_nodes():
+                logging.debug(f"Getting interfaces for node {node.get_name()}")
+                for interface in node.get_interfaces():
+                    logging.debug(
+                        f"Getting interface {interface.get_name()} for node {node.get_name()}: \n{interface}"
+                    )
+                    self.interfaces.append(interface)
+        return self.interfaces
 
     def get_interface(self, name: str = None) -> Interface:
         """
         Gets a particular interface from this slice.
 
         :param name: the name of the interface to search for
         :type name: str
@@ -1690,30 +1707,32 @@
         from IPython.display import clear_output
         import time
 
         logging.debug(f"wait_jupyter: slice {self.get_name()}")
 
         start = time.time()
 
-        if len(self.get_interfaces()) > 0:
-            hasNetworks = True
-        else:
-            hasNetworks = False
+        # if len(self.get_interfaces()) > 0:
+        #    hasNetworks = True
+        # else:
+        #    hasNetworks = False
 
         count = 0
         # while not self.isStable():
         # while not self.isReady():
         while True:
             if time.time() > start + timeout:
                 raise Exception(f"Timeout {timeout} sec exceeded in Jupyter wait")
 
             time.sleep(interval)
+
             stable = False
             self.update_slice()
             self.update_slivers()
+
             if self.isStable():
                 stable = True
                 self.update()
                 if len(self.get_interfaces()) > 0:
                     hasNetworks = True
                 else:
                     hasNetworks = False
@@ -2139,18 +2158,24 @@
             if sliver.sliver_type == "NetworkServiceSliver":
                 type = "network"
             elif sliver.sliver_type == "NodeSliver":
                 type = "node"
             else:
                 type = sliver.sliver_type
 
+            if "Site" in sliver.sliver:
+                site = sliver.sliver["Site"]
+            else:
+                site = ""
+
             table.append(
                 {
                     "id": sliver.sliver_id,
                     "name": sliver.sliver["Name"],
+                    "site": site,
                     "type": type,
                     "state": sliver.state,
                     "error": error,
                 }
             )
 
             logging.debug(sliver)
@@ -2158,14 +2183,15 @@
 
         logging.debug(f"table: {table}")
 
         if pretty_names:
             pretty_names_dict = {
                 "name": "Name",
                 "id": "ID",
+                "site": "Site",
                 "type": "Type",
                 "state": "State",
                 "error": "Error",
             }
         else:
             pretty_names_dict = {}
```

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.4.2rc6/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc5/pyproject.toml` & `fabrictestbed-extensions-1.4.2rc6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "ipycytoscape",
     "tabulate",
     "fabrictestbed==1.4.4",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
+    "ipython"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `fabrictestbed-extensions-1.4.2rc5/PKG-INFO` & `fabrictestbed-extensions-1.4.2rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.4.2rc5
+Version: 1.4.2rc6
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
 Requires-Dist: fabrictestbed==1.4.4
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: ipython
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: ChangeLog, https://github.com/fabric-testbed/fabrictestbed-extensions/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://fabric-fablib.readthedocs.io/
 Project-URL: Homepage, https://fabric-testbed.net/
```

