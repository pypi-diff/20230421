# Comparing `tmp/dctrackclient-0.2.1.tar.gz` & `tmp/dctrackclient-0.2.2.tar.gz`

## Comparing `dctrackclient-0.2.1.tar` & `dctrackclient-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/.github/workflows/doc.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/LICENSE
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 dctrackclient-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 dctrackclient-0.2.2/.github/workflows/doc.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 dctrackclient-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 dctrackclient-0.2.2/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 dctrackclient-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5978 2020-02-02 00:00:00.000000 dctrackclient-0.2.2/README.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 dctrackclient-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 dctrackclient-0.2.2/PKG-INFO
```

### Comparing `dctrackclient-0.2.1/.github/workflows/python-publish.yml` & `dctrackclient-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.2.1/src/dcTrackClient/__init__.py` & `dctrackclient-0.2.2/src/dcTrackClient/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -107,7 +107,37 @@
     def deleteConnector(self, ids: list[int]):
         """Delete one or more Connector records."""
         return self.__request('POST', '/api/v2/settings/connectors/delete', ids)
 
     def searchConnectors(self, data: dict, pageNumber: int, pageSize: int, usedCount: bool):
         """Retrieve a List of Connectors."""
         return self.__request('POST', '/api/v2/settings/connectors/quicksearch?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&usedCount=' + str(usedCount).lower(), data)
+
+    # Item Ports
+
+    def createDataPorts(self, itemId: int, data: dict):
+        """Use the REST API to create data ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item."""
+        return self.__request('POST', '/api/v1/items/' + str(itemId) + '/dataports/', data)
+
+    def updateDataPorts(self, itemId: int, portId: int, data: dict):
+        """Update an item's data port details using the REST API. To do this, specify the item and data port ID, and provide the updated parameter value(s)."""
+        return self.__request('PUT', '/api/v1/items/' + str(itemId) + '/dataports/' + str(portId), data)
+
+    def deleteDataPorts(self, itemId: int, portId: int):
+        """Delete an item's data port using the REST API by specifying the item ID and data port ID."""
+        return self.__request('DELETE', '/api/v1/items/' + str(itemId) + '/dataports/' + str(portId))
+
+    def getDataPorts(self, itemId: int):
+        """Use the REST API to retrieve details from all data ports on an item."""
+        return self.__request('GET', '/api/v1/items/' + str(itemId) + '/dataports/')
+
+    def getDataPort(self, itemId: int, portId: int):
+        """Use the REST API to read the details of an item's data port. To do this, specify the item and item data port ID."""
+        return self.__request('GET', '/api/v1/items/' + str(itemId) + '/dataports/' + str(portId))
+
+    def updatePowerPort(self, itemId: int, portId: int, data: dict, proceedOnWarning: bool = True):
+        """Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item."""
+        return self.__request('PUT', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '?proceedOnWarning=' + str(proceedOnWarning), data)
+
+    def compatibleConnector(self, itemId: int, portId: int, connectorId: int):
+        """Use the REST API to determine if a Connector is compatible with a specific Power Port."""
+        return self.__request('GET', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '/connectors/' + str(connectorId) + '/isCompatible')
```

### Comparing `dctrackclient-0.2.1/LICENSE` & `dctrackclient-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.2.1/README.md` & `dctrackclient-0.2.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -158,7 +158,35 @@
 def deleteConnector(self, ids: list[int]):
 ```
 > Delete one or more Connector records.
 ```py
 def searchConnectors(self, data: dict, pageNumber: int, pageSize: int, usedCount: bool):
 ```
 > Retrieve a List of Connectors.
+```py
+def createDataPorts(self, itemId: int, data: dict):
+```
+> Use the REST API to create data ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item.
+```py
+def updateDataPorts(self, itemId: int, portId: int, data: dict):
+```
+> Update an item's data port details using the REST API. To do this, specify the item and data port ID, and provide the updated parameter value(s).
+```py
+def deleteDataPorts(self, itemId: int, portId: int):
+```
+> Delete an item's data port using the REST API by specifying the item ID and data port ID.
+```py
+def getDataPorts(self, itemId: int):
+```
+> Use the REST API to retrieve details from all data ports on an item.
+```py
+def getDataPort(self, itemId: int, portId: int):
+```
+> Use the REST API to read the details of an item's data port. To do this, specify the item and item data port ID.
+```py
+def updatePowerPort(self, itemId: int, portId: int, data: dict, proceedOnWarning: bool = True):
+```
+> Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item.
+```py
+def compatibleConnector(self, itemId: int, portId: int, connectorId: int):
+```
+> Use the REST API to determine if a Connector is compatible with a specific Power Port.
```

### Comparing `dctrackclient-0.2.1/pyproject.toml` & `dctrackclient-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.2.1/PKG-INFO` & `dctrackclient-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -172,7 +172,35 @@
 def deleteConnector(self, ids: list[int]):
 ```
 > Delete one or more Connector records.
 ```py
 def searchConnectors(self, data: dict, pageNumber: int, pageSize: int, usedCount: bool):
 ```
 > Retrieve a List of Connectors.
+```py
+def createDataPorts(self, itemId: int, data: dict):
+```
+> Use the REST API to create data ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item.
+```py
+def updateDataPorts(self, itemId: int, portId: int, data: dict):
+```
+> Update an item's data port details using the REST API. To do this, specify the item and data port ID, and provide the updated parameter value(s).
+```py
+def deleteDataPorts(self, itemId: int, portId: int):
+```
+> Delete an item's data port using the REST API by specifying the item ID and data port ID.
+```py
+def getDataPorts(self, itemId: int):
+```
+> Use the REST API to retrieve details from all data ports on an item.
+```py
+def getDataPort(self, itemId: int, portId: int):
+```
+> Use the REST API to read the details of an item's data port. To do this, specify the item and item data port ID.
+```py
+def updatePowerPort(self, itemId: int, portId: int, data: dict, proceedOnWarning: bool = True):
+```
+> Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item.
+```py
+def compatibleConnector(self, itemId: int, portId: int, connectorId: int):
+```
+> Use the REST API to determine if a Connector is compatible with a specific Power Port.
```

