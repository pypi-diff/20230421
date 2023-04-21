# Comparing `tmp/driveup-0.2.1.tar.gz` & `tmp/driveup-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driveup-0.2.1.tar", last modified: Wed Apr 19 12:25:30 2023, max compression
+gzip compressed data, was "driveup-0.2.2.tar", last modified: Thu Apr 20 13:00:56 2023, max compression
```

## Comparing `driveup-0.2.1.tar` & `driveup-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:25:30.934874 driveup-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:25:30.934874 driveup-0.2.1/Driveup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:25:19.000000 driveup-0.2.1/Driveup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-19 12:25:19.000000 driveup-0.2.1/Driveup/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 12:25:19.000000 driveup-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 12:25:30.934874 driveup-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 12:25:19.000000 driveup-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:25:30.934874 driveup-0.2.1/driveup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:25:30.934874 driveup-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-19 12:25:19.000000 driveup-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:00:56.156671 driveup-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:00:56.152671 driveup-0.2.2/Driveup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:00:41.000000 driveup-0.2.2/Driveup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-20 13:00:41.000000 driveup-0.2.2/Driveup/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 13:00:41.000000 driveup-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 13:00:56.156671 driveup-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 13:00:41.000000 driveup-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:00:56.156671 driveup-0.2.2/driveup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 13:00:56.000000 driveup-0.2.2/driveup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-20 13:00:56.000000 driveup-0.2.2/driveup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:00:56.000000 driveup-0.2.2/driveup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 13:00:56.000000 driveup-0.2.2/driveup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 13:00:56.000000 driveup-0.2.2/driveup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:00:56.156671 driveup-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-20 13:00:41.000000 driveup-0.2.2/setup.py
```

### Comparing `driveup-0.2.1/Driveup/drive.py` & `driveup-0.2.2/Driveup/drive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,41 @@
-from pydrive.auth import GoogleAuth
 from pydrive.drive import GoogleDrive
-import re
+from .features.auth import Auth
 import os
+import re
 
 class Drive:
     def __init__(self,client_secret_path=None,credentials_path=None):
         self.client_secret_path = client_secret_path
-        self.credentials_path = credentials_path
-        self.gauth = self.authorize(client_secret_path,credentials_path)
+        self.gauth,self.credentials_path = Auth().authorize(client_secret_path,credentials_path)
         self.drive = GoogleDrive(self.gauth)
-
-    def authorize(self,secret,credentials_path):
-        if credentials_path == None:
-            secret_path = 'credentials.json'
-            if secret != None:
-                GoogleAuth.DEFAULT_SETTINGS['client_config_file'] = secret
-                secret_path = os.path.dirname(secret) + '/' + secret_path
-            gauth = GoogleAuth()
-            gauth.LocalWebserverAuth()
-            gauth.SaveCredentialsFile(secret_path)
-        else:
-            gauth = GoogleAuth()
-            gauth.LoadCredentialsFile(credentials_path)
-
-        return gauth
     
     def upload(self,file_path,folder_id,file_title=None,file_id=None,update=True,convert=False,url=True):
-        
         if url == True:
             folder_id = self.url_to_id(folder_id)
 
         if file_title == None:
             file_title = self.get_filename(file_path)
 
         gfile = None
 
         if update == True:
             gfile = self.update(file_title,file_id,folder_id)
-            
+                
         if gfile == None: # Doesn't exist in the folder already or update=False
             gfile = self.drive.CreateFile({'title': file_title,'parents': [{'id': folder_id}]})
 
         # Read file and set it as the content of this instance.
         gfile.SetContentFile(str(file_path))
 
         if convert == True:
             supported_types = ['application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
-                               'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
-                               'application/vnd.ms-excel',
-                               'application/vnd.openxmlformats-officedocument.presentationml.presentation']
+                                'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
+                                'application/vnd.ms-excel',
+                                'application/vnd.openxmlformats-officedocument.presentationml.presentation']
             if gfile['mimeType'] in supported_types:
                 gfile.Upload(param={'convert':convert}) # Upload the file with conversion. 
             else:
                 gfile.Upload()   
         else:
             gfile.Upload() # Upload the file without conversion.
 
@@ -82,15 +65,15 @@
         file_id = None
         for file in list:
             if file['title'] == name:
                 file_id = file['id']
         
         return file_id
     
-    def upload_folder(self,local_folder_path,folder_id=None,update=True,subfolder=True,subfolder_name=None,subfolder_id=None,recursive=True,convert=False,url=True):
+    def upload_folder(self,local_folder_path,folder_id,update=True,subfolder=True,subfolder_name=None,subfolder_id=None,recursive=True,convert=False,url=True):
 
         if url == True:
             folder_id = self.url_to_id(folder_id)
 
         files_list = os.listdir(local_folder_path)
 
         if subfolder_name == None:
```

### Comparing `driveup-0.2.1/LICENSE` & `driveup-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `driveup-0.2.1/setup.py` & `driveup-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # ...
 
 setup(
     long_description=README_DESCRIPTION,
     long_description_content_type="text/markdown",
     name='driveup',
-    version='0.2.1',
+    version='0.2.2',
     author='Raúl M.R.',
     author_email="raul.martin4bc@gmail.com",
     license="MIT",
     description='Python package for uploading files and folders to Google Drive',
     packages=find_packages(),
     install_requires=[
         'pandas',
```

