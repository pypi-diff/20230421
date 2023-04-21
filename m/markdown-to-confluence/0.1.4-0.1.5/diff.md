# Comparing `tmp/markdown-to-confluence-0.1.4.tar.gz` & `tmp/markdown-to-confluence-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-to-confluence-0.1.4.tar", last modified: Fri Dec  9 12:37:15 2022, max compression
+gzip compressed data, was "markdown-to-confluence-0.1.5.tar", last modified: Fri Apr 21 20:22:41 2023, max compression
```

## Comparing `markdown-to-confluence-0.1.4.tar` & `markdown-to-confluence-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-12-09 12:37:15.358985 markdown-to-confluence-0.1.4/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1072 2022-06-10 16:20:40.000000 markdown-to-confluence-0.1.4/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3534 2022-12-09 12:37:15.359135 markdown-to-confluence-0.1.4/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2907 2022-06-17 11:33:19.000000 markdown-to-confluence-0.1.4/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-12-09 12:37:15.356415 markdown-to-confluence-0.1.4/markdown_to_confluence.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3534 2022-12-09 12:37:15.000000 markdown-to-confluence-0.1.4/markdown_to_confluence.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      420 2022-12-09 12:37:15.000000 markdown-to-confluence-0.1.4/markdown_to_confluence.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2022-12-09 12:37:15.000000 markdown-to-confluence-0.1.4/markdown_to_confluence.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       42 2022-12-09 12:37:15.000000 markdown-to-confluence-0.1.4/markdown_to_confluence.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        8 2022-12-09 12:37:15.000000 markdown-to-confluence-0.1.4/markdown_to_confluence.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2022-12-09 12:37:15.000000 markdown-to-confluence-0.1.4/markdown_to_confluence.egg-info/zip-safe
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-12-09 12:37:15.358648 markdown-to-confluence-0.1.4/md2conf/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       22 2022-12-09 12:36:05.000000 markdown-to-confluence-0.1.4/md2conf/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1574 2022-07-15 10:45:42.000000 markdown-to-confluence-0.1.4/md2conf/__main__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8954 2022-07-15 11:42:07.000000 markdown-to-confluence-0.1.4/md2conf/api.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      804 2022-07-15 11:37:19.000000 markdown-to-confluence-0.1.4/md2conf/application.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8257 2022-07-15 11:44:13.000000 markdown-to-confluence-0.1.4/md2conf/converter.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-06-17 11:04:46.000000 markdown-to-confluence-0.1.4/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      818 2022-12-09 12:37:15.359803 markdown-to-confluence-0.1.4/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-06-17 11:09:13.000000 markdown-to-confluence-0.1.4/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 20:22:41.874459 markdown-to-confluence-0.1.5/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1077 2023-04-21 19:22:25.000000 markdown-to-confluence-0.1.5/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3720 2023-04-21 20:22:41.874640 markdown-to-confluence-0.1.5/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2907 2022-12-09 13:01:59.000000 markdown-to-confluence-0.1.5/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 20:22:41.870827 markdown-to-confluence-0.1.5/markdown_to_confluence.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3720 2023-04-21 20:22:41.000000 markdown-to-confluence-0.1.5/markdown_to_confluence.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      455 2023-04-21 20:22:41.000000 markdown-to-confluence-0.1.5/markdown_to_confluence.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-21 20:22:41.000000 markdown-to-confluence-0.1.5/markdown_to_confluence.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      105 2023-04-21 20:22:41.000000 markdown-to-confluence-0.1.5/markdown_to_confluence.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        8 2023-04-21 20:22:41.000000 markdown-to-confluence-0.1.5/markdown_to_confluence.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-21 20:22:41.000000 markdown-to-confluence-0.1.5/markdown_to_confluence.egg-info/zip-safe
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 20:22:41.873672 markdown-to-confluence-0.1.5/md2conf/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      402 2023-04-21 19:21:10.000000 markdown-to-confluence-0.1.5/md2conf/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1574 2022-07-15 10:45:42.000000 markdown-to-confluence-0.1.5/md2conf/__main__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10672 2023-04-21 20:09:24.000000 markdown-to-confluence-0.1.5/md2conf/api.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      786 2022-12-09 13:03:45.000000 markdown-to-confluence-0.1.5/md2conf/application.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8506 2023-04-21 20:13:41.000000 markdown-to-confluence-0.1.5/md2conf/converter.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 19:11:21.000000 markdown-to-confluence-0.1.5/md2conf/py.typed
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-06-17 11:04:46.000000 markdown-to-confluence-0.1.5/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1082 2023-04-21 20:22:41.875537 markdown-to-confluence-0.1.5/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-06-17 11:09:13.000000 markdown-to-confluence-0.1.5/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 20:22:41.874047 markdown-to-confluence-0.1.5/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2358 2023-04-21 19:25:53.000000 markdown-to-confluence-0.1.5/tests/test_api.py
```

### Comparing `markdown-to-confluence-0.1.4/LICENSE` & `markdown-to-confluence-0.1.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Levente Hunyadi
+Copyright (c) 2022-2023 Levente Hunyadi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `markdown-to-confluence-0.1.4/PKG-INFO` & `markdown-to-confluence-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: markdown-to-confluence
-Version: 0.1.4
+Version: 0.1.5
 Summary: Publish Markdown files to Confluence wiki
 Home-page: https://github.com/hunyadi/md2conf
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Publish Markdown files to Confluence wiki
 
 Contributors to software projects typically write documentation in Markdown format and host Markdown files in collaborative version control systems (VCS) such as GitHub or GitLab to track changes and facilitate the review process. However, not everyone at a company has access to VCS, and documents are often circulated in Confluence wiki instead.
 
@@ -35,15 +39,15 @@
 * Ordered and unordered lists
 * Code blocks (e.g. Python, JSON, XML)
 * Image references (uploaded as Confluence page attachments)
 
 ## Getting started
 
 In order to get started, you will need
-* your organization URL (e.g. `https://instructure.atlassian.net`),
+* your organization domain name (e.g. `instructure.atlassian.net`),
 * your Confluence username (e.g. `levente.hunyadi@instructure.com`),
 * a Confluence API token (a string of alphanumeric characters), and
 * the space key in Confluence (e.g. `DAP`) you are publishing content to.
 
 ### Obtaining an API token
 
 1. Log in to https://id.atlassian.com/manage/api-tokens.
```

### Comparing `markdown-to-confluence-0.1.4/README.md` & `markdown-to-confluence-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 * Ordered and unordered lists
 * Code blocks (e.g. Python, JSON, XML)
 * Image references (uploaded as Confluence page attachments)
 
 ## Getting started
 
 In order to get started, you will need
-* your organization URL (e.g. `https://instructure.atlassian.net`),
+* your organization domain name (e.g. `instructure.atlassian.net`),
 * your Confluence username (e.g. `levente.hunyadi@instructure.com`),
 * a Confluence API token (a string of alphanumeric characters), and
 * the space key in Confluence (e.g. `DAP`) you are publishing content to.
 
 ### Obtaining an API token
 
 1. Log in to https://id.atlassian.com/manage/api-tokens.
```

### Comparing `markdown-to-confluence-0.1.4/markdown_to_confluence.egg-info/PKG-INFO` & `markdown-to-confluence-0.1.5/markdown_to_confluence.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: markdown-to-confluence
-Version: 0.1.4
+Version: 0.1.5
 Summary: Publish Markdown files to Confluence wiki
 Home-page: https://github.com/hunyadi/md2conf
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Publish Markdown files to Confluence wiki
 
 Contributors to software projects typically write documentation in Markdown format and host Markdown files in collaborative version control systems (VCS) such as GitHub or GitLab to track changes and facilitate the review process. However, not everyone at a company has access to VCS, and documents are often circulated in Confluence wiki instead.
 
@@ -35,15 +39,15 @@
 * Ordered and unordered lists
 * Code blocks (e.g. Python, JSON, XML)
 * Image references (uploaded as Confluence page attachments)
 
 ## Getting started
 
 In order to get started, you will need
-* your organization URL (e.g. `https://instructure.atlassian.net`),
+* your organization domain name (e.g. `instructure.atlassian.net`),
 * your Confluence username (e.g. `levente.hunyadi@instructure.com`),
 * a Confluence API token (a string of alphanumeric characters), and
 * the space key in Confluence (e.g. `DAP`) you are publishing content to.
 
 ### Obtaining an API token
 
 1. Log in to https://id.atlassian.com/manage/api-tokens.
```

### Comparing `markdown-to-confluence-0.1.4/md2conf/__main__.py` & `markdown-to-confluence-0.1.5/md2conf/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown-to-confluence-0.1.4/md2conf/api.py` & `markdown-to-confluence-0.1.5/md2conf/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 import json
 import logging
 import mimetypes
 import os
 import os.path
-import urllib.parse
+import typing
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Dict, Generator
+from types import TracebackType
+from typing import Dict, Generator, List, Optional, Type, Union
+from urllib.parse import urlencode, urlparse, urlunparse
 
 import requests
 
 from .converter import ParseError, sanitize_confluence
 
+# a JSON type with possible `null` values
+JsonType = Union[
+    None,
+    bool,
+    int,
+    float,
+    str,
+    Dict[str, "JsonType"],
+    List["JsonType"],
+]
 
-def build_url(base_url: str, query: Dict[str, str] = None):
+
+def build_url(base_url: str, query: Optional[Dict[str, str]] = None) -> str:
     "Builds a URL with scheme, host, port, path and query string parameters."
 
-    scheme, netloc, path, params, query_str, fragment = urllib.parse.urlparse(base_url)
+    scheme, netloc, path, params, query_str, fragment = urlparse(base_url)
 
     if params:
         raise ValueError("expected: url with no parameters")
     if query_str:
         raise ValueError("expected: url with no query string")
     if fragment:
         raise ValueError("expected: url with no fragment")
 
-    query_str = urllib.parse.urlencode(query) if query else None
-    url_parts = (scheme, netloc, path, None, query_str, None)
-    return urllib.parse.urlunparse(url_parts)
+    url_parts = (scheme, netloc, path, None, urlencode(query) if query else None, None)
+    return urlunparse(url_parts)
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ConfluenceError(RuntimeError):
     pass
@@ -55,44 +67,62 @@
 
 class ConfluenceAPI:
     domain: str
     space_key: str
     user_name: str
     api_key: str
 
-    session: "ConfluenceSession"
+    session: Optional["ConfluenceSession"] = None
 
     def __init__(
         self,
-        domain: str = None,
-        user_name: str = None,
-        api_key: str = None,
-        space_key: str = None,
+        domain: Optional[str] = None,
+        user_name: Optional[str] = None,
+        api_key: Optional[str] = None,
+        space_key: Optional[str] = None,
     ) -> None:
-        self.domain = domain or os.getenv("CONFLUENCE_DOMAIN")
-        self.user_name = user_name or os.getenv("CONFLUENCE_USER_NAME")
-        self.api_key = api_key or os.getenv("CONFLUENCE_API_KEY")
-        self.space_key = space_key or os.getenv("CONFLUENCE_SPACE_KEY")
+        opt_domain = domain or os.getenv("CONFLUENCE_DOMAIN")
+        opt_user_name = user_name or os.getenv("CONFLUENCE_USER_NAME")
+        opt_api_key = api_key or os.getenv("CONFLUENCE_API_KEY")
+        opt_space_key = space_key or os.getenv("CONFLUENCE_SPACE_KEY")
 
-        if not self.domain:
+        if not opt_domain:
             raise ConfluenceError("Confluence domain not specified")
-        if not self.user_name:
+        if not opt_user_name:
             raise ConfluenceError("Confluence user name not specified")
-        if not self.api_key:
+        if not opt_api_key:
             raise ConfluenceError("Confluence API key not specified")
+        if not opt_space_key:
+            raise ConfluenceError("Confluence space key not specified")
+
+        if opt_domain.startswith(("http://", "https://")):
+            raise ConfluenceError(
+                "Confluence domain looks like a URL; only host name required"
+            )
 
-    def __enter__(self):
+        self.domain = opt_domain
+        self.user_name = opt_user_name
+        self.api_key = opt_api_key
+        self.space_key = opt_space_key
+
+    def __enter__(self) -> "ConfluenceSession":
         session = requests.Session()
         session.auth = (self.user_name, self.api_key)
         self.session = ConfluenceSession(session, self.domain, self.space_key)
         return self.session
 
-    def __exit__(self, type, value, traceback):
-        self.session.close()
-        self.session = None
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
+    ) -> None:
+        if self.session is not None:
+            self.session.close()
+            self.session = None
 
 
 class ConfluenceSession:
     session: requests.Session
     domain: str
     space_key: str
 
@@ -109,19 +139,19 @@
         old_space_key = self.space_key
         self.space_key = new_space_key
         try:
             yield
         finally:
             self.space_key = old_space_key
 
-    def _build_url(self, path: str, query: Dict[str, str] = None) -> str:
+    def _build_url(self, path: str, query: Optional[Dict[str, str]] = None) -> str:
         base_url = f"https://{self.domain}/wiki/rest/api{path}"
         return build_url(base_url, query)
 
-    def _invoke(self, path: str, query: Dict[str, str]) -> str:
+    def _invoke(self, path: str, query: Dict[str, str]) -> JsonType:
         url = self._build_url(path, query)
         response = self.session.get(url)
         response.raise_for_status()
         return response.json()
 
     def _save(self, path: str, data: dict) -> None:
         url = self._build_url(path)
@@ -133,35 +163,35 @@
         response.raise_for_status()
 
     def get_attachment_by_name(
         self, page_id: str, filename: str
     ) -> ConfluenceAttachment:
         path = f"/content/{page_id}/child/attachment"
         query = {"spaceKey": self.space_key, "filename": filename}
-        data = self._invoke(path, query)
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
 
-        results = data["results"]
+        results = typing.cast(List[JsonType], data["results"])
         if len(results) != 1:
             raise ConfluenceError(f"no such attachment on page {page_id}: {filename}")
+        result = typing.cast(Dict[str, JsonType], results[0])
 
-        id = results[0]["id"]
-        extensions = results[0]["extensions"]
-        media_type = extensions["mediaType"]
-        file_size = extensions["fileSize"]
-        comment = extensions["comment"]
+        id = typing.cast(str, result["id"])
+        extensions = typing.cast(Dict[str, JsonType], result["extensions"])
+        media_type = typing.cast(str, extensions["mediaType"])
+        file_size = typing.cast(int, extensions["fileSize"])
+        comment = typing.cast(str, extensions["comment"])
         return ConfluenceAttachment(id, media_type, file_size, comment)
 
     def upload_attachment(
         self,
         page_id: str,
         attachment_path: str,
         attachment_name: str,
-        comment: str = None,
+        comment: Optional[str] = None,
     ) -> None:
-
         content_type = mimetypes.guess_type(attachment_path, strict=True)[0]
 
         if not os.path.isfile(attachment_path):
             raise ConfluenceError(f"file not found: {attachment_path}")
 
         try:
             attachment = self.get_attachment_by_name(page_id, attachment_name)
@@ -186,15 +216,17 @@
                     attachment_file,
                     content_type,
                     {"Expires": "0"},
                 ),
             }
             LOGGER.info("Uploading attachment: %s", attachment_name)
             response = self.session.post(
-                url, files=file_to_upload, headers={"X-Atlassian-Token": "no-check"}
+                url,
+                files=file_to_upload,  # type: ignore
+                headers={"X-Atlassian-Token": "no-check"},
             )
 
         response.raise_for_status()
         data = response.json()
 
         if "results" in data:
             result = data["results"][0]
@@ -206,15 +238,14 @@
 
         # ensure path component is retained in attachment name
         self._update_attachment(page_id, attachment_id, version, attachment_name)
 
     def _update_attachment(
         self, page_id: str, attachment_id: str, version: int, attachment_title: str
     ) -> None:
-
         id = attachment_id.removeprefix("att")
         path = f"/content/{page_id}/child/attachment/{id}"
         data = {
             "id": attachment_id,
             "type": "attachment",
             "status": "current",
             "title": attachment_title,
@@ -232,46 +263,51 @@
         :param title: The page title.
         :returns: Confluence page info.
         """
 
         LOGGER.info("Looking up page with title: %s", title)
         path = "/content"
         query = {"title": title, "spaceKey": self.space_key}
-        data = self._invoke(path, query)
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
 
-        results = data["results"]
+        results = typing.cast(List[JsonType], data["results"])
         if len(results) != 1:
             raise ConfluenceError(f"page not found with title: {title}")
 
-        id = results[0]["id"]
+        result = typing.cast(Dict[str, JsonType], results[0])
+        id = typing.cast(str, result["id"])
         return id
 
     def get_page(self, page_id: str) -> ConfluencePage:
         path = f"/content/{page_id}"
         query = {
             "spaceKey": self.space_key,
             "expand": "body.storage,version",
         }
-        data = self._invoke(path, query)
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+        version = typing.cast(Dict[str, JsonType], data["version"])
+        body = typing.cast(Dict[str, JsonType], data["body"])
+        storage = typing.cast(Dict[str, JsonType], body["storage"])
 
         return ConfluencePage(
             id=page_id,
-            title=data["title"],
-            version=data["version"]["number"],
-            content=data["body"]["storage"]["value"],
+            title=typing.cast(str, data["title"]),
+            version=typing.cast(int, version["number"]),
+            content=typing.cast(str, storage["value"]),
         )
 
     def get_page_version(self, page_id: str) -> int:
         path = f"/content/{page_id}"
         query = {
             "spaceKey": self.space_key,
             "expand": "version",
         }
-        data = self._invoke(path, query)
-        return data["version"]["number"]
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+        version = typing.cast(Dict[str, JsonType], data["version"])
+        return typing.cast(int, version["number"])
 
     def update_page(self, page_id: str, new_content: str) -> None:
         page = self.get_page(page_id)
 
         try:
             old_content = sanitize_confluence(page.content)
             if old_content == new_content:
```

### Comparing `markdown-to-confluence-0.1.4/md2conf/application.py` & `markdown-to-confluence-0.1.5/md2conf/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os.path
 
 from .api import ConfluenceSession
-from .converter import ConfluenceDocument, markdown_to_html
+from .converter import ConfluenceDocument
 
 
 def update_document(
     api: ConfluenceSession, document: ConfluenceDocument, base_path: str
 ) -> None:
     for image in document.images:
         api.upload_attachment(
```

### Comparing `markdown-to-confluence-0.1.4/md2conf/converter.py` & `markdown-to-confluence-0.1.5/md2conf/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 RI = ElementMaker(namespace=namespaces["ri"])
 
 
 class ParseError(RuntimeError):
     pass
 
 
-def is_absolute_url(url):
+def is_absolute_url(url: str) -> bool:
     return bool(urlparse(url).netloc)
 
 
 def markdown_to_html(content: str) -> str:
     return markdown.markdown(
         content,
         extensions=[
@@ -149,15 +149,19 @@
             RI("attachment", {ET.QName(namespaces["ri"], "filename"): path}),
             AC("caption", HTML.p(caption)),
         )
 
     def _transform_block(self, code: ET.Element) -> ET.Element:
         language = code.attrib.get("class")
         if language:
-            language = re.match("^language-(.*)$", language).group(1)
+            m = re.match("^language-(.*)$", language)
+            if m:
+                language = m.group(1)
+            else:
+                language = "none"
         if language not in _languages:
             language = "none"
         content: str = code.text
         content = content.rstrip()
         return AC(
             "structured-macro",
             {
@@ -171,19 +175,19 @@
             ),
             AC("plain-text-body", ET.CDATA(content)),
         )
 
     def transform(self, child: ET.Element) -> Optional[ET.Element]:
         # normalize line breaks to regular space in element text
         if child.text:
-            s: str = child.text
-            child.text = s.replace("\n", " ")
+            text: str = child.text
+            child.text = text.replace("\n", " ")
         if child.tail:
-            s: str = child.tail
-            child.tail = s.replace("\n", " ")
+            tail: str = child.tail
+            child.tail = tail.replace("\n", " ")
 
         # <p><img src="..." /></p>
         if child.tag == "p" and len(child) == 1 and child[0].tag == "img":
             return self._transform_image(child[0])
 
         # <img src="..." alt="..." />
         elif child.tag == "img":
@@ -193,28 +197,31 @@
         elif child.tag == "a":
             return self._transform_link(child)
 
         # <pre><code class="language-java"> ... </code></pre>
         elif child.tag == "pre" and len(child) == 1 and child[0].tag == "code":
             return self._transform_block(child[0])
 
+        return None
+
 
 class ConfluenceStorageFormatCleaner(NodeVisitor):
     "Removes volatile attributes from a Confluence storage format XHTML document."
 
     def transform(self, child: ET.Element) -> Optional[ET.Element]:
         child.attrib.pop(ET.QName(namespaces["ac"], "macro-id"), None)
         child.attrib.pop(ET.QName(namespaces["ri"], "version-at-save"), None)
+        return None
 
 
 class DocumentError(RuntimeError):
     pass
 
 
-def _extract_value(pattern, string) -> Tuple[Optional[str], str]:
+def _extract_value(pattern: str, string: str) -> Tuple[Optional[str], str]:
     values: List[str] = []
 
     def _repl_func(matchobj: re.Match) -> str:
         values.append(matchobj.group(1))
         return ""
 
     string = re.sub(pattern, _repl_func, string, 1, re.ASCII)
@@ -277,8 +284,11 @@
     ConfluenceStorageFormatCleaner().visit(root)
     return _content_to_string(root)
 
 
 def _content_to_string(root: ET.Element) -> str:
     xml = ET.tostring(root, encoding="utf8", method="xml").decode("utf8")
     m = re.match(r"^<root\s+[^>]*>(.*)</root>\s*$", xml, re.DOTALL)
-    return m.group(1)
+    if m:
+        return m.group(1)
+    else:
+        raise ValueError("expected: Confluence content")
```

### Comparing `markdown-to-confluence-0.1.4/setup.cfg` & `markdown-to-confluence-0.1.5/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -5,33 +5,43 @@
 author = Levente Hunyadi
 author_email = hunyadi@gmail.com
 url = https://github.com/hunyadi/md2conf
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers = 
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
+	Intended Audience :: End Users/Desktop
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Typing :: Typed
 
 [options]
 zip_safe = True
 include_package_data = True
 packages = find:
 install_requires = 
-	lxml
-	markdown
-	pymdown-extensions
-	requests
+	lxml >= 4.9
+	markdown >= 3.4
+	pymdown-extensions >= 9.11
+	requests >= 2.28
+	types-markdown >= 3.4
+	types-requests >= 2.28
 
 [options.packages.find]
 exclude = 
 	tests*
 
+[options.package_data]
+md2conf = 
+	py.typed
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

