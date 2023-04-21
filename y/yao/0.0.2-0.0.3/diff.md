# Comparing `tmp/yao-0.0.2.tar.gz` & `tmp/yao-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao-0.0.2.tar", last modified: Tue Apr 18 07:27:56 2023, max compression
+gzip compressed data, was "yao-0.0.3.tar", last modified: Fri Apr 21 11:21:32 2023, max compression
```

## Comparing `yao-0.0.2.tar` & `yao-0.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.426909 yao-0.0.2/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-04-18 07:27:56.426647 yao-0.0.2/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)       38 2023-04-18 07:27:56.426957 yao-0.0.2/setup.cfg
--rw-r--r--   0 ke         (501) wheel        (0)      971 2023-04-18 07:22:00.000000 yao-0.0.2/setup.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.421226 yao-0.0.2/yao/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-17 09:50:59.000000 yao-0.0.2/yao/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    19246 2023-04-02 06:21:11.000000 yao-0.0.2/yao/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-04-02 04:59:57.000000 yao-0.0.2/yao/db.py
--rw-r--r--   0 ke         (501) wheel        (0)     7904 2023-04-02 03:13:11.000000 yao-0.0.2/yao/depends.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.422379 yao-0.0.2/yao/function/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:08:06.000000 yao-0.0.2/yao/function/__init__.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.423055 yao-0.0.2/yao/function/annex/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:09.000000 yao-0.0.2/yao/function/annex/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      187 2023-03-13 11:43:18.000000 yao-0.0.2/yao/function/annex/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-04-02 03:15:28.000000 yao-0.0.2/yao/function/annex/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-03-29 09:20:32.000000 yao-0.0.2/yao/function/annex/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.423608 yao-0.0.2/yao/function/appointment/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:09.000000 yao-0.0.2/yao/function/appointment/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-03-11 07:41:38.000000 yao-0.0.2/yao/function/appointment/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/appointment/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-03-11 08:51:27.000000 yao-0.0.2/yao/function/appointment/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.424213 yao-0.0.2/yao/function/company/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:09:21.000000 yao-0.0.2/yao/function/company/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      192 2023-02-27 07:13:36.000000 yao-0.0.2/yao/function/company/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/company/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-03-11 07:41:38.000000 yao-0.0.2/yao/function/company/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.424782 yao-0.0.2/yao/function/department/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:01.000000 yao-0.0.2/yao/function/department/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      189 2023-03-11 05:26:27.000000 yao-0.0.2/yao/function/department/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/department/main.py
--rw-r--r--   0 ke         (501) wheel        (0)      992 2023-03-11 07:41:38.000000 yao-0.0.2/yao/function/department/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.425329 yao-0.0.2/yao/function/log/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:09:21.000000 yao-0.0.2/yao/function/log/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      169 2023-03-10 11:36:17.000000 yao-0.0.2/yao/function/log/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/log/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-03-11 07:41:38.000000 yao-0.0.2/yao/function/log/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      665 2023-03-13 11:51:16.000000 yao-0.0.2/yao/function/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-04-07 10:50:08.000000 yao-0.0.2/yao/function/model.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.425885 yao-0.0.2/yao/function/permission/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:19.000000 yao-0.0.2/yao/function/permission/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      199 2023-03-11 05:25:41.000000 yao-0.0.2/yao/function/permission/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/permission/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-03-11 08:51:04.000000 yao-0.0.2/yao/function/permission/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.426441 yao-0.0.2/yao/function/user/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:21:23.000000 yao-0.0.2/yao/function/user/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-03-11 05:25:26.000000 yao-0.0.2/yao/function/user/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-04-18 07:25:25.000000 yao-0.0.2/yao/function/user/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-03-25 03:02:47.000000 yao-0.0.2/yao/function/user/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-04-08 07:18:19.000000 yao-0.0.2/yao/helpers.py
--rw-r--r--   0 ke         (501) wheel        (0)    11459 2023-04-12 11:57:41.000000 yao-0.0.2/yao/method.py
--rw-r--r--   0 ke         (501) wheel        (0)     1803 2023-03-30 03:35:08.000000 yao-0.0.2/yao/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.421937 yao-0.0.2/yao.egg-info/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/SOURCES.txt
--rw-r--r--   0 ke         (501) wheel        (0)        1 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/dependency_links.txt
--rw-r--r--   0 ke         (501) wheel        (0)      166 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/requires.txt
--rw-r--r--   0 ke         (501) wheel        (0)        4 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/top_level.txt
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.154589 yao-0.0.3/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-04-21 11:21:32.154396 yao-0.0.3/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)       38 2023-04-21 11:21:32.154639 yao-0.0.3/setup.cfg
+-rw-r--r--   0 ke         (501) wheel        (0)      971 2023-04-21 11:17:18.000000 yao-0.0.3/setup.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.149113 yao-0.0.3/yao/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    19246 2023-04-18 07:31:04.000000 yao-0.0.3/yao/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-04-18 07:31:04.000000 yao-0.0.3/yao/db.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7904 2023-04-18 07:31:04.000000 yao-0.0.3/yao/depends.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.150192 yao-0.0.3/yao/function/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/__init__.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.150719 yao-0.0.3/yao/function/annex/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/annex/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      187 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/annex/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/annex/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/annex/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.151339 yao-0.0.3/yao/function/appointment/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/appointment/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/appointment/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/appointment/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/appointment/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.151998 yao-0.0.3/yao/function/company/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/company/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      192 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/company/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/company/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/company/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.152548 yao-0.0.3/yao/function/department/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/department/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      189 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/department/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/department/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)      992 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/department/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.153096 yao-0.0.3/yao/function/log/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/log/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      169 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/log/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/log/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/log/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      665 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-04-21 10:39:40.000000 yao-0.0.3/yao/function/model.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.153651 yao-0.0.3/yao/function/permission/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/permission/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      199 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/permission/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/permission/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/permission/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.154182 yao-0.0.3/yao/function/user/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/user/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/user/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/user/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/user/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-04-18 07:31:04.000000 yao-0.0.3/yao/helpers.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11459 2023-04-18 07:31:04.000000 yao-0.0.3/yao/method.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1803 2023-04-18 07:31:04.000000 yao-0.0.3/yao/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.149781 yao-0.0.3/yao.egg-info/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/SOURCES.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        1 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/dependency_links.txt
+-rw-r--r--   0 ke         (501) wheel        (0)      166 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/requires.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        4 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/top_level.txt
```

### Comparing `yao-0.0.2/setup.py` & `yao-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yao",
-    version="0.0.2",
+    version="0.0.3",
     description="Dev",
     python_requires=">=3.9",
     author="Lsshu",
     author_email="admin@lsshu.cn",
     url="https://github.com/lsshu/yao",
     packages=find_packages(),
     long_description=long_description,
```

### Comparing `yao-0.0.2/yao/crud.py` & `yao-0.0.3/yao/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/db.py` & `yao-0.0.3/yao/db.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/depends.py` & `yao-0.0.3/yao/depends.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/annex/main.py` & `yao-0.0.3/yao/function/annex/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/annex/schema.py` & `yao-0.0.3/yao/function/annex/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/appointment/crud.py` & `yao-0.0.3/yao/function/appointment/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/appointment/main.py` & `yao-0.0.3/yao/function/appointment/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/appointment/schema.py` & `yao-0.0.3/yao/function/appointment/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/company/main.py` & `yao-0.0.3/yao/function/company/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/company/schema.py` & `yao-0.0.3/yao/function/company/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/department/main.py` & `yao-0.0.3/yao/function/department/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/department/schema.py` & `yao-0.0.3/yao/function/department/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/log/main.py` & `yao-0.0.3/yao/function/log/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/log/schema.py` & `yao-0.0.3/yao/function/log/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/main.py` & `yao-0.0.3/yao/function/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/model.py` & `yao-0.0.3/yao/function/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return Column(String(20), ForeignKey('%s.prefix_name' % function_company_table_name, ondelete="CASCADE", onupdate="CASCADE"), index=True, nullable=False,
                       comment="公司前缀")
 
 
 class ModelFunctionDepartments(BaseCompanyModel, BaseNestedSets):
     """公司部门"""
     __tablename__ = function_department_table_name
-    name = Column(String(20), unique=True, nullable=False, comment="名称")
+    name = Column(String(40), unique=True, nullable=False, comment="名称")
 
 
 class ModelFunctionPermissions(BaseModel, BaseNestedSets):
     """ 权限 """
     __tablename__ = function_permission_table_name
     sqlalchemy_mptt_pk_name = "uuid"
     name = Column(String(15), unique=True, nullable=False, comment="名称")
@@ -109,29 +109,29 @@
 def permission_receive_before_insert(target, initiator):
     target.path = "/%s" % target.scope.replace('.', '/').lower()
 
 
 class ModelFunctionAppointments(BaseCompanyModel):
     """员工职位"""
     __tablename__ = function_appointment_table_name
-    department = Column(String(20), ForeignKey('%s.name' % function_department_table_name, ondelete="CASCADE", onupdate="CASCADE"), index=True, nullable=True, comment="公司部门")
+    department = Column(String(40), ForeignKey('%s.name' % function_department_table_name, ondelete="CASCADE", onupdate="CASCADE"), index=True, nullable=True, comment="公司部门")
     name = Column(String(40), unique=True, nullable=False, comment="名称")
     scopes = Column(Text, nullable=False, comment="Scope")
     permissions = relationship(ModelFunctionPermissions, backref='appointments', lazy="joined", secondary=Table(
         "%s_appointment_has_permissions" % function_name,
         Model.metadata,
         Column('per_id', Integer, ForeignKey("%s.id" % function_permission_table_name, ondelete="CASCADE"), primary_key=True, comment="权限"),
         Column('app_id', Integer, ForeignKey("%s.id" % function_appointment_table_name, ondelete="CASCADE"), primary_key=True, comment="职位")
     ))
 
 
 class ModelFunctionUsers(BaseCompanyModel, BaseNestedSets):
     """登录用户"""
     __tablename__ = function_user_table_name
-    username = Column(String(35), nullable=False, unique=True, index=True, comment="名称")
+    username = Column(String(40), nullable=False, unique=True, index=True, comment="名称")
     password = Column(String(128), nullable=False, comment="密码")
     user_phone = Column(String(11), nullable=True, comment="手机")
     available = Column(Boolean, default=1, comment="是否有效")
 
     permissions = relationship(ModelFunctionPermissions, backref='function_users', secondary=Table(
         "%s_user_has_permissions" % function_name,
         Model.metadata,
```

### Comparing `yao-0.0.2/yao/function/permission/main.py` & `yao-0.0.3/yao/function/permission/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/permission/schema.py` & `yao-0.0.3/yao/function/permission/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/user/crud.py` & `yao-0.0.3/yao/function/user/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/user/main.py` & `yao-0.0.3/yao/function/user/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/function/user/schema.py` & `yao-0.0.3/yao/function/user/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/helpers.py` & `yao-0.0.3/yao/helpers.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/method.py` & `yao-0.0.3/yao/method.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao/schema.py` & `yao-0.0.3/yao/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.2/yao.egg-info/SOURCES.txt` & `yao-0.0.3/yao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

