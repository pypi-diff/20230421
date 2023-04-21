# Comparing `tmp/onevizion-1.1.1.tar.gz` & `tmp/onevizion-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onevizion-1.1.1.tar", last modified: Tue Nov 22 03:55:49 2022, max compression
+gzip compressed data, was "dist/onevizion-1.1.2.tar", last modified: Fri Apr 21 17:45:51 2023, max compression
```

## Comparing `onevizion-1.1.1.tar` & `onevizion-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2022-11-22 03:55:49.000000 onevizion-1.1.1/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2022-11-22 03:55:49.000000 onevizion-1.1.1/onevizion.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)      583 2022-11-22 03:55:48.000000 onevizion-1.1.1/onevizion.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      668 2022-11-22 03:55:48.000000 onevizion-1.1.1/onevizion.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        9 2022-11-22 03:55:48.000000 onevizion-1.1.1/onevizion.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)       10 2022-11-22 03:55:48.000000 onevizion-1.1.1/onevizion.egg-info/top_level.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2022-11-22 03:55:48.000000 onevizion-1.1.1/onevizion.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)      583 2022-11-22 03:55:49.000000 onevizion-1.1.1/PKG-INFO
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2022-11-22 03:55:49.000000 onevizion-1.1.1/onevizion/
--rw-r--r--   0 mike       (501) staff       (20)     8184 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/Import.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2022-11-22 03:55:49.000000 onevizion-1.1.1/onevizion/notif/
--rw-r--r--   0 mike       (501) staff       (20)     2902 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/notif/queue.py
--rw-r--r--   0 mike       (501) staff       (20)      138 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/notif/queuestatus.py
--rw-r--r--   0 mike       (501) staff       (20)     5113 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/notif/service.py
--rw-r--r--   0 mike       (501) staff       (20)      548 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/notif/queuerecord.py
--rw-r--r--   0 mike       (501) staff       (20)      150 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/notif/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     4153 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/task.py
--rw-r--r--   0 mike       (501) staff       (20)     2539 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/curl.py
--rw-r--r--   0 mike       (501) staff       (20)     2399 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/ovimport.py
--rw-r--r--   0 mike       (501) staff       (20)     3978 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/util.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2022-11-22 03:55:49.000000 onevizion-1.1.1/onevizion/integration/
--rw-r--r--   0 mike       (501) staff       (20)     2213 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/integration/log.py
--rw-r--r--   0 mike       (501) staff       (20)      693 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/integration/loglevel.py
--rw-r--r--   0 mike       (501) staff       (20)       81 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/integration/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     1578 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)    20386 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/trackor.py
--rw-r--r--   0 mike       (501) staff       (20)     8769 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/export.py
--rw-r--r--   0 mike       (501) staff       (20)     5932 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/EMail.py
--rw-r--r--   0 mike       (501) staff       (20)     3037 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/singleton.py
--rw-r--r--   0 mike       (501) staff       (20)     3274 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/workplan.py
--rw-r--r--   0 mike       (501) staff       (20)      483 2022-11-22 03:53:43.000000 onevizion-1.1.1/onevizion/httpbearer.py
--rw-r--r--   0 mike       (501) staff       (20)     2593 2018-01-30 14:57:48.000000 onevizion-1.1.1/README.md
--rwxr-xr-x   0 mike       (501) staff       (20)     1063 2022-11-22 03:53:43.000000 onevizion-1.1.1/setup.py
--rw-r--r--   0 mike       (501) staff       (20)       38 2022-11-22 03:55:49.000000 onevizion-1.1.1/setup.cfg
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-21 17:45:51.000000 onevizion-1.1.2/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion.egg-info/
+-rw-r--r--   0 mike       (501) staff       (20)      583 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion.egg-info/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)      668 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion.egg-info/SOURCES.txt
+-rw-r--r--   0 mike       (501) staff       (20)        9 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion.egg-info/requires.txt
+-rw-r--r--   0 mike       (501) staff       (20)       10 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion.egg-info/top_level.txt
+-rw-r--r--   0 mike       (501) staff       (20)        1 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion.egg-info/dependency_links.txt
+-rw-r--r--   0 mike       (501) staff       (20)      583 2023-04-21 17:45:51.000000 onevizion-1.1.2/PKG-INFO
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion/
+-rw-r--r--   0 mike       (501) staff       (20)     8184 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/Import.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion/notif/
+-rw-r--r--   0 mike       (501) staff       (20)     2902 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/notif/queue.py
+-rw-r--r--   0 mike       (501) staff       (20)      138 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/notif/queuestatus.py
+-rw-r--r--   0 mike       (501) staff       (20)     5113 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/notif/service.py
+-rw-r--r--   0 mike       (501) staff       (20)      548 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/notif/queuerecord.py
+-rw-r--r--   0 mike       (501) staff       (20)      150 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/notif/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)     4153 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/task.py
+-rw-r--r--   0 mike       (501) staff       (20)     2539 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/curl.py
+-rw-r--r--   0 mike       (501) staff       (20)     2399 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/ovimport.py
+-rw-r--r--   0 mike       (501) staff       (20)     3978 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/util.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-21 17:45:51.000000 onevizion-1.1.2/onevizion/integration/
+-rw-r--r--   0 mike       (501) staff       (20)     2213 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/integration/log.py
+-rw-r--r--   0 mike       (501) staff       (20)      693 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/integration/loglevel.py
+-rw-r--r--   0 mike       (501) staff       (20)       81 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/integration/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)     1578 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)    20386 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/trackor.py
+-rw-r--r--   0 mike       (501) staff       (20)     8769 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/export.py
+-rw-r--r--   0 mike       (501) staff       (20)     5961 2023-04-21 17:45:43.000000 onevizion-1.1.2/onevizion/EMail.py
+-rw-r--r--   0 mike       (501) staff       (20)     3037 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/singleton.py
+-rw-r--r--   0 mike       (501) staff       (20)     3274 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/workplan.py
+-rw-r--r--   0 mike       (501) staff       (20)      483 2022-11-22 03:53:43.000000 onevizion-1.1.2/onevizion/httpbearer.py
+-rw-r--r--   0 mike       (501) staff       (20)     2593 2018-01-30 14:57:48.000000 onevizion-1.1.2/README.md
+-rwxr-xr-x   0 mike       (501) staff       (20)     1063 2023-04-21 17:45:43.000000 onevizion-1.1.2/setup.py
+-rw-r--r--   0 mike       (501) staff       (20)       38 2023-04-21 17:45:51.000000 onevizion-1.1.2/setup.cfg
```

### Comparing `onevizion-1.1.1/onevizion.egg-info/PKG-INFO` & `onevizion-1.1.2/onevizion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: onevizion
-Version: 1.1.1
+Version: 1.1.2
 Summary: onevizion wraps the version 3 API for a OneVizion system, and provides a few optional other utilities.
 Home-page: https://github.com/Onevizion/API-v3
 Author: OneVizion
 Author-email: development@onevizion.com
 License: MIT
 Description: UNKNOWN
 Platform: Unix
```

### Comparing `onevizion-1.1.1/onevizion.egg-info/SOURCES.txt` & `onevizion-1.1.2/onevizion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/PKG-INFO` & `onevizion-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: onevizion
-Version: 1.1.1
+Version: 1.1.2
 Summary: onevizion wraps the version 3 API for a OneVizion system, and provides a few optional other utilities.
 Home-page: https://github.com/Onevizion/API-v3
 Author: OneVizion
 Author-email: development@onevizion.com
 License: MIT
 Description: UNKNOWN
 Platform: Unix
```

### Comparing `onevizion-1.1.1/onevizion/Import.py` & `onevizion-1.1.2/onevizion/Import.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/notif/queue.py` & `onevizion-1.1.2/onevizion/notif/queue.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/notif/service.py` & `onevizion-1.1.2/onevizion/notif/service.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/notif/queuerecord.py` & `onevizion-1.1.2/onevizion/notif/queuerecord.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/task.py` & `onevizion-1.1.2/onevizion/task.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/curl.py` & `onevizion-1.1.2/onevizion/curl.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/ovimport.py` & `onevizion-1.1.2/onevizion/ovimport.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/util.py` & `onevizion-1.1.2/onevizion/util.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/integration/log.py` & `onevizion-1.1.2/onevizion/integration/log.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/integration/loglevel.py` & `onevizion-1.1.2/onevizion/integration/loglevel.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/__init__.py` & `onevizion-1.1.2/onevizion/__init__.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/trackor.py` & `onevizion-1.1.2/onevizion/trackor.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/export.py` & `onevizion-1.1.2/onevizion/export.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/EMail.py` & `onevizion-1.1.2/onevizion/EMail.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 		from email.mime.text import MIMEText
 		msg = MIMEMultipart()
 		msg['To'] = ", ".join(self.to )
 		if self.sender != '':
 			msg['From'] = self.sender
 		else:
 			msg['From'] = self.userName
+			self.sender = self.userName
 		msg['Subject'] = self.subject
 
 		body = self.message + "\n"
 
 		for key,value in self.info.items():
 			body = body + "\n\n" + key + ":"
 			if isinstance(value, basestring):
@@ -174,14 +175,14 @@
 			send = smtplib.SMTP(self.server, int(self.port))
 			send.starttls()
 		elif self.security.upper() in ['SSL','SSL/TLS']:
 			send = smtplib.SMTP_SSL(self.server, self.port)
 		else:
 			send = smtplib.SMTP(self.server, int(self.port))
 		send.login(str(self.userName), str(self.password))
-		send.sendmail(str(self.userName),self.to, msg.as_string())
+		send.sendmail(str(self.sender),self.to, msg.as_string())
 		send.quit()
 
 		after = datetime.utcnow()
 		delta = after - before
 		self.duration = delta.total_seconds()
 		Message("Sent Mail in {Duration} seconds.".format(Duration=self.duration),1)
```

### Comparing `onevizion-1.1.1/onevizion/singleton.py` & `onevizion-1.1.2/onevizion/singleton.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/onevizion/workplan.py` & `onevizion-1.1.2/onevizion/workplan.py`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/README.md` & `onevizion-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `onevizion-1.1.1/setup.py` & `onevizion-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import os
 import sys
 from setuptools import setup, find_packages
 #from onevizion import __version__
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 
 #following PyPI guide: https://hynek.me/articles/sharing-your-labor-of-love-pypi-quick-and-dirty/
 
 def read(*paths):
 	"""Build a file path from *paths* and return the contents."""
 	from io import open
 	with open(os.path.join(*paths), 'rb') as f:
```

