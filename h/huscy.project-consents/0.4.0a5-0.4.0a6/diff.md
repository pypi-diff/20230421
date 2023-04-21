# Comparing `tmp/huscy.project_consents-0.4.0a5.tar.gz` & `tmp/huscy.project_consents-0.4.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_consents-0.4.0a5.tar", last modified: Mon Jan 30 13:37:41 2023, max compression
+gzip compressed data, was "huscy.project_consents-0.4.0a6.tar", last modified: Fri Apr 21 14:34:44 2023, max compression
```

## Comparing `huscy.project_consents-0.4.0a5.tar` & `huscy.project_consents-0.4.0a6.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-01-30 13:37:41.950101 huscy.project_consents-0.4.0a5/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    34523 2022-12-08 10:33:28.000000 huscy.project_consents-0.4.0a5/LICENSE
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1084 2023-01-30 13:37:41.950101 huscy.project_consents-0.4.0a5/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       19 2022-12-08 10:33:28.000000 huscy.project_consents-0.4.0a5/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-01-30 13:37:41.946100 huscy.project_consents-0.4.0a5/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-01-30 13:37:41.950101 huscy.project_consents-0.4.0a5/huscy/project_consents/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       81 2023-01-30 13:08:18.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      235 2023-01-30 13:08:18.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      479 2023-01-13 15:29:15.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      194 2022-12-08 10:33:28.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-01-30 13:37:41.950101 huscy.project_consents-0.4.0a5/huscy/project_consents/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1961 2023-01-30 13:37:41.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-12-08 10:34:52.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1184 2023-01-24 10:54:32.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1304 2023-01-30 13:08:18.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1171 2023-01-24 10:54:32.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      399 2022-12-08 10:34:52.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1869 2022-12-08 10:34:52.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/views.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1527 2023-01-13 15:29:15.000000 huscy.project_consents-0.4.0a5/huscy/project_consents/viewsets.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-01-30 13:37:41.950101 huscy.project_consents-0.4.0a5/huscy.project_consents.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1084 2023-01-30 13:37:41.000000 huscy.project_consents-0.4.0a5/huscy.project_consents.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      687 2023-01-30 13:37:41.000000 huscy.project_consents-0.4.0a5/huscy.project_consents.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-01-30 13:37:41.000000 huscy.project_consents-0.4.0a5/huscy.project_consents.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      100 2023-01-30 13:37:41.000000 huscy.project_consents-0.4.0a5/huscy.project_consents.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-01-30 13:37:41.000000 huscy.project_consents-0.4.0a5/huscy.project_consents.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-01-30 13:37:41.950101 huscy.project_consents-0.4.0a5/setup.cfg
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1602 2022-12-08 10:34:52.000000 huscy.project_consents-0.4.0a5/setup.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a6/LICENSE
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.4.0a6/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/huscy/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/huscy/project_consents/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-04-21 14:34:31.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      435 2023-04-21 12:57:46.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/admin.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/api_urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/apps.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-04-21 08:48:37.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/forms.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/huscy/project_consents/migrations/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2492 2023-04-21 14:34:41.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/migrations/0001_initial.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/migrations/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1495 2023-04-20 11:49:39.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/models.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1304 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1171 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/services.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      430 2023-04-21 09:36:45.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2919 2023-04-21 12:54:19.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/views.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      833 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/SOURCES.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/dependency_links.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/requires.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/top_level.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/setup.cfg
+-rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1642 2023-04-20 09:24:18.000000 huscy.project_consents-0.4.0a6/setup.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/tests/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a6/tests/test_project_consent_category_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a6/tests/test_project_consent_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     5532 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a6/tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.4.0a5/LICENSE` & `huscy.project_consents-0.4.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a5/PKG-INFO` & `huscy.project_consents-0.4.0a6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: huscy.project_consents
-Version: 0.4.0a5
+Version: 0.4.0a6
 Summary: projects_consents
-Home-page: https://bitbucket.org/huscy/consents
+Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
-Description: # project consents
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
+License-File: LICENSE
+
+# project consents
+
+
```

### Comparing `huscy.project_consents-0.4.0a5/huscy/project_consents/migrations/0001_initial.py` & `huscy.project_consents-0.4.0a6/huscy/project_consents/migrations/0001_initial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,43 @@
-# Generated by Django 4.1.5 on 2023-01-30 13:37
+# Generated by Django 4.2 on 2023-04-21 14:34
 
 from django.db import migrations, models
 import django.db.models.deletion
+import uuid
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        ('projects', '0002_alter_membership_options'),
         ('consents', '0001_initial'),
+        ('projects', '0002_alter_membership_options'),
         ('subjects', '0001_squashed_0009_delete_contactold'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='ProjectConsent',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('consent', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='consents.consent')),
                 ('project', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to='projects.project')),
             ],
         ),
         migrations.CreateModel(
+            name='ProjectConsentToken',
+            fields=[
+                ('id', models.UUIDField(default=uuid.uuid4, primary_key=True, serialize=False)),
+                ('created_at', models.DateTimeField(auto_now_add=True)),
+                ('project', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='projects.project')),
+                ('subject', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='subjects.subject')),
+            ],
+        ),
+        migrations.CreateModel(
             name='ProjectConsentCategory',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('consent_category', models.OneToOneField(on_delete=django.db.models.deletion.PROTECT, to='consents.consentcategory')),
             ],
         ),
         migrations.CreateModel(
```

### Comparing `huscy.project_consents-0.4.0a5/huscy/project_consents/models.py` & `huscy.project_consents-0.4.0a6/huscy/project_consents/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import uuid
+
 from django.db import models
 
 from huscy.consents.models import Consent, ConsentCategory, ConsentFile
 from huscy.projects.models import Project
 from huscy.subjects.models import Subject
 
 
@@ -13,14 +15,21 @@
         return self.consent_category.name
 
     @property
     def template_text_fragments(self):
         return self.consent_category.template_text_fragments
 
 
+class ProjectConsentToken(models.Model):
+    id = models.UUIDField(primary_key=True, default=uuid.uuid4)
+    project = models.ForeignKey(Project, on_delete=models.CASCADE)
+    subject = models.ForeignKey(Subject, on_delete=models.CASCADE)
+    created_at = models.DateTimeField(auto_now_add=True)
+
+
 class ProjectConsent(models.Model):
     project = models.OneToOneField(Project, on_delete=models.CASCADE)
     consent = models.ForeignKey(Consent, on_delete=models.PROTECT)
 
     @property
     def name(self):
         return self.consent.name
```

### Comparing `huscy.project_consents-0.4.0a5/huscy/project_consents/serializer.py` & `huscy.project_consents-0.4.0a6/huscy/project_consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a5/huscy/project_consents/services.py` & `huscy.project_consents-0.4.0a6/huscy/project_consents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a5/huscy/project_consents/viewsets.py` & `huscy.project_consents-0.4.0a6/huscy/project_consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a5/huscy.project_consents.egg-info/PKG-INFO` & `huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: huscy.project-consents
-Version: 0.4.0a5
+Version: 0.4.0a6
 Summary: projects_consents
-Home-page: https://bitbucket.org/huscy/consents
+Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
-Description: # project consents
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
+License-File: LICENSE
+
+# project consents
+
+
```

### Comparing `huscy.project_consents-0.4.0a5/huscy.project_consents.egg-info/SOURCES.txt` & `huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 huscy.project_consents.egg-info/dependency_links.txt
 huscy.project_consents.egg-info/requires.txt
 huscy.project_consents.egg-info/top_level.txt
 huscy/project_consents/__init__.py
 huscy/project_consents/admin.py
 huscy/project_consents/api_urls.py
 huscy/project_consents/apps.py
+huscy/project_consents/forms.py
 huscy/project_consents/models.py
 huscy/project_consents/serializer.py
 huscy/project_consents/services.py
 huscy/project_consents/urls.py
 huscy/project_consents/views.py
 huscy/project_consents/viewsets.py
 huscy/project_consents/migrations/0001_initial.py
-huscy/project_consents/migrations/__init__.py
+huscy/project_consents/migrations/__init__.py
+tests/test_project_consent_category_serializer.py
+tests/test_project_consent_serializer.py
+tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.4.0a5/setup.py` & `huscy.project_consents-0.4.0a6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,20 @@
     description='projects_consents',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     author='Gefan Qian, Stefan Bunde',
     author_email='gefan.qian@gmail.com, stefanbunde+git@posteo.de',
 
-    url='https://bitbucket.org/huscy/consents',
+    url='https://bitbucket.org/huscy/project_consents',
 
     packages=find_namespace_packages(include=['huscy.*']),
 
     install_requires=[
+        'django-qr-code',
         'huscy.consents',
         'huscy.projects',
         'huscy.subjects',
     ],
     extras_require={
         'development': ['psycopg2-binary'],
         'testing': ['tox', 'watchdog'],
@@ -36,18 +37,18 @@
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
 )
```

