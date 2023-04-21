# Comparing `tmp/cakemail-1.6.4.tar.gz` & `tmp/cakemail-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cakemail-1.6.4.tar", last modified: Tue Aug 10 15:39:36 2021, max compression
+gzip compressed data, was "cakemail-1.9.0.tar", last modified: Wed Dec 22 14:32:18 2021, max compression
```

## Comparing `cakemail-1.6.4.tar` & `cakemail-1.9.0.tar`

### file list

```diff
@@ -1,42 +1,37 @@
-drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-08-10 15:39:36.153953 cakemail-1.6.4/
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4685 2021-08-10 15:39:36.153953 cakemail-1.6.4/PKG-INFO
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3240 2021-03-10 20:09:08.000000 cakemail-1.6.4/README.md
-drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-08-10 15:39:36.153953 cakemail-1.6.4/cakemail/
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       56 2020-12-09 14:31:27.000000 cakemail-1.6.4/cakemail/__init__.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      443 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/account.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      891 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/action.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4031 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/api.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1921 2020-12-09 14:31:27.000000 cakemail-1.6.4/cakemail/automation.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1671 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/campaign.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      597 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/campaign_blueprint.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      989 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/contact.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      683 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/custom_attribute.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      492 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/domain.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      592 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/form.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      855 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/list.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      593 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/log.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      352 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/logo.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      958 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/report.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1734 2020-12-09 14:31:27.000000 cakemail-1.6.4/cakemail/response.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      643 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/segment.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      838 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/sender.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1076 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/sub_account.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      587 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/suppressed_email.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      533 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/system_email.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      745 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/template.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     2050 2020-12-09 14:31:27.000000 cakemail-1.6.4/cakemail/token.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      356 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/transactional_email.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1495 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/user.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      741 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/webhook.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1016 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/workflow.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      751 2021-08-10 15:28:02.000000 cakemail-1.6.4/cakemail/workflow_blueprint.py
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      461 2020-12-09 14:31:27.000000 cakemail-1.6.4/cakemail/wrapper.py
-drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-08-10 15:39:36.153953 cakemail-1.6.4/cakemail.egg-info/
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4685 2021-08-10 15:39:36.000000 cakemail-1.6.4/cakemail.egg-info/PKG-INFO
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      831 2021-08-10 15:39:36.000000 cakemail-1.6.4/cakemail.egg-info/SOURCES.txt
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        1 2021-08-10 15:39:36.000000 cakemail-1.6.4/cakemail.egg-info/dependency_links.txt
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        1 2021-02-19 14:47:00.000000 cakemail-1.6.4/cakemail.egg-info/not-zip-safe
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       60 2021-08-10 15:39:36.000000 cakemail-1.6.4/cakemail.egg-info/requires.txt
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        9 2021-08-10 15:39:36.000000 cakemail-1.6.4/cakemail.egg-info/top_level.txt
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       38 2021-08-10 15:39:36.153953 cakemail-1.6.4/setup.cfg
--rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      646 2021-08-10 15:29:05.000000 cakemail-1.6.4/setup.py
+drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:32:18.744560 cakemail-1.9.0/
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3482 2021-12-22 14:32:18.744560 cakemail-1.9.0/PKG-INFO
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3240 2021-03-10 20:09:08.000000 cakemail-1.9.0/README.md
+drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:32:18.744560 cakemail-1.9.0/cakemail/
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      443 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/account.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      891 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/action.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     4031 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/api.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1671 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/campaign.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      597 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/campaign_blueprint.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      989 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/contact.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      683 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/custom_attribute.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      492 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/domain.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      592 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/form.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      855 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/list.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      593 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/log.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      352 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/logo.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      958 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/report.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      643 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/segment.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      838 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/sender.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1076 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/sub_account.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      587 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/suppressed_email.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      533 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/system_email.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      745 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/template.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      356 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/transactional_email.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1495 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/user.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      741 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/webhook.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     1016 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/workflow.py
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      751 2021-12-22 14:31:44.000000 cakemail-1.9.0/cakemail/workflow_blueprint.py
+drwxr-xr-x   0 sgregoire  (1000) sgregoire  (1000)        0 2021-12-22 14:32:18.744560 cakemail-1.9.0/cakemail.egg-info/
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)     3482 2021-12-22 14:32:18.000000 cakemail-1.9.0/cakemail.egg-info/PKG-INFO
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      728 2021-12-22 14:32:18.000000 cakemail-1.9.0/cakemail.egg-info/SOURCES.txt
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        1 2021-12-22 14:32:18.000000 cakemail-1.9.0/cakemail.egg-info/dependency_links.txt
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        1 2021-02-19 14:47:00.000000 cakemail-1.9.0/cakemail.egg-info/not-zip-safe
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       60 2021-12-22 14:32:18.000000 cakemail-1.9.0/cakemail.egg-info/requires.txt
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)        9 2021-12-22 14:32:18.000000 cakemail-1.9.0/cakemail.egg-info/top_level.txt
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)       38 2021-12-22 14:32:18.744560 cakemail-1.9.0/setup.cfg
+-rw-r--r--   0 sgregoire  (1000) sgregoire  (1000)      646 2021-12-22 14:28:19.000000 cakemail-1.9.0/setup.py
```

### Comparing `cakemail-1.6.4/README.md` & `cakemail-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/action.py` & `cakemail-1.9.0/cakemail/action.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/api.py` & `cakemail-1.9.0/cakemail/api.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/campaign.py` & `cakemail-1.9.0/cakemail/campaign.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/campaign_blueprint.py` & `cakemail-1.9.0/cakemail/campaign_blueprint.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/contact.py` & `cakemail-1.9.0/cakemail/contact.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/custom_attribute.py` & `cakemail-1.9.0/cakemail/custom_attribute.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/form.py` & `cakemail-1.9.0/cakemail/form.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/list.py` & `cakemail-1.9.0/cakemail/list.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/log.py` & `cakemail-1.9.0/cakemail/log.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/report.py` & `cakemail-1.9.0/cakemail/report.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/segment.py` & `cakemail-1.9.0/cakemail/segment.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/sender.py` & `cakemail-1.9.0/cakemail/sender.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/sub_account.py` & `cakemail-1.9.0/cakemail/sub_account.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/suppressed_email.py` & `cakemail-1.9.0/cakemail/suppressed_email.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/system_email.py` & `cakemail-1.9.0/cakemail/system_email.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/template.py` & `cakemail-1.9.0/cakemail/template.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/user.py` & `cakemail-1.9.0/cakemail/user.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/webhook.py` & `cakemail-1.9.0/cakemail/webhook.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/workflow.py` & `cakemail-1.9.0/cakemail/workflow.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail/workflow_blueprint.py` & `cakemail-1.9.0/cakemail/workflow_blueprint.py`

 * *Files identical despite different names*

### Comparing `cakemail-1.6.4/cakemail.egg-info/SOURCES.txt` & `cakemail-1.9.0/cakemail.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 README.md
 setup.py
-cakemail/__init__.py
 cakemail/account.py
 cakemail/action.py
 cakemail/api.py
-cakemail/automation.py
 cakemail/campaign.py
 cakemail/campaign_blueprint.py
 cakemail/contact.py
 cakemail/custom_attribute.py
 cakemail/domain.py
 cakemail/form.py
 cakemail/list.py
 cakemail/log.py
 cakemail/logo.py
 cakemail/report.py
-cakemail/response.py
 cakemail/segment.py
 cakemail/sender.py
 cakemail/sub_account.py
 cakemail/suppressed_email.py
 cakemail/system_email.py
 cakemail/template.py
-cakemail/token.py
 cakemail/transactional_email.py
 cakemail/user.py
 cakemail/webhook.py
 cakemail/workflow.py
 cakemail/workflow_blueprint.py
-cakemail/wrapper.py
 cakemail.egg-info/PKG-INFO
 cakemail.egg-info/SOURCES.txt
 cakemail.egg-info/dependency_links.txt
 cakemail.egg-info/not-zip-safe
 cakemail.egg-info/requires.txt
 cakemail.egg-info/top_level.txt
```

### Comparing `cakemail-1.6.4/setup.py` & `cakemail-1.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 README = (HERE / "README.md").read_text()
 
 requirements = [
     'six',
     'urllib3',
     'certifi',
     'python-dateutil',
-    'cakemail-openapi==1.6.4'
+    'cakemail-openapi==1.9.1'
 ]
 
 setup(
     name='cakemail',
-    version='1.6.4',
+    version='1.9.0',
     description='Cakemail Next-gen API client',
     python_requires='>=3.6',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/cakemail/cakemail-python',
     license='MIT',
     packages=[
```

