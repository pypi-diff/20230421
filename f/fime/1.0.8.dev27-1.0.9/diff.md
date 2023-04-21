# Comparing `tmp/fime-1.0.8.dev27-py3-none-any.whl.zip` & `tmp/fime-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 26146 bytes, number of entries: 22
+Zip file size: 26051 bytes, number of entries: 22
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-17 19:59 fime/__init__.py
 -rw-r--r--  2.0 unx     1610 b- defN 21-Nov-18 21:12 fime/config.py
 -rw-r--r--  2.0 unx    14840 b- defN 21-Dec-02 17:50 fime/data.py
 -rw-r--r--  2.0 unx       41 b- defN 21-Nov-17 12:20 fime/exceptions.py
 -rw-r--r--  2.0 unx     2784 b- defN 21-Dec-02 17:46 fime/import_task.py
--rw-r--r--  2.0 unx     5407 b- defN 21-Dec-02 17:41 fime/main.py
+-rw-r--r--  2.0 unx     5408 b- defN 22-Jan-12 16:41 fime/main.py
 -rw-r--r--  2.0 unx     3562 b- defN 21-Nov-30 18:04 fime/progressindicator.py
 -rw-r--r--  2.0 unx     8825 b- defN 21-Dec-02 17:55 fime/report.py
 -rw-r--r--  2.0 unx     5695 b- defN 21-Nov-30 19:55 fime/task_completer.py
 -rw-r--r--  2.0 unx     3038 b- defN 21-Dec-02 17:47 fime/task_edit.py
 -rw-r--r--  2.0 unx     1234 b- defN 21-Nov-28 19:29 fime/test.py
 -rw-r--r--  2.0 unx     1403 b- defN 21-Nov-30 18:04 fime/util.py
 -rw-r--r--  2.0 unx    14715 b- defN 21-Dec-02 17:54 fime/worklog.py
 -rw-r--r--  2.0 unx     8546 b- defN 21-Dec-02 17:51 fime/worklog_rest.py
 -rw-r--r--  2.0 unx    10197 b- defN 21-Nov-30 18:04 fime/icons/__init__.py
--rw-r--r--  2.0 unx     1510 b- defN 21-Dec-02 17:55 fime-1.0.8.dev27.dist-info/LICENSE
--rw-r--r--  2.0 unx     1726 b- defN 21-Dec-02 17:55 fime-1.0.8.dev27.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-02 17:55 fime-1.0.8.dev27.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 21-Dec-02 17:55 fime-1.0.8.dev27.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 21-Dec-02 17:55 fime-1.0.8.dev27.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Dec-02 17:55 fime-1.0.8.dev27.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     1690 b- defN 21-Dec-02 17:55 fime-1.0.8.dev27.dist-info/RECORD
-22 files, 86958 bytes uncompressed, 23448 bytes compressed:  73.0%
+-rw-r--r--  2.0 unx     1510 b- defN 22-Jan-12 16:42 fime-1.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1720 b- defN 22-Jan-12 16:42 fime-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jan-12 16:42 fime-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 22-Jan-12 16:42 fime-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 22-Jan-12 16:42 fime-1.0.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 22-Jan-12 16:42 fime-1.0.9.dist-info/zip-safe
+?rw-rw-r--  2.0 unx     1648 b- defN 22-Jan-12 16:42 fime-1.0.9.dist-info/RECORD
+22 files, 86911 bytes uncompressed, 23437 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -39,29 +39,29 @@
 
 Filename: fime/worklog_rest.py
 Comment: 
 
 Filename: fime/icons/__init__.py
 Comment: 
 
-Filename: fime-1.0.8.dev27.dist-info/LICENSE
+Filename: fime-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: fime-1.0.8.dev27.dist-info/METADATA
+Filename: fime-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: fime-1.0.8.dev27.dist-info/WHEEL
+Filename: fime-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: fime-1.0.8.dev27.dist-info/entry_points.txt
+Filename: fime-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: fime-1.0.8.dev27.dist-info/top_level.txt
+Filename: fime-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fime-1.0.8.dev27.dist-info/zip-safe
+Filename: fime-1.0.9.dist-info/zip-safe
 Comment: 
 
-Filename: fime-1.0.8.dev27.dist-info/RECORD
+Filename: fime-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fime/main.py

```diff
@@ -102,15 +102,15 @@
         self.menu.clear()
         add_tasks(self.tasks.tasks)
 
         self.menu.addSeparator()
         already_taken = (len(self.tasks.tasks) + 4) * action_height
         available_space = get_screen_height(self.menu) * 0.8 - already_taken
         jira_entry_count = int(available_space // action_height)
-        add_tasks(self.tasks.jira_tasks[:jira_entry_count])
+        add_tasks(self.tasks.jira_tasks[-jira_entry_count:])
 
         self.menu.addSeparator()
         add_tasks(["Pause"])
         if self.active_task == "Nothing":
             add_tasks(["Nothing"])
 
         self.menu.addSeparator()
```

## Comparing `fime-1.0.8.dev27.dist-info/LICENSE` & `fime-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fime-1.0.8.dev27.dist-info/METADATA` & `fime-1.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fime
-Version: 1.0.8.dev27
+Version: 1.0.9
 Summary: Simple time tracking app written with Python and Qt
 Home-page: https://git.faerb.it/faerbit/fime
 Author: Faerbit
 Author-email: faerbit@posteo.net
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `fime-1.0.8.dev27.dist-info/RECORD` & `fime-1.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 fime/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fime/config.py,sha256=5EhZ0Q_n8NUPXzxQ8bHKMDubk60HT32AnQE-p9k8Qz0,1610
 fime/data.py,sha256=mbV2GXsIY_k4cKv8rSKYA8gO5GLYYTBsvyq9wu9AgUo,14840
 fime/exceptions.py,sha256=W_-XKL--Y-4fXjkkMNgZ95LLKefH2TkLhbggJOw5mKw,41
 fime/import_task.py,sha256=6tSTUUVsdRjxOUsGQ0cnbLESJKWs-KQYVSHTrq7MJic,2784
-fime/main.py,sha256=Rldr2qLAQPneNPzcYKDWn9EUkUQnAX8Cuq8uZNWoGco,5407
+fime/main.py,sha256=bFBsk97uxduAC-5JkqcxMLS3EvQyjFxamvplwsiHsjU,5408
 fime/progressindicator.py,sha256=dg6b0er2be_jha0IDVcPoif_Y7B0BDTpXNRZ5Koe5YQ,3562
 fime/report.py,sha256=lkd2G09_OM75sdP6spoBcPiOWGJGtafOlpbPExDLv9Y,8825
 fime/task_completer.py,sha256=NNfR_z_-LObhpuhg8V7fIJvRDOTWcI_IugYnaEW1fjk,5695
 fime/task_edit.py,sha256=5t9VYjOTKu9V4CyWxOBzj4xS3XD4ILTJFbs-HZM01HA,3038
 fime/test.py,sha256=rad_eviE5ww3DN1YSTiRaW3jOr-sKD0w4wTOvb_I8FI,1234
 fime/util.py,sha256=npeu63A_fhPZxyNnjCyAIxK9OO6UvrOg65IXddy8vKE,1403
 fime/worklog.py,sha256=2__ZaTNXUWxiBp58-3Rx3ivUpkw4JanmhHgJPFS6AZw,14715
 fime/worklog_rest.py,sha256=oxsO4JgOlc7KASKiaHxFse6kB7n_IKy4ahbHO06xSg8,8546
 fime/icons/__init__.py,sha256=Px3yciQj1J6A7Ftl4Jijgf0rBZ1YqxyNOtDkvX-i_wQ,10197
-fime-1.0.8.dev27.dist-info/LICENSE,sha256=S81a3379xPyh-dTnAnVhZJZUqZ_CdZ-1tJcHRZcVqns,1510
-fime-1.0.8.dev27.dist-info/METADATA,sha256=2tE0MeonNu217zNatb_9ChWn2CWbPD6oy91vT3wrfAI,1726
-fime-1.0.8.dev27.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-fime-1.0.8.dev27.dist-info/entry_points.txt,sha256=iQxntHZyUaYQUEkMrPRrLG_i7elCSdPegTZyS60NaEU,37
-fime-1.0.8.dev27.dist-info/top_level.txt,sha256=J4T8Q_j0W-0vp8s0dTw54RVPoKQT8ywugOqkJsSisVE,5
-fime-1.0.8.dev27.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-fime-1.0.8.dev27.dist-info/RECORD,,
+fime-1.0.9.dist-info/LICENSE,sha256=S81a3379xPyh-dTnAnVhZJZUqZ_CdZ-1tJcHRZcVqns,1510
+fime-1.0.9.dist-info/METADATA,sha256=gBfRqlj6JYHYPYv044iWBbis8yK_mYHOPTC0tgP50a0,1720
+fime-1.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+fime-1.0.9.dist-info/entry_points.txt,sha256=iQxntHZyUaYQUEkMrPRrLG_i7elCSdPegTZyS60NaEU,37
+fime-1.0.9.dist-info/top_level.txt,sha256=J4T8Q_j0W-0vp8s0dTw54RVPoKQT8ywugOqkJsSisVE,5
+fime-1.0.9.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+fime-1.0.9.dist-info/RECORD,,
```

