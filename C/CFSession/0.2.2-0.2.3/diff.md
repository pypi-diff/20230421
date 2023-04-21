# Comparing `tmp/CFSession-0.2.2.tar.gz` & `tmp/CFSession-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CFSession-0.2.2.tar", last modified: Sun Apr  2 07:44:37 2023, max compression
+gzip compressed data, was "dist\CFSession-0.2.3.tar", last modified: Fri Apr 21 13:19:48 2023, max compression
```

## Comparing `CFSession-0.2.2.tar` & `CFSession-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 07:44:37.935091 CFSession-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-04-02 07:44:37.923089 CFSession-0.2.2/CFSession/
--rw-rw-rw-   0        0        0      472 2022-11-30 08:50:37.000000 CFSession-0.2.2/CFSession/__init__.py
--rw-rw-rw-   0        0        0     6200 2023-04-02 07:08:32.000000 CFSession-0.2.2/CFSession/cf.py
--rw-rw-rw-   0        0        0    11573 2023-04-02 06:02:58.000000 CFSession-0.2.2/CFSession/cfbrowser.py
--rw-rw-rw-   0        0        0      802 2022-10-24 18:04:11.000000 CFSession-0.2.2/CFSession/cfcookie.py
--rw-rw-rw-   0        0        0     1738 2023-03-26 15:42:03.000000 CFSession-0.2.2/CFSession/cfdefaults.py
--rw-rw-rw-   0        0        0     1338 2022-10-24 18:04:11.000000 CFSession-0.2.2/CFSession/cfdirmodel.py
--rw-rw-rw-   0        0        0     2559 2023-04-02 06:47:59.000000 CFSession-0.2.2/CFSession/cfexception.py
-drwxrwxrwx   0        0        0        0 2023-04-02 07:44:37.934089 CFSession-0.2.2/CFSession.egg-info/
--rw-rw-rw-   0        0        0     3705 2023-04-02 07:44:37.000000 CFSession-0.2.2/CFSession.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-02 07:44:37.000000 CFSession-0.2.2/CFSession.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 07:44:37.000000 CFSession-0.2.2/CFSession.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-02 07:44:37.000000 CFSession-0.2.2/CFSession.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-02 07:44:37.000000 CFSession-0.2.2/CFSession.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-10-24 18:04:11.000000 CFSession-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     3705 2023-04-02 07:44:37.935091 CFSession-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2022-12-18 07:13:04.000000 CFSession-0.2.2/README.md
--rw-rw-rw-   0        0        0       86 2023-04-02 07:44:37.937089 CFSession-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-04-02 07:27:25.000000 CFSession-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:19:48.000000 CFSession-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession/
+-rw-rw-rw-   0        0        0      472 2022-11-30 08:50:37.000000 CFSession-0.2.3/CFSession/__init__.py
+-rw-rw-rw-   0        0        0     6200 2023-04-02 08:05:39.000000 CFSession-0.2.3/CFSession/cf.py
+-rw-rw-rw-   0        0        0    11568 2023-04-21 13:07:00.000000 CFSession-0.2.3/CFSession/cfbrowser.py
+-rw-rw-rw-   0        0        0      802 2022-10-24 18:04:11.000000 CFSession-0.2.3/CFSession/cfcookie.py
+-rw-rw-rw-   0        0        0     1738 2023-04-02 08:05:39.000000 CFSession-0.2.3/CFSession/cfdefaults.py
+-rw-rw-rw-   0        0        0     1338 2022-10-24 18:04:11.000000 CFSession-0.2.3/CFSession/cfdirmodel.py
+-rw-rw-rw-   0        0        0     2882 2023-04-09 04:00:18.000000 CFSession-0.2.3/CFSession/cfexception.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/
+-rw-rw-rw-   0        0        0     3664 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 13:19:48.000000 CFSession-0.2.3/CFSession.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-10-24 18:04:11.000000 CFSession-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3664 2023-04-21 13:19:48.000000 CFSession-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2655 2022-12-18 07:13:04.000000 CFSession-0.2.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-21 13:19:48.000000 CFSession-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-04-21 13:18:38.000000 CFSession-0.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `CFSession-0.2.2/CFSession/cf.py` & `CFSession-0.2.3/CFSession/cf.py`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.2/CFSession/cfbrowser.py` & `CFSession-0.2.3/CFSession/cfbrowser.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             except requests.exceptions.URLRequired as e:
                 self.exception = URLRequired(response=e.response)
                 break
             except requests.exceptions.TooManyRedirects as e:
                 self.exception = TooManyRedirects(response=e.response)
                 break
             except requests.exceptions.Timeout as e:
-                self.exception = TimeoutError(response=e.response)
+                self.exception = Timeout(response=e.response)
                 break
             except requests.exceptions.RequestException as e: #When an arbitrary error occurs
                 self.exception = CFException(response=e.response)
                 break
         else:
             caught_code = caught_exception.response.status_code
             if caught_code == 503:
```

### Comparing `CFSession-0.2.2/CFSession/cfcookie.py` & `CFSession-0.2.3/CFSession/cfcookie.py`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.2/CFSession/cfdefaults.py` & `CFSession-0.2.3/CFSession/cfdefaults.py`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.2/CFSession/cfdirmodel.py` & `CFSession-0.2.3/CFSession/cfdirmodel.py`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.2/CFSession/cfexception.py` & `CFSession-0.2.3/CFSession/cfexception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 """
 CFSession.cfexception
 ~~~~~~~~~~~~~
 This module contains the exceptions for CFSession
 """
 
-class CFException(Exception):
+class CFException(Exception): #Parent class
     def __init__(self,message=None,response=None,request=None, *args, **kwargs):
         """There was an ambiguous exception that occurred while handling your
     request."""
         super().__init__(message,*args, **kwargs)
         self.response = response
 
 
 
-class NetworkError(CFException):
+class NetworkError(CFException): #Main class
     def __init__(self, response=None,*args,**kwargs):
         default_message = repr(response)
         super().__init__(default_message,response=response, *args, **kwargs)
 
-class HTTPError(CFException):
+class HTTPError(CFException): #Main class
     def __init__(self, response=None, *args,**kwargs):
         default_message = repr(response)
         super().__init__(default_message,response=response, *args, **kwargs)
 
-class NotFound(HTTPError): 
+class NotFound(HTTPError): #Subclass
     #subclass
     def __init__(self, response=None,*args, **kwargs):
         # if any arguments are passed...
         # If you inherit from the exception that takes message as a keyword
         # maybe you will need to check kwargs here
         super().__init__(response=response, *args, **kwargs)
 
-class CloudflareBlocked(HTTPError):
+class CloudflareBlocked(HTTPError): #Subclass
     #subclass
     def __init__(self, response=None, *args, **kwargs):
         # if any arguments are passed...
         # If you inherit from the exception that takes message as a keyword
         # maybe you will need to check kwargs here
         super().__init__(response=response, *args, **kwargs)
 
-class URLRequired(CFException):
+class URLRequired(CFException): #Main class
     def __init__(self, response, *args, **kwargs):
         default_message = repr(response)
         super().__init__(default_message,response=response, *args, **kwargs)
 
-class TooManyRedirects(CFException):
+class TooManyRedirects(CFException): #Main class
     def __init__(self, response, *args, **kwargs):
         default_message = repr(response)
         super().__init__(default_message,response=response, *args, **kwargs)
 
-class Timeout(CFException):
-    """The request timed out.
-
-    Catching this error will catch both
-    :exc:`~requests.exceptions.ConnectTimeout` and
-    :exc:`~requests.exceptions.ReadTimeout` errors.
-    """
-
-    pass
-
-class ConnectTimeout(Timeout):
-    def __init__(self, response, *args, **kwargs):
+class Timeout(CFException): #Main class
+    def __init__(self, response=None, *args,**kwargs):
         default_message = repr(response)
         super().__init__(default_message,response=response, *args, **kwargs)
 
-class ReadTimeout(Timeout):
-    def __init__(self, response, *args, **kwargs):
-        default_message = repr(response)
-        super().__init__(default_message,response=response, *args, **kwargs)
+class ConnectTimeout(Timeout): #Subclass
+    def __init__(self, response=None,*args, **kwargs):
+        # if any arguments are passed...
+        # If you inherit from the exception that takes message as a keyword
+        # maybe you will need to check kwargs here
+        super().__init__(response=response, *args, **kwargs)
+
+class ReadTimeout(Timeout): #Subclass
+    def __init__(self, response=None,*args, **kwargs):
+        # if any arguments are passed...
+        # If you inherit from the exception that takes message as a keyword
+        # maybe you will need to check kwargs here
+        super().__init__(response=response, *args, **kwargs)
```

### Comparing `CFSession-0.2.2/CFSession.egg-info/PKG-INFO` & `CFSession-0.2.3/CFSession.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: CFSession
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Cloudflare IUAM session grabber
 Home-page: https://github.com/Kinuseka/CFSession
 Author: Kinuseka
 Author-email: realkingseeker1089@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -98,9 +96,7 @@
 cfs = cfSession()
 cfs.session #<--- A requests.Session object
 ```
 
 ## Disclaimer:
 This library was created with the sole purpose of educational purposes only, any rules/laws/ToS broken should only be held at the sole responsibility of the user.
 
-
-
```

### Comparing `CFSession-0.2.2/LICENSE` & `CFSession-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.2/PKG-INFO` & `CFSession-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: CFSession
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Cloudflare IUAM session grabber
 Home-page: https://github.com/Kinuseka/CFSession
 Author: Kinuseka
 Author-email: realkingseeker1089@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -98,9 +96,7 @@
 cfs = cfSession()
 cfs.session #<--- A requests.Session object
 ```
 
 ## Disclaimer:
 This library was created with the sole purpose of educational purposes only, any rules/laws/ToS broken should only be held at the sole responsibility of the user.
 
-
-
```

### Comparing `CFSession-0.2.2/README.md` & `CFSession-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `CFSession-0.2.2/setup.py` & `CFSession-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setup(
     name='CFSession',
-    version='0.2.2',
+    version='0.2.3',
     author='Kinuseka',
     author_email='realkingseeker1089@gmail.com',
     description='A Cloudflare IUAM session grabber',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Kinuseka/CFSession',
     classifiers=[
```

