# Comparing `tmp/sv_ttk-2.4.3.tar.gz` & `tmp/sv_ttk-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sv_ttk-2.4.3.tar", last modified: Wed Mar 29 23:00:16 2023, max compression
+gzip compressed data, was "sv_ttk-2.4.4.tar", last modified: Fri Apr 21 21:37:41 2023, max compression
```

## Comparing `sv_ttk-2.4.3.tar` & `sv_ttk-2.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:16.208026 sv_ttk-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-29 23:00:07.000000 sv_ttk-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-29 23:00:16.208026 sv_ttk-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-29 23:00:07.000000 sv_ttk-2.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 23:00:16.208026 sv_ttk-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-29 23:00:07.000000 sv_ttk-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:16.204026 sv_ttk-2.4.3/sv_ttk/
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-29 23:00:15.000000 sv_ttk-2.4.3/sv_ttk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-03-29 23:00:15.000000 sv_ttk-2.4.3/sv_ttk/sv.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:16.208026 sv_ttk-2.4.3/sv_ttk/theme/
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-03-29 23:00:15.000000 sv_ttk-2.4.3/sv_ttk/theme/dark.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-03-29 23:00:15.000000 sv_ttk-2.4.3/sv_ttk/theme/light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-29 23:00:15.000000 sv_ttk-2.4.3/sv_ttk/theme/sprites_dark.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-03-29 23:00:15.000000 sv_ttk-2.4.3/sv_ttk/theme/sprites_light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-03-29 23:00:15.000000 sv_ttk-2.4.3/sv_ttk/theme/spritesheet_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-03-29 23:00:15.000000 sv_ttk-2.4.3/sv_ttk/theme/spritesheet_light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:16.208026 sv_ttk-2.4.3/sv_ttk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-29 23:00:16.000000 sv_ttk-2.4.3/sv_ttk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-29 23:00:16.000000 sv_ttk-2.4.3/sv_ttk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 23:00:16.000000 sv_ttk-2.4.3/sv_ttk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-29 23:00:16.000000 sv_ttk-2.4.3/sv_ttk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:37:41.045469 sv_ttk-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-21 21:37:30.000000 sv_ttk-2.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 21:37:41.045469 sv_ttk-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-21 21:37:30.000000 sv_ttk-2.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:37:41.045469 sv_ttk-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-21 21:37:30.000000 sv_ttk-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:37:41.045469 sv_ttk-2.4.4/sv_ttk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-21 21:37:40.000000 sv_ttk-2.4.4/sv_ttk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-21 21:37:40.000000 sv_ttk-2.4.4/sv_ttk/sv.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:37:41.045469 sv_ttk-2.4.4/sv_ttk/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-04-21 21:37:40.000000 sv_ttk-2.4.4/sv_ttk/theme/dark.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-04-21 21:37:40.000000 sv_ttk-2.4.4/sv_ttk/theme/light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-21 21:37:40.000000 sv_ttk-2.4.4/sv_ttk/theme/sprites_dark.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-21 21:37:40.000000 sv_ttk-2.4.4/sv_ttk/theme/sprites_light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-04-21 21:37:40.000000 sv_ttk-2.4.4/sv_ttk/theme/spritesheet_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-04-21 21:37:40.000000 sv_ttk-2.4.4/sv_ttk/theme/spritesheet_light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:37:41.045469 sv_ttk-2.4.4/sv_ttk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 21:37:41.000000 sv_ttk-2.4.4/sv_ttk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-21 21:37:41.000000 sv_ttk-2.4.4/sv_ttk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:37:41.000000 sv_ttk-2.4.4/sv_ttk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 21:37:41.000000 sv_ttk-2.4.4/sv_ttk.egg-info/top_level.txt
```

### Comparing `sv_ttk-2.4.3/LICENSE` & `sv_ttk-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.4.3/PKG-INFO` & `sv_ttk-2.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sv_ttk
-Version: 2.4.3
+Version: 2.4.4
 Summary: A gorgeous theme for Tkinter, based on Windows 11's UI
 Home-page: https://github.com/rdbende/Sun-Valley-ttk-theme
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/rdbende/Sun-Valley-ttk-theme
 Project-URL: Documentation, https://github.com/rdbende/Sun-Valley-ttk-theme/wiki
@@ -35,14 +35,18 @@
 
 ```
 pip install sv-ttk
 ```
 
 
 ### Usage
+❕**Note:**
+_The theme will only work with themable (`tkinter.ttk`) widgets, and not with plain Tkinter widgets, these will only get the colorscheme.
+Please don't open issues about the theme not working with plain Tkinter widgets._
+
 For detailed documentation, see the [wiki page](https://github.com/rdbende/Sun-Valley-ttk-theme/wiki/Usage-with-Python)
 
 ```python
 import tkinter
 from tkinter import ttk
 
 import sv_ttk
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sv_ttk-2.4.3/README.md` & `sv_ttk-2.4.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 ```
 pip install sv-ttk
 ```
 
 
 ### Usage
+❕**Note:**
+_The theme will only work with themable (`tkinter.ttk`) widgets, and not with plain Tkinter widgets, these will only get the colorscheme.
+Please don't open issues about the theme not working with plain Tkinter widgets._
+
 For detailed documentation, see the [wiki page](https://github.com/rdbende/Sun-Valley-ttk-theme/wiki/Usage-with-Python)
 
 ```python
 import tkinter
 from tkinter import ttk
 
 import sv_ttk
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sv_ttk-2.4.3/setup.py` & `sv_ttk-2.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         '<img alt="Cover image" src="https://raw.githubusercontent.com/rdbende/Sun-Valley-ttk-theme/master/assets/hero_light.png">',
         file.read(),
     )
 
 
 setup(
     name="sv_ttk",
-    version="2.4.3",
+    version="2.4.4",
     license="MIT",
     author="rdbende",
     author_email="rdbende@gmail.com",
     url="https://github.com/rdbende/Sun-Valley-ttk-theme",
     project_urls={
         "Source": "https://github.com/rdbende/Sun-Valley-ttk-theme",
         "Documentation": "https://github.com/rdbende/Sun-Valley-ttk-theme/wiki",
```

### Comparing `sv_ttk-2.4.3/sv_ttk/__init__.py` & `sv_ttk-2.4.4/sv_ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.4.3/sv_ttk/sv.tcl` & `sv_ttk-2.4.4/sv_ttk/sv.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.4.3/sv_ttk/theme/dark.tcl` & `sv_ttk-2.4.4/sv_ttk/theme/dark.tcl`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       Button.button -children {
         Button.padding -children {
           Button.label -side left -expand 1
         } 
       }
     }
 
-    ttk::style configure TButton -padding {8 2 8 3} -anchor center -foreground $theme_colors(-fg) -width 12
+    ttk::style configure TButton -padding {8 2 8 3} -anchor center -foreground $theme_colors(-fg)
     ttk::style map TButton -foreground [list disabled "#7a7a7a" pressed "#d0d0d0"]
     
     ttk::style element create Button.button image \
       [list $I(button-rest) \
         {selected disabled} $I(button-dis) \
         disabled $I(button-dis) \
         selected $I(button-rest) \
@@ -53,15 +53,15 @@
       Toolbutton.button -children {
         Toolbutton.padding -children {
           Toolbutton.label -side left -expand 1
         } 
       }
     }
 
-    ttk::style configure Toolbutton -padding {8 2 8 3} -anchor center -width 12
+    ttk::style configure Toolbutton -padding {8 2 8 3} -anchor center
     
     ttk::style element create Toolbutton.button image \
       [list $I(empty) \
         disabled $I(button-dis) \
         pressed $I(button-pressed) \
         {active focus} $I(button-focus-hover) \
         active $I(button-hover) \
@@ -97,15 +97,15 @@
         Menubutton.padding -children {
           Menubutton.label -side left -expand 1
           Menubutton.indicator -side right -sticky nsew
         }
       }
     }
 
-    ttk::style configure TMenubutton -padding {8 2 13 3} -width 10
+    ttk::style configure TMenubutton -padding {8 2 13 3}
 
     ttk::style element create Menubutton.button image \
       [list $I(button-rest) \
         disabled $I(button-dis) \
         pressed $I(button-pressed) \
         {active focus} $I(button-focus-hover) \
         active $I(button-hover) \
@@ -120,15 +120,15 @@
         OptionMenu.padding -children {
           OptionMenu.label -side left -expand 1
           OptionMenu.indicator -side right -sticky nsew
         }
       }
     }
     
-    ttk::style configure TOptionMenu -padding {8 2 13 3} -width 10
+    ttk::style configure TOptionMenu -padding {8 2 13 3}
 
     ttk::style element create OptionMenu.button image \
       [list $I(button-rest) \
         disabled $I(button-dis) \
         pressed $I(button-pressed) \
         {active focus} $I(button-focus-hover) \
         active $I(button-hover) \
```

### Comparing `sv_ttk-2.4.3/sv_ttk/theme/light.tcl` & `sv_ttk-2.4.4/sv_ttk/theme/light.tcl`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       Button.button -children {
         Button.padding -children {
           Button.label -side left -expand 1
         } 
       }
     }
 
-    ttk::style configure TButton -padding {8 2 8 3} -anchor center -foreground $theme_colors(-fg) -width 12
+    ttk::style configure TButton -padding {8 2 8 3} -anchor center -foreground $theme_colors(-fg)
     ttk::style map TButton -foreground [list disabled "#a2a2a2" pressed "#636363" active "#1a1a1a"]
     
     ttk::style element create Button.button image \
       [list $I(button-rest) \
         {selected disabled} $I(button-dis) \
         disabled $I(button-dis) \
         selected $I(button-rest) \
@@ -53,15 +53,15 @@
       Toolbutton.button -children {
         Toolbutton.padding -children {
           Toolbutton.label -side left -expand 1
         } 
       }
     }
 
-    ttk::style configure Toolbutton -padding {8 2 8 3} -anchor center -width 12
+    ttk::style configure Toolbutton -padding {8 2 8 3} -anchor center
     
     ttk::style element create Toolbutton.button image \
       [list $I(empty) \
         disabled $I(button-dis) \
         pressed $I(button-pressed) \
         {active focus} $I(button-focus-hover) \
         active $I(button-hover) \
@@ -97,15 +97,15 @@
         Menubutton.padding -children {
           Menubutton.label -side left -expand 1
           Menubutton.indicator -side right -sticky nsew
         }
       }
     }
 
-    ttk::style configure TMenubutton -padding {8 2 13 3} -width 10
+    ttk::style configure TMenubutton -padding {8 2 13 3}
 
     ttk::style element create Menubutton.button image \
       [list $I(button-rest) \
         disabled $I(button-dis) \
         pressed $I(button-pressed) \
         {active focus} $I(button-focus-hover) \
         active $I(button-hover) \
@@ -120,15 +120,15 @@
         OptionMenu.padding -children {
           OptionMenu.label -side left -expand 1
           OptionMenu.indicator -side right -sticky nsew
         }
       }
     }
     
-    ttk::style configure TOptionMenu -padding {8 2 13 3} -width 10
+    ttk::style configure TOptionMenu -padding {8 2 13 3}
 
     ttk::style element create OptionMenu.button image \
       [list $I(button-rest) \
         disabled $I(button-dis) \
         pressed $I(button-pressed) \
         {active focus} $I(button-focus-hover) \
         active $I(button-hover) \
```

### Comparing `sv_ttk-2.4.3/sv_ttk/theme/sprites_dark.tcl` & `sv_ttk-2.4.4/sv_ttk/theme/sprites_dark.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.4.3/sv_ttk/theme/sprites_light.tcl` & `sv_ttk-2.4.4/sv_ttk/theme/sprites_light.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.4.3/sv_ttk/theme/spritesheet_dark.png` & `sv_ttk-2.4.4/sv_ttk/theme/spritesheet_dark.png`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.4.3/sv_ttk/theme/spritesheet_light.png` & `sv_ttk-2.4.4/sv_ttk/theme/spritesheet_light.png`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.4.3/sv_ttk.egg-info/PKG-INFO` & `sv_ttk-2.4.4/sv_ttk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sv-ttk
-Version: 2.4.3
+Version: 2.4.4
 Summary: A gorgeous theme for Tkinter, based on Windows 11's UI
 Home-page: https://github.com/rdbende/Sun-Valley-ttk-theme
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/rdbende/Sun-Valley-ttk-theme
 Project-URL: Documentation, https://github.com/rdbende/Sun-Valley-ttk-theme/wiki
@@ -35,14 +35,18 @@
 
 ```
 pip install sv-ttk
 ```
 
 
 ### Usage
+❕**Note:**
+_The theme will only work with themable (`tkinter.ttk`) widgets, and not with plain Tkinter widgets, these will only get the colorscheme.
+Please don't open issues about the theme not working with plain Tkinter widgets._
+
 For detailed documentation, see the [wiki page](https://github.com/rdbende/Sun-Valley-ttk-theme/wiki/Usage-with-Python)
 
 ```python
 import tkinter
 from tkinter import ttk
 
 import sv_ttk
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

