# Comparing `tmp/ovos-backend-client-0.0.7a2.tar.gz` & `tmp/ovos-backend-client-0.0.7a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.0.7a2.tar", last modified: Wed Feb 15 17:41:49 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.0.7a3.tar", last modified: Fri Apr 21 20:42:35 2023, max compression
```

## Comparing `ovos-backend-client-0.0.7a2.tar` & `ovos-backend-client-0.0.7a3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 17:41:49.082086 ovos-backend-client-0.0.7a2/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-15 17:41:49.082086 ovos-backend-client-0.0.7a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 17:41:49.078086 ovos-backend-client-0.0.7a2/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 17:41:49.082086 ovos-backend-client-0.0.7a2/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22656 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/backends/ovos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/backends/selene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-15 17:41:39.000000 ovos-backend-client-0.0.7a2/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 17:41:49.078086 ovos-backend-client-0.0.7a2/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-15 17:41:48.000000 ovos-backend-client-0.0.7a2/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-15 17:41:49.000000 ovos-backend-client-0.0.7a2/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 17:41:48.000000 ovos-backend-client-0.0.7a2/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-15 17:41:48.000000 ovos-backend-client-0.0.7a2/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-15 17:41:48.000000 ovos-backend-client-0.0.7a2/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 17:41:49.082086 ovos-backend-client-0.0.7a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-02-15 17:41:36.000000 ovos-backend-client-0.0.7a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:42:35.868020 ovos-backend-client-0.0.7a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 20:42:35.868020 ovos-backend-client-0.0.7a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:42:35.864020 ovos-backend-client-0.0.7a3/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:42:35.868020 ovos-backend-client-0.0.7a3/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/backends/ovos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/backends/selene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-21 20:42:27.000000 ovos-backend-client-0.0.7a3/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:42:35.868020 ovos-backend-client-0.0.7a3/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 20:42:35.000000 ovos-backend-client-0.0.7a3/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-21 20:42:35.000000 ovos-backend-client-0.0.7a3/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:42:35.000000 ovos-backend-client-0.0.7a3/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 20:42:35.000000 ovos-backend-client-0.0.7a3/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 20:42:35.000000 ovos-backend-client-0.0.7a3/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 20:42:35.868020 ovos-backend-client-0.0.7a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-21 20:42:21.000000 ovos-backend-client-0.0.7a3/setup.py
```

### Comparing `ovos-backend-client-0.0.7a2/README.md` & `ovos-backend-client-0.0.7a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/api.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/api.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/backends/offline.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,14 +551,16 @@
 
         Args:
             audio (bytes): The recorded audio, as in a FLAC file
             language (str): A BCP-47 language code, e.g. "en-US"
             limit (int): Maximum alternate transcriptions
 
        """
+        from speech_recognition import Recognizer, AudioFile
+
         if self.stt is None:
             self.load_stt_plugin(lang=language)
         with NamedTemporaryFile() as fp:
             fp.write(audio)
             with AudioFile(fp.name) as source:
                 audio = Recognizer().record(source)
         tx = self.stt.execute(audio, language)
```

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/backends/ovos.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/backends/ovos.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/backends/personal.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/backends/selene.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/backends/selene.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/cloud.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/config.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/database.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/database.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/identity.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/identity.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/pairing.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client/settings.py` & `ovos-backend-client-0.0.7a3/ovos_backend_client/settings.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.0.7a3/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a2/setup.py` & `ovos-backend-client-0.0.7a3/setup.py`

 * *Files identical despite different names*

