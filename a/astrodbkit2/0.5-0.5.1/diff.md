# Comparing `tmp/astrodbkit2-0.5.tar.gz` & `tmp/astrodbkit2-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrodbkit2-0.5.tar", last modified: Tue Mar 14 20:52:44 2023, max compression
+gzip compressed data, was "astrodbkit2-0.5.1.tar", last modified: Fri Apr 21 18:10:55 2023, max compression
```

## Comparing `astrodbkit2-0.5.tar` & `astrodbkit2-0.5.1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.733507 astrodbkit2-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-14 20:52:25.000000 astrodbkit2-0.5/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.729507 astrodbkit2-0.5/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-14 20:52:25.000000 astrodbkit2-0.5/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.729507 astrodbkit2-0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.733507 astrodbkit2-0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-14 20:52:25.000000 astrodbkit2-0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-14 20:52:25.000000 astrodbkit2-0.5/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-14 20:52:25.000000 astrodbkit2-0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-14 20:52:25.000000 astrodbkit2-0.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-14 20:52:25.000000 astrodbkit2-0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-14 20:52:44.733507 astrodbkit2-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-14 20:52:25.000000 astrodbkit2-0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.733507 astrodbkit2-0.5/astrodbkit2/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34534 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/astrodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/schema_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.733507 astrodbkit2-0.5/astrodbkit2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/tests/test_astrodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/tests/test_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-03-14 20:52:25.000000 astrodbkit2-0.5/astrodbkit2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-14 20:52:44.000000 astrodbkit2-0.5/astrodbkit2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.733507 astrodbkit2-0.5/astrodbkit2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-14 20:52:44.000000 astrodbkit2-0.5/astrodbkit2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 20:52:44.000000 astrodbkit2-0.5/astrodbkit2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 20:52:44.000000 astrodbkit2-0.5/astrodbkit2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-14 20:52:44.000000 astrodbkit2-0.5/astrodbkit2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 20:52:44.000000 astrodbkit2-0.5/astrodbkit2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-14 20:52:44.000000 astrodbkit2-0.5/astrodbkit2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-14 20:52:44.000000 astrodbkit2-0.5/astrodbkit2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.733507 astrodbkit2-0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-03-14 20:52:25.000000 astrodbkit2-0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-14 20:52:25.000000 astrodbkit2-0.5/docs/astrodb.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-03-14 20:52:25.000000 astrodbkit2-0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-03-14 20:52:25.000000 astrodbkit2-0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-03-14 20:52:25.000000 astrodbkit2-0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-14 20:52:25.000000 astrodbkit2-0.5/docs/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:52:44.733507 astrodbkit2-0.5/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-14 20:52:25.000000 astrodbkit2-0.5/licenses/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-14 20:52:25.000000 astrodbkit2-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-14 20:52:44.733507 astrodbkit2-0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-03-14 20:52:25.000000 astrodbkit2-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.840833 astrodbkit2-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/astrodbkit2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34548 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/astrodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/schema_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/astrodbkit2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/test_astrodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/test_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/astrodbkit2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/astrodbkit2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 18:10:55.000000 astrodbkit2-0.5.1/astrodbkit2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/astrodb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/spectra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/docs/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:10:55.844833 astrodbkit2-0.5.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/licenses/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-21 18:10:55.848833 astrodbkit2-0.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-04-21 18:10:33.000000 astrodbkit2-0.5.1/setup.py
```

### Comparing `astrodbkit2-0.5/.devcontainer/devcontainer.json` & `astrodbkit2-0.5.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/.github/workflows/python-publish.yml` & `astrodbkit2-0.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/.github/workflows/test-package.yml` & `astrodbkit2-0.5.1/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/.gitignore` & `astrodbkit2-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/PKG-INFO` & `astrodbkit2-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrodbkit2
-Version: 0.5
+Version: 0.5.1
 Summary: Astronomical database handler code
 Home-page: 
 Author: David Rodriguez
 Author-email: drodriguez@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `astrodbkit2-0.5/README.rst` & `astrodbkit2-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/astrodbkit2/__init__.py` & `astrodbkit2-0.5.1/astrodbkit2/__init__.py`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/astrodbkit2/astrodb.py` & `astrodbkit2-0.5.1/astrodbkit2/astrodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 spectra = [spectra]
             for col in spectra:
                 if col in df.columns.to_list():
                     df[col] = df[col].apply(lambda x: load_spectrum(x, spectra_format=spectra_format))
 
         return df
 
-    def spectra(self, spectra=['spectrum'], fmt='astropy', **kwargs):
+    def spectra(self, spectra=['spectrum', 'access_url'], fmt='astropy', **kwargs):
         """
         Convenience method fo that uses default column name for spectra conversion
 
         Parameters
         ----------
         spectra : str or list
             List of columns to process as spectra
```

### Comparing `astrodbkit2-0.5/astrodbkit2/spectra.py` & `astrodbkit2-0.5.1/astrodbkit2/spectra.py`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/astrodbkit2/tests/test_astrodb.py` & `astrodbkit2-0.5.1/astrodbkit2/tests/test_astrodb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Testing for astrodb
 
 import os
 import json
 import pytest
 import io
 import pandas as pd
-from sqlalchemy import select, func
+import sqlalchemy as sa
 from sqlalchemy.exc import IntegrityError
 from astropy.table import Table
 from astropy.coordinates import SkyCoord
 from astropy.units.quantity import Quantity
 from astropy.io import ascii
 from astrodbkit2.astrodb import Database, create_database, Base, copy_database_schema
+from astrodbkit2.views import view
 from astrodbkit2.schema_example import *
 try:
     import mock
 except ImportError:
     from unittest import mock
 
 
@@ -334,14 +335,58 @@
                                     'comments': None,
                                     'reference': 'Cutr12'}]
                  }
 
     assert db.inventory('2MASS J13571237+1428398') == test_dict
 
 
+def test_views(db):
+    # Test database views
+
+    # Create one manually
+    PhotView = view(
+        "PhotView",
+        db.metadata,
+        sa.select(
+            db.Sources.c.source.label("source"),
+            db.Sources.c.ra.label("s_ra"),
+            db.Sources.c.dec.label("s_dec"),
+            db.Photometry.c.band.label("band"),
+            db.Photometry.c.magnitude.label("value"),
+        ).select_from(db.Sources).join(db.Photometry, db.Sources.c.source == db.Photometry.c.source)
+        )
+    # Explicitly create
+    with db.engine.begin() as conn:
+        db.metadata.create_all(conn)
+
+    # Query the view
+    t = db.query(PhotView).table()
+    print(t)
+    assert len(t) == 3 # 3 Photometry values for the single source
+
+    # Query one created in schema file
+    t = db.query(SampleView).table()
+    print(t)
+    assert len(t) == 1
+
+    # Test views are listed when inspected
+    insp = sa.inspect(db.engine)
+    view_list = insp.get_view_names()
+    assert 'PhotView' in view_list and 'SampleView' in view_list
+
+    # Reflect a view and query it
+    ViewCopy = sa.Table('SampleView', sa.MetaData())  
+    insp.reflect_table(ViewCopy, include_columns=None)
+    assert db.query(ViewCopy).count() == 1
+
+    # Confirm that views are not used in inventory
+    assert 'PhotView' not in db.inventory('2MASS J13571237+1428398').keys()
+    assert 'SampleView' not in db.inventory('2MASS J13571237+1428398').keys()
+
+
 def test_save_reference_table(db, db_dir):
     # Test saving a reference table
     if os.path.exists(os.path.join(db_dir, 'Publications.json')):
         os.remove(os.path.join(db_dir, 'Publications.json'))
     db.save_reference_table('Publications', db_dir)
     assert os.path.exists(os.path.join(db_dir, 'Publications.json'))
     os.remove(os.path.join(db_dir, 'Publications.json'))  # explicitly removing so that the next step will get verified
```

### Comparing `astrodbkit2-0.5/astrodbkit2/tests/test_spectra.py` & `astrodbkit2-0.5.1/astrodbkit2/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/astrodbkit2/tests/test_utils.py` & `astrodbkit2-0.5.1/astrodbkit2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/astrodbkit2/utils.py` & `astrodbkit2-0.5.1/astrodbkit2/utils.py`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/astrodbkit2.egg-info/PKG-INFO` & `astrodbkit2-0.5.1/astrodbkit2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrodbkit2
-Version: 0.5
+Version: 0.5.1
 Summary: Astronomical database handler code
 Home-page: 
 Author: David Rodriguez
 Author-email: drodriguez@stsci.edu
 License: BSD 3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `astrodbkit2-0.5/astrodbkit2.egg-info/SOURCES.txt` & `astrodbkit2-0.5.1/astrodbkit2.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,28 @@
 .github/workflows/test-package.yml
 astrodbkit2/__init__.py
 astrodbkit2/astrodb.py
 astrodbkit2/schema_example.py
 astrodbkit2/spectra.py
 astrodbkit2/utils.py
 astrodbkit2/version.py
+astrodbkit2/views.py
 astrodbkit2.egg-info/PKG-INFO
 astrodbkit2.egg-info/SOURCES.txt
 astrodbkit2.egg-info/dependency_links.txt
 astrodbkit2.egg-info/entry_points.txt
 astrodbkit2.egg-info/not-zip-safe
 astrodbkit2.egg-info/requires.txt
 astrodbkit2.egg-info/top_level.txt
 astrodbkit2/tests/__init__.py
 astrodbkit2/tests/test_astrodb.py
 astrodbkit2/tests/test_spectra.py
 astrodbkit2/tests/test_utils.py
+astrodbkit2/tests/test_views.py
 docs/Makefile
 docs/astrodb.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
+docs/spectra.rst
 docs/utils.rst
 licenses/LICENSE.rst
```

### Comparing `astrodbkit2-0.5/docs/Makefile` & `astrodbkit2-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/docs/conf.py` & `astrodbkit2-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/docs/index.rst` & `astrodbkit2-0.5.1/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -306,14 +306,50 @@
 The parameter `spectra_format` can be specified if **specutils** is having trouble determining the type of spectrum.
 
 Spectra need to be specified as either URL or paths relative to an environment variable,
 for example `$ASTRODB_SPECTRA/infrared/myfile.fits`.
 **AstrodbKit2** would examine the environment variable `$ASTRODB_SPECTRA` and use that as
 part of the absolute path to the file.
 
+Working With Views
+------------------
+
+If your database contains views, they will not be included in the inventory methods or in the output JSON files. 
+However, you can still work with and query data in them. 
+The best way to define them is in the schema file, for example, with something like::
+
+    SampleView = view(
+        "SampleView",
+        Base.metadata,
+        sa.select(
+            Sources.source.label("source"),
+            Sources.ra.label("s_ra"),
+            Sources.dec.label("s_dec"),
+            SpectralTypes.spectral_type.label("spectral_type"),
+        ).select_from(Sources).join(SpectralTypes, Sources.source == SpectralTypes.source)
+        )
+
+When created, the database will contain these views and users can reflect them to access them::
+    
+    import sqlalchemy as sa
+
+    # Inspect the database to get a list of available views
+    insp = sa.inspect(db.engine)
+    print(insp.get_view_names())
+
+    # Reflect a view and query it
+    SampleView = sa.Table('SampleView', sa.MetaData())  
+    insp.reflect_table(SampleView, include_columns=None)
+    db.query(SampleView).table()
+
+It is important that `sa.MetaData()` be used in the `sa.Table()` call as you don't want to modify 
+the metadata of the actual database. 
+If you don't do this and instead use `db.metadata`, you may end up with errors in other parts of AstrodbKit2 
+functionality as the view will be treated as a physical table.
+
 Modifying Data
 ==============
 
 As a wrapper against standard SQLAlchemy calls, data can be added fairly simply.
 
 .. note:: Primary and Foreign keys, if present in the database, are verified when modifying data.
           This can prevent duplicated keys from being created and can propagate deletes or updates as specified
@@ -385,13 +421,14 @@
 =============
 
 .. toctree::
    :maxdepth: 2
 
    astrodb.rst
    utils.rst
+   spectra.rst
 
 Indices and tables
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `astrodbkit2-0.5/docs/make.bat` & `astrodbkit2-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/licenses/LICENSE.rst` & `astrodbkit2-0.5.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/setup.cfg` & `astrodbkit2-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `astrodbkit2-0.5/setup.py` & `astrodbkit2-0.5.1/setup.py`

 * *Files identical despite different names*

