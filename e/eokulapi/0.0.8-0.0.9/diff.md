# Comparing `tmp/eokulapi-0.0.8.tar.gz` & `tmp/eokulapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eokulapi-0.0.8.tar", last modified: Fri Jan  6 16:27:12 2023, max compression
+gzip compressed data, was "eokulapi-0.0.9.tar", last modified: Tue Jan 10 14:23:13 2023, max compression
```

## Comparing `eokulapi-0.0.8.tar` & `eokulapi-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 16:27:12.232214 eokulapi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-06 16:27:01.000000 eokulapi-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-06 16:27:12.232214 eokulapi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-06 16:27:01.000000 eokulapi-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-06 16:27:01.000000 eokulapi-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 16:27:12.232214 eokulapi-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 16:27:12.224213 eokulapi-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 16:27:12.224213 eokulapi-0.0.8/src/eokulapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 16:27:12.232214 eokulapi-0.0.8/src/eokulapi/Models/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/Absenteeism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/AbsenteeismContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/AdditionalExam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/AvgMark.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/AvgMarkContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/AvgMarkLesson.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/Document.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/DocumentContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/EndtermMark.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/EndtermMarkContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/EokulStudent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/ExamSchedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/ExamScheduleContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/Lesson.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/LessonDay.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/LessonSchedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/MarkContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/MarkLesson.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/Responsibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/Transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-01-06 16:27:01.000000 eokulapi-0.0.8/src/eokulapi/eokulapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 16:27:12.228213 eokulapi-0.0.8/src/eokulapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-06 16:27:12.000000 eokulapi-0.0.8/src/eokulapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-06 16:27:12.000000 eokulapi-0.0.8/src/eokulapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 16:27:12.000000 eokulapi-0.0.8/src/eokulapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-06 16:27:12.000000 eokulapi-0.0.8/src/eokulapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-06 16:27:12.000000 eokulapi-0.0.8/src/eokulapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:23:13.465160 eokulapi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-10 14:23:03.000000 eokulapi-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-10 14:23:13.465160 eokulapi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-10 14:23:03.000000 eokulapi-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-10 14:23:03.000000 eokulapi-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 14:23:13.465160 eokulapi-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:23:13.453160 eokulapi-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:23:13.457160 eokulapi-0.0.9/src/eokulapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:23:13.465160 eokulapi-0.0.9/src/eokulapi/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/Absenteeism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/AbsenteeismContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/AdditionalExam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/AvgMark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/AvgMarkContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/AvgMarkLesson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/Document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/DocumentContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/EndtermMark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/EndtermMarkContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/EokulStudent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/ExamSchedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/ExamScheduleContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/Lesson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/LessonDay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/LessonSchedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/MarkContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/MarkLesson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/Responsibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/Transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-01-10 14:23:03.000000 eokulapi-0.0.9/src/eokulapi/eokulapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 14:23:13.457160 eokulapi-0.0.9/src/eokulapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-10 14:23:13.000000 eokulapi-0.0.9/src/eokulapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-10 14:23:13.000000 eokulapi-0.0.9/src/eokulapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 14:23:13.000000 eokulapi-0.0.9/src/eokulapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-10 14:23:13.000000 eokulapi-0.0.9/src/eokulapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-10 14:23:13.000000 eokulapi-0.0.9/src/eokulapi.egg-info/top_level.txt
```

### Comparing `eokulapi-0.0.8/LICENSE` & `eokulapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/PKG-INFO` & `eokulapi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eokulapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: eokul vbs api
 Author: insanolanbiri
 Project-URL: Homepage, https://github.com/insanolanbiri/eokulapi
 Project-URL: Bug Tracker, https://github.com/insanolanbiri/eokulapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `eokulapi-0.0.8/pyproject.toml` & `eokulapi-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eokulapi"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="insanolanbiri" },
 ]
 description = "eokul vbs api"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/Absenteeism.py` & `eokulapi-0.0.9/src/eokulapi/Models/Absenteeism.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/AbsenteeismContainer.py` & `eokulapi-0.0.9/src/eokulapi/Models/AbsenteeismContainer.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/AdditionalExam.py` & `eokulapi-0.0.9/src/eokulapi/Models/AdditionalExam.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/AvgMark.py` & `eokulapi-0.0.9/src/eokulapi/Models/AvgMark.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/AvgMarkContainer.py` & `eokulapi-0.0.9/src/eokulapi/Models/AvgMarkContainer.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/AvgMarkLesson.py` & `eokulapi-0.0.9/src/eokulapi/Models/AvgMarkLesson.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,8 @@
                     "value": obj.get(f"Y{i}"),
                     "description": obj.get(f"Y{i}ACIKLAMA"),
                     "description_value": obj.get(f"Y{i}ACIKLAMADEGER"),
                     "avg_mark": obj.get(f"Y{i}SUBEORT"),
                 }
             )
             marks[i] = mark
-            return cls(ders, donem, marks)
+        return cls(ders, donem, marks)
```

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/Document.py` & `eokulapi-0.0.9/src/eokulapi/Models/Document.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/DocumentContainer.py` & `eokulapi-0.0.9/src/eokulapi/Models/DocumentContainer.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/EndtermMark.py` & `eokulapi-0.0.9/src/eokulapi/Models/EndtermMark.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/EndtermMarkContainer.py` & `eokulapi-0.0.9/src/eokulapi/Models/EndtermMarkContainer.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/EokulStudent.py` & `eokulapi-0.0.9/src/eokulapi/Models/EokulStudent.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/ExamSchedule.py` & `eokulapi-0.0.9/src/eokulapi/Models/ExamSchedule.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/ExamScheduleContainer.py` & `eokulapi-0.0.9/src/eokulapi/Models/ExamScheduleContainer.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/Lesson.py` & `eokulapi-0.0.9/src/eokulapi/Models/Lesson.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/LessonDay.py` & `eokulapi-0.0.9/src/eokulapi/Models/LessonDay.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/LessonSchedule.py` & `eokulapi-0.0.9/src/eokulapi/Models/LessonSchedule.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/MarkContainer.py` & `eokulapi-0.0.9/src/eokulapi/Models/MarkContainer.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/MarkLesson.py` & `eokulapi-0.0.9/src/eokulapi/Models/MarkLesson.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/Models/__init__.py` & `eokulapi-0.0.9/src/eokulapi/Models/__init__.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi/eokulapi.py` & `eokulapi-0.0.9/src/eokulapi/eokulapi.py`

 * *Files identical despite different names*

### Comparing `eokulapi-0.0.8/src/eokulapi.egg-info/PKG-INFO` & `eokulapi-0.0.9/src/eokulapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eokulapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: eokul vbs api
 Author: insanolanbiri
 Project-URL: Homepage, https://github.com/insanolanbiri/eokulapi
 Project-URL: Bug Tracker, https://github.com/insanolanbiri/eokulapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `eokulapi-0.0.8/src/eokulapi.egg-info/SOURCES.txt` & `eokulapi-0.0.9/src/eokulapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

