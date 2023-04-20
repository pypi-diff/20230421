# Comparing `tmp/fringes_gui-0.1.2.tar.gz` & `tmp/fringes_gui-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fringes_gui-0.1.2.tar", max compression
+gzip compressed data, was "fringes_gui-0.1.3.tar", max compression
```

## Comparing `fringes_gui-0.1.2.tar` & `fringes_gui-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       90 2023-04-12 20:02:53.369380 fringes_gui-0.1.2/fringes_gui/__init__.py
--rw-r--r--   0        0        0    16385 2023-04-12 20:02:20.615647 fringes_gui-0.1.2/fringes_gui/gui.py
--rw-r--r--   0        0        0    18072 2023-04-12 19:56:33.023246 fringes_gui-0.1.2/fringes_gui/logic.py
--rw-r--r--   0        0        0      231 2023-04-12 07:45:19.000000 fringes_gui-0.1.2/fringes_gui/main.py
--rw-r--r--   0        0        0    26876 2023-04-12 13:19:40.997785 fringes_gui-0.1.2/fringes_gui/params.py
--rw-r--r--   0        0        0    27386 2023-04-12 13:20:41.909708 fringes_gui-0.1.2/fringes_gui/setters.py
--rw-r--r--   0        0        0   250284 2023-04-01 09:49:27.000000 fringes_gui-0.1.2/fringes_gui/spirals.png
--rw-r--r--   0        0        0      715 2023-04-12 20:02:53.377359 fringes_gui-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3858 2023-04-12 19:21:58.331433 fringes_gui-0.1.2/README.md
--rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 fringes_gui-0.1.2/setup.py
--rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 fringes_gui-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-04-20 22:27:40.520619 fringes_gui-0.1.3/fringes_gui/__init__.py
+-rw-r--r--   0        0        0    16423 2023-04-20 15:30:56.137009 fringes_gui-0.1.3/fringes_gui/gui.py
+-rw-r--r--   0        0        0    18737 2023-04-15 13:36:30.383769 fringes_gui-0.1.3/fringes_gui/logic.py
+-rw-r--r--   0        0        0      231 2023-04-12 07:45:19.000000 fringes_gui-0.1.3/fringes_gui/main.py
+-rw-r--r--   0        0        0    26900 2023-04-20 15:28:07.681543 fringes_gui-0.1.3/fringes_gui/params.py
+-rw-r--r--   0        0        0    28027 2023-04-20 15:30:05.785088 fringes_gui-0.1.3/fringes_gui/setters.py
+-rw-r--r--   0        0        0   250284 2023-04-01 09:49:27.000000 fringes_gui-0.1.3/fringes_gui/spirals.png
+-rw-r--r--   0        0        0      725 2023-04-20 22:27:59.073929 fringes_gui-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4159 2023-04-20 22:01:27.760312 fringes_gui-0.1.3/README.md
+-rw-r--r--   0        0        0     5008 1970-01-01 00:00:00.000000 fringes_gui-0.1.3/setup.py
+-rw-r--r--   0        0        0     4956 1970-01-01 00:00:00.000000 fringes_gui-0.1.3/PKG-INFO
```

### Comparing `fringes_gui-0.1.2/fringes_gui/gui.py` & `fringes_gui-0.1.3/fringes_gui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,30 +18,23 @@
 
 class FringesGUI(QApplication):
     """Simple graphical user interface for the 'fringes' package."""
 
     def __init__(self):
         super(FringesGUI, self).__init__([])
 
-        myappid = "Fringes-GUI"  # arbitrary string
-        try:
-            fname = os.path.join(os.path.dirname(__file__), "..", "pyproject.toml")
-            version = toml.load(fname)["tool"]["poetry"]["version"]
-            myappid += "_" + version
-        except Exception:
-            pass
+        fname = os.path.join(os.path.dirname(__file__), "..", "pyproject.toml")
+        version = toml.load(fname)["tool"]["poetry"]["version"]
+        myappid = "Fringes-GUI" + " " + version  # arbitrary string
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
 
         pg.setConfigOptions(imageAxisOrder="row-major", useNumba=True)  # useCupy
 
         self.fringes = frng.Fringes(X=1920, Y=1200)
         self.fringes.logger.setLevel("INFO")
-        fname = os.path.join(os.path.dirname(__file__), "params.yaml")
-        if os.path.isfile(fname):
-            self.fringes.load(fname)
         self.initials = self.fringes.params
         self.key = ""
         self.visibility = "Expert"
         self.digits = 8  # todo: len(str(self.fringes._Pmax))  # 4 (digits) + 1 (point) + 3 (decimals) = 8 == current length of Pmax?
         self.sub = str.maketrans("1234567890", "₁₂₃₄₅₆₇₈₉₀")
         self.sup = str.maketrans("₁₂₃₄₅₆₇₈₉₀", "1234567890")
 
@@ -156,14 +149,15 @@
         self.encode_label = QtWidgets.QLabel("      Encode on parameter change")
         self.decode_checkbox = QtWidgets.QCheckBox()
         self.decode_label = QtWidgets.QLabel("      Decode on parameter change")
         self.reset_button = QtWidgets.QPushButton("Reset")
         self.reset_button.setEnabled(False)
         self.reset_button.setToolTip("Press 'Ctrl+R'.")
         self.default_key = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+Shift+D"), self.win)
+        self.coordinates_key = QtGui.QShortcut(QtGui.QKeySequence("G"), self.win)
         self.encode_button = QtWidgets.QPushButton("Encode")
         self.encode_button.setToolTip("Press 'E'.")
         self.encode_button.setStyleSheet("" if self.encodeOK else "QPushButton{color: red}")
         self.encode_key = QtGui.QShortcut(QtGui.QKeySequence("E"), self.win)
         self.decode_button = QtWidgets.QPushButton("Decode")
         self.decode_button.setEnabled(False)
         self.decode_button.setToolTip("Press 'D'.")
@@ -289,14 +283,19 @@
         handler.widget = self.log_widget
         self.fringes.logger.addHandler(handler)
 
         # todo: reset button or simply restart? save current config on shutdown
 
         set_functionality(self)
 
+        fname = os.path.join(os.path.expanduser("~"), ".fringes.yaml")
+        if os.path.isfile(fname):
+            self.fringes.load(fname)
+            self.update_parameter_tree()
+
         self.show()
         # self.fringes.logger.info(f"Started {myappid}.")
 
     def show(self):
         """Display the Application."""
         pg.exec()
         # if (sys.flags.interactive != 1) or not hasattr(QtCore, "PYQT_VERSION"):
```

### Comparing `fringes_gui-0.1.2/fringes_gui/logic.py` & `fringes_gui-0.1.3/fringes_gui/logic.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 from pyqtgraph.Qt import QtWidgets
 from PyQt6.QtWidgets import QFileDialog
 import pyqtgraph as pg
 import cv2
 import json
 import yaml
+import asdf
 import toml
 import fringes as frng
 
 
 config = {
-    ".toml": toml.load,
-    ".yml": yaml.safe_load,
-    ".yaml": yaml.safe_load,
     ".json": json.load,
+    ".yaml": yaml.safe_load,
+    ".toml": toml.load,
+    ".asdf": asdf.open,
 }
 
 image = {
     ".bmp": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     # ".dip": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),  # i.e. ".bmp"
     # ".jpeg": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
     # ".jpg": functools.partial(cv2.imread, flags=cv2.IMREAD_UNCHANGED),
@@ -66,17 +67,19 @@
         clear()
 
     def load():
         """Load data from given directory."""
 
         flist = QFileDialog.getOpenFileNames(
             caption="Select file(s)",
-            directory=os.path.join(os.path.expanduser("~"), "Videos"),
+            # directory=os.path.join(os.path.expanduser("~"), "Videos"),
             # options=QFileDialog.Option.DontUseNativeDialog,
-            filter=f"Images {tuple('*' + key for key in image.keys())};;Numpy {tuple('*' + key for key in numpy.keys())};;Config {tuple('*' + key for key in config.keys())}".replace(",", "").replace("'", "")
+            filter=f"Images {tuple('*' + key for key in image.keys())};;"
+                   f"Numpy {tuple('*' + key for key in numpy.keys())};;"
+                   f"Config {tuple('*' + key for key in config.keys())}".replace(",", "").replace("'", "")
         )
 
         if flist[0]:
             with pg.BusyCursor():
                 path, base = os.path.split(flist[0][0])
                 name, ext = os.path.splitext(base)
 
@@ -125,26 +128,26 @@
             gui.set_button.setEnabled(gui.set_dataOK)
 
     def save():
         """Save all data to current directory."""
 
         path = QFileDialog.getExistingDirectory(
             caption="Select directory",
-            directory=os.path.join(os.path.expanduser("~"), "Videos"),
+            # directory=os.path.join(os.path.expanduser("~"), "Videos"),
             # options=QFileDialog.Option.DontUseNativeDialog,
         )
 
         if os.path.isdir(os.path.abspath(path)):
             with pg.BusyCursor():
                 gui.fringes.save(os.path.join(path, "params.yaml"))
 
                 for k, v in gui.con.__dict__.items():
                     if isinstance(v, np.ndarray) and v.size > 0:
                         T, Y, X, C = v.shape = frng.vshape(v).shape
-                        color_order = (2, 1, 0, 3) if C == 4 else (2, 1, 0) if C == 3 else 0  # to compensate OpenCV color order
+                        color_order = (2, 1, 0, 3) if C == 4 else (2, 1, 0) if C == 3 else 0  # compensate OpenCV color order
                         color_channels = (1, 3, 4)
                         is_img_shape = v.ndim <= 2 or v.ndim == 3 and v.shape[-1] in color_channels
                         is_vid_shape = v.ndim == 3 or v.ndim == 4 and v.shape[-1] in color_channels
                         is_img_dtype = v.dtype in (bool, np.uint8, np.uint16) or \
                                        v.dtype in (np.float32,) and np.min(v) >= 0 and np.max(v) <= 1  # todo: np.float16, np.float64
 
                         if is_img_dtype and is_img_shape:  # save as image
@@ -201,14 +204,29 @@
                 gui.key = None
 
             gui.decode_button.setEnabled(gui.decodeOK)
             gui.decode_key.setEnabled(gui.decodeOK)
         except Exception:
             pass
 
+    def coordinates():
+        """Coordinates being encoded."""
+        if hasattr(gui.con, "coordinates"):
+            delattr(gui.con, "coordinates")
+
+        gui.data_table.setData(gui.con.info)
+        QtWidgets.QApplication.processEvents()  # refresh event queue
+
+        with pg.BusyCursor():
+            gui.con.coordinates = gui.fringes.coordinates()
+
+        view(getattr(gui.con, "coordinates").astype(float))
+        gui.data_table.setData(gui.con.info)
+        QtWidgets.QApplication.processEvents()  # refresh event queue
+
     def encode():
         """Encode fringes based on the given parameters."""
         if hasattr(gui.con, "fringes"):
             delattr(gui.con, "fringes")
 
         gui.data_table.setData(gui.con.info)
         QtWidgets.QApplication.processEvents()  # refresh event queue
@@ -440,14 +458,15 @@
     gui.clear_button.clicked.connect(clear)
     gui.clear_key.activated.connect(clear)
 
     gui.set_button.clicked.connect(set_data)
     gui.set_key.activated.connect(set_data)
     gui.data_table.itemSelectionChanged.connect(selection_changed)
 
+    gui.coordinates_key.activated.connect(coordinates)
     gui.encode_button.clicked.connect(encode)
     gui.encode_key.activated.connect(encode)
     gui.decode_button.clicked.connect(decode)
     gui.decode_key.activated.connect(decode)
 
     gui.remap_button.clicked.connect(remap)
     gui.remap_key.activated.connect(remap)
```

### Comparing `fringes_gui-0.1.2/fringes_gui/params.py` & `fringes_gui-0.1.3/fringes_gui/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             },
             {
                 "title": "alpha",
                 "name": "alpha",
                 "type": "float",
                 "value": gui.fringes.alpha,
                 "default": gui.fringes.defaults["alpha"],
-                "limits": (1, 2),
+                "limits": (1, gui.fringes._alphamax),
                 "step": 0.1,
                 "decimals": gui.digits,
                 "visible": gui.visibility == "Guru",
                 "tip": gui.fringes.__class__.alpha.__doc__,
             },
             {
                 "title": "Length",
@@ -132,15 +132,15 @@
                 },
                 {
                     "title": "Angle",
                     "name": "angle",
                     "type": "float",
                     "value": gui.fringes.angle,
                     "default": gui.fringes.defaults["angle"],
-                    "limits": (-360, 360),  # todo: +-45
+                    "limits": (-360, 360),
                     "decimals": gui.digits,
                     "suffix": "°",
                     "visible": gui.visibility == "Guru",
                     "tip": gui.fringes.__class__.angle.__doc__,
                 },
                 {
                     "title": "Directions",
@@ -190,15 +190,15 @@
                             "name": "N" + str(d).translate(gui.sub) + ", " + str(k).translate(gui.sub),
                             "type": "int",
                             "value": gui.fringes._N[d, k],
                             "default": gui.fringes.Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0],
                             "limits": (max(gui.fringes.Nmin, 1 if gui.visibility == "Guru" else 2 if gui.visibility == "Expert" else 3), gui.fringes._Nmax),
                             "tip": gui.fringes.__class__.N.__doc__,
                         } for d in range(gui.fringes.D) for k in range(gui.fringes.K)
-                    ] if gui.visibility == "Guru" or gui.fringes.N.ndim > 1 else [
+                    ] if gui.visibility == "Guru" or gui.fringes.N.ndim > 1 else [  # todo: FDM: N_i
                         {
                             "name": "N" + str(k).translate(gui.sub),
                             "type": "int",
                             "value": gui.fringes.N[k],
                             "default": gui.fringes.Nmin if gui.fringes.FDM else gui.fringes.defaults["N"][0, 0],
                             "limits": (max(gui.fringes.Nmin, 1 if gui.visibility == "Guru" else 2 if gui.visibility == "Expert" else 3), gui.fringes._Nmax),
                             "tip": gui.fringes.__class__.N.__doc__,
```

### Comparing `fringes_gui-0.1.2/fringes_gui/setters.py` & `fringes_gui-0.1.3/fringes_gui/setters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import numpy as np
 import pyqtgraph as pg
 from pyqtgraph.Qt import QtWidgets
 
 from .params import set_params
 from .logic import set_logic
 
@@ -9,15 +11,15 @@
 def set_functionality(gui):
     """Give the list of parameters defined in Gui their functionality, i.e. set listeners for when they are changed."""
 
     set_params(gui)
 
     gui.params = pg.parametertree.Parameter.create(name="Settings", type="group", children=gui.params)
     gui.tree.setParameters(gui.params, showTop=False)
-    gui.params_initial = gui.params.saveState()
+    # gui.params_initial = gui.params.saveState()
 
     set_logic(gui)
 
     vis = gui.visibility
     if gui.visibility != "Guru":
         gui.params.param("vis").setValue(
             "Guru")  # switching back from Guru mode prevents loading params which don't fit user options
@@ -30,15 +32,19 @@
 
         if change[0][1] != "value":
             return
 
         key = change[0][0].opts["name"]
         val = change[0][2]
 
-        if key not in ["mode", "verbose"] or \
+        if key in ["grid", "angle", "D"]:
+            if hasattr(gui.con, "coordinates"):
+                delattr(gui.con, "coordinates")
+
+        if key not in ["mode", "Vmin", "verbose"] or \
                 key == "axis" and gui.fringes.D == 2:
             if hasattr(gui.con, "fringes"):
                 delattr(gui.con, "fringes")
 
                 if hasattr(gui.con, "registration"):
                     gui.view(gui.con.registration)
                 elif hasattr(gui.con, gui.key):
@@ -120,23 +126,25 @@
                 val_old[:, k] = val
 
             val = val_old
         elif key == "o":
             val *= np.pi
 
         setattr(gui.fringes, key, val)
+        fname = os.path.join(os.path.expanduser("~"), ".fringes.yaml")
+        gui.fringes.save(fname)
 
         update_parameter_tree()
 
     def set_user(val):
         user_old = gui.visibility  # used if setting user to experimental
         gui.visibility = val
 
-        with gui.params.treeChangeBlocker():
-            if gui.visibility == "Beginner":
+        if gui.visibility == "Beginner":
+            with gui.params.treeChangeBlocker():
                 gui.params.param("vid", "T").setLimits((3, gui.fringes._Tmax))
                 gui.params.param("vid", "C").hide()
                 gui.params.param("vid", "alpha").hide()
                 gui.params.param("sys", "grid").setValue(gui.fringes.defaults["grid"])
                 gui.params.param("sys", "grid").hide()
                 gui.params.param("sys", "angle").setValue(gui.fringes.defaults["angle"])
                 gui.params.param("sys", "angle").hide()
@@ -167,15 +175,16 @@
                 gui.params.param("uwr", "mode").hide()
                 gui.params.param("uwr", "Vmin").setValue(gui.fringes.defaults["Vmin"])
                 gui.params.param("uwr", "Vmin").hide()
                 gui.params.param("uwr", "verbose").setValue(gui.fringes.defaults["verbose"])
                 gui.params.param("uwr", "verbose").hide()
                 gui.params.param("quali").hide()
                 gui.params.param("quali", "dark").setValue(gui.fringes.defaults["dark"])
-            elif gui.visibility == "Expert":
+        elif gui.visibility == "Expert":
+            with gui.params.treeChangeBlocker():
                 gui.params.param("vid", "T").setLimits((3, gui.fringes._Tmax))
                 gui.params.param("vid", "alpha").hide()
                 gui.params.param("sys", "grid").setValue(gui.fringes.defaults["grid"])
                 gui.params.param("sys", "grid").hide()
                 gui.params.param("sys", "angle").setValue(gui.fringes.defaults["angle"])
                 gui.params.param("sys", "angle").hide()
                 gui.fringes.N = np.maximum(gui.fringes._N, 2)
@@ -205,15 +214,16 @@
                 gui.params.param("uwr", "mode").hide()
                 gui.params.param("uwr", "Vmin").setValue(gui.fringes.defaults["Vmin"])
                 gui.params.param("uwr", "Vmin").hide()
                 gui.params.param("uwr", "verbose").show()
                 gui.params.param("quali").show()
                 gui.params.param("quali", "dark").hide()  # Experimental
                 gui.params.param("quali", "shot").hide()  # Experimental
-            elif gui.visibility == "Guru":
+        elif gui.visibility == "Guru":
+            with gui.params.treeChangeBlocker():
                 gui.params.param("vid", "T").setLimits((1, gui.fringes._Tmax))
                 gui.params.param("sys", "grid").setValue(gui.fringes.defaults["grid"])
                 gui.params.param("sys", "grid").hide()  # todo: experimantal -> guru
                 gui.params.param("sys", "angle").setValue(gui.fringes.defaults["angle"])
                 gui.params.param("sys", "angle").hide()  # todo: experimantal -> guru
                 gui.params.param("vid", "alpha").show()
                 gui.params.param("set", "K").setLimits((1, (gui.fringes._Nmax - 1) / 2 / gui.fringes.D if gui.fringes.FDM else gui.fringes._Kmax))
@@ -222,40 +232,44 @@
                 gui.params.param("val", "dtype").show()
                 gui.params.param("val", "Imax").show()
                 gui.params.param("col", "H").setLimits((1, gui.fringes._Hmax))
                 gui.params.param("col", "H").show()
                 gui.params.param("mux").show()
                 gui.params.param("col").show()
                 gui.params.param("uwr", "mode").setValue(gui.fringes.defaults["mode"])
-                gui.params.param("uwr", "mode").hide()
+                gui.params.param("uwr", "mode").hide()  # todo: experimantal -> guru
                 gui.params.param("uwr", "Vmin").setValue(gui.fringes.defaults["Vmin"])
-                gui.params.param("uwr", "Vmin").hide()
+                gui.params.param("uwr", "Vmin").hide()  # todo: experimantal -> guru
                 gui.params.param("quali").show()
-                gui.params.param("quali", "dark").hide()  # Experimental
-                gui.params.param("quali", "shot").hide()  # Experimental
-            elif gui.visibility == "Experimental":
-                if user_old not in ["Guru", "Experimental"]:
-                    gui.params.param("vis").setValue("Guru")  # get the settings from Guru mode first
-                    gui.params.param("vis").setValue("Experimental")
+                gui.params.param("quali", "dark").hide()  # todo: experimantal -> guru
+                gui.params.param("quali", "shot").hide()  # todo: experimantal -> guru
+        elif gui.visibility == "Experimental":
+            if user_old != "Guru":
+                gui.params.param("vis").setValue("Guru")  # get the settings from Guru mode first
+                gui.params.param("vis").setValue("Experimental")
+
+            with gui.params.treeChangeBlocker():
                 gui.params.param("sys", "grid").show()
                 gui.params.param("sys", "angle").show()
                 gui.params.param("uwr", "mode").show()
                 gui.params.param("uwr", "Vmin").show()
                 gui.params.param("quali", "dark").show()
                 gui.params.param("quali", "shot").show()
 
-            update_parameter_tree()
+        update_parameter_tree()
 
     def update_parameter_tree():
         is2D = max(gui.fringes.N.ndim, gui.fringes.l.ndim, gui.fringes.v.ndim, gui.fringes.f.ndim) == 2 or \
                gui.fringes.FDM or gui.visibility in ["Guru", "Experimental"]
 
         children = gui.fringes.D * gui.fringes.K if is2D else gui.fringes.K
+        children_N = gui.fringes.K if gui.fringes.FDM else gui.fringes.D * gui.fringes.K
 
-        change_indices = len(gui.params.param("set", "v").children()) != children or \
+        change_indices = len(gui.params.param("set", "N").children()) != children_N or \
+                         len(gui.params.param("set", "v").children()) != children or \
                          gui.fringes.D != gui.params.param("sys", "D").value() or \
                          gui.fringes.K != gui.params.param("set", "K").value() or \
                          gui.fringes.FDM != gui.params.param("mux", "FDM").value() or \
                          gui.params.param("vis").value() in ["Guru", "Experimental"] and \
                          "," not in gui.params.param("set", "v").children()[0].name() or \
                          gui.params.param("vis").value() not in ["Guru", "Experimental"] and \
                          "," in gui.params.param("set", "v").children()[0].name() or \
```

### Comparing `fringes_gui-0.1.2/fringes_gui/spirals.png` & `fringes_gui-0.1.3/fringes_gui/spirals.png`

 * *Files identical despite different names*

### Comparing `fringes_gui-0.1.2/pyproject.toml` & `fringes_gui-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "Fringes-GUI"
-version = "0.1.2"
+version = "0.1.3"
 description = "Graphical user interface for the 'fringes' package."
 license = "CC-BY-NC-SA-4.0"
 authors = ["Christian Kludt"]
 readme = "README.md"
 repository = "https://github.com/comimag/fringes-gui"
 keywords = ["phase shifting", "fringe analysis", "fringe projection", "deflectometry", "computational imaging"]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.11"
 opencv-contrib-python = "^4.7.0"
 pyyaml = "^6.0"
 scikit-image = "^0.19.3"
-fringes = "^0.1.5"  # {path = "../fringes", develop = true}
+fringes = "^0.1.6"
+ #fringes = {path = "../fringes", develop = true}
 pyqt6 = "^6.4.2"
 pyqtgraph = "^0.13.2"
 toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fringes_gui-0.1.2/README.md` & `fringes_gui-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```
 
 Now the graphical user interface should appear:
 
 ![Screenshot](docs/GUI.png)\
 Screenshot of the GUI.
 
-### Parameter Tree
+### Attributes
 In the top left corner the attribute widget is located.
 It contains the parameter tree with which all the properties of the `Fringes` class
 from the [fringes](https://pypi.org/project/fringes/) package can be controlled.
 Check out its website for more details.
 However, if you select a parameter and hover over it, a tool tip will appear
 containing the docstring of the respective property of the `Fringes` class.
 
@@ -48,15 +48,20 @@
   functionality. This is the preferred visibility level for all advanced features.
 - Guru:\
   Advanced features that usually only people with a sound background in phase shifting can make good use of.
 - Experimental:\
   New features that have not been tested yet
   and are likely to crash the system at some point.
 
-### Function Buttons
+Upon every parameter change, the complete parameter set of the `Fringes` instance is saved
+to the file `.fringes.yaml` in the user home directory.
+When the GUI starts again, the previous parameter set is loaded.
+To avoid this, just delete the config file or press the `reset` button in the `Methods` widget.
+
+### Methods
 In the bottem left corner you will find buttons for the associated methods of the `Fringes` class.
 Alternatively, you can use the keyboard shortcuts which are displayed when you hover over the buttons.
 The buttons are only active if the necessary data has been enoded, decoded or loaded.
 
 ### Viewer
 In the center resides the viewer.
 If float data is to be displayed, `nan` is replaced by zeros.
```

### Comparing `fringes_gui-0.1.2/setup.py` & `fringes_gui-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['fringes_gui']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fringes>=0.1.5,<0.2.0',
+['fringes>=0.1.6,<0.2.0',
  'opencv-contrib-python>=4.7.0,<5.0.0',
  'pyqt6>=6.4.2,<7.0.0',
  'pyqtgraph>=0.13.2,<0.14.0',
  'pyyaml>=6.0,<7.0',
  'scikit-image>=0.19.3,<0.20.0',
  'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'fringes-gui',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': "Graphical user interface for the 'fringes' package.",
-    'long_description': "# Fringes-GUI\nAuthor: Christian Kludt\n\n## Description\nGraphical user interface for the [fringes](https://pypi.org/project/fringes/) package.\n\n## Installation\nYou can install `fringes-gui` directly from [PyPi](https://pypi.org/project/fringes-gui) via `pip`:\n\n```\npip install fringes-gui\n```\n\n## Usage\nYou import the `fringes-gui` package and call the function `run()`.\n\n```python\nimport fringes_gui as fgui\nfgui.run()\n```\n\nNow the graphical user interface should appear:\n\n![Screenshot](docs/GUI.png)\\\nScreenshot of the GUI.\n\n### Parameter Tree\nIn the top left corner the attribute widget is located.\nIt contains the parameter tree with which all the properties of the `Fringes` class\nfrom the [fringes](https://pypi.org/project/fringes/) package can be controlled.\nCheck out its website for more details.\nHowever, if you select a parameter and hover over it, a tool tip will appear\ncontaining the docstring of the respective property of the `Fringes` class.\n\nThe Visibility defines the type of user that should get access to the feature.\nIt does not affect the functionality of the features but is used by the GUI to\ndecide which features to display based on the current user level. The purpose\nis mainly to ensure that the GUI is not cluttered with information that is not\nintended at the current visibility level. The following criteria have been used\nfor the assignment of the recommended visibility:\n- Beginner:\\\n  Features that should be visible for all users via the GUI. This\n  is the default visibility. The number of features with 'Beginner' visibility\n  should be limited to all basic features so the GUI display is well-organized\n  and easy to use.\n- Expert:\\\n  Features that require a more in-depth knowledge of the system\n  functionality. This is the preferred visibility level for all advanced features.\n- Guru:\\\n  Advanced features that usually only people with a sound background in phase shifting can make good use of.\n- Experimental:\\\n  New features that have not been tested yet\n  and are likely to crash the system at some point.\n\n### Function Buttons\nIn the bottem left corner you will find buttons for the associated methods of the `Fringes` class.\nAlternatively, you can use the keyboard shortcuts which are displayed when you hover over the buttons.\nThe buttons are only active if the necessary data has been enoded, decoded or loaded.\n\n### Viewer\nIn the center resides the viewer.\nIf float data is to be displayed, `nan` is replaced by zeros.\n\n### Data\nIn the top right corner the data widget is located.\nIt lists the data which has been encoded, decoded or was loaded.\n\nIn order to keep the [Parameter Tree](#parameter-tree) consistent with the data,\nonce a parameter has changed, certain data will be removed\nand also certain [buttons](#function-buttons) will be deactivated.\nAs a consequence, if you load data - e.g. the acquired (deflected) fringe pattern sequence - \nthe first element of its videoshape has to match the parameter `Frames` in order to be able to decode it.\n\nTo display any datum listed in the table in the [Viewer](#viewer), simly select the name of it in the table.\n\nKlick the `Load` button to choose a data or parameter set to load.\nWith the `Save` button, all data including the parameter set are saved to the selected directory.\nUse the `Clear all` button to delete all data.\n\nPlease note: By default, the datum `fringes` is decoded.\nIf you want to decode a datum with a different name (e.g. one that you just loaded),\nselect its name in the table and klick `Set data (to be decoded)`.\n\n### Log\nThe logging of the `Fringes` class is displayed here.\nThe logging level can be set in the [Parameter Tree](#parameter-tree).\n\n## License\nCreative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License\n",
+    'long_description': "# Fringes-GUI\nAuthor: Christian Kludt\n\n## Description\nGraphical user interface for the [fringes](https://pypi.org/project/fringes/) package.\n\n## Installation\nYou can install `fringes-gui` directly from [PyPi](https://pypi.org/project/fringes-gui) via `pip`:\n\n```\npip install fringes-gui\n```\n\n## Usage\nYou import the `fringes-gui` package and call the function `run()`.\n\n```python\nimport fringes_gui as fgui\nfgui.run()\n```\n\nNow the graphical user interface should appear:\n\n![Screenshot](docs/GUI.png)\\\nScreenshot of the GUI.\n\n### Attributes\nIn the top left corner the attribute widget is located.\nIt contains the parameter tree with which all the properties of the `Fringes` class\nfrom the [fringes](https://pypi.org/project/fringes/) package can be controlled.\nCheck out its website for more details.\nHowever, if you select a parameter and hover over it, a tool tip will appear\ncontaining the docstring of the respective property of the `Fringes` class.\n\nThe Visibility defines the type of user that should get access to the feature.\nIt does not affect the functionality of the features but is used by the GUI to\ndecide which features to display based on the current user level. The purpose\nis mainly to ensure that the GUI is not cluttered with information that is not\nintended at the current visibility level. The following criteria have been used\nfor the assignment of the recommended visibility:\n- Beginner:\\\n  Features that should be visible for all users via the GUI. This\n  is the default visibility. The number of features with 'Beginner' visibility\n  should be limited to all basic features so the GUI display is well-organized\n  and easy to use.\n- Expert:\\\n  Features that require a more in-depth knowledge of the system\n  functionality. This is the preferred visibility level for all advanced features.\n- Guru:\\\n  Advanced features that usually only people with a sound background in phase shifting can make good use of.\n- Experimental:\\\n  New features that have not been tested yet\n  and are likely to crash the system at some point.\n\nUpon every parameter change, the complete parameter set of the `Fringes` instance is saved\nto the file `.fringes.yaml` in the user home directory.\nWhen the GUI starts again, the previous parameter set is loaded.\nTo avoid this, just delete the config file or press the `reset` button in the `Methods` widget.\n\n### Methods\nIn the bottem left corner you will find buttons for the associated methods of the `Fringes` class.\nAlternatively, you can use the keyboard shortcuts which are displayed when you hover over the buttons.\nThe buttons are only active if the necessary data has been enoded, decoded or loaded.\n\n### Viewer\nIn the center resides the viewer.\nIf float data is to be displayed, `nan` is replaced by zeros.\n\n### Data\nIn the top right corner the data widget is located.\nIt lists the data which has been encoded, decoded or was loaded.\n\nIn order to keep the [Parameter Tree](#parameter-tree) consistent with the data,\nonce a parameter has changed, certain data will be removed\nand also certain [buttons](#function-buttons) will be deactivated.\nAs a consequence, if you load data - e.g. the acquired (deflected) fringe pattern sequence - \nthe first element of its videoshape has to match the parameter `Frames` in order to be able to decode it.\n\nTo display any datum listed in the table in the [Viewer](#viewer), simly select the name of it in the table.\n\nKlick the `Load` button to choose a data or parameter set to load.\nWith the `Save` button, all data including the parameter set are saved to the selected directory.\nUse the `Clear all` button to delete all data.\n\nPlease note: By default, the datum `fringes` is decoded.\nIf you want to decode a datum with a different name (e.g. one that you just loaded),\nselect its name in the table and klick `Set data (to be decoded)`.\n\n### Log\nThe logging of the `Fringes` class is displayed here.\nThe logging level can be set in the [Parameter Tree](#parameter-tree).\n\n## License\nCreative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License\n",
     'author': 'Christian Kludt',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/comimag/fringes-gui',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fringes_gui-0.1.2/PKG-INFO` & `fringes_gui-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fringes-gui
-Version: 0.1.2
+Version: 0.1.3
 Summary: Graphical user interface for the 'fringes' package.
 Home-page: https://github.com/comimag/fringes-gui
 License: CC-BY-NC-SA-4.0
 Keywords: phase shifting,fringe analysis,fringe projection,deflectometry,computational imaging
 Author: Christian Kludt
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: fringes (>=0.1.5,<0.2.0)
+Requires-Dist: fringes (>=0.1.6,<0.2.0)
 Requires-Dist: opencv-contrib-python (>=4.7.0,<5.0.0)
 Requires-Dist: pyqt6 (>=6.4.2,<7.0.0)
 Requires-Dist: pyqtgraph (>=0.13.2,<0.14.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/comimag/fringes-gui
@@ -42,15 +42,15 @@
 ```
 
 Now the graphical user interface should appear:
 
 ![Screenshot](docs/GUI.png)\
 Screenshot of the GUI.
 
-### Parameter Tree
+### Attributes
 In the top left corner the attribute widget is located.
 It contains the parameter tree with which all the properties of the `Fringes` class
 from the [fringes](https://pypi.org/project/fringes/) package can be controlled.
 Check out its website for more details.
 However, if you select a parameter and hover over it, a tool tip will appear
 containing the docstring of the respective property of the `Fringes` class.
 
@@ -70,15 +70,20 @@
   functionality. This is the preferred visibility level for all advanced features.
 - Guru:\
   Advanced features that usually only people with a sound background in phase shifting can make good use of.
 - Experimental:\
   New features that have not been tested yet
   and are likely to crash the system at some point.
 
-### Function Buttons
+Upon every parameter change, the complete parameter set of the `Fringes` instance is saved
+to the file `.fringes.yaml` in the user home directory.
+When the GUI starts again, the previous parameter set is loaded.
+To avoid this, just delete the config file or press the `reset` button in the `Methods` widget.
+
+### Methods
 In the bottem left corner you will find buttons for the associated methods of the `Fringes` class.
 Alternatively, you can use the keyboard shortcuts which are displayed when you hover over the buttons.
 The buttons are only active if the necessary data has been enoded, decoded or loaded.
 
 ### Viewer
 In the center resides the viewer.
 If float data is to be displayed, `nan` is replaced by zeros.
```

