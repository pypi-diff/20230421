# Comparing `tmp/wbpFonttools-0.1.7.tar.gz` & `tmp/wbpFonttools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpFonttools-0.1.7.tar", last modified: Mon Apr 10 06:10:14 2023, max compression
+gzip compressed data, was "wbpFonttools-0.1.8.tar", last modified: Fri Apr 21 13:01:40 2023, max compression
```

## Comparing `wbpFonttools-0.1.7.tar` & `wbpFonttools-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 06:10:14.269726 wbpFonttools-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 06:10:14.262725 wbpFonttools-0.1.7/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 06:10:14.267726 wbpFonttools-0.1.7/Lib/wbpFonttools/
--rw-rw-rw-   0 root         (0) root         (0)     1630 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4895 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6687 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/control.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/selectFontsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2955 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/template.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/view.py
--rw-rw-rw-   0 root         (0) root         (0)    12103 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/window.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/Lib/wbpFonttools/windowUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 06:10:14.269726 wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1955 2023-04-10 06:10:14.000000 wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      594 2023-04-10 06:10:14.000000 wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 06:10:14.000000 wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-10 06:10:14.000000 wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-10 06:10:14.000000 wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 06:10:14.000000 wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1955 2023-04-10 06:10:14.269726 wbpFonttools-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-10 06:10:14.270726 wbpFonttools-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-10 06:10:12.000000 wbpFonttools-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:01:40.662122 wbpFonttools-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:01:40.655121 wbpFonttools-0.1.8/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:01:40.660122 wbpFonttools-0.1.8/Lib/wbpFonttools/
+-rw-rw-rw-   0 root         (0) root         (0)     1684 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4895 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6779 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/control.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/selectFontsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2332 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    12103 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/window.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/windowUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:01:40.662122 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      594 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-04-21 13:01:40.662122 wbpFonttools-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-04-21 13:01:40.663122 wbpFonttools-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/setup.py
```

### Comparing `wbpFonttools-0.1.7/LICENSE` & `wbpFonttools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/__init__.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 import wx
 
 from .config import FonttoolsPreferences, ObjectViewPreferences, XmlViewPreferences
 from .dialog import SelectFontsDialog
 from .document import FontToolsDocument
 from .template import (
     OpenType_OTF_Template,
+    OpenType_TTC_Template,
     OpenType_TTF_Template,
     WebFont_WOFF_2_Template,
     WebFont_WOFF_Template,
 )
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
     from .document import TTFont
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 
 def CurrentFont() -> Optional[TTFont]:
     """
     Get the currently active font
     """
     app: App = wx.GetApp()
@@ -50,16 +51,17 @@
     with SelectFontsDialog(message) as dlg:
         if dlg.ShowModal() == wx.ID_OK:
             fonts = dlg.selectedFonts
     return fonts
 
 
 doctemplates = (
-    OpenType_TTF_Template,
     OpenType_OTF_Template,
-    WebFont_WOFF_Template,
+    OpenType_TTC_Template,
+    OpenType_TTF_Template,
     WebFont_WOFF_2_Template,
+    WebFont_WOFF_Template,
 )
 
 preferencepages = (FonttoolsPreferences, XmlViewPreferences, ObjectViewPreferences)
 
 globalObjects = ("CurrentFont", "AllFonts", "SelectFonts")
```

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/config.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/config.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/control.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,24 @@
     from .window import FontToolsWindow
 
 
 class FontTableListCrtl(wx.ListCtrl, ListCtrlAutoWidthMixin):
     """
     List control to show all table tags of a font.
     """
+
     def __init__(
         self,
-        parent:wx.Window,
-        id:int=wx.ID_ANY,
+        parent: wx.Window,
+        id: int = wx.ID_ANY,
         pos=wx.DefaultPosition,
-        size:wx.Size=wx.DefaultSize,
-        style:int=wx.LC_REPORT | wx.LC_SINGLE_SEL | wx.LC_VIRTUAL,
-        validator:wx.Validator=wx.DefaultValidator,
-        name:str="TTXtableListCrtl",
+        size: wx.Size = wx.DefaultSize,
+        style: int = wx.LC_REPORT | wx.LC_SINGLE_SEL | wx.LC_VIRTUAL,
+        validator: wx.Validator = wx.DefaultValidator,
+        name: str = "TTXtableListCrtl",
     ):
         wx.ListCtrl.__init__(self, parent, id, pos, size, style, validator, name)
         ListCtrlAutoWidthMixin.__init__(self)
         self.Parent: FontToolsWindow
         imgSize = 16
         self.imglist = wx.ImageList(imgSize, imgSize)
         self.imgDefault = self.imglist.Add(
@@ -59,15 +60,15 @@
         self.InsertColumn(0, "Table")
         self.SetItemCount(0)
 
     @property
     def font(self) -> TTFont:
         return self.Parent.document.font
 
-    def OnGetItemText(self, item:int, col:int) -> str:
+    def OnGetItemText(self, item: int, col: int) -> str:
         """
         :return: table tag of the specified item
         """
         return self.font.keys()[item]
 
     def OnGetItemImage(self, item) -> int:
         """
@@ -162,19 +163,21 @@
     def __init__(self, numFonts):
         parent = wx.GetApp().TopWindow
         id = wx.ID_ANY
         title = "Open TrueType Collection"
         pos = wx.DefaultPosition
         size = wx.DefaultSize
         style = wx.CAPTION | wx.RESIZE_BORDER
-        message = f"""This Font Collection contains {numFonts} fonts.
-Please specify the font you want to open.
-Enter a font number between 0 and {numFonts - 1} (inclusive).""" 
+        message = (
+            f"This Font Collection contains {numFonts} fonts.\n"
+            + "Please specify the font you want to open.\n"
+            + f"Enter a font number between 0 and {numFonts - 1} (inclusive)."
+        )
         wx.Dialog.__init__(self, parent, id, title, pos, size, style)
-        self.SetSizeHintsSz(wx.DefaultSize, wx.DefaultSize)
+        self.SetSizeHints(wx.DefaultSize, wx.DefaultSize)
         sizer = wx.BoxSizer(wx.VERTICAL)
         self.lbl_Message = wx.StaticText(
             self, wx.ID_ANY, message, wx.DefaultPosition, wx.DefaultSize, 0
         )
         self.lbl_Message.Wrap(-1)
         sizer.Add(self.lbl_Message, 0, wx.ALL | wx.EXPAND, 5)
         self.spinCtrl_fontNumber = wx.SpinCtrl(
@@ -185,30 +188,31 @@
             wx.DefaultSize,
             wx.SP_ARROW_KEYS | wx.SP_WRAP,
             0,
             numFonts - 1,
             0,
         )
         sizer.Add(self.spinCtrl_fontNumber, 0, wx.ALL, 5)
-        sizer.AddSpacer((0, 0), 1, wx.EXPAND, 5)
+        sizer.Add((0, 0), 1, wx.EXPAND, 5)
         sdbSizer = wx.StdDialogButtonSizer()
         self.sdbSizerOK = wx.Button(self, wx.ID_OK)
         sdbSizer.AddButton(self.sdbSizerOK)
         # self.sdbSizerCancel = wx.Button(self, wx.ID_CANCEL)
         # sdbSizer.AddButton(self.sdbSizerCancel)
         sdbSizer.Realize()
         sdbSizer.SetMinSize(wx.Size(10, -1))
         sizer.Add(sdbSizer, 0, wx.ALL | wx.EXPAND, 5)
         self.SetSizer(sizer)
         self.Layout()
+        sizer.Fit(self)
         self.Centre(wx.BOTH)
 
     @property
     def fontNumber(self):
         return int(self.spinCtrl_fontNumber.Value)
 
 
-def getFontNumber(numFonts:int) -> int:
+def getFontNumber(numFonts: int) -> int:
     with DlgFontNumber(numFonts) as dlg:
         if dlg.ShowModal() == wx.ID_OK:
             return dlg.fontNumber
     return -1
```

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/dialog.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/dialog.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/document.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/document.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/selectFontsDialogUI.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/selectFontsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/template.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,7 +99,17 @@
     "OpenType-WOFF-2 WebFont"
     def __init__(self, manager: DocumentManager):
         description = "OpenType-WOFF-2 WebFont"
         filter = "*.woff2"
         dir = ""
         ext = ".woff2"
         FontToolsTemplate.__init__(self, manager, description, filter, dir, ext)
+
+
+class OpenType_TTC_Template(FontToolsTemplate):
+    "OpenType-TTC Collection"
+    def __init__(self, manager: DocumentManager):
+        description = "OpenType-TTC Collection"
+        filter = "*.ttc"
+        dir = ""
+        ext = ".ttc"
+        FontToolsTemplate.__init__(self, manager, description, filter, dir, ext)
```

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/tools.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/tools.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/view.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/view.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/window.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/window.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools/windowUI.py` & `wbpFonttools-0.1.8/Lib/wbpFonttools/windowUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/PKG-INFO` & `wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.1.7
+Version: 0.1.8
 Summary: FontTools font editor for Workbench applications.
+Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
+Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
+Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
+Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +33,15 @@
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpFonttools
 
-FontTools plugin for Workbench applications.
+FontTools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
 
 This plugin provides Workbench document templates for the following font formats:
 - OpenType-TTF Font
 - OpenType-OTF Font
 - OpenType-WOFF WebFont
 - OpenType-WOFF-2 WebFont
 
@@ -50,17 +54,17 @@
 pip install wbpFonttools
 ```
 
 Installing this plugin registers an entry point 
 in the group "*wbbase.plugin*" named "*fonttools*".
 
 To use the plugin in your application, 
-add it to your *application.yaml* file as follows:
+add it to your *application.yml* file as follows:
 ```yaml
 AppName: myApp
 Plugins:
 - Name: fonttools
 ```
 
 ## Documentation
 
-For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpFonttools/).
+For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpfonttools).
```

### Comparing `wbpFonttools-0.1.7/Lib/wbpFonttools.egg-info/SOURCES.txt` & `wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.7/PKG-INFO` & `wbpFonttools-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.1.7
+Version: 0.1.8
 Summary: FontTools font editor for Workbench applications.
+Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
+Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
+Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
+Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +33,15 @@
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpFonttools
 
-FontTools plugin for Workbench applications.
+FontTools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
 
 This plugin provides Workbench document templates for the following font formats:
 - OpenType-TTF Font
 - OpenType-OTF Font
 - OpenType-WOFF WebFont
 - OpenType-WOFF-2 WebFont
 
@@ -50,17 +54,17 @@
 pip install wbpFonttools
 ```
 
 Installing this plugin registers an entry point 
 in the group "*wbbase.plugin*" named "*fonttools*".
 
 To use the plugin in your application, 
-add it to your *application.yaml* file as follows:
+add it to your *application.yml* file as follows:
 ```yaml
 AppName: myApp
 Plugins:
 - Name: fonttools
 ```
 
 ## Documentation
 
-For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpFonttools/).
+For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpfonttools).
```

### Comparing `wbpFonttools-0.1.7/README.md` & `wbpFonttools-0.1.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # wbpFonttools
 
-FontTools plugin for Workbench applications.
+FontTools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
 
 This plugin provides Workbench document templates for the following font formats:
 - OpenType-TTF Font
 - OpenType-OTF Font
 - OpenType-WOFF WebFont
 - OpenType-WOFF-2 WebFont
 
@@ -17,17 +17,17 @@
 pip install wbpFonttools
 ```
 
 Installing this plugin registers an entry point 
 in the group "*wbbase.plugin*" named "*fonttools*".
 
 To use the plugin in your application, 
-add it to your *application.yaml* file as follows:
+add it to your *application.yml* file as follows:
 ```yaml
 AppName: myApp
 Plugins:
 - Name: fonttools
 ```
 
 ## Documentation
 
-For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpFonttools/).
+For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpfonttools).
```

### Comparing `wbpFonttools-0.1.7/setup.cfg` & `wbpFonttools-0.1.8/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.7
+current_version = 0.1.8
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -12,14 +12,19 @@
 version = attr: wbpFonttools.__version__
 author = Andreas Eigendorf
 description = FontTools font editor for Workbench applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
+url = https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
+project_urls = 
+	Source = https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
+	Documentation = https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
+	Tracker = https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
 platforms = 
 	WIN32
 	WIN64
 	OSX
 	POSIX
 keywords = 
 	workbench
```

