# Comparing `tmp/cc-lvs-2.1.5.tar.gz` & `tmp/cc-lvs-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc-lvs-2.1.5.tar", last modified: Sun Apr 16 14:47:18 2023, max compression
+gzip compressed data, was "cc-lvs-2.1.6.tar", last modified: Fri Apr 21 07:42:55 2023, max compression
```

## Comparing `cc-lvs-2.1.5.tar` & `cc-lvs-2.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.594856 cc-lvs-2.1.5/
--rw-r--r--   0 namle      (501) staff       (20)      258 2023-04-16 14:47:18.594934 cc-lvs-2.1.5/PKG-INFO
--rw-r--r--   0 namle      (501) staff       (20)      107 2023-02-07 10:24:58.000000 cc-lvs-2.1.5/README.md
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.593415 cc-lvs-2.1.5/cc_lvs.egg-info/
--rw-r--r--   0 namle      (501) staff       (20)      258 2023-04-16 14:47:18.000000 cc-lvs-2.1.5/cc_lvs.egg-info/PKG-INFO
--rw-r--r--   0 namle      (501) staff       (20)      227 2023-04-16 14:47:18.000000 cc-lvs-2.1.5/cc_lvs.egg-info/SOURCES.txt
--rw-r--r--   0 namle      (501) staff       (20)        1 2023-04-16 14:47:18.000000 cc-lvs-2.1.5/cc_lvs.egg-info/dependency_links.txt
--rw-r--r--   0 namle      (501) staff       (20)        4 2023-04-16 14:47:18.000000 cc-lvs-2.1.5/cc_lvs.egg-info/top_level.txt
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.594565 cc-lvs-2.1.5/lvs/
--rw-r--r--   0 namle      (501) staff       (20)       96 2023-04-16 14:46:12.000000 cc-lvs-2.1.5/lvs/__init__.py
--rw-r--r--   0 namle      (501) staff       (20)     2542 2023-04-16 14:44:13.000000 cc-lvs-2.1.5/lvs/client.py
--rw-r--r--   0 namle      (501) staff       (20)      148 2023-02-07 10:32:57.000000 cc-lvs-2.1.5/lvs/exceptions.py
--rw-r--r--   0 namle      (501) staff       (20)      482 2022-03-25 10:38:44.000000 cc-lvs-2.1.5/lvs/settings.py
--rw-r--r--   0 namle      (501) staff       (20)       94 2023-02-07 10:24:58.000000 cc-lvs-2.1.5/pyproject.toml
--rw-r--r--   0 namle      (501) staff       (20)      296 2023-04-16 14:47:18.595185 cc-lvs-2.1.5/setup.cfg
--rw-r--r--   0 namle      (501) staff       (20)       51 2023-02-07 10:24:58.000000 cc-lvs-2.1.5/setup.py
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-21 07:42:55.462261 cc-lvs-2.1.6/
+-rw-r--r--   0 namle      (501) staff       (20)      258 2023-04-21 07:42:55.462350 cc-lvs-2.1.6/PKG-INFO
+-rw-r--r--   0 namle      (501) staff       (20)      107 2023-02-07 10:24:58.000000 cc-lvs-2.1.6/README.md
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-21 07:42:55.461033 cc-lvs-2.1.6/cc_lvs.egg-info/
+-rw-r--r--   0 namle      (501) staff       (20)      258 2023-04-21 07:42:55.000000 cc-lvs-2.1.6/cc_lvs.egg-info/PKG-INFO
+-rw-r--r--   0 namle      (501) staff       (20)      227 2023-04-21 07:42:55.000000 cc-lvs-2.1.6/cc_lvs.egg-info/SOURCES.txt
+-rw-r--r--   0 namle      (501) staff       (20)        1 2023-04-21 07:42:55.000000 cc-lvs-2.1.6/cc_lvs.egg-info/dependency_links.txt
+-rw-r--r--   0 namle      (501) staff       (20)        4 2023-04-21 07:42:55.000000 cc-lvs-2.1.6/cc_lvs.egg-info/top_level.txt
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-21 07:42:55.462013 cc-lvs-2.1.6/lvs/
+-rw-r--r--   0 namle      (501) staff       (20)       96 2023-04-16 14:46:12.000000 cc-lvs-2.1.6/lvs/__init__.py
+-rw-r--r--   0 namle      (501) staff       (20)     2560 2023-04-21 07:42:01.000000 cc-lvs-2.1.6/lvs/client.py
+-rw-r--r--   0 namle      (501) staff       (20)      148 2023-02-07 10:32:57.000000 cc-lvs-2.1.6/lvs/exceptions.py
+-rw-r--r--   0 namle      (501) staff       (20)      482 2022-03-25 10:38:44.000000 cc-lvs-2.1.6/lvs/settings.py
+-rw-r--r--   0 namle      (501) staff       (20)       94 2023-02-07 10:24:58.000000 cc-lvs-2.1.6/pyproject.toml
+-rw-r--r--   0 namle      (501) staff       (20)      296 2023-04-21 07:42:55.462571 cc-lvs-2.1.6/setup.cfg
+-rw-r--r--   0 namle      (501) staff       (20)       51 2023-02-07 10:24:58.000000 cc-lvs-2.1.6/setup.py
```

### Comparing `cc-lvs-2.1.5/lvs/client.py` & `cc-lvs-2.1.6/lvs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         try:
             soup = BeautifulSoup(html, 'html.parser')
             rows = soup.find('tbody').find_all('tr', attrs={'class': 'report-info'})
 
             for row in rows:
                 cols = row.find_all('td')
 
-                username = cols[0].text.lower().replace('\n', '')
+                username = cols[0].find_all('h6')[1].text.lower().replace('\n', '')
 
                 yield {
                     'username': username,
                     'turnover': LvsClient.format_float(cols[5].text),
                     'net_turnover': LvsClient.format_float(cols[12].text),
                     'commission': LvsClient.format_float(cols[7].text),
                     'win_lose': LvsClient.format_float(cols[9].text),
```

