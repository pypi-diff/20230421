# Comparing `tmp/python-timeout-4.7.tar.gz` & `tmp/python-timeout-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-timeout-4.7.tar", last modified: Fri Mar 31 15:22:42 2023, max compression
+gzip compressed data, was "python-timeout-4.8.tar", last modified: Thu Apr 20 18:21:59 2023, max compression
```

## Comparing `python-timeout-4.7.tar` & `python-timeout-4.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 15:22:42.226952 python-timeout-4.7/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-4.7/.gitignore
--rw-rw-rw-   0        0        0      973 2023-03-31 15:22:42.227951 python-timeout-4.7/PKG-INFO
--rw-rw-rw-   0        0        0      757 2022-05-11 17:10:57.000000 python-timeout-4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 15:22:42.225953 python-timeout-4.7/python_timeout.egg-info/
--rw-rw-rw-   0        0        0      973 2023-03-31 15:22:40.000000 python-timeout-4.7/python_timeout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-03-31 15:22:40.000000 python-timeout-4.7/python_timeout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 15:22:40.000000 python-timeout-4.7/python_timeout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-31 15:22:40.000000 python-timeout-4.7/python_timeout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-31 15:22:40.000000 python-timeout-4.7/python_timeout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-31 15:22:42.227951 python-timeout-4.7/setup.cfg
--rw-rw-rw-   0        0        0      394 2023-03-31 15:22:35.000000 python-timeout-4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 15:22:42.225953 python-timeout-4.7/timeout/
--rw-rw-rw-   0        0        0     5797 2023-03-31 15:22:31.000000 python-timeout-4.7/timeout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:21:59.492435 python-timeout-4.8/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-4.8/.gitignore
+-rw-rw-rw-   0        0        0      973 2023-04-20 18:21:59.493435 python-timeout-4.8/PKG-INFO
+-rw-rw-rw-   0        0        0      757 2022-05-11 17:10:57.000000 python-timeout-4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 18:21:59.490437 python-timeout-4.8/python_timeout.egg-info/
+-rw-rw-rw-   0        0        0      973 2023-04-20 18:21:59.000000 python-timeout-4.8/python_timeout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-04-20 18:21:59.000000 python-timeout-4.8/python_timeout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 18:21:59.000000 python-timeout-4.8/python_timeout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-20 18:21:59.000000 python-timeout-4.8/python_timeout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-20 18:21:59.000000 python-timeout-4.8/python_timeout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 18:21:59.494434 python-timeout-4.8/setup.cfg
+-rw-rw-rw-   0        0        0      394 2023-04-20 18:21:40.000000 python-timeout-4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 18:21:59.491436 python-timeout-4.8/timeout/
+-rw-rw-rw-   0        0        0     5861 2023-04-20 18:21:37.000000 python-timeout-4.8/timeout/__init__.py
```

### Comparing `python-timeout-4.7/PKG-INFO` & `python-timeout-4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 4.7
+Version: 4.8
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
 
 ### Timeout
 Random timeout between minimum and maximum values
```

### Comparing `python-timeout-4.7/README.md` & `python-timeout-4.8/README.md`

 * *Files identical despite different names*

### Comparing `python-timeout-4.7/python_timeout.egg-info/PKG-INFO` & `python-timeout-4.8/python_timeout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 4.7
+Version: 4.8
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
 
 ### Timeout
 Random timeout between minimum and maximum values
```

### Comparing `python-timeout-4.7/timeout/__init__.py` & `python-timeout-4.8/timeout/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,31 +49,31 @@
                 
         timeout_in_seconds = uniform(minimum, maximum) # Random float between minimum and maximum
         if not silent:
             if timeout_in_seconds < 60:
                 printr('Sleeping', timeout_in_seconds, 'seconds', level='debug')
             elif timeout_in_seconds > 86400:
                 timeout_in_days = round(timeout_in_seconds / 86400) # Convert sleep time in seconds to days
-                til = datetime.now() + timedelta(days=timeout_in_days)
+                til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%A, %B %e')
                 if timeout_in_days == 1:
                     printr('Sleeping 1 day until', til)
                 else:
                     printr('Sleeping', timeout_in_days, 'days until', til)
             elif timeout_in_seconds > 3600:
                 timeout_in_hours = round(timeout_in_seconds / 3600) # Convert sleep time in seconds to hours
-                til = datetime.now() + timedelta(hours=timeout_in_hours)
+                til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_hours == 1:
                     printr('Sleeping 1 hour until', til)
                 else:
                     printr('Sleeping', timeout_in_hours, 'hours until', til)
             elif timeout_in_seconds >= 60:
                 timeout_in_minutes = round(timeout_in_seconds / 60) # Convert sleep time in seconds to minutes
-                til = datetime.now() + timedelta(minutes=timeout_in_minutes)
+                til = datetime.now() + timedelta(timeout_in_seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_minutes == 1:
                     printr('Sleeping 1 minute until', til)
                 else:
                     printr('Sleeping', timeout_in_minutes, 'minutes until', til)
 
         sleep(timeout_in_seconds)
@@ -91,31 +91,31 @@
             timeout_in_seconds = days * 86400
 
         if not silent:
             if timeout_in_seconds < 60:
                 printr('Sleeping', timeout_in_seconds, 'seconds', level='debug')
             elif timeout_in_seconds > 86400:
                 timeout_in_days = round(timeout_in_seconds / 86400) # Convert sleep time in seconds to days
-                til = datetime.now() + timedelta(days=timeout_in_days)
+                til = datetime.now() + timedelta(timeout_in_seconds=timeout_in_seconds)
                 til = til.strftime('%A, %B %e')
                 if timeout_in_days == 1:
                     printr('Sleeping 1 day until', til)
                 else:
                     printr('Sleeping', timeout_in_days, 'days until', til)
             elif timeout_in_seconds > 3600:
                 timeout_in_hours = round(timeout_in_seconds / 3600) # Convert sleep time in seconds to hours
-                til = datetime.now() + timedelta(hours=timeout_in_hours)
+                til = datetime.now() + timedelta(timeout_in_seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_hours == 1:
                     printr('Sleeping 1 hour until', til)
                 else:
                     printr('Sleeping', timeout_in_hours, 'hours until', til)
             elif timeout_in_seconds >= 60:
                 timeout_in_minutes = round(timeout_in_seconds / 60) # Convert sleep time in seconds to minutes
-                til = datetime.now() + timedelta(minutes=timeout_in_minutes)
+                til = datetime.now() + timedelta(timeout_in_seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_minutes == 1:
                     printr('Sleeping 1 minute until', til)
                 else:
                     printr('Sleeping', timeout_in_minutes, 'minutes until', til)
 
         sleep(timeout_in_seconds)
```

