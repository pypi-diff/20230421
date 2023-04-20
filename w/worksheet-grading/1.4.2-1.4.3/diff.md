# Comparing `tmp/worksheet_grading-1.4.2.tar.gz` & `tmp/worksheet_grading-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worksheet_grading-1.4.2.tar", last modified: Fri Jan 20 19:49:39 2023, max compression
+gzip compressed data, was "worksheet_grading-1.4.3.tar", last modified: Thu Apr 20 23:35:06 2023, max compression
```

## Comparing `worksheet_grading-1.4.2.tar` & `worksheet_grading-1.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-01-20 19:49:39.181835 worksheet_grading-1.4.2/
--rw-r--r--   0 klaus     (1000) users      (100)     1074 2022-12-02 02:11:23.000000 worksheet_grading-1.4.2/LICENSE
--rw-r--r--   0 klaus     (1000) users      (100)     9783 2023-01-20 19:49:39.181835 worksheet_grading-1.4.2/PKG-INFO
--rwxr-xr-x   0 klaus     (1000) users      (100)     9368 2023-01-20 19:39:13.000000 worksheet_grading-1.4.2/README.md
--rw-r--r--   0 klaus     (1000) users      (100)      781 2023-01-20 19:49:39.181835 worksheet_grading-1.4.2/setup.cfg
--rw-r--r--   0 klaus     (1000) users      (100)       37 2022-12-02 02:11:23.000000 worksheet_grading-1.4.2/setup.py
-drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-01-20 19:49:39.180835 worksheet_grading-1.4.2/worksheet_grading/
--rw-r--r--   0 klaus     (1000) users      (100)      322 2023-01-20 19:47:56.000000 worksheet_grading-1.4.2/worksheet_grading/__init__.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     2156 2023-01-20 05:17:20.000000 worksheet_grading-1.4.2/worksheet_grading/config.py
--rwxr-xr-x   0 klaus     (1000) users      (100)    28092 2023-01-20 06:09:41.000000 worksheet_grading-1.4.2/worksheet_grading/grade.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     3913 2023-01-20 02:01:10.000000 worksheet_grading-1.4.2/worksheet_grading/grade_export.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     6040 2023-01-20 04:02:29.000000 worksheet_grading-1.4.2/worksheet_grading/grade_import.py
--rwxr-xr-x   0 klaus     (1000) users      (100)    24260 2023-01-20 06:32:52.000000 worksheet_grading-1.4.2/worksheet_grading/gradelib.py
--rw-r--r--   0 klaus     (1000) users      (100)      473 2023-01-20 02:00:29.000000 worksheet_grading-1.4.2/worksheet_grading/moodle_util.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     2984 2022-12-04 01:35:57.000000 worksheet_grading-1.4.2/worksheet_grading/split.py
--rwxr-xr-x   0 klaus     (1000) users      (100)     2943 2023-01-19 03:56:33.000000 worksheet_grading-1.4.2/worksheet_grading/util.py
-drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-01-20 19:49:39.181835 worksheet_grading-1.4.2/worksheet_grading.egg-info/
--rw-r--r--   0 klaus     (1000) users      (100)     9783 2023-01-20 19:49:39.000000 worksheet_grading-1.4.2/worksheet_grading.egg-info/PKG-INFO
--rw-r--r--   0 klaus     (1000) users      (100)      553 2023-01-20 19:49:39.000000 worksheet_grading-1.4.2/worksheet_grading.egg-info/SOURCES.txt
--rw-r--r--   0 klaus     (1000) users      (100)        1 2023-01-20 19:49:39.000000 worksheet_grading-1.4.2/worksheet_grading.egg-info/dependency_links.txt
--rw-r--r--   0 klaus     (1000) users      (100)      194 2023-01-20 19:49:39.000000 worksheet_grading-1.4.2/worksheet_grading.egg-info/entry_points.txt
--rw-r--r--   0 klaus     (1000) users      (100)       25 2023-01-20 19:49:39.000000 worksheet_grading-1.4.2/worksheet_grading.egg-info/requires.txt
--rw-r--r--   0 klaus     (1000) users      (100)       18 2023-01-20 19:49:39.000000 worksheet_grading-1.4.2/worksheet_grading.egg-info/top_level.txt
+drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-04-20 23:35:06.573657 worksheet_grading-1.4.3/
+-rw-r--r--   0 klaus     (1000) users      (100)     1074 2022-12-02 02:11:23.000000 worksheet_grading-1.4.3/LICENSE
+-rw-r--r--   0 klaus     (1000) users      (100)     9783 2023-04-20 23:35:06.574657 worksheet_grading-1.4.3/PKG-INFO
+-rwxr-xr-x   0 klaus     (1000) users      (100)     9368 2023-01-20 19:39:13.000000 worksheet_grading-1.4.3/README.md
+-rw-r--r--   0 klaus     (1000) users      (100)      781 2023-04-20 23:35:06.574657 worksheet_grading-1.4.3/setup.cfg
+-rw-r--r--   0 klaus     (1000) users      (100)       37 2022-12-02 02:11:23.000000 worksheet_grading-1.4.3/setup.py
+drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-04-20 23:35:06.573657 worksheet_grading-1.4.3/worksheet_grading/
+-rw-r--r--   0 klaus     (1000) users      (100)      322 2023-04-20 21:47:46.000000 worksheet_grading-1.4.3/worksheet_grading/__init__.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     2156 2023-01-20 05:17:20.000000 worksheet_grading-1.4.3/worksheet_grading/config.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)    28101 2023-04-20 21:47:00.000000 worksheet_grading-1.4.3/worksheet_grading/grade.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     3913 2023-01-20 02:01:10.000000 worksheet_grading-1.4.3/worksheet_grading/grade_export.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     6040 2023-01-20 04:02:29.000000 worksheet_grading-1.4.3/worksheet_grading/grade_import.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)    24260 2023-01-20 06:32:52.000000 worksheet_grading-1.4.3/worksheet_grading/gradelib.py
+-rw-r--r--   0 klaus     (1000) users      (100)      473 2023-01-20 02:00:29.000000 worksheet_grading-1.4.3/worksheet_grading/moodle_util.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     2984 2022-12-04 01:35:57.000000 worksheet_grading-1.4.3/worksheet_grading/split.py
+-rwxr-xr-x   0 klaus     (1000) users      (100)     2943 2023-01-19 03:56:33.000000 worksheet_grading-1.4.3/worksheet_grading/util.py
+drwxr-xr-x   0 klaus     (1000) users      (100)        0 2023-04-20 23:35:06.573657 worksheet_grading-1.4.3/worksheet_grading.egg-info/
+-rw-r--r--   0 klaus     (1000) users      (100)     9783 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/PKG-INFO
+-rw-r--r--   0 klaus     (1000) users      (100)      553 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/SOURCES.txt
+-rw-r--r--   0 klaus     (1000) users      (100)        1 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/dependency_links.txt
+-rw-r--r--   0 klaus     (1000) users      (100)      194 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/entry_points.txt
+-rw-r--r--   0 klaus     (1000) users      (100)       25 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/requires.txt
+-rw-r--r--   0 klaus     (1000) users      (100)       18 2023-04-20 23:35:06.000000 worksheet_grading-1.4.3/worksheet_grading.egg-info/top_level.txt
```

### Comparing `worksheet_grading-1.4.2/LICENSE` & `worksheet_grading-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/PKG-INFO` & `worksheet_grading-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worksheet_grading
-Version: 1.4.2
+Version: 1.4.3
 Summary: Exercise sheet grading utility with Moodle support
 Home-page: https://gitlab.com/kdvkrs/worksheet_grading
 Author: Klaus Kraßnitzer
 Author-email: klaus@krss.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `worksheet_grading-1.4.2/README.md` & `worksheet_grading-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/setup.cfg` & `worksheet_grading-1.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/worksheet_grading/config.py` & `worksheet_grading-1.4.3/worksheet_grading/config.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/worksheet_grading/grade.py` & `worksheet_grading-1.4.3/worksheet_grading/grade.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,15 +741,15 @@
 
 def act_sanity_check(state: State):
     points = sc_points()
     sane = True
     for e in state.frame.data.values():
         for ex in e.sheet.exercises.values():
             for a in ex.answers:
-                if a.deductions.deducted_points() < -1 * points[ex.number][a.num - 1]:
+                if a.deductions.deducted_points() < -1 * points[ex.number - 1][a.num - 1]:
                     print(red("Invalid deduction found for group \"{}\" exercise {}.{}").format(e.group,
                                                                                                 ex.number, a.num))
                     sane = False
 
     if not sane:
         print()
         print(red("Invalid deductions found, see above output"))
@@ -758,15 +758,15 @@
     
 
 def act_statistics(state: State):
     stat_frame = state.frame.csv_df
     groups = state.frame.data.keys()
     stat_pts = []
     for g in groups:
-        if state.frame.data[g].sheet.grade_status() == config.GRADED:
+        if state.frame.data[g].sheet.grade_status() == GradeStatus.GRADED:
             stat_pts.append(stat_frame[stat_frame.group == g]["points"].sum())
 
     try:
         mean = statistics.mean(stat_pts)
         stdev = statistics.stdev(stat_pts)
         median = statistics.median(stat_pts)
         print(bright("Statistics of graded exercises:"))
```

### Comparing `worksheet_grading-1.4.2/worksheet_grading/grade_export.py` & `worksheet_grading-1.4.3/worksheet_grading/grade_export.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/worksheet_grading/grade_import.py` & `worksheet_grading-1.4.3/worksheet_grading/grade_import.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/worksheet_grading/gradelib.py` & `worksheet_grading-1.4.3/worksheet_grading/gradelib.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/worksheet_grading/split.py` & `worksheet_grading-1.4.3/worksheet_grading/split.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/worksheet_grading/util.py` & `worksheet_grading-1.4.3/worksheet_grading/util.py`

 * *Files identical despite different names*

### Comparing `worksheet_grading-1.4.2/worksheet_grading.egg-info/PKG-INFO` & `worksheet_grading-1.4.3/worksheet_grading.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worksheet-grading
-Version: 1.4.2
+Version: 1.4.3
 Summary: Exercise sheet grading utility with Moodle support
 Home-page: https://gitlab.com/kdvkrs/worksheet_grading
 Author: Klaus Kraßnitzer
 Author-email: klaus@krss.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `worksheet_grading-1.4.2/worksheet_grading.egg-info/SOURCES.txt` & `worksheet_grading-1.4.3/worksheet_grading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

