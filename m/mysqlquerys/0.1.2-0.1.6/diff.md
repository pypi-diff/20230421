# Comparing `tmp/mysqlquerys-0.1.2.tar.gz` & `tmp/mysqlquerys-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlquerys-0.1.2.tar", last modified: Fri May 27 06:24:17 2022, max compression
+gzip compressed data, was "mysqlquerys-0.1.6.tar", last modified: Fri Apr 21 15:28:33 2023, max compression
```

## Comparing `mysqlquerys-0.1.2.tar` & `mysqlquerys-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-05-27 06:24:17.048694 mysqlquerys-0.1.2/
--rw-rw-rw-   0        0        0       24 2022-02-14 15:35:33.000000 mysqlquerys-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      680 2022-05-27 06:24:17.048694 mysqlquerys-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      174 2022-02-14 09:59:42.000000 mysqlquerys-0.1.2/README.md
--rw-rw-rw-   0        0        0     1073 2022-02-14 15:35:11.000000 mysqlquerys-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0      741 2022-05-27 06:24:17.048694 mysqlquerys-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-05-27 06:07:35.000000 mysqlquerys-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-27 06:24:17.029971 mysqlquerys-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2022-05-27 06:24:17.043506 mysqlquerys-0.1.2/src/mysqlquerys/
--rw-rw-rw-   0        0        0        0 2022-02-14 09:59:42.000000 mysqlquerys-0.1.2/src/mysqlquerys/__init__.py
--rw-rw-rw-   0        0        0     1615 2022-02-14 15:20:50.000000 mysqlquerys-0.1.2/src/mysqlquerys/config.py
--rw-rw-rw-   0        0        0    18517 2022-02-14 15:26:04.000000 mysqlquerys-0.1.2/src/mysqlquerys/connect.py
-drwxrwxrwx   0        0        0        0 2022-05-27 06:24:17.044839 mysqlquerys-0.1.2/src/mysqlquerys.egg-info/
--rw-rw-rw-   0        0        0      680 2022-05-27 06:24:16.000000 mysqlquerys-0.1.2/src/mysqlquerys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2022-05-27 06:24:17.000000 mysqlquerys-0.1.2/src/mysqlquerys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-27 06:24:16.000000 mysqlquerys-0.1.2/src/mysqlquerys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-05-27 06:24:16.000000 mysqlquerys-0.1.2/src/mysqlquerys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-05-27 06:24:16.000000 mysqlquerys-0.1.2/src/mysqlquerys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:33.495576 mysqlquerys-0.1.6/
+-rw-rw-rw-   0        0        0       24 2022-02-14 15:35:33.000000 mysqlquerys-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      680 2023-04-21 15:28:33.495576 mysqlquerys-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2022-02-14 09:59:42.000000 mysqlquerys-0.1.6/README.md
+-rw-rw-rw-   0        0        0       70 2023-04-21 14:52:22.000000 mysqlquerys-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0      741 2023-04-21 15:28:33.496700 mysqlquerys-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-05-27 06:07:35.000000 mysqlquerys-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:33.483543 mysqlquerys-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:33.491579 mysqlquerys-0.1.6/src/mysqlquerys/
+-rw-rw-rw-   0        0        0        0 2022-11-14 10:44:12.000000 mysqlquerys-0.1.6/src/mysqlquerys/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-04-21 13:18:36.000000 mysqlquerys-0.1.6/src/mysqlquerys/config.py
+-rw-rw-rw-   0        0        0    18831 2023-04-21 13:51:26.000000 mysqlquerys-0.1.6/src/mysqlquerys/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:28:33.494578 mysqlquerys-0.1.6/src/mysqlquerys.egg-info/
+-rw-rw-rw-   0        0        0      680 2023-04-21 15:28:33.000000 mysqlquerys-0.1.6/src/mysqlquerys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-21 15:28:33.000000 mysqlquerys-0.1.6/src/mysqlquerys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 15:28:33.000000 mysqlquerys-0.1.6/src/mysqlquerys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-21 15:28:33.000000 mysqlquerys-0.1.6/src/mysqlquerys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 15:28:33.000000 mysqlquerys-0.1.6/src/mysqlquerys.egg-info/top_level.txt
```

### Comparing `mysqlquerys-0.1.2/PKG-INFO` & `mysqlquerys-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlquerys
-Version: 0.1.2
+Version: 0.1.6
 Summary: Query-uri personale pentru a scrie in MySQL
 Home-page: https://github.com/pypa/sampleproject
 Author: Radu M.
 Author-email: radu.mircea@yahoo.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysqlquerys-0.1.2/setup.cfg` & `mysqlquerys-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7973 716c 7175 6572 7973 0d0a   = mysqlquerys..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 320d  version = 0.1.2.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 360d  version = 0.1.6.
 00000030: 0a61 7574 686f 7220 3d20 5261 6475 204d  .author = Radu M
 00000040: 2e0d 0a61 7574 686f 725f 656d 6169 6c20  ...author_email 
 00000050: 3d20 7261 6475 2e6d 6972 6365 6140 7961  = radu.mircea@ya
 00000060: 686f 6f2e 636f 6d0d 0a64 6573 6372 6970  hoo.com..descrip
 00000070: 7469 6f6e 203d 2051 7565 7279 2d75 7269  tion = Query-uri
 00000080: 2070 6572 736f 6e61 6c65 2070 656e 7472   personale pentr
 00000090: 7520 6120 7363 7269 6520 696e 204d 7953  u a scrie in MyS
```

### Comparing `mysqlquerys-0.1.2/src/mysqlquerys/connect.py` & `mysqlquerys-0.1.6/src/mysqlquerys/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-import sys
 import mysql.connector
 import traceback
+import sys
 import csv
 from datetime import datetime
 import json
-from MySQLquerys.config import config
+from mysqlquerys.config import config
 
 
 class DbConnection:
     def __init__(self, ini_file):
         self.iniFile = ini_file
         try:
-            print('reading configuration parameters from {}'.format(self.iniFile))
             params = config(self.iniFile)
-            print('successfully')
-
-            print('establishing connection to data base'.format(self.iniFile))
             self.connection = mysql.connector.connect(**params)
-            print('successfully')
         except Exception as err:
-            print(traceback.format_exc())
+            print(err)
+            print(traceback.print_exc())
 
     @property
     def version(self):
         cursor = self.connection.cursor()
         cursor.execute('SELECT version()')
         db_version = cursor.fetchone()
         cursor.close()
@@ -157,15 +153,16 @@
         colNames = ['Field', 'Type', 'Null', 'Key', 'Default', 'Extra']
         cursor = self.connection.cursor()
         cursor.execute(query)
         res = cursor.fetchall()
         cols = {}
         for col in res:
             colName, colType, null, key, default, extra = col
-            colType = str(colType.decode("utf-8"))
+            if isinstance(colType, bytes):
+                colType = str(colType.decode("utf-8"))
             cols[colName] = [colType, null, key, default, extra]
         cursor.close()
         return cols
 
     @property
     def noOfRows(self):
         query = 'SELECT * FROM {}'.format(self.table_name)
@@ -490,18 +487,28 @@
         values = []
         for i in records:
             values.append(i)
         return values
 
 
 if __name__ == '__main__':
-    # try:
-    iniFile = r"D:\Python\MySQL\database.ini"
+    # iniFile = r"D:\Python\MySQL\database.ini"
+    iniFile = r"D:\Python\MySQL\web_db.ini"
     db = DbConnection(iniFile)
-
     # print(db.version)
-    # db = DataBase(iniFile, 'myfolderstructure')
+    # db = DataBase(iniFile, 'heroku_6ed6d828b97b626')
     # print(db.tables)
-    # table = Table(iniFile, 'myfolderstructure', 'apartament')
-    # print(table.columnsNames)
+    table = Table(iniFile, 'heroku_6ed6d828b97b626', 'apartament')
+    # table = Table(iniFile, 'cheltuieli', 'apartament')
+    print(table.columnsProperties)
+    #
+    # try:
+    #     iniFile = r"D:\Python\MySQL\database.ini"
+    #     iniFile = r"D:\Python\MySQL\web_db.ini"
+    #     db = DbConnection(iniFile)
+    #     print(db.version)
+    #     db = DataBase(iniFile, 'heroku_6ed6d828b97b626')
+    #     print(db.tables)
+    #     table = Table(iniFile, 'heroku_6ed6d828b97b626', 'apartament')
+    #     print(table.columnsProperties)
     # except Exception as error:
-    #     print(traceback.format_exc())
+    #     print(error)
```

### Comparing `mysqlquerys-0.1.2/src/mysqlquerys.egg-info/PKG-INFO` & `mysqlquerys-0.1.6/src/mysqlquerys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlquerys
-Version: 0.1.2
+Version: 0.1.6
 Summary: Query-uri personale pentru a scrie in MySQL
 Home-page: https://github.com/pypa/sampleproject
 Author: Radu M.
 Author-email: radu.mircea@yahoo.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

