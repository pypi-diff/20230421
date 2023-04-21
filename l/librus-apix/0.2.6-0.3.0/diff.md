# Comparing `tmp/librus_apix-0.2.6.tar.gz` & `tmp/librus_apix-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.2.6.tar", last modified: Wed Apr 19 20:21:06 2023, max compression
+gzip compressed data, was "librus_apix-0.3.0.tar", last modified: Fri Apr 21 20:44:00 2023, max compression
```

## Comparing `librus_apix-0.2.6.tar` & `librus_apix-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-19 20:21:06.407740 librus_apix-0.2.6/
--rw-r--r--   0 poro      (1000) poro      (1000)     1722 2022-09-08 20:51:34.000000 librus_apix-0.2.6/LICENSE
--rw-r--r--   0 poro      (1000) poro      (1000)     1722 2022-09-08 20:51:34.000000 librus_apix-0.2.6/LICENSE.orig
--rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-19 20:21:06.407740 librus_apix-0.2.6/PKG-INFO
--rw-r--r--   0 poro      (1000) poro      (1000)     2430 2023-04-19 11:50:28.000000 librus_apix-0.2.6/README.md
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-19 20:21:06.404405 librus_apix-0.2.6/librus_apix/
--rw-r--r--   0 poro      (1000) poro      (1000)      346 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/__init__.py
--rw-r--r--   0 poro      (1000) poro      (1000)     1156 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/announcements.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2277 2023-04-19 19:19:28.000000 librus_apix-0.2.6/librus_apix/attendance.py
--rw-r--r--   0 poro      (1000) poro      (1000)      210 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/exceptions.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2367 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/get_token.py
--rw-r--r--   0 poro      (1000) poro      (1000)     4693 2023-04-19 14:24:01.000000 librus_apix-0.2.6/librus_apix/grades.py
--rw-r--r--   0 poro      (1000) poro      (1000)      287 2022-12-30 11:55:28.000000 librus_apix-0.2.6/librus_apix/helpers.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2175 2023-04-19 12:13:37.000000 librus_apix-0.2.6/librus_apix/homework.py
--rw-r--r--   0 poro      (1000) poro      (1000)     2108 2023-01-12 19:56:33.000000 librus_apix-0.2.6/librus_apix/messages.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3053 2023-04-19 11:50:10.000000 librus_apix-0.2.6/librus_apix/schedule.py
--rw-r--r--   0 poro      (1000) poro      (1000)     3098 2022-12-14 21:45:32.000000 librus_apix-0.2.6/librus_apix/timetable.py
--rw-r--r--   0 poro      (1000) poro      (1000)      422 2022-09-08 20:51:34.000000 librus_apix-0.2.6/librus_apix/urls.py
-drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-19 20:21:06.407740 librus_apix-0.2.6/librus_apix.egg-info/
--rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 poro      (1000) poro      (1000)      530 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 poro      (1000) poro      (1000)        1 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       18 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/requires.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       12 2023-04-19 20:21:06.000000 librus_apix-0.2.6/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 poro      (1000) poro      (1000)       89 2022-09-08 20:51:34.000000 librus_apix-0.2.6/pyproject.toml
--rw-r--r--   0 poro      (1000) poro      (1000)      589 2023-04-19 20:21:06.407740 librus_apix-0.2.6/setup.cfg
--rw-r--r--   0 poro      (1000) poro      (1000)       37 2022-09-08 20:51:34.000000 librus_apix-0.2.6/setup.py
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-21 20:44:00.805606 librus_apix-0.3.0/
+-rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-04-21 20:43:44.000000 librus_apix-0.3.0/LICENSE
+-rw-r--r--   0 poro      (1000) poro      (1000)     1722 2023-04-21 20:43:44.000000 librus_apix-0.3.0/LICENSE.orig
+-rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-21 20:44:00.805606 librus_apix-0.3.0/PKG-INFO
+-rw-r--r--   0 poro      (1000) poro      (1000)     2430 2023-04-21 20:43:44.000000 librus_apix-0.3.0/README.md
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-21 20:44:00.805606 librus_apix-0.3.0/librus_apix/
+-rw-r--r--   0 poro      (1000) poro      (1000)      346 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/__init__.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     1156 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/announcements.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2810 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/attendance.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2810 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/completed_lessons.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      210 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/exceptions.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2367 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/get_token.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     4693 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/grades.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      287 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/helpers.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2175 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/homework.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     2616 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/messages.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3053 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/schedule.py
+-rw-r--r--   0 poro      (1000) poro      (1000)     3098 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/timetable.py
+-rw-r--r--   0 poro      (1000) poro      (1000)      480 2023-04-21 20:43:44.000000 librus_apix-0.3.0/librus_apix/urls.py
+drwxr-xr-x   0 poro      (1000) poro      (1000)        0 2023-04-21 20:44:00.805606 librus_apix-0.3.0/librus_apix.egg-info/
+-rw-r--r--   0 poro      (1000) poro      (1000)      470 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 poro      (1000) poro      (1000)      563 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)        1 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       18 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       12 2023-04-21 20:44:00.000000 librus_apix-0.3.0/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 poro      (1000) poro      (1000)       89 2023-04-21 20:43:44.000000 librus_apix-0.3.0/pyproject.toml
+-rw-r--r--   0 poro      (1000) poro      (1000)      589 2023-04-21 20:44:00.808940 librus_apix-0.3.0/setup.cfg
+-rw-r--r--   0 poro      (1000) poro      (1000)       37 2023-04-21 20:43:44.000000 librus_apix-0.3.0/setup.py
```

### Comparing `librus_apix-0.2.6/LICENSE` & `librus_apix-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/LICENSE.orig` & `librus_apix-0.3.0/LICENSE.orig`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/README.md` & `librus_apix-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/librus_apix/announcements.py` & `librus_apix-0.3.0/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/librus_apix/attendance.py` & `librus_apix-0.3.0/librus_apix/attendance.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,28 @@
 @dataclass
 class Attendance:
     symbol: str
     href: str
     semester: int
     attributes: dict
 
+def get_detail(token: Token, detail_url: str) -> dict[str, str]:
+    details = {}
+    div = no_access_check(
+        BeautifulSoup(token.get(ATTENDANCE_URL + detail_url).text, "lxml")
+    ).find("div", attrs={"class": "container-background"})
+    line = div.find_all("tr", attrs={"class": ["line0", "line1"]})
+    if len(line) < 1:
+        raise ParseError("Error in parsing attendance.")
+    for l in line:
+        if not l.find("th"):
+            continue
+        details[l.find("th").text] = l.find("td").text
+    return details
+
 def get_attendance(token: Token, sort_by: dict[str, str] = {'zmiany_logowanie_wszystkie': ''}) -> list[list[Attendance]]:
     soup = no_access_check(
             BeautifulSoup(token.post(BASE_URL + "/przegladaj_nb/uczen", data=sort_by).text, "lxml")
     )
     table = soup.find("table", attrs={"class": "center big decorated"})
     if table is None:
         raise ParseError("Error parsing attendance.")
```

### Comparing `librus_apix-0.2.6/librus_apix/get_token.py` & `librus_apix-0.3.0/librus_apix/get_token.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/librus_apix/grades.py` & `librus_apix-0.3.0/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/librus_apix/homework.py` & `librus_apix-0.3.0/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/librus_apix/messages.py` & `librus_apix-0.3.0/librus_apix/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from bs4 import BeautifulSoup
 from librus_apix.get_token import get_token, Token
 from librus_apix.urls import BASE_URL, MESSAGE_URL
 from librus_apix.exceptions import TokenError, ParseError
 from librus_apix.helpers import no_access_check
 from dataclasses import dataclass
-
+import re
 
 @dataclass
 class Message:
     author: str
     title: str
     date: str
     href: str
@@ -47,14 +47,25 @@
         author = str(author.text)
         title = str(title.text)
         date = str(date.text)
         m = Message(author, title, date, href, unread, hasAttachment)
         msgs.append(m)
     return msgs
 
+def get_max_page_number(token: Token) -> int:
+    soup = no_access_check(BeautifulSoup(token.get(BASE_URL + '/wiadomosci').text, 'lxml'))
+    try:
+        pages = soup.select_one('div.pagination > span')
+        if not pages:
+            return 0
+        max_pages = pages.text.replace("\xa0", "")
+        max_pages_number = int(re.search('z[0-9]*', max_pages).group(0).replace('z', ""))
+    except:
+        raise ParseError("Error while trying to get max page number.")
+    return max_pages_number
 
 def get_recieved(token: Token, page: int) -> list[Message]:
     payload = {
         "numer_strony105": page,
         "porcjowanie_pojemnik105": 105,
     }
     response = token.post(BASE_URL + "/wiadomosci", data=payload)
```

### Comparing `librus_apix-0.2.6/librus_apix/schedule.py` & `librus_apix-0.3.0/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/librus_apix/timetable.py` & `librus_apix-0.3.0/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.2.6/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.3.0/librus_apix.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 librus_apix/__init__.py
 librus_apix/announcements.py
 librus_apix/attendance.py
+librus_apix/completed_lessons.py
 librus_apix/exceptions.py
 librus_apix/get_token.py
 librus_apix/grades.py
 librus_apix/helpers.py
 librus_apix/homework.py
 librus_apix/messages.py
 librus_apix/schedule.py
```

### Comparing `librus_apix-0.2.6/setup.cfg` & `librus_apix-0.3.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.2.6
+version = 0.3.0
 license = MIT
 description = Web Scraper for Librus Synergia
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers = 
 	License :: OSI Approved :: MIT License
```

