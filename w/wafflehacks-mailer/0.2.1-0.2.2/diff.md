# Comparing `tmp/wafflehacks-mailer-0.2.1.tar.gz` & `tmp/wafflehacks_mailer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafflehacks-mailer-0.2.1.tar", max compression
+gzip compressed data, was "wafflehacks_mailer-0.2.2.tar", max compression
```

## Comparing `wafflehacks-mailer-0.2.1.tar` & `wafflehacks_mailer-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      189 2022-05-14 22:48:36.785575 wafflehacks-mailer-0.2.1/README.md
--rw-r--r--   0        0        0      137 2022-05-14 22:48:36.785575 wafflehacks-mailer-0.2.1/mailer/__init__.py
--rw-r--r--   0        0        0     4348 2022-05-14 22:48:36.785575 wafflehacks-mailer-0.2.1/mailer/aio.py
--rw-r--r--   0        0        0     3841 2022-05-14 22:48:36.785575 wafflehacks-mailer-0.2.1/mailer/blocking.py
--rw-r--r--   0        0        0      198 2022-05-14 22:48:36.785575 wafflehacks-mailer-0.2.1/mailer/shared.py
--rw-r--r--   0        0        0      508 2022-05-14 22:48:36.785575 wafflehacks-mailer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      857 2022-05-14 22:48:49.198584 wafflehacks-mailer-0.2.1/setup.py
--rw-r--r--   0        0        0      713 2022-05-14 22:48:49.198861 wafflehacks-mailer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-21 18:36:23.653596 wafflehacks_mailer-0.2.2/README.md
+-rw-r--r--   0        0        0      135 2023-04-21 18:36:23.653596 wafflehacks_mailer-0.2.2/mailer/__init__.py
+-rw-r--r--   0        0        0     4065 2023-04-21 18:36:23.653596 wafflehacks_mailer-0.2.2/mailer/aio.py
+-rw-r--r--   0        0        0     3558 2023-04-21 18:36:23.653596 wafflehacks_mailer-0.2.2/mailer/blocking.py
+-rw-r--r--   0        0        0      176 2023-04-21 18:36:23.653596 wafflehacks_mailer-0.2.2/mailer/shared.py
+-rw-r--r--   0        0        0      509 2023-04-21 18:36:23.657595 wafflehacks_mailer-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 wafflehacks_mailer-0.2.2/PKG-INFO
```

### Comparing `wafflehacks-mailer-0.2.1/mailer/blocking.py` & `wafflehacks_mailer-0.2.2/mailer/blocking.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from requests import Session
 from typing import Dict, List, Optional
 from yarl import URL
 
-from .shared import BodyType, InvalidArgumentException
+from .shared import Format, InvalidArgumentException
 
 
 class Client(object):
     """
     A blocking mailer client for sending messages
     """
 
@@ -32,100 +32,93 @@
 
     def send(
         self,
         to_email: str,
         from_email: str,
         subject: str,
         body: str,
-        body_type: BodyType = BodyType.PLAIN,
+        format: Format = Format.PLAIN,
         reply_to: Optional[str] = None,
     ):
         """
         Send a single email
         :param to_email: the address of the recipient
         :param from_email: the address of the sender in RFC 5322
         :param subject: the email subject
         :param body: the message body
-        :param body_type: the content type of the body
+        :param format: the content type of the body
         :param reply_to: an optional email to reply to
         """
 
         self._dispatch(
             "/send",
             {
                 "to": to_email,
                 "from": from_email,
                 "subject": subject,
                 "body": body,
-                "type": body_type.value,
+                "format": format.value,
                 "reply_to": reply_to,
             },
         )
 
     def send_batch(
         self,
-        to_email: List[str],
+        to_emails: List[str],
         from_email: str,
         subject: str,
         body: str,
-        body_type: BodyType = BodyType.PLAIN,
+        format: Format = Format.PLAIN,
         reply_to: Optional[str] = None,
     ):
         """
         Send an email to many recipients
-        :param to_email: the addresses of the recipients
+        :param to_emails: the addresses of the recipients
         :param from_email: the address of the sender in RFC 5322
         :param subject: the email subject
         :param body: the message body
-        :param body_type: the content type of the body
+        :param format: the content type of the body
         :param reply_to: an optional email to reply to
         """
 
         self._dispatch(
             "/send/batch",
             {
-                "to": to_email,
+                "to": to_emails,
                 "from": from_email,
                 "subject": subject,
                 "body": body,
-                "type": body_type.value,
+                "format": format.value,
                 "reply_to": reply_to,
             },
         )
 
     def send_template(
         self,
         to: Dict[str, Dict[str, str]],
         from_email: str,
         subject: str,
         body: str,
-        body_type: BodyType = BodyType.PLAIN,
+        format: Format = Format.PLAIN,
         reply_to: Optional[str] = None,
     ):
         """
         Send a templated email to many recipients
         :param to: the addresses of the recipients in RFC 5322 format with their associated contexts
         :param from_email: the address of the sender in RFC 5322 format
         :param subject: the email subject
         :param body: the message body template
-        :param body_type: the content type of the body
+        :param format: the content type of the body
         :param reply_to: an optional email to reply to
         """
-        # Transform the to contexts
-        prepared_to = {}
-        for key, context in to.items():
-            prepared_to[key] = {
-                "key": list(context.keys()),
-                "value": list(context.values()),
-            }
 
         self._dispatch(
             "/send/template",
             {
-                "to": prepared_to,
+                "to": to,
                 "from": from_email,
                 "subject": subject,
                 "body": body,
-                "type": body_type.value,
+                "format": format.value,
                 "reply_to": reply_to,
             },
         )
```

### Comparing `wafflehacks-mailer-0.2.1/PKG-INFO` & `wafflehacks_mailer-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: wafflehacks-mailer
-Version: 0.2.1
+Version: 0.2.2
 Summary: The Python SDK for the WaffleHacks mailer
 Author: Alex Krantz
 Author-email: alex@krantz.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: aiohttp[speedups] (>=3.8.1,<4.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Mailer
 
 The Python SDK for the WaffleHacks [mailer](https://github.com/WaffleHacks/mailer) service.
 The SDK uses the HTTP API, providing blocking and non-blocking (asynchronous) variants.
```

