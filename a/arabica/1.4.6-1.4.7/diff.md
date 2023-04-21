# Comparing `tmp/arabica-1.4.6.tar.gz` & `tmp/arabica-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.4.6.tar", last modified: Mon Apr 17 22:10:11 2023, max compression
+gzip compressed data, was "arabica-1.4.7.tar", last modified: Fri Apr 21 14:07:25 2023, max compression
```

## Comparing `arabica-1.4.6.tar` & `arabica-1.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:10:11.499354 arabica-1.4.6/
--rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.6/LICENSE
--rw-rw-rw-   0        0        0     7537 2023-04-17 22:10:11.499354 arabica-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 22:10:11.440319 arabica-1.4.6/arabica/
--rw-rw-rw-   0        0        0      105 2023-04-17 22:07:56.000000 arabica-1.4.6/arabica/__init__.py
--rw-rw-rw-   0        0        0    11740 2023-04-17 21:41:36.000000 arabica-1.4.6/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    29482 2023-04-16 21:15:43.000000 arabica-1.4.6/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.6/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.6/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.6/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.6/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.6/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.6/arabica/sentiment.py
--rw-rw-rw-   0        0        0      449 2022-10-18 19:06:35.000000 arabica-1.4.6/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:10:11.497356 arabica-1.4.6/arabica.egg-info/
--rw-rw-rw-   0        0        0     7537 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 22:10:11.000000 arabica-1.4.6/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-04-17 22:07:56.000000 arabica-1.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 22:10:11.510482 arabica-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-04-17 22:07:56.000000 arabica-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:07:25.477142 arabica-1.4.7/
+-rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0     7537 2023-04-21 14:07:25.477142 arabica-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:07:25.421147 arabica-1.4.7/arabica/
+-rw-rw-rw-   0        0        0      105 2023-04-21 14:06:32.000000 arabica-1.4.7/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11740 2023-04-17 21:41:36.000000 arabica-1.4.7/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    29525 2023-04-20 22:52:23.000000 arabica-1.4.7/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.7/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.7/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.7/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.7/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.7/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.7/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      449 2023-04-20 22:52:23.000000 arabica-1.4.7/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:07:25.469143 arabica-1.4.7/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7537 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-04-21 14:06:32.000000 arabica-1.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:07:25.477142 arabica-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-04-21 14:06:32.000000 arabica-1.4.7/setup.py
```

### Comparing `arabica-1.4.6/PKG-INFO` & `arabica-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.6
+Version: 1.4.7
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
```

### Comparing `arabica-1.4.6/README.md` & `arabica-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `arabica-1.4.6/arabica/arabica_freq.py` & `arabica-1.4.7/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.6/arabica/cappuccino.py` & `arabica-1.4.7/arabica/cappuccino.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from arabica import arabica_freq
 from wordcloud import WordCloud
 import matplotlib.pyplot as plt
 from matplotlib.pyplot import figure
 import pandas as pd
 import numpy as np
 
+import nltk
+nltk.download('stopwords')
+
 
 def cappuccino(text: str,                  # Text
                time: str,                  # Time
                date_format: str,           # Date format: 'eur' - European, 'us' - American
                stopwords: [],              # Languages for stop words
                skip: [ ],                  # Remove additional strings
                plot: str = '',             # Chart type: 'wordcloud'/'heatmap'/'line'
```

### Comparing `arabica-1.4.6/arabica/clean_ngram.py` & `arabica-1.4.7/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.6/arabica/coffee_break.py` & `arabica-1.4.7/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.6/arabica/group.py` & `arabica-1.4.7/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.6/arabica/preprocess.py` & `arabica-1.4.7/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.6/arabica.egg-info/PKG-INFO` & `arabica-1.4.7/arabica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.6
+Version: 1.4.7
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
```

### Comparing `arabica-1.4.6/pyproject.toml` & `arabica-1.4.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.4.6"
+version = "1.4.7"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.4.6/setup.py` & `arabica-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.4.6",
+        version="1.4.7",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

