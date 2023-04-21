# Comparing `tmp/tzconv-1.0.tar.gz` & `tmp/tzconv-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tzconv-1.0.tar", last modified: Fri Apr 21 02:17:00 2023, max compression
+gzip compressed data, was "tzconv-1.1.tar", last modified: Fri Apr 21 02:49:34 2023, max compression
```

## Comparing `tzconv-1.0.tar` & `tzconv-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 02:17:00.304402 tzconv-1.0/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     2934 2023-04-21 02:17:00.304402 tzconv-1.0/PKG-INFO
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     2695 2023-04-21 02:15:37.000000 tzconv-1.0/README.md
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       38 2023-04-21 02:17:00.304402 tzconv-1.0/setup.cfg
--rw-r--r--   0 bigmac    (1000) bigmac    (1000)      608 2023-04-21 01:55:55.000000 tzconv-1.0/setup.py
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 02:17:00.304402 tzconv-1.0/tzconv/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     1787 2023-04-21 01:58:59.000000 tzconv-1.0/tzconv/__init__.py
-drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 02:17:00.304402 tzconv-1.0/tzconv.egg-info/
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     2934 2023-04-21 02:17:00.000000 tzconv-1.0/tzconv.egg-info/PKG-INFO
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)      219 2023-04-21 02:17:00.000000 tzconv-1.0/tzconv.egg-info/SOURCES.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        1 2023-04-21 02:17:00.000000 tzconv-1.0/tzconv.egg-info/dependency_links.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       39 2023-04-21 02:17:00.000000 tzconv-1.0/tzconv.egg-info/entry_points.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        6 2023-04-21 02:17:00.000000 tzconv-1.0/tzconv.egg-info/requires.txt
--rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        7 2023-04-21 02:17:00.000000 tzconv-1.0/tzconv.egg-info/top_level.txt
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 02:49:34.645566 tzconv-1.1/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3343 2023-04-21 02:49:34.645566 tzconv-1.1/PKG-INFO
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3104 2023-04-21 02:47:40.000000 tzconv-1.1/README.md
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       38 2023-04-21 02:49:34.645566 tzconv-1.1/setup.cfg
+-rw-r--r--   0 bigmac    (1000) bigmac    (1000)      608 2023-04-21 02:45:57.000000 tzconv-1.1/setup.py
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 02:49:34.645566 tzconv-1.1/tzconv/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     2087 2023-04-21 02:42:53.000000 tzconv-1.1/tzconv/__init__.py
+drwxrwxr-x   0 bigmac    (1000) bigmac    (1000)        0 2023-04-21 02:49:34.645566 tzconv-1.1/tzconv.egg-info/
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)     3343 2023-04-21 02:49:34.000000 tzconv-1.1/tzconv.egg-info/PKG-INFO
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)      219 2023-04-21 02:49:34.000000 tzconv-1.1/tzconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        1 2023-04-21 02:49:34.000000 tzconv-1.1/tzconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)       39 2023-04-21 02:49:34.000000 tzconv-1.1/tzconv.egg-info/entry_points.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        6 2023-04-21 02:49:34.000000 tzconv-1.1/tzconv.egg-info/requires.txt
+-rw-rw-r--   0 bigmac    (1000) bigmac    (1000)        7 2023-04-21 02:49:34.000000 tzconv-1.1/tzconv.egg-info/top_level.txt
```

### Comparing `tzconv-1.0/PKG-INFO` & `tzconv-1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tzconv
-Version: 1.0
+Version: 1.1
 Summary: command-line tool to convert a date and time to several time zones at once
 Home-page: https://codeberg.org/gnyeki/tzconv
 Author: Gabor Nyeki
 Description-Content-Type: text/markdown
 
 
 # `tzconv`: convert a date and time to several time zones at once
@@ -44,14 +44,32 @@
 PDT: 2023-04-25 07:00 (America/Los_Angeles)
 ADT: 2023-04-25 11:00 (America/Halifax)
 PKT: 2023-04-25 19:00 (Asia/Karachi)
 IST: 2023-04-25 19:30 (Asia/Calcutta)
 $
 ```
 
+If the date is omitted, it imputes today's date:
+
+```
+$ tzconv \
+    -f America/New_York \
+    -t America/Los_Angeles \
+    -t America/Halifax \
+    -t Asia/Karachi \
+    -t Asia/Calcutta \
+    "10:00"
+EDT: 2023-04-20 10:00 (America/New_York)
+PDT: 2023-04-20 07:00 (America/Los_Angeles)
+ADT: 2023-04-20 11:00 (America/Halifax)
+PKT: 2023-04-20 19:00 (Asia/Karachi)
+IST: 2023-04-20 19:30 (Asia/Calcutta)
+$
+```
+
 ### Daylight savings
 
 Daylight savings can complicate conversions.
 However, thanks to the Python standard library, `tzconv` is aware of changes to daylight savings, and it infers the correct offsets.
 For example, in March 2023, New York switched to daylight savings two weeks earlier than Budapest.
 Notice the switch from EST/CET to EDT/CET, and finally to EDT/CEST:
```

### Comparing `tzconv-1.0/README.md` & `tzconv-1.1/tzconv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: tzconv
+Version: 1.1
+Summary: command-line tool to convert a date and time to several time zones at once
+Home-page: https://codeberg.org/gnyeki/tzconv
+Author: Gabor Nyeki
+Description-Content-Type: text/markdown
+
 
 # `tzconv`: convert a date and time to several time zones at once
 
 This Python package provides a small command-line utility to convert a `YYYY-MM-DD HH:MM` formatted date and time to several other time zones.
 
 ## Installation
 
@@ -36,14 +44,32 @@
 PDT: 2023-04-25 07:00 (America/Los_Angeles)
 ADT: 2023-04-25 11:00 (America/Halifax)
 PKT: 2023-04-25 19:00 (Asia/Karachi)
 IST: 2023-04-25 19:30 (Asia/Calcutta)
 $
 ```
 
+If the date is omitted, it imputes today's date:
+
+```
+$ tzconv \
+    -f America/New_York \
+    -t America/Los_Angeles \
+    -t America/Halifax \
+    -t Asia/Karachi \
+    -t Asia/Calcutta \
+    "10:00"
+EDT: 2023-04-20 10:00 (America/New_York)
+PDT: 2023-04-20 07:00 (America/Los_Angeles)
+ADT: 2023-04-20 11:00 (America/Halifax)
+PKT: 2023-04-20 19:00 (Asia/Karachi)
+IST: 2023-04-20 19:30 (Asia/Calcutta)
+$
+```
+
 ### Daylight savings
 
 Daylight savings can complicate conversions.
 However, thanks to the Python standard library, `tzconv` is aware of changes to daylight savings, and it infers the correct offsets.
 For example, in March 2023, New York switched to daylight savings two weeks earlier than Budapest.
 Notice the switch from EST/CET to EDT/CET, and finally to EDT/CEST:
```

### Comparing `tzconv-1.0/setup.py` & `tzconv-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as handle:
     readme = handle.read()
 
 setup(
     name="tzconv",
-    version="1.0",
+    version="1.1",
     description="command-line tool to convert a date and time to several time zones at once",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Gabor Nyeki",
     url="https://codeberg.org/gnyeki/tzconv",
     packages=["tzconv"],
     install_requires=["click"],
```

### Comparing `tzconv-1.0/tzconv/__init__.py` & `tzconv-1.1/tzconv/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,32 +6,37 @@
 from typing import cast
 
 import click
 
 
 def make_datetime(date_time: str, timezone: zi.ZoneInfo) -> dt.datetime:
     """Construct a `datetime` instance from a date-time string formatted
-    as `YYYY-MM-DD HH:MM` and attach timezone information."""
+    as `YYYY-MM-DD HH:MM` or `HH:MM` and attach timezone information."""
 
-    match = re.match(
-        r"^\s*(\d{4})-(\d{2})-(\d{2})\s+(\d{1,2}):(\d{2})\s*$",
-        date_time)
+    match = (
+        re.match(r"^\s*(\d{4})-(\d{2})-(\d{2})\s+(\d{1,2}):(\d{2})\s*$",
+                 date_time)
+        or re.match(r"^\s*(\d{1,2}):(\d{2})\s*$", date_time)
+    )
 
     if match is None:
         raise ValueError(
-            f"Date and time '{date_time}' does not match format "
-            + "YYYY-MM-DD HH:MM.")
+            f"Date and time '{date_time}' matches neither "
+            + "'YYYY-MM-DD HH:MM' nor 'HH:MM'.")
 
-    return dt.datetime(
-        int(match.group(1)),
-        int(match.group(2)),
-        int(match.group(3)),
-        int(match.group(4)),
-        int(match.group(5)),
-        tzinfo=timezone)
+    if len(match.groups()) == 5:
+        year, month, day, hour, minute = tuple(int(x)
+                                               for x in match.groups())
+    else:
+        today = dt.date.today()
+
+        year, month, day = today.year, today.month, today.day
+        hour, minute = tuple(int(x) for x in match.groups())
+
+    return dt.datetime(year, month, day, hour, minute, tzinfo=timezone)
 
 
 def format_datetime(obj: dt.datetime) -> str:
     """Create a human-readable representation of a `datetime`
     object. The resulting string includes the timezone's name and its
     `zoneinfo` key."""
```

### Comparing `tzconv-1.0/tzconv.egg-info/PKG-INFO` & `tzconv-1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: tzconv
-Version: 1.0
-Summary: command-line tool to convert a date and time to several time zones at once
-Home-page: https://codeberg.org/gnyeki/tzconv
-Author: Gabor Nyeki
-Description-Content-Type: text/markdown
-
 
 # `tzconv`: convert a date and time to several time zones at once
 
 This Python package provides a small command-line utility to convert a `YYYY-MM-DD HH:MM` formatted date and time to several other time zones.
 
 ## Installation
 
@@ -44,14 +36,32 @@
 PDT: 2023-04-25 07:00 (America/Los_Angeles)
 ADT: 2023-04-25 11:00 (America/Halifax)
 PKT: 2023-04-25 19:00 (Asia/Karachi)
 IST: 2023-04-25 19:30 (Asia/Calcutta)
 $
 ```
 
+If the date is omitted, it imputes today's date:
+
+```
+$ tzconv \
+    -f America/New_York \
+    -t America/Los_Angeles \
+    -t America/Halifax \
+    -t Asia/Karachi \
+    -t Asia/Calcutta \
+    "10:00"
+EDT: 2023-04-20 10:00 (America/New_York)
+PDT: 2023-04-20 07:00 (America/Los_Angeles)
+ADT: 2023-04-20 11:00 (America/Halifax)
+PKT: 2023-04-20 19:00 (Asia/Karachi)
+IST: 2023-04-20 19:30 (Asia/Calcutta)
+$
+```
+
 ### Daylight savings
 
 Daylight savings can complicate conversions.
 However, thanks to the Python standard library, `tzconv` is aware of changes to daylight savings, and it infers the correct offsets.
 For example, in March 2023, New York switched to daylight savings two weeks earlier than Budapest.
 Notice the switch from EST/CET to EDT/CET, and finally to EDT/CEST:
```

