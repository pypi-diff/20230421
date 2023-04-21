# Comparing `tmp/mplgrid-0.2.1.tar.gz` & `tmp/mplgrid-0.3.0.tar.gz`

## Comparing `mplgrid-0.2.1.tar` & `mplgrid-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.readthedocs.yml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 mplgrid-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mplgrid-0.2.1/environment.yml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 mplgrid-0.2.1/requirements.txt
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 mplgrid-0.2.1/setup.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.idea/.gitignore
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.idea/modules.xml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.idea/mplgrid.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mplgrid-0.2.1/mplgrid/__about__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mplgrid-0.2.1/mplgrid/__init__.py
--rw-r--r--   0        0        0     8786 2020-02-02 00:00:00.000000 mplgrid-0.2.1/mplgrid/mplgrid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mplgrid-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 mplgrid-0.2.1/tests/test_grid.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mplgrid-0.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mplgrid-0.2.1/LICENSE
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 mplgrid-0.2.1/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mplgrid-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 mplgrid-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mplgrid-0.3.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 mplgrid-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mplgrid-0.3.0/environment.yml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 mplgrid-0.3.0/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mplgrid-0.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mplgrid-0.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mplgrid-0.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mplgrid-0.3.0/.idea/mplgrid.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 mplgrid-0.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mplgrid-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mplgrid-0.3.0/mplgrid/__about__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mplgrid-0.3.0/mplgrid/__init__.py
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 mplgrid-0.3.0/mplgrid/mplgrid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mplgrid-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 mplgrid-0.3.0/tests/test_grid.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mplgrid-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mplgrid-0.3.0/LICENSE
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 mplgrid-0.3.0/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mplgrid-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 mplgrid-0.3.0/PKG-INFO
```

### Comparing `mplgrid-0.2.1/CHANGELOG.md` & `mplgrid-0.3.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+:rocket: Version 0.3.0
+----------------------
+
+Fixes
+- Fix the aspect argument as it was setting the aspect ratio, which produced the wrong size \
+of chart when data was added.
+
 :rocket: Version 0.2.1
 ----------------------
 
 Fixes
 - Fix docstrings for aspect (height / width)
 
 :rocket: Version 0.2
```

### Comparing `mplgrid-0.2.1/mplgrid/mplgrid.py` & `mplgrid-0.3.0/mplgrid/mplgrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,14 @@
                            nrows=nrows,
                            ncols=ncols,
                            space=space,
                            left=left,
                            bottom=bottom)
     fig, ax = plt.subplots(figsize=(dim['figwidth'], dim['figheight']),
                            nrows=dim['nrows'], ncols=dim['ncols'],
-                           subplot_kw={'aspect': dim['aspect']},
                            gridspec_kw={'left': dim['left'],
                                         'bottom': dim['bottom'],
                                         'right': dim['right'],
                                         'top': dim['top'],
                                         'wspace': dim['wspace'],
                                         'hspace': dim['hspace'],
                                         },
```

### Comparing `mplgrid-0.2.1/tests/test_grid.py` & `mplgrid-0.3.0/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `mplgrid-0.2.1/.gitignore` & `mplgrid-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mplgrid-0.2.1/LICENSE` & `mplgrid-0.3.0/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Andrew Rowlinson
+Copyright (c) 2023 Andrew Rowlinson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mplgrid-0.2.1/pyproject.toml` & `mplgrid-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mplgrid-0.2.1/PKG-INFO` & `mplgrid-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplgrid
-Version: 0.2.1
+Version: 0.3.0
 Summary: mplgrid is a Python library for creating a grid of axes in Matplotlib.
 Project-URL: Documentation, https://github.com/andrewRowlinson/mplgrid#readme
 Project-URL: Issues, https://github.com/andrewRowlinson/mplgrid/issues
 Project-URL: Source, https://github.com/andrewRowlinson/mplgrid/
 Author-email: Andrew Rowlinson <rowlinsonandy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

