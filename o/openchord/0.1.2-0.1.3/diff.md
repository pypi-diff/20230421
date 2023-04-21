# Comparing `tmp/openchord-0.1.2.tar.gz` & `tmp/openchord-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openchord-0.1.2.tar", last modified: Thu Apr 20 16:58:00 2023, max compression
+gzip compressed data, was "openchord-0.1.3.tar", last modified: Thu Apr 20 17:02:40 2023, max compression
```

## Comparing `openchord-0.1.2.tar` & `openchord-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:58:00.193435 openchord-0.1.2/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)    35149 2023-04-20 13:29:24.000000 openchord-0.1.2/LICENSE
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     2042 2023-04-20 16:58:00.193435 openchord-0.1.2/PKG-INFO
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     1525 2023-04-20 16:54:19.000000 openchord-0.1.2/README.md
--rw-rw-r--   0 kenny     (1000) kenny     (1000)      685 2023-04-20 16:57:45.000000 openchord-0.1.2/pyproject.toml
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       38 2023-04-20 16:58:00.193435 openchord-0.1.2/setup.cfg
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:58:00.193435 openchord-0.1.2/src/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)        0 2023-04-20 13:36:13.000000 openchord-0.1.2/src/__init__.py
-drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 16:58:00.193435 openchord-0.1.2/src/openchord.egg-info/
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     2042 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/PKG-INFO
--rw-rw-r--   0 kenny     (1000) kenny     (1000)      249 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/SOURCES.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)        1 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/dependency_links.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       30 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/requires.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)       19 2023-04-20 16:58:00.000000 openchord-0.1.2/src/openchord.egg-info/top_level.txt
--rw-rw-r--   0 kenny     (1000) kenny     (1000)     6261 2023-04-20 13:29:24.000000 openchord-0.1.2/src/openchord.py
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 17:02:40.191742 openchord-0.1.3/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)    35149 2023-04-20 13:29:24.000000 openchord-0.1.3/LICENSE
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     2052 2023-04-20 17:02:40.191742 openchord-0.1.3/PKG-INFO
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     1535 2023-04-20 17:02:08.000000 openchord-0.1.3/README.md
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)      685 2023-04-20 17:02:34.000000 openchord-0.1.3/pyproject.toml
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       38 2023-04-20 17:02:40.191742 openchord-0.1.3/setup.cfg
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 17:02:40.191742 openchord-0.1.3/src/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)        0 2023-04-20 13:36:13.000000 openchord-0.1.3/src/__init__.py
+drwxrwxr-x   0 kenny     (1000) kenny     (1000)        0 2023-04-20 17:02:40.191742 openchord-0.1.3/src/openchord.egg-info/
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     2052 2023-04-20 17:02:40.000000 openchord-0.1.3/src/openchord.egg-info/PKG-INFO
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)      249 2023-04-20 17:02:40.000000 openchord-0.1.3/src/openchord.egg-info/SOURCES.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)        1 2023-04-20 17:02:40.000000 openchord-0.1.3/src/openchord.egg-info/dependency_links.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       30 2023-04-20 17:02:40.000000 openchord-0.1.3/src/openchord.egg-info/requires.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)       19 2023-04-20 17:02:40.000000 openchord-0.1.3/src/openchord.egg-info/top_level.txt
+-rw-rw-r--   0 kenny     (1000) kenny     (1000)     6261 2023-04-20 13:29:24.000000 openchord-0.1.3/src/openchord.py
```

### Comparing `openchord-0.1.2/LICENSE` & `openchord-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openchord-0.1.2/PKG-INFO` & `openchord-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -44,8 +44,8 @@
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
-![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/media/figure.png)
+![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
```

### Comparing `openchord-0.1.2/README.md` & `openchord-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
-![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/media/figure.png)
+![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
```

### Comparing `openchord-0.1.2/pyproject.toml` & `openchord-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openchord"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Kenny Pang", email = "pangkhangee@gmail.com"},
 ]
 description = "A library for ploting chord diagrams"
 readme = "README.md"
 requires-python = ">=3.6"
 keywords = ["plot", "data science", "Jupyter", "network", "graph"]
```

### Comparing `openchord-0.1.2/src/openchord.egg-info/PKG-INFO` & `openchord-0.1.3/src/openchord.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openchord
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for ploting chord diagrams
 Author-email: Kenny Pang <pangkhangee@gmail.com>
 Project-URL: Homepage, https://github.com/pke1029/open-chord
 Keywords: plot,data science,Jupyter,network,graph
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -44,8 +44,8 @@
 fig.color_map = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52']
 fig.show()
 ```
 You can export the figure as an .svg file and open it in a vector graphics software such as [Inkscape](https://inkscape.org/)
 ```python
 fig.save_svg("figure.svg")
 ```
-![Chord diagram using OpenChord](https://github.com/pke1029/open-chord/blob/main/media/figure.png)
+![Chord diagram using OpenChord](https://raw.githubusercontent.com/pke1029/open-chord/main/media/figure.png)
```

### Comparing `openchord-0.1.2/src/openchord.py` & `openchord-0.1.3/src/openchord.py`

 * *Files identical despite different names*

