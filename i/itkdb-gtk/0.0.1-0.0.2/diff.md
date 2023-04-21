# Comparing `tmp/itkdb_gtk-0.0.1.tar.gz` & `tmp/itkdb_gtk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itkdb_gtk-0.0.1.tar", last modified: Tue Apr 11 16:16:00 2023, max compression
+gzip compressed data, was "itkdb_gtk-0.0.2.tar", last modified: Fri Apr 21 08:56:08 2023, max compression
```

## Comparing `itkdb_gtk-0.0.1.tar` & `itkdb_gtk-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-11 16:16:00.124181 itkdb_gtk-0.0.1/
--rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-04-11 16:16:00.123760 itkdb_gtk-0.0.1/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     1997 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.1/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-11 16:16:00.121034 itkdb_gtk-0.0.1/itkdb_gtk/
--rw-r--r--   0 lacasta    (503) staff       (20)    12174 2023-04-11 15:49:02.000000 itkdb_gtk-0.0.1/itkdb_gtk/GlueWeight.py
--rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.1/itkdb_gtk/ITkDBlogin.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14205 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.1/itkdb_gtk/ITkDButils.py
--rw-r--r--   0 lacasta    (503) staff       (20)      552 2023-04-11 16:04:01.000000 itkdb_gtk-0.0.1/itkdb_gtk/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3892 2023-04-11 15:10:48.000000 itkdb_gtk-0.0.1/itkdb_gtk/dashBoard.py
--rw-r--r--   0 lacasta    (503) staff       (20)    20708 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.1/itkdb_gtk/dbGtkUtils.py
--rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.1/itkdb_gtk/getShipments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7140 2023-04-11 15:50:48.000000 itkdb_gtk-0.0.1/itkdb_gtk/groundingTest.py
--rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.1/itkdb_gtk/readAVSdata.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.1/itkdb_gtk/readGoogleSheet.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.1/itkdb_gtk/sendShipments.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    21093 2023-04-11 15:23:27.000000 itkdb_gtk-0.0.1/itkdb_gtk/uploadPetalInformation.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    12171 2023-04-11 15:53:15.000000 itkdb_gtk-0.0.1/itkdb_gtk/uploadTest.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-11 16:16:00.123255 itkdb_gtk-0.0.1/itkdb_gtk.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-04-11 16:16:00.000000 itkdb_gtk-0.0.1/itkdb_gtk.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      559 2023-04-11 16:16:00.000000 itkdb_gtk-0.0.1/itkdb_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-11 16:16:00.000000 itkdb_gtk-0.0.1/itkdb_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      234 2023-04-11 16:16:00.000000 itkdb_gtk-0.0.1/itkdb_gtk.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-04-11 16:16:00.000000 itkdb_gtk-0.0.1/itkdb_gtk.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-04-11 16:16:00.000000 itkdb_gtk-0.0.1/itkdb_gtk.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      968 2023-04-11 16:15:28.000000 itkdb_gtk-0.0.1/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-11 16:16:00.124292 itkdb_gtk-0.0.1/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-21 08:56:08.121190 itkdb_gtk-0.0.2/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-04-21 08:56:08.120980 itkdb_gtk-0.0.2/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     1997 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.2/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-21 08:56:08.119181 itkdb_gtk-0.0.2/itkdb_gtk/
+-rw-r--r--   0 lacasta    (503) staff       (20)    12180 2023-04-21 08:10:24.000000 itkdb_gtk-0.0.2/itkdb_gtk/GlueWeight.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.2/itkdb_gtk/ITkDBlogin.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14205 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.2/itkdb_gtk/ITkDButils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      552 2023-04-11 16:04:01.000000 itkdb_gtk-0.0.2/itkdb_gtk/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3342 2023-04-13 14:46:29.000000 itkdb_gtk-0.0.2/itkdb_gtk/checkComponent.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4181 2023-04-21 08:06:29.000000 itkdb_gtk-0.0.2/itkdb_gtk/dashBoard.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    20708 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.2/itkdb_gtk/dbGtkUtils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.2/itkdb_gtk/getShipments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7140 2023-04-11 15:50:48.000000 itkdb_gtk-0.0.2/itkdb_gtk/groundingTest.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.2/itkdb_gtk/readAVSdata.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.2/itkdb_gtk/readGoogleSheet.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.2/itkdb_gtk/sendShipments.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    21093 2023-04-11 15:23:27.000000 itkdb_gtk-0.0.2/itkdb_gtk/uploadPetalInformation.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    12171 2023-04-11 15:53:15.000000 itkdb_gtk-0.0.2/itkdb_gtk/uploadTest.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-21 08:56:08.120694 itkdb_gtk-0.0.2/itkdb_gtk.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-04-21 08:56:08.000000 itkdb_gtk-0.0.2/itkdb_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      587 2023-04-21 08:56:08.000000 itkdb_gtk-0.0.2/itkdb_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-21 08:56:08.000000 itkdb_gtk-0.0.2/itkdb_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      239 2023-04-21 08:56:08.000000 itkdb_gtk-0.0.2/itkdb_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-04-21 08:56:08.000000 itkdb_gtk-0.0.2/itkdb_gtk.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-04-21 08:56:08.000000 itkdb_gtk-0.0.2/itkdb_gtk.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)     1083 2023-04-21 08:56:00.000000 itkdb_gtk-0.0.2/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-21 08:56:08.121250 itkdb_gtk-0.0.2/setup.cfg
```

### Comparing `itkdb_gtk-0.0.1/PKG-INFO` & `itkdb_gtk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb_gtk
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.1/README.md` & `itkdb_gtk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/GlueWeight.py` & `itkdb_gtk-0.0.2/itkdb_gtk/GlueWeight.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         image = Gtk.Image.new_from_gicon(icon, Gtk.IconSize.BUTTON)
         button.add(image)
         button.set_tooltip_text("Click to upload test shown in notebook.")
         button.connect("clicked", self.upload_current_test)
         hb.pack_end(button)
 
         self.userLabel = Gtk.Label()
-        self.userLabel.set_text(session.user.name)
+        self.userLabel.set_text(self.session.user.name)
         hb.pack_start(self.userLabel)
 
         # Create main content box
         self.mainBox = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
         self.add(self.mainBox)
         # file entry and search button
         self.file_name = Gtk.FileChooserButton()
@@ -361,14 +361,15 @@
             for m in self.modules:
                 print("### Uploading {} for module {}".format(m["testType"], m["component"]))
                 resp = ITkDButils.upload_test(session, m)
 
                 if resp is not None:
                     print(resp)
 
+
 def main():
     """Main entry."""
     # Get input file
     parser = argparse.ArgumentParser(description="GlueTest")
     parser.add_argument('files', nargs='*', help="Input files")
     parser.add_argument("--separator", default="MODULE_SN", help="Key for module serial number.")
     options = parser.parse_args()
```

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/ITkDBlogin.py` & `itkdb_gtk-0.0.2/itkdb_gtk/ITkDBlogin.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/ITkDButils.py` & `itkdb_gtk-0.0.2/itkdb_gtk/ITkDButils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/__init__.py` & `itkdb_gtk-0.0.2/itkdb_gtk/__init__.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/dashBoard.py` & `itkdb_gtk-0.0.2/itkdb_gtk/dashBoard.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 try:
     import dbGtkUtils
     import getShipments
     import groundingTest
     import ITkDBlogin
     import sendShipments
     import uploadTest
+    import GlueWeight
 
 except Exception:
-    from itkdb_gtk import dbGtkUtils, getShipments, groundingTest, ITkDBlogin, sendShipments, uploadTest
+    from itkdb_gtk import dbGtkUtils, getShipments, groundingTest, ITkDBlogin, sendShipments, uploadTest, GlueWeight
 
 import gi
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 
 
@@ -50,14 +51,19 @@
         grid.attach(btnTest, 0, irow, 1, 1)
 
         btnGnd = Gtk.Button(label="Petal VI/GND")
         btnGnd.connect("clicked", self.petal_gnd)
         grid.attach(btnGnd, 1, irow, 1, 1)
 
         irow += 1
+        btnWeight = Gtk.Button(label="GlueWeight")
+        btnWeight.connect("clicked", self.glue_weight)
+        grid.attach(btnWeight, 0, irow, 1, 1)
+
+        irow += 1
         grid.attach(Gtk.Label(), 0, irow, 1, 1)
 
         irow += 1
         lbl = Gtk.Label()
         lbl.set_markup("<b>Shipments</b>")
         lbl.set_xalign(0)
         grid.attach(lbl, 0, irow, 1, 1)
@@ -70,14 +76,18 @@
         recS = Gtk.Button(label="Receive Shipment")
         recS.connect("clicked", self.receive_shipment)
         grid.attach(recS, 1, irow, 1, 1,)
 
         self.mainBox.pack_start(Gtk.Separator(orientation=Gtk.Orientation.HORIZONTAL), False, True, 5)
 
         self.show_all()
+        
+    def glue_weight(self, *args):
+        """Glue Weight test."""
+        
 
     def upload_test(self, *args):
         """Launch upload test."""
         bitn = 1
         bt = 1 << bitn
         if self.mask & bt:
             return
```

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/dbGtkUtils.py` & `itkdb_gtk-0.0.2/itkdb_gtk/dbGtkUtils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/getShipments.py` & `itkdb_gtk-0.0.2/itkdb_gtk/getShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/groundingTest.py` & `itkdb_gtk-0.0.2/itkdb_gtk/groundingTest.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/readAVSdata.py` & `itkdb_gtk-0.0.2/itkdb_gtk/readAVSdata.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/readGoogleSheet.py` & `itkdb_gtk-0.0.2/itkdb_gtk/readGoogleSheet.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/sendShipments.py` & `itkdb_gtk-0.0.2/itkdb_gtk/sendShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/uploadPetalInformation.py` & `itkdb_gtk-0.0.2/itkdb_gtk/uploadPetalInformation.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk/uploadTest.py` & `itkdb_gtk-0.0.2/itkdb_gtk/uploadTest.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk.egg-info/PKG-INFO` & `itkdb_gtk-0.0.2/itkdb_gtk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb-gtk
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.1/itkdb_gtk.egg-info/SOURCES.txt` & `itkdb_gtk-0.0.2/itkdb_gtk.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 pyproject.toml
 itkdb_gtk/GlueWeight.py
 itkdb_gtk/ITkDBlogin.py
 itkdb_gtk/ITkDButils.py
 itkdb_gtk/__init__.py
+itkdb_gtk/checkComponent.py
 itkdb_gtk/dashBoard.py
 itkdb_gtk/dbGtkUtils.py
 itkdb_gtk/getShipments.py
 itkdb_gtk/groundingTest.py
 itkdb_gtk/readAVSdata.py
 itkdb_gtk/readGoogleSheet.py
 itkdb_gtk/sendShipments.py
```

### Comparing `itkdb_gtk-0.0.1/pyproject.toml` & `itkdb_gtk-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itkdb_gtk"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of Gtk based GUI to access ITkDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -21,17 +21,23 @@
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [project.gui-scripts]
-dash_board = "itkdb_gtk:dash_board"
+itkdb_dashBoard = "itkdb_gtk:dash_board"
 getShipments = "itkdb_gtk:getShipments"
 glueWeight = "itkdb_gtk:glueWeight"
 groundingTest = "itkdb_gtk:groundingTest"
 sendShipments = "itkdb_gtk:sendShipments"
 uploadTest = "itkdb_gtk:uploadTest"
 
+[tool.setuptools]
+include-package-data = true
+
+[tool.setuptools.package-data]
+mypkg = ["*.desktop", "*.svg"]
+
 [project.urls]
 "Homepage" = "https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils"
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues"
```

