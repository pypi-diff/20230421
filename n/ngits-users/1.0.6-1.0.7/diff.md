# Comparing `tmp/ngits-users-1.0.6.tar.gz` & `tmp/ngits-users-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngits-users-1.0.6.tar", last modified: Fri Apr 21 08:18:49 2023, max compression
+gzip compressed data, was "ngits-users-1.0.7.tar", last modified: Fri Apr 21 08:27:58 2023, max compression
```

## Comparing `ngits-users-1.0.6.tar` & `ngits-users-1.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      136 2023-04-21 06:52:22.000000 ngits-users-1.0.6/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     8497 2023-04-21 08:18:49.673721 ngits-users-1.0.6/PKG-INFO
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     5773 2023-04-21 08:17:08.000000 ngits-users-1.0.6/README.rst
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      736 2023-04-21 06:52:22.000000 ngits-users-1.0.6/pyproject.toml
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      823 2023-04-21 08:18:49.673721 ngits-users-1.0.6/setup.cfg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2023-04-21 06:52:22.000000 ngits-users-1.0.6/setup.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.669721 ngits-users-1.0.6/src/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.669721 ngits-users-1.0.6/src/ngits_users.egg-info/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     8497 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1078 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      116 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        6 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/top_level.txt
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/__init__.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      368 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/admin.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      193 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/apps.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1997 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/forms.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/migrations/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3021 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/migrations/0001_initial.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/migrations/__init__.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      344 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/models.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3657 2023-04-21 08:17:08.000000 ngits-users-1.0.6/src/users/schemas.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3122 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/serializers.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      357 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/signals.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.669721 ngits-users-1.0.6/src/users/static/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.669721 ngits-users-1.0.6/src/users/static/users/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/static/users/css/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     2333 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/static/users/css/style.css
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/static/users/img/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11327 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/static/users/img/fail.svg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    20062 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/static/users/img/success.svg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      603 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/tasks.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/templates/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      538 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/change_password.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      118 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/change_password_email.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       71 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/change_password_email.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      602 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/form_site.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      575 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/info_site.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      395 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/password_changed.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      117 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/registration_email.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       70 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/registration_email.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      384 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/verify_error.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      389 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/verify_ok.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1302 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/urls.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3047 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/utils.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11600 2023-04-21 08:17:08.000000 ngits-users-1.0.6/src/users/views.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.518382 ngits-users-1.0.7/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      136 2023-04-21 06:52:22.000000 ngits-users-1.0.7/MANIFEST.in
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    10028 2023-04-21 08:27:58.518382 ngits-users-1.0.7/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     6888 2023-04-21 08:22:27.000000 ngits-users-1.0.7/README.rst
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      736 2023-04-21 06:52:22.000000 ngits-users-1.0.7/pyproject.toml
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      823 2023-04-21 08:27:58.518382 ngits-users-1.0.7/setup.cfg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2023-04-21 06:52:22.000000 ngits-users-1.0.7/setup.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.510382 ngits-users-1.0.7/src/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.514382 ngits-users-1.0.7/src/ngits_users.egg-info/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    10028 2023-04-21 08:27:58.000000 ngits-users-1.0.7/src/ngits_users.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1078 2023-04-21 08:27:58.000000 ngits-users-1.0.7/src/ngits_users.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2023-04-21 08:27:58.000000 ngits-users-1.0.7/src/ngits_users.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      116 2023-04-21 08:27:58.000000 ngits-users-1.0.7/src/ngits_users.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        6 2023-04-21 08:27:58.000000 ngits-users-1.0.7/src/ngits_users.egg-info/top_level.txt
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.514382 ngits-users-1.0.7/src/users/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/__init__.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      368 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/admin.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      193 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/apps.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1997 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/forms.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.514382 ngits-users-1.0.7/src/users/migrations/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3021 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/migrations/0001_initial.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/migrations/__init__.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      344 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/models.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3657 2023-04-21 08:17:08.000000 ngits-users-1.0.7/src/users/schemas.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3122 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/serializers.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      357 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/signals.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.510382 ngits-users-1.0.7/src/users/static/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.510382 ngits-users-1.0.7/src/users/static/users/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.514382 ngits-users-1.0.7/src/users/static/users/css/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     2333 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/static/users/css/style.css
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.514382 ngits-users-1.0.7/src/users/static/users/img/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11327 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/static/users/img/fail.svg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    20062 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/static/users/img/success.svg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      603 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/tasks.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:27:58.518382 ngits-users-1.0.7/src/users/templates/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      538 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/change_password.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      118 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/change_password_email.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       71 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/change_password_email.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      602 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/form_site.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      575 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/info_site.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      395 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/password_changed.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      117 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/registration_email.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       70 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/registration_email.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      384 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/verify_error.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      389 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/templates/verify_ok.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1302 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/urls.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3047 2023-04-21 06:52:22.000000 ngits-users-1.0.7/src/users/utils.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    12257 2023-04-21 08:22:27.000000 ngits-users-1.0.7/src/users/views.py
```

### Comparing `ngits-users-1.0.6/PKG-INFO` & `ngits-users-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ngits-users
-Version: 1.0.6
+Version: 1.0.7
 Summary: Base users application for Django projects
 Home-page: https://ngits.dev
 Author: NGITs
 License: BSD-3-Clause
 Description: ngits-users
         ============
         
@@ -242,14 +242,67 @@
                 /templates
                     /change_password_email.html
                     /change_password_email.txt
                     /change_password.html
         
         *For fore details check out library default templates*
         
+        9. Optional ``TokenSerializer`` override:
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        You can override ``TokenSerializer`` - the default response serializer on ``LoginView`` `(/login)`.
+        
+        In order to use your own serializer, you need to follow these steps:
+        
+        1. Create your custom serializer:
+        
+        e.g.:
+        
+        ::
+        
+            from rest_framework import serializers
+            from rest_framework.authtoken.models import Token
+        
+            ...
+        
+            class TestSerializer(serializers.ModelSerializer):
+                foo = serializers.SerializerMethodField()
+        
+                class Meta:
+                    model = Token
+                    fields = ("key", "user_id", "foo")
+        
+                def get_foo(self, obj):
+                    return "bar"
+        
+        **Warning!** Your custom serializer must handle incoming DRF ``Token`` object!
+        
+        2. Set serializer path in your ``settings`` file
+        
+        e.g.:
+        
+        ::
+        
+            LOGIN_RESPONSE_SERIALIZER_PATH = "app.serializers.TestSerializer"
+        
+        3. Take it for a spin!
+        
+        ::
+        
+            HTTP 200 OK
+            Allow: POST, OPTIONS
+            Content-Type: application/json
+            Vary: Accept
+        
+            {
+                "key": "a5851e7359d1d04cd99a26014e47fcbedaa0beea",
+                "user_id": 1,
+                "foo": "bar"
+            }
+        
         Login response codes
         --------------------
         
         400 response:
         
         +---------------+--------------------+
         | error_code    | error_msg          |
@@ -262,15 +315,14 @@
         +---------------+--------------------+
         
         Additional information
         ----------------------
         
         This package also support *django tranlations*.
         
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ngits-users-1.0.6/README.rst` & `ngits-users-1.0.7/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -323,39 +323,109 @@
 00001420: 616e 6765 5f70 6173 7377 6f72 645f 656d  ange_password_em
 00001430: 6169 6c2e 7478 740a 2020 2020 2020 2020  ail.txt.        
 00001440: 2020 2020 2f63 6861 6e67 655f 7061 7373      /change_pass
 00001450: 776f 7264 2e68 746d 6c0a 0a2a 466f 7220  word.html..*For 
 00001460: 666f 7265 2064 6574 6169 6c73 2063 6865  fore details che
 00001470: 636b 206f 7574 206c 6962 7261 7279 2064  ck out library d
 00001480: 6566 6175 6c74 2074 656d 706c 6174 6573  efault templates
-00001490: 2a0a 0a4c 6f67 696e 2072 6573 706f 6e73  *..Login respons
-000014a0: 6520 636f 6465 730a 2d2d 2d2d 2d2d 2d2d  e codes.--------
-000014b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 3430  ------------..40
-000014c0: 3020 7265 7370 6f6e 7365 3a0a 0a2b 2d2d  0 response:..+--
-000014d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-000014e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000014f0: 2d2d 2b0a 7c20 6572 726f 725f 636f 6465  --+.| error_code
-00001500: 2020 2020 7c20 6572 726f 725f 6d73 6720      | error_msg 
-00001510: 2020 2020 2020 2020 207c 0a2b 3d3d 3d3d           |.+====
-00001520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  ===========+====
-00001530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001540: 2b0a 7c20 3030 2020 2020 2020 2020 2020  +.| 00          
-00001550: 2020 7c20 4c6f 6769 6e20 6661 696c 6564    | Login failed
-00001560: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-00001570: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00001580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
-00001590: 7c20 3031 2020 2020 2020 2020 2020 2020  | 01            
-000015a0: 7c20 5573 6572 206e 6f74 2066 6f75 6e64  | User not found
-000015b0: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
-000015c0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000015d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
-000015e0: 3032 2020 2020 2020 2020 2020 2020 7c20  02            | 
-000015f0: 5573 6572 206e 6f74 2061 6374 6976 6520  User not active 
-00001600: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00001610: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00001620: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a41 6464  ----------+..Add
-00001630: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
-00001640: 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ion.------------
-00001650: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6973  ----------..This
-00001660: 2070 6163 6b61 6765 2061 6c73 6f20 7375   package also su
-00001670: 7070 6f72 7420 2a64 6a61 6e67 6f20 7472  pport *django tr
-00001680: 616e 6c61 7469 6f6e 732a 2e0a 0a         anlations*...
+00001490: 2a0a 0a39 2e20 4f70 7469 6f6e 616c 2060  *..9. Optional `
+000014a0: 6054 6f6b 656e 5365 7269 616c 697a 6572  `TokenSerializer
+000014b0: 6060 206f 7665 7272 6964 653a 0a7e 7e7e  `` override:.~~~
+000014c0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+000014d0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+000014e0: 7e7e 7e7e 7e7e 0a0a 596f 7520 6361 6e20  ~~~~~~..You can 
+000014f0: 6f76 6572 7269 6465 2060 6054 6f6b 656e  override ``Token
+00001500: 5365 7269 616c 697a 6572 6060 202d 2074  Serializer`` - t
+00001510: 6865 2064 6566 6175 6c74 2072 6573 706f  he default respo
+00001520: 6e73 6520 7365 7269 616c 697a 6572 206f  nse serializer o
+00001530: 6e20 6060 4c6f 6769 6e56 6965 7760 6020  n ``LoginView`` 
+00001540: 6028 2f6c 6f67 696e 2960 2e0a 0a49 6e20  `(/login)`...In 
+00001550: 6f72 6465 7220 746f 2075 7365 2079 6f75  order to use you
+00001560: 7220 6f77 6e20 7365 7269 616c 697a 6572  r own serializer
+00001570: 2c20 796f 7520 6e65 6564 2074 6f20 666f  , you need to fo
+00001580: 6c6c 6f77 2074 6865 7365 2073 7465 7073  llow these steps
+00001590: 3a0a 0a31 2e20 4372 6561 7465 2079 6f75  :..1. Create you
+000015a0: 7220 6375 7374 6f6d 2073 6572 6961 6c69  r custom seriali
+000015b0: 7a65 723a 0a0a 652e 672e 3a0a 0a3a 3a0a  zer:..e.g.:..::.
+000015c0: 0a20 2020 2066 726f 6d20 7265 7374 5f66  .    from rest_f
+000015d0: 7261 6d65 776f 726b 2069 6d70 6f72 7420  ramework import 
+000015e0: 7365 7269 616c 697a 6572 730a 2020 2020  serializers.    
+000015f0: 6672 6f6d 2072 6573 745f 6672 616d 6577  from rest_framew
+00001600: 6f72 6b2e 6175 7468 746f 6b65 6e2e 6d6f  ork.authtoken.mo
+00001610: 6465 6c73 2069 6d70 6f72 7420 546f 6b65  dels import Toke
+00001620: 6e0a 0a20 2020 202e 2e2e 0a0a 2020 2020  n..    .....    
+00001630: 636c 6173 7320 5465 7374 5365 7269 616c  class TestSerial
+00001640: 697a 6572 2873 6572 6961 6c69 7a65 7273  izer(serializers
+00001650: 2e4d 6f64 656c 5365 7269 616c 697a 6572  .ModelSerializer
+00001660: 293a 0a20 2020 2020 2020 2066 6f6f 203d  ):.        foo =
+00001670: 2073 6572 6961 6c69 7a65 7273 2e53 6572   serializers.Ser
+00001680: 6961 6c69 7a65 724d 6574 686f 6446 6965  ializerMethodFie
+00001690: 6c64 2829 0a0a 2020 2020 2020 2020 636c  ld()..        cl
+000016a0: 6173 7320 4d65 7461 3a0a 2020 2020 2020  ass Meta:.      
+000016b0: 2020 2020 2020 6d6f 6465 6c20 3d20 546f        model = To
+000016c0: 6b65 6e0a 2020 2020 2020 2020 2020 2020  ken.            
+000016d0: 6669 656c 6473 203d 2028 226b 6579 222c  fields = ("key",
+000016e0: 2022 7573 6572 5f69 6422 2c20 2266 6f6f   "user_id", "foo
+000016f0: 2229 0a0a 2020 2020 2020 2020 6465 6620  ")..        def 
+00001700: 6765 745f 666f 6f28 7365 6c66 2c20 6f62  get_foo(self, ob
+00001710: 6a29 3a0a 2020 2020 2020 2020 2020 2020  j):.            
+00001720: 7265 7475 726e 2022 6261 7222 0a0a 2a2a  return "bar"..**
+00001730: 5761 726e 696e 6721 2a2a 2059 6f75 7220  Warning!** Your 
+00001740: 6375 7374 6f6d 2073 6572 6961 6c69 7a65  custom serialize
+00001750: 7220 6d75 7374 2068 616e 646c 6520 696e  r must handle in
+00001760: 636f 6d69 6e67 2044 5246 2060 6054 6f6b  coming DRF ``Tok
+00001770: 656e 6060 206f 626a 6563 7421 0a0a 322e  en`` object!..2.
+00001780: 2053 6574 2073 6572 6961 6c69 7a65 7220   Set serializer 
+00001790: 7061 7468 2069 6e20 796f 7572 2060 6073  path in your ``s
+000017a0: 6574 7469 6e67 7360 6020 6669 6c65 0a0a  ettings`` file..
+000017b0: 652e 672e 3a0a 0a3a 3a0a 0a20 2020 204c  e.g.:..::..    L
+000017c0: 4f47 494e 5f52 4553 504f 4e53 455f 5345  OGIN_RESPONSE_SE
+000017d0: 5249 414c 495a 4552 5f50 4154 4820 3d20  RIALIZER_PATH = 
+000017e0: 2261 7070 2e73 6572 6961 6c69 7a65 7273  "app.serializers
+000017f0: 2e54 6573 7453 6572 6961 6c69 7a65 7222  .TestSerializer"
+00001800: 0a0a 332e 2054 616b 6520 6974 2066 6f72  ..3. Take it for
+00001810: 2061 2073 7069 6e21 0a0a 3a3a 0a0a 2020   a spin!..::..  
+00001820: 2020 4854 5450 2032 3030 204f 4b0a 2020    HTTP 200 OK.  
+00001830: 2020 416c 6c6f 773a 2050 4f53 542c 204f    Allow: POST, O
+00001840: 5054 494f 4e53 0a20 2020 2043 6f6e 7465  PTIONS.    Conte
+00001850: 6e74 2d54 7970 653a 2061 7070 6c69 6361  nt-Type: applica
+00001860: 7469 6f6e 2f6a 736f 6e0a 2020 2020 5661  tion/json.    Va
+00001870: 7279 3a20 4163 6365 7074 0a0a 2020 2020  ry: Accept..    
+00001880: 7b0a 2020 2020 2020 2020 226b 6579 223a  {.        "key":
+00001890: 2022 6135 3835 3165 3733 3539 6431 6430   "a5851e7359d1d0
+000018a0: 3463 6439 3961 3236 3031 3465 3437 6663  4cd99a26014e47fc
+000018b0: 6265 6461 6130 6265 6561 222c 0a20 2020  bedaa0beea",.   
+000018c0: 2020 2020 2022 7573 6572 5f69 6422 3a20       "user_id": 
+000018d0: 312c 0a20 2020 2020 2020 2022 666f 6f22  1,.        "foo"
+000018e0: 3a20 2262 6172 220a 2020 2020 7d0a 0a4c  : "bar".    }..L
+000018f0: 6f67 696e 2072 6573 706f 6e73 6520 636f  ogin response co
+00001900: 6465 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  des.------------
+00001910: 2d2d 2d2d 2d2d 2d2d 0a0a 3430 3020 7265  --------..400 re
+00001920: 7370 6f6e 7365 3a0a 0a2b 2d2d 2d2d 2d2d  sponse:..+------
+00001930: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00001940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
+00001950: 7c20 6572 726f 725f 636f 6465 2020 2020  | error_code    
+00001960: 7c20 6572 726f 725f 6d73 6720 2020 2020  | error_msg     
+00001970: 2020 2020 207c 0a2b 3d3d 3d3d 3d3d 3d3d       |.+========
+00001980: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
+00001990: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2b0a 7c20  ============+.| 
+000019a0: 3030 2020 2020 2020 2020 2020 2020 7c20  00            | 
+000019b0: 4c6f 6769 6e20 6661 696c 6564 2020 2020  Login failed    
+000019c0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
+000019d0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+000019e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 3031  ----------+.| 01
+000019f0: 2020 2020 2020 2020 2020 2020 7c20 5573              | Us
+00001a00: 6572 206e 6f74 2066 6f75 6e64 2020 2020  er not found    
+00001a10: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+00001a20: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+00001a30: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 3032 2020  --------+.| 02  
+00001a40: 2020 2020 2020 2020 2020 7c20 5573 6572            | User
+00001a50: 206e 6f74 2061 6374 6976 6520 2020 207c   not active    |
+00001a60: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+00001a70: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00001a80: 2d2d 2d2d 2d2d 2b0a 0a41 6464 6974 696f  ------+..Additio
+00001a90: 6e61 6c20 696e 666f 726d 6174 696f 6e0a  nal information.
+00001aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001ab0: 2d2d 2d2d 2d2d 0a0a 5468 6973 2070 6163  ------..This pac
+00001ac0: 6b61 6765 2061 6c73 6f20 7375 7070 6f72  kage also suppor
+00001ad0: 7420 2a64 6a61 6e67 6f20 7472 616e 6c61  t *django tranla
+00001ae0: 7469 6f6e 732a 2e0a                      tions*..
```

### Comparing `ngits-users-1.0.6/pyproject.toml` & `ngits-users-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/setup.cfg` & `ngits-users-1.0.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ngits-users
-version = 1.0.6
+version = 1.0.7
 description = Base users application for Django projects
 long_description = file: README.rst
 url = https://ngits.dev
 author = NGITs
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
```

### Comparing `ngits-users-1.0.6/src/ngits_users.egg-info/PKG-INFO` & `ngits-users-1.0.7/src/ngits_users.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ngits-users
-Version: 1.0.6
+Version: 1.0.7
 Summary: Base users application for Django projects
 Home-page: https://ngits.dev
 Author: NGITs
 License: BSD-3-Clause
 Description: ngits-users
         ============
         
@@ -242,14 +242,67 @@
                 /templates
                     /change_password_email.html
                     /change_password_email.txt
                     /change_password.html
         
         *For fore details check out library default templates*
         
+        9. Optional ``TokenSerializer`` override:
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        You can override ``TokenSerializer`` - the default response serializer on ``LoginView`` `(/login)`.
+        
+        In order to use your own serializer, you need to follow these steps:
+        
+        1. Create your custom serializer:
+        
+        e.g.:
+        
+        ::
+        
+            from rest_framework import serializers
+            from rest_framework.authtoken.models import Token
+        
+            ...
+        
+            class TestSerializer(serializers.ModelSerializer):
+                foo = serializers.SerializerMethodField()
+        
+                class Meta:
+                    model = Token
+                    fields = ("key", "user_id", "foo")
+        
+                def get_foo(self, obj):
+                    return "bar"
+        
+        **Warning!** Your custom serializer must handle incoming DRF ``Token`` object!
+        
+        2. Set serializer path in your ``settings`` file
+        
+        e.g.:
+        
+        ::
+        
+            LOGIN_RESPONSE_SERIALIZER_PATH = "app.serializers.TestSerializer"
+        
+        3. Take it for a spin!
+        
+        ::
+        
+            HTTP 200 OK
+            Allow: POST, OPTIONS
+            Content-Type: application/json
+            Vary: Accept
+        
+            {
+                "key": "a5851e7359d1d04cd99a26014e47fcbedaa0beea",
+                "user_id": 1,
+                "foo": "bar"
+            }
+        
         Login response codes
         --------------------
         
         400 response:
         
         +---------------+--------------------+
         | error_code    | error_msg          |
@@ -262,15 +315,14 @@
         +---------------+--------------------+
         
         Additional information
         ----------------------
         
         This package also support *django tranlations*.
         
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ngits-users-1.0.6/src/ngits_users.egg-info/SOURCES.txt` & `ngits-users-1.0.7/src/ngits_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/forms.py` & `ngits-users-1.0.7/src/users/forms.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/migrations/0001_initial.py` & `ngits-users-1.0.7/src/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/schemas.py` & `ngits-users-1.0.7/src/users/schemas.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/serializers.py` & `ngits-users-1.0.7/src/users/serializers.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/static/users/css/style.css` & `ngits-users-1.0.7/src/users/static/users/css/style.css`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/static/users/img/fail.svg` & `ngits-users-1.0.7/src/users/static/users/img/fail.svg`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/static/users/img/success.svg` & `ngits-users-1.0.7/src/users/static/users/img/success.svg`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/tasks.py` & `ngits-users-1.0.7/src/users/tasks.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/templates/change_password.html` & `ngits-users-1.0.7/src/users/templates/change_password.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/templates/form_site.html` & `ngits-users-1.0.7/src/users/templates/form_site.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/templates/info_site.html` & `ngits-users-1.0.7/src/users/templates/info_site.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/urls.py` & `ngits-users-1.0.7/src/users/urls.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/utils.py` & `ngits-users-1.0.7/src/users/utils.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.6/src/users/views.py` & `ngits-users-1.0.7/src/users/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from uuid import uuid4
 
+from django.conf import settings
 from django.contrib.auth import authenticate, get_user_model
+from django.core.exceptions import ImproperlyConfigured
 from django.http import HttpResponse
 from django.template.loader import get_template
+from django.utils.module_loading import import_string
 from django.utils.translation import gettext as _
 from django.views.generic import TemplateView
 from django.views.generic.edit import FormView
 from drf_spectacular.utils import (
     OpenApiTypes,
     extend_schema,
     extend_schema_view,
@@ -89,14 +92,28 @@
         responses={200: TokenSerializer, 400: OpenApiTypes.OBJECT},
         examples=[
             schemas.ACCOUNT_LOGIN_FAILED_RESPONSE,
         ],
     )
 )
 class StandardLoginView(APIView):
+    @classmethod
+    def get_response_serializer_class(self):
+        LOGIN_RESPONSE_SERIALIZER_PATH = getattr(
+            settings, "LOGIN_RESPONSE_SERIALIZER_PATH", None
+        )
+
+        if LOGIN_RESPONSE_SERIALIZER_PATH:
+            try:
+                return import_string(LOGIN_RESPONSE_SERIALIZER_PATH)
+            except ImportError:
+                raise ImproperlyConfigured("Module cannot be resolved.")
+
+        return TokenSerializer
+
     def post(self, request):
         serializer = StandardLoginSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         try:
             user = User.objects.get(email=serializer.data["email"])
             if not user.is_active:
@@ -112,16 +129,17 @@
 
         user = authenticate(
             username=serializer.data["email"],
             password=serializer.data["password"],
         )
 
         if user is not None:
-            token_serializer = TokenSerializer(user.auth_token)
-            return Response(token_serializer.data, status=status.HTTP_200_OK)
+            serializer_class = self.get_response_serializer_class()
+            response_data = serializer_class(user.auth_token).data
+            return Response(response_data, status=status.HTTP_200_OK)
         else:
             return Response(
                 {"error_code": "00", "error_msg": _("Login failed!")},
                 status=status.HTTP_400_BAD_REQUEST,
             )
```

