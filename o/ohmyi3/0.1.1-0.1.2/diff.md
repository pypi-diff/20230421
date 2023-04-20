# Comparing `tmp/ohmyi3-0.1.1.tar.gz` & `tmp/ohmyi3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmyi3-0.1.1.tar", max compression
+gzip compressed data, was "ohmyi3-0.1.2.tar", max compression
```

## Comparing `ohmyi3-0.1.1.tar` & `ohmyi3-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0     1082 2023-04-15 19:45:51.088364 ohmyi3-0.1.1/LICENSE
--rw-r--r--   0        0        0       43 2023-04-15 22:50:07.408756 ohmyi3-0.1.1/README.md
--rw-r--r--   0        0        0     1659 2023-04-16 19:21:21.603562 ohmyi3-0.1.1/ohmyi3/app.py
--rw-r--r--   0        0        0     1131 2023-04-16 01:52:38.895592 ohmyi3-0.1.1/ohmyi3/commands/entrypoint.py
--rw-r--r--   0        0        0     2867 2023-04-16 19:17:23.069039 ohmyi3-0.1.1/ohmyi3/commands/generate.py
--rw-r--r--   0        0        0      582 2023-04-16 19:17:41.632714 ohmyi3-0.1.1/ohmyi3/commands/info.py
--rw-r--r--   0        0        0     1221 2023-04-16 19:02:29.594220 ohmyi3-0.1.1/ohmyi3/commands/init.py
--rw-r--r--   0        0        0      591 2023-04-16 02:01:06.406276 ohmyi3-0.1.1/ohmyi3/config/app.py
--rw-r--r--   0        0        0     2384 2023-04-16 05:45:45.284535 ohmyi3-0.1.1/ohmyi3/config/package.py
--rw-r--r--   0        0        0     1141 2023-04-16 19:18:58.080807 ohmyi3-0.1.1/ohmyi3/configurator.py
--rw-r--r--   0        0        0      814 2023-04-15 19:45:51.085030 ohmyi3-0.1.1/ohmyi3/services/bootstrap.py
--rw-r--r--   0        0        0     2529 2023-04-16 19:40:39.743720 ohmyi3-0.1.1/ohmyi3/services/ohmyi3.py
--rw-r--r--   0        0        0      188 2023-04-16 20:00:12.022854 ohmyi3-0.1.1/ohmyi3/stubs/README.md
--rw-r--r--   0        0        0      810 2023-04-16 19:50:22.554902 ohmyi3-0.1.1/ohmyi3/stubs/config.d/00-header.conf
--rw-r--r--   0        0        0     1734 2023-04-16 19:50:22.558236 ohmyi3-0.1.1/ohmyi3/stubs/config.d/05-system.conf
--rw-r--r--   0        0        0     2014 2023-04-16 19:50:22.561569 ohmyi3-0.1.1/ohmyi3/stubs/config.d/10-autostart.conf
--rw-r--r--   0        0        0      552 2023-04-16 19:50:22.561569 ohmyi3-0.1.1/ohmyi3/stubs/config.d/15-borders.conf
--rw-r--r--   0        0        0     6209 2023-04-16 19:50:22.564903 ohmyi3-0.1.1/ohmyi3/stubs/config.d/20-navigation.conf
--rw-r--r--   0        0        0     2962 2023-04-16 19:50:22.564903 ohmyi3-0.1.1/ohmyi3/stubs/config.d/80-applications.conf
--rw-r--r--   0        0        0     6686 2023-04-16 19:50:22.568236 ohmyi3-0.1.1/ohmyi3/stubs/config.d/85-windows.conf
--rw-r--r--   0        0        0     3141 2023-04-16 19:50:22.571569 ohmyi3-0.1.1/ohmyi3/stubs/config.d/90-gaps.conf
--rw-r--r--   0        0        0     6361 2023-04-16 19:57:35.033223 ohmyi3-0.1.1/ohmyi3/stubs/configurator.py
--rw-r--r--   0        0        0       29 2023-04-16 19:50:30.758322 ohmyi3-0.1.1/ohmyi3/stubs/plugins/archey3/__init__.py
--rw-r--r--   0        0        0      962 2023-04-16 19:50:30.761655 ohmyi3-0.1.1/ohmyi3/stubs/plugins/archey3/archey3.py
--rw-r--r--   0        0        0       31 2023-04-16 19:50:30.761655 ohmyi3-0.1.1/ohmyi3/stubs/plugins/nitrogen/__init__.py
--rw-r--r--   0        0        0     1607 2023-04-16 19:50:30.764989 ohmyi3-0.1.1/ohmyi3/stubs/plugins/nitrogen/nitrogen.py
--rw-r--r--   0        0        0   385109 2023-04-16 19:50:38.535071 ohmyi3-0.1.1/ohmyi3/stubs/themes/amber/background.jpg
--rw-r--r--   0        0        0     1841 2023-04-16 19:50:38.535071 ohmyi3-0.1.1/ohmyi3/stubs/themes/amber/theme.conf
--rw-r--r--   0        0        0   198158 2023-04-16 19:50:38.538404 ohmyi3-0.1.1/ohmyi3/stubs/themes/archlinux/background.jpg
--rw-r--r--   0        0        0     1882 2023-04-16 19:50:38.541738 ohmyi3-0.1.1/ohmyi3/stubs/themes/archlinux/theme.conf
--rw-r--r--   0        0        0     1869 2023-04-16 19:50:38.541738 ohmyi3-0.1.1/ohmyi3/stubs/themes/i3status.conf
--rw-r--r--   0        0        0   108928 2023-04-16 19:50:38.545071 ohmyi3-0.1.1/ohmyi3/stubs/themes/manjaro/background.jpg
--rw-r--r--   0        0        0     1901 2023-04-16 19:50:38.545071 ohmyi3-0.1.1/ohmyi3/stubs/themes/manjaro/theme.conf
--rw-r--r--   0        0        0   514555 2023-04-16 19:50:38.548405 ohmyi3-0.1.1/ohmyi3/stubs/themes/pink/background.jpg
--rw-r--r--   0        0        0     2389 2023-04-16 19:50:38.548405 ohmyi3-0.1.1/ohmyi3/stubs/themes/pink/theme.conf
--rw-r--r--   0        0        0     1660 2023-04-16 19:32:43.375019 ohmyi3-0.1.1/ohmyi3/util.py
--rw-r--r--   0        0        0      703 2023-04-16 20:01:27.091497 ohmyi3-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 ohmyi3-0.1.1/setup.py
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 ohmyi3-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-15 19:45:51.088364 ohmyi3-0.1.2/LICENSE
+-rw-r--r--   0        0        0       43 2023-04-15 22:50:07.408756 ohmyi3-0.1.2/README.md
+-rw-r--r--   0        0        0     1131 2023-04-16 01:52:38.895592 ohmyi3-0.1.2/ohmyi3/commands/entrypoint.py
+-rw-r--r--   0        0        0     3204 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/commands/generate.py
+-rw-r--r--   0        0        0      411 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/commands/info.py
+-rw-r--r--   0        0        0     1529 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/commands/init.py
+-rw-r--r--   0        0        0      591 2023-04-16 02:01:06.406276 ohmyi3-0.1.2/ohmyi3/config/app.py
+-rw-r--r--   0        0        0     2238 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/config/package.py
+-rw-r--r--   0        0        0      446 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/i3ctl.py
+-rw-r--r--   0        0        0      814 2023-04-15 19:45:51.085030 ohmyi3-0.1.2/ohmyi3/services/bootstrap.py
+-rw-r--r--   0        0        0     2529 2023-04-16 19:40:39.743720 ohmyi3-0.1.2/ohmyi3/services/ohmyi3.py
+-rw-r--r--   0        0        0      188 2023-04-16 20:00:12.022854 ohmyi3-0.1.2/ohmyi3/stubs/README.md
+-rw-r--r--   0        0        0      810 2023-04-20 22:44:05.536672 ohmyi3-0.1.2/ohmyi3/stubs/config.d/00-header.conf
+-rw-r--r--   0        0        0     1985 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/05-system.conf
+-rw-r--r--   0        0        0     2904 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/10-autostart.conf
+-rw-r--r--   0        0        0      662 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/15-borders.conf
+-rw-r--r--   0        0        0     6436 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/20-navigation.conf
+-rw-r--r--   0        0        0     3212 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/80-applications.conf
+-rw-r--r--   0        0        0     6720 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/85-windows.conf
+-rw-r--r--   0        0        0     3195 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/90-gaps.conf
+-rw-r--r--   0        0        0    10089 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.py
+-rw-r--r--   0        0        0       33 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/alacritty/__init__.py
+-rw-r--r--   0        0        0      893 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/alacritty/alacritty.py
+-rw-r--r--   0        0        0       29 2023-04-20 22:44:15.316835 ohmyi3-0.1.2/ohmyi3/stubs/plugins/archey3/__init__.py
+-rw-r--r--   0        0        0      958 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/archey3/archey3.py
+-rw-r--r--   0        0        0       31 2023-04-20 22:44:15.316835 ohmyi3-0.1.2/ohmyi3/stubs/plugins/nitrogen/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/nitrogen/nitrogen.py
+-rw-r--r--   0        0        0       29 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/polybar/__init__.py
+-rw-r--r--   0        0        0     2188 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/polybar/polybar.py
+-rw-r--r--   0        0        0   385109 2023-04-20 22:44:29.983747 ohmyi3-0.1.2/ohmyi3/stubs/themes/amber/background.jpg
+-rw-r--r--   0        0        0     1874 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/themes/amber/theme.conf
+-rw-r--r--   0        0        0   198158 2023-04-20 22:44:29.987080 ohmyi3-0.1.2/ohmyi3/stubs/themes/archlinux/background.jpg
+-rw-r--r--   0        0        0     1915 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/themes/archlinux/theme.conf
+-rw-r--r--   0        0        0     1869 2023-04-20 22:44:29.987080 ohmyi3-0.1.2/ohmyi3/stubs/themes/i3status.conf
+-rw-r--r--   0        0        0   108928 2023-04-20 22:44:29.987080 ohmyi3-0.1.2/ohmyi3/stubs/themes/manjaro/background.jpg
+-rw-r--r--   0        0        0     1935 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/themes/manjaro/theme.conf
+-rw-r--r--   0        0        0   514555 2023-04-20 22:44:29.987080 ohmyi3-0.1.2/ohmyi3/stubs/themes/pink/background.jpg
+-rw-r--r--   0        0        0     2422 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/themes/pink/theme.conf
+-rw-r--r--   0        0        0     3747 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/util.py
+-rw-r--r--   0        0        0      703 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 ohmyi3-0.1.2/PKG-INFO
```

### Comparing `ohmyi3-0.1.1/LICENSE` & `ohmyi3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/commands/entrypoint.py` & `ohmyi3-0.1.2/ohmyi3/commands/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/commands/generate.py` & `ohmyi3-0.1.2/ohmyi3/commands/generate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,93 @@
 import os
 import sys
 import shutil
 import uvicore
 from glob import glob
 from uvicore.typing import Dict
-from ohmyi3.app import Application
 from ohmyi3.util import path, now, template
 from uvicore.support.dumper import dump, dd
 from uvicore.exceptions import SmartException
 
 from uvicore.console import command, argument, option
 
+
+from ohmyi3 import i3ctl
+
+
 @command()
 async def cli():
     """Dynamically Generate a new i3 config using Ohmyi3"""
 
-    # Get the application instance
-    app = Application()
+    # Get the user config files
+    userconfig = i3ctl.import_userconfig()
 
-    # Shortcut to user configurator
-    configurator = app.configurator
+    # Get the actual user config Superdict
+    config = userconfig.config()
+
+    # Get ohmyi3 paths
+    ohmyi3_path = uvicore.config('ohmyi3.config_path')
+    ohmyi3_configd_path = config.paths.ohmyi3_configd
+    ohmyi3_themes_path = config.paths.ohmyi3_themes
 
     # Start the generation
     uvicore.log.header("Generating new i3 config using ohmyi3")
 
     # Fire off user defined before_generate_hook
     uvicore.log.item3("Firing user defined before_generate hook")
-    await configurator.before_generate()
+    await userconfig.before_generate(config)
 
     # If i3 config exists, back it up
-    i3config_file = f"{app.i3config_folder}/config"
+    i3config_file = f"{config.paths.i3}/config"
     if os.path.exists(i3config_file):
-        backup = path([app.i3config_folder, 'backup-' + now()])
+        backup = path([config.paths.i3, 'backup-' + now()])
         uvicore.log.item(f"Backing up {i3config_file} to {backup}")
         shutil.copy(i3config_file, backup)
 
     # Get all config.d/* files
-    os.chdir(app.configd_folder)
-    files = sorted(glob("*.conf"))
+    files = sorted(glob(ohmyi3_configd_path + "/*.conf"))
+
+    # Get active theme path
+    active_theme_path = f"{ohmyi3_themes_path}/{config.theme}"
 
     # Append config.d/* and theme.d/theme to new i3 config
     with open(i3config_file, "w") as f:
         # Loop and merge each config and append to
         for file in files:
             uvicore.log.item2(f"Appending {file}")
-            f.write(template(app.configd_folder, file, **configurator))
+            f.write(template(file, values=config))
             f.write("\n\n\n")
 
         # Append the selected theme files
-        theme_folder = f"{app.themes_folder}/{configurator.theme}"
-        theme_file = path([theme_folder, 'theme.conf'])
+        theme_file = path([active_theme_path, 'theme.conf'])
         if os.path.exists(theme_file):
-            uvicore.log.item(f"Appending THEME {configurator.theme}")
-            f.write(template(theme_folder, 'theme.conf', **configurator))
+            uvicore.log.item(f"Appending THEME {config.theme}")
+            f.write(template(theme_file, values=config))
 
     # Copy themed i3status or a default if no theme specific file exists
-    i3status_folder = None
-    if os.path.exists(f"{theme_folder}/i3status.conf"):
+    i3status_template_path = None
+    if os.path.exists(f"{active_theme_path}/i3status.conf"):
         # Use themed i3status.conf
-        i3status_folder = f"{theme_folder}"
-    elif os.path.exists(f"{app.themes_folder}/i3status.conf"):
+        i3status_template_path = active_theme_path
+    elif os.path.exists(f"{ohmyi3_themes_path}/i3status.conf"):
         # Use default i3status.conf
-        i3status_folder = f"{app.themes_folder}"
-    if i3status_folder:
-        uvicore.log.item(f"Copying {i3status_folder}/i3status.conf to {app.i3status_folder}/config")
-        with open(f"{app.i3status_folder}/config", "w") as f:
-            f.write(template(i3status_folder, 'i3status.conf', **configurator))
+        i3status_template_path = f"{ohmyi3_themes_path}"
+
+    if i3status_template_path:
+        uvicore.log.item(f"Copying {i3status_template_path}/i3status.conf to {config.paths.i3status}/config")
+        with open(f"{config.paths.i3status}/config", "w") as f:
+            f.write(template('i3status.conf', base=i3status_template_path, values=config))
 
     # Fire off user defined afer_generate_hook
     uvicore.log.item3("Firing user defined after_generate hook")
-    await configurator.after_generate()
+    await userconfig.after_generate(config)
 
-    # Cleanup
-    app._cleanup()
+    # Cleanup __pycache__
+    pycache = path([ohmyi3_path, '__pycache__'])
+    if os.path.exists(pycache):
+        shutil.rmtree(pycache)
 
     # Done
     uvicore.log.nl()
     uvicore.log("Done!")
     uvicore.log(f"New {i3config_file} generated!")
     uvicore.log("Please reload i3!")
```

### Comparing `ohmyi3-0.1.1/ohmyi3/commands/init.py` & `ohmyi3-0.1.2/ohmyi3/commands/init.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 import os
 import shutil
 import uvicore
-from ohmyi3.app import Application
+from ohmyi3 import i3ctl
+from ohmyi3.util import path
 from uvicore.support.dumper import dump, dd
 from uvicore.exceptions import SmartException
 from uvicore.console import command, argument, option
 
 @command()
 async def cli():
     """Initialize a stock ~/.config/ohmyi3/* configuration"""
 
-    # Get the application instance
-    app = Application(must_exist=False);
+    # Get the user config
+    config_path = path(uvicore.config('ohmyi3.config_path'))
+    app_path = path(uvicore.app.package(main=True).path, True)
+    stubs_path = path([app_path, 'stubs'], True)
 
-    uvicore.log.header('Initializing ohmyi3')
+    uvicore.log.header(f'Initializing ohmyi3 to {config_path}')
 
     # Create ~/.config/ohmyi3/ and copy stubs
-    if not os.path.exists(app.config_folder):
-        uvicore.log.item(f"Creating {app.config_folder} folder")
-        #os.mkdir(app.config_folder)
-        uvicore.log.item(f"Copying base configs into {app.config_folder} folder")
-        shutil.copytree(app.stubs_folder + '/', app.config_folder + '/')
+    if not os.path.exists(config_path):
+        uvicore.log.item(f"Creating {config_path} folder")
+        uvicore.log.item(f"Copying base configs into {config_path} folder")
+        shutil.copytree(stubs_path, config_path)
+
+    # Get the user config
+    config = i3ctl.import_userconfig().config()
+
+    # Get i3 and i3status path
+    i3_path = config.paths.i3 if config.paths.i3 else path('~/.config/i3')
+    i3status_path = config.paths.i3status if config.paths.i3status else path('~/.config/i3status')
 
     # Create ~/.config/i3
-    if not os.path.exists(app.i3config_folder):
-        uvicore.log.item(f"Creating {app.i3config_folder} folder")
-        os.mkdir(app.i3config_folder)
+    if not os.path.exists(i3_path):
+        uvicore.log.item(f"Creating {i3_path} folder")
+        os.mkdir(i3_path)
 
     # Create ~/.config/i3status
-    if not os.path.exists(app.i3status_folder):
-        uvicore.log.item(f"Creating {app.i3status_folder} folder")
-        os.mkdir(app.i3status_folder)
+    if not os.path.exists(i3status_path):
+        uvicore.log.item(f"Creating {i3status_path} folder")
+        os.mkdir(i3status_path)
 
     uvicore.log.nl()
     uvicore.log('Done!  Now run: i3ctl generate')
```

### Comparing `ohmyi3-0.1.1/ohmyi3/config/app.py` & `ohmyi3-0.1.2/ohmyi3/config/app.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/config/package.py` & `ohmyi3-0.1.2/ohmyi3/config/package.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 # when used inside other applications.  Accessible at config('ohmyi3')
 
 config = {
 
     # --------------------------------------------------------------------------
     # Package Custom Configuration
     # --------------------------------------------------------------------------
-    'config_path': env('OHMYI3_CONFIG_PATH', '~/.config/ohmyi3'),
-    'i3config_path': env('OHMYI3_I3CONFIG_PATH', '~/.config/i3'),
-    'i3status_path': env('OHMYI3_I3STATUS_PATH', '~/.config/i3status'),
-
+    'config_path': env('OHMYI3_PATH', '~/.config/ohmyi3'),
 
 
     # --------------------------------------------------------------------------
     # Package Information
     #
     # Most other info like name, short_name, vendor are derived automatically
     # --------------------------------------------------------------------------
```

### Comparing `ohmyi3-0.1.1/ohmyi3/services/bootstrap.py` & `ohmyi3-0.1.2/ohmyi3/services/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/services/ohmyi3.py` & `ohmyi3-0.1.2/ohmyi3/services/ohmyi3.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/config.d/00-header.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/config.d/00-header.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/config.d/05-system.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/config.d/05-system.conf`

 * *Files 14% similar despite different names*

```diff
@@ -5,40 +5,46 @@
 # Set default desktop layout (default is tiling)
 # workspace_layout tabbed <stacking|tabbed>
 
 # Switch to workspace with urgent window automatically
 for_window [urgent=latest] focus
 
 # Reload the configuration file
-bindsym $mod+Shift+q reload
+# bindsym $mod+Shift+q reload
 
 # Restart i3 inplace (preserves your layout/session, can be used to upgrade i3)
-bindsym $mod+Shift+r restart
+#bindsym $mod+Shift+r restart
+bindsym $mod+Shift+r exec --no-startup-id "{{ i3_restart }}"
 
 {% if desktop == 'i3' %}
     # Lock screen
-    bindsym Ctrl+$alt+l exec --no-startup-id blurlock
+    bindsym Ctrl+$alt+l exec --no-startup-id "{{ apps.screenlock }}"
 {% endif %}
 
 # Exit i3 (logs you out of your X session)
 bindsym $mod+Shift+e exec "i3-nagbar -t warning -m 'You pressed the exit shortcut. Do you really want to exit i3? This will end your X session.' -b 'Yes, exit i3' 'i3-msg exit'"
 
 # Brightness keys
-bindsym XF86MonBrightnessDown exec --no-startup-id brightnessctl --min-val=2 -q set 3%-
-bindsym XF86MonBrightnessUp exec --no-startup-id brightnessctl -q set 3%+
+bindsym XF86MonBrightnessUp exec --no-startup-id "{{ brightness.up }}"
+bindsym XF86MonBrightnessDown exec --no-startup-id "{{ brightness.down }}"
 
-# Set shut down, restart and locking features
-bindsym Ctrl+$alt+Delete mode "$mode_system"
-set $mode_system (l)ock, (e)xit, switch_(u)ser, (s)uspend, (h)ibernate, (r)eboot, (Shift+s)hutdown
-mode "$mode_system" {
-    bindsym l exec --no-startup-id i3exit lock, mode "default"
-    bindsym s exec --no-startup-id i3exit suspend, mode "default"
-    bindsym u exec --no-startup-id i3exit switch_user, mode "default"
-    bindsym e exec --no-startup-id i3exit logout, mode "default"
-    bindsym h exec --no-startup-id i3exit hibernate, mode "default"
-    bindsym r exec --no-startup-id i3exit reboot, mode "default"
-    bindsym Shift+s exec --no-startup-id i3exit shutdown, mode "default"
-
-    # exit system mode: "Enter" or "Escape"
-    bindsym Return mode "default"
-    bindsym Escape mode "default"
-}
+# Rofi Powermenu
+bindsym Ctrl+$alt+Delete exec --no-startup-id "{{ rofi.powermenu }}"
+
+{% if bar.enabled == True %}
+    # Set shut down, restart and locking features
+    bindsym Ctrl+$alt+Delete mode "$mode_system"
+    set $mode_system (l)ock, (e)xit, switch_(u)ser, (s)uspend, (h)ibernate, (r)eboot, (Shift+s)hutdown
+    mode "$mode_system" {
+        bindsym l exec --no-startup-id i3exit lock, mode "default"
+        bindsym s exec --no-startup-id i3exit suspend, mode "default"
+        bindsym u exec --no-startup-id i3exit switch_user, mode "default"
+        bindsym e exec --no-startup-id i3exit logout, mode "default"
+        bindsym h exec --no-startup-id i3exit hibernate, mode "default"
+        bindsym r exec --no-startup-id i3exit reboot, mode "default"
+        bindsym Shift+s exec --no-startup-id i3exit shutdown, mode "default"
+
+        # exit system mode: "Enter" or "Escape"
+        bindsym Return mode "default"
+        bindsym Escape mode "default"
+    }
+{% endif %}
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/config.d/10-autostart.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/config.d/10-autostart.conf`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,59 @@
 ################################################################################
 # Autostart Applications
 ################################################################################
 # Note: exec means run once, exec_always means every time i3 is restarted ($mod+Shift+r)
 
+# The --no-startup-id parameter disables startup-notification support for this
+# particular exec command. With startup-notification, i3 can make sure that a window
+# appears on the workspace on which you used the exec command. Also, it will change
+# the X11 cursor to watch (a clock) while the application is launching. So, if an
+# application is not startup-notification aware (most GTK and Qt using applications
+# seem to be, though), you will end up with a watch cursor for 60 seconds.
+
 {% if desktop == 'i3' %}
+
     # Policy Kit authenticator
     #exec --no-startup-id /usr/lib/polkit-gnome/polkit-gnome-authentication-agent-1
     exec --no-startup-id /usr/lib/polkit-kde-authentication-agent-1
 
     # arandr/xrandr to force default screen/monitor layout
     exec --no-startup-id ~/.screenlayout/screen-laptop.sh; sleep 1
 
+    # Clipboard manager
+    exec --no-startup-id {{ apps.clipboard }}
+
+    {% if os == 'manjaro' %}
+    exec --no-startup-id matray
+    {% endif %}
+
     # Network Manager icon in i3 bar
-    exec --no-startup-id nm-applet
+    exec --no-startup-id {{ tray.network }}
 
     # Volumn icon in i3 bar
-    exec --no-startup-id volumeicon
+    exec --no-startup-id {{ tray.volume }}
 
     # Power Management and Screen Locking
-    # xss-lock waits until xfce4-power-manager screen turn off time, then starts i3lock
-    exec_always --no-startup-id xfce4-power-manager
-    #exec_always --no-startup-id xss-lock -- i3lock --nofork --image /home/mreschke/Wallpaper/Manjaro/Bamboo\ Night.png
+    # xss-lock waits until xfce4-power-manager (or any manager) turns off screen, then starts i3lock
+    exec_always --no-startup-id {{ apps.powermanager }}
+    exec_always --no-startup-id {{ apps.xsslock }}
     #exec --no-startup-id xautolock -time 10 -locker blurlock
     #exec --no-startup-id xss-lock -- blurlock
 
     # Reset keyboard speed and fix_xcursor
     exec_always --no-startup-id xset r rate 250 50
-    exec_always --no-startup-id fix_xcursor
+    #exec_always --no-startup-id fix_xcursor
+
+    # Start xfsettingsd to get xfce GTK themes (if running in i3 code with xfce desktop tools)
+    {% if desktop_tools == 'xfce' %}
+    exec --no-startup-id xfsettingsd
+    {% endif %}
+
+    # Polybar
+    exec_always --no-startup-id ~/.config/polybar/launch.sh --{{ polybar.theme }}
 
 {% endif %}
 
 
 # Nitrogen to set i3 background wallpaper
 # AND picom compositor after nitrogen has loaded
 #exec --no-startup-id nitrogen --restore; sleep 1; picom -b
@@ -40,13 +63,15 @@
 # Pamac out of date packages icon in i3 bar
 #exec --no-startup-id pamac-tray
 
 # Windows like alttab for i3
 # Colors: manjaro green
 exec_always --no-startup-id "alttab -fg '#106E5C' -bg '#0E2229' -frame '#106E5C' -t 128x150 -i 127x64"
 
+
+
 # Not Used
 #exec --no-startup-id clipit
 #exec --no-startup-id blueman-applet
 #exec_always --no-startup-id sbxkb
 #exec --no-startup-id start_conky_maia
 #exec --no-startup-id start_conky_green
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/config.d/20-navigation.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/config.d/20-navigation.conf`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 bindsym $mod+Shift+Right move right
 
 # Workspace back and forth (with/without active container)
 # auto_back_and_forth means pressing original desktop key goes back and forth, its confusing for me
 # workspace_auto_back_and_forth yes
 # grave is ` backtik
 bindsym $mod+grave workspace back_and_forth
-bindsym $mod+b workspace back_and_forth
-bindsym $mod+Shift+b move container to workspace back_and_forth; workspace back_and_forth
+# bindsym $mod+b workspace back_and_forth
+# bindsym $mod+Shift+b move container to workspace back_and_forth; workspace back_and_forth
 
 # Split orientation
 #bindsym $mod+h split h;exec notify-send 'tile horizontally'
 #bindsym $mod+v split v;exec notify-send 'tile vertically'
 bindsym $mod+q split toggle
 
 # Toggle fullscreen mode for the focused container
@@ -77,24 +77,28 @@
 bindsym Shift+F12 move scratchpad
 
 # Show the next scratchpad window or hide the focused scratchpad window.
 # If there are multiple scratchpad windows, this command cycles through them.
 #bindsym $mod+minus scratchpad show
 bindsym F12 scratchpad show
 bindsym $alt+grave scratchpad show
-bindsym $mod+Tab exec xwinmosaic
-bindsym $mod+$alt+Tab exec "rofi -show window"
-#bindsym $alt+Tab exec "rofi -show combi run,window"
+bindsym $mod+Tab exec --no-startup-id xwinmosaic
+bindsym $mod+$alt+Tab exec --no-startup-id "rofi -show window"
+#bindsym $alt+Tab exec --no-startup-id "rofi -show combi run,window"
 #bindsym $alt+Tab exec --no-startup-id rofi -modi combi -combi-modi window -show combi
-#bindsym $alt+Tab exec "/home/mreschke/.files/configs/i3/i3wins/env/bin/i3wins -kb-row-down 'Down,Control+n,Alt+Tab' -kb-accept-entry '!Alt+Tab,!Alt_L,!Alt+Alt_L,Return'"
-#bindsym Mod1+space exec "/home/mreschke/.files/configs/i3/i3wins/env/bin/i3lastc"
-#bindsym $alt+Tab exec skippy-xd
+#bindsym $alt+Tab exec --no-startup-id "/home/mreschke/.files/configs/i3/i3wins/env/bin/i3wins -kb-row-down 'Down,Control+n,Alt+Tab' -kb-accept-entry '!Alt+Tab,!Alt_L,!Alt+Alt_L,Return'"
+#bindsym Mod1+space exec --no-startup-id "/home/mreschke/.files/configs/i3/i3wins/env/bin/i3lastc"
+#bindsym $alt+Tab exec --no-startup-id skippy-xd
 
 # hide/unhide i3status bar
-bindsym $mod+m bar mode toggle
+{% if bar.enabled %}
+    bindsym $mod+m bar mode toggle
+{% elif polybar.enabled %}
+    bindsym $mod+m exec --no-startup-id polybar-msg cmd toggle
+{% endif %}
 
 # Kill focused window
 bindsym $mod+Shift+c kill
 bindsym $alt+F4 kill
 
 # Navigate workspaces next / previous
 bindsym $mod+Ctrl+Right workspace next
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/config.d/80-applications.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/config.d/80-applications.conf`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ################################################################################
 # Application Configuration
 ################################################################################
 
 # Terminal
-bindsym $mod+Return exec {{ terminal }}
+bindsym $mod+Return exec --no-startup-id {{ apps.terminal }}
 #bindsym $mod+Return exec terminal
 #bindsym $mod+Shift+Return exec terminal-urxvt
 
 # CLI settings application
-bindsym $mod+Ctrl+b exec terminal -e 'bmenu'
+bindsym $mod+Ctrl+b exec --no-startup-id {{ apps.terminal }} -e 'bmenu'
 
 # F1-4 Browsers
 #bindsym $mod+F1 exec firefox
 #bindsym $mod+F2 exec chromium
 #bindsym $mod+F3 exec waterfox-g4
 #bindsym $mod+F4 exec vivaldi-stable
 
@@ -28,51 +28,54 @@
 #bindsym $mod+Shift+F3 exec pcmanfm_pkexec
 #bindsym $mod+F5 exec terminal -e 'mocp'
 
 # Volume Control Wheel
 #bindsym XF86AudioRaiseVolume exec --no-startup-id pactl set-sink-volume 1 +5% && killall -SIGUSR1 i3status
 #bindsym XF86AudioLowerVolume exec --no-startup-id pactl set-sink-volume 1 -5% && killall -SIGUSR1 i3status
 #bindsym XF86AudioMute exec --no-startup-id pactl set-sink-mute 1 toggle
-bindsym XF86AudioRaiseVolume exec --no-startup-id amixer -D pulse sset Master 5%+
-bindsym XF86AudioLowerVolume exec --no-startup-id amixer -D pulse sset Master 5%-
-bindsym XF86AudioMute exec --no-startup-id amixer -D pulse set Master 1+ toggle
+bindsym XF86AudioRaiseVolume exec --no-startup-id {{ volume.up }}
+bindsym XF86AudioLowerVolume exec --no-startup-id {{ volume.down }}
+bindsym XF86AudioMute exec --no-startup-id {{ volume.mute }}
+
+# Sound control panel
+#bindsym $mod+Ctrl+m exec --no-startup-id terminal -e 'alsamixer'
+bindsym $mod+Ctrl+m exec --no-startup-id {{ volume.mixer }}
 
 # Media Buttons
-bindsym XF86AudioPlay exec --no-startup-id playerctl play-pause
-bindsym XF86AudioPause exec --no-startup-id playerctl play-pause
-bindsym XF86AudioNext exec --no-startup-id playerctl next
-bindsym XF86AudioPrev exec --no-startup-id playerctl previous
+bindsym XF86AudioPlay exec --no-startup-id {{ media.play_pause }}
+bindsym XF86AudioPause exec --no-startup-id {{ media.play_pause }}
+bindsym XF86AudioNext exec --no-startup-id {{ media.next }}
+bindsym XF86AudioPrev exec --no-startup-id {{ media.previous }}
 
 # Calculator
-bindsym $mod+minus exec --no-startup-id {{ calculator }}
+bindsym $mod+minus exec --no-startup-id {{ apps.calculator }}
+#bindsym $mod+minus [class="kcalc"] scratchpad show; move position center
 
 # Start/Kill picom (which is the tiny composit manager)
 bindsym $mod+Ctrl+t exec --no-startup-id picom -b
 bindsym $mod+t exec --no-startup-id pkill picom
 
 # Dunst is a lightweight notification-daemon
 #bindsym $mod+Shift+d --release exec "killall dunst; exec notify-send 'restart dunst'"
 
 # Screenshots with scrot or spectacle
-bindsym Print exec --no-startup-id {{ screenshot}}
+bindsym Print exec --no-startup-id {{ apps.screenshot }}
 #bindsym Print exec --no-startup-id i3-scrot
 #bindsym $mod+Print --release exec --no-startup-id i3-scrot -w
 #bindsym $mod+Shift+Print --release exec --no-startup-id i3-scrot -s
 
 # i3 help dialog
-#bindsym $mod+Shift+h exec xdg-open /usr/share/doc/manjaro/i2_help.pdf
+#bindsym $mod+Shift+h exec --no-startup-id xdg-open /usr/share/doc/manjaro/i2_help.pdf
 
 # Start xkill, use mouse to pick which window to kill
 bindsym $mod+Ctrl+x --release exec --no-startup-id xkill
 
 # Dmenu or rofi application launcher
-#bindsym $mod+d exec --no-startup-id dmenu_recency
-bindsym $mod+d exec --no-startup-id {{ dmenu }}
-bindsym $mod+$alt+d exec "rofi -show drun"
-bindsym $mod+Shift+d exec "rofi -show run"
+bindsym $mod+d exec --no-startup-id {{ rofi.launcher }}
+bindsym $mod+Shift+d exec --no-startup-id {{ apps.dmenu }}
+#bindsym $mod+Shift+d exec --no-startup-id dmenu_recency
+#bindsym $mod+Shift+d exec --no-startup-id "rofi -show drun"
+#bindsym $mod+$alt+d exec --no-startup-id "rofi -show run"
 
 # Morc application launcher
 bindsym $mod+z exec --no-startup-id morc_menu
 
-# Sound control panel
-#bindsym $mod+Ctrl+m exec terminal -e 'alsamixer'
-bindsym $mod+Ctrl+m exec {{ volumectrl }}
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/config.d/85-windows.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/config.d/85-windows.conf`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 # Open applications on specific workspaces
 # assign [class="Thunderbird"] $ws1
 # assign [class="Pale moon"] $ws2
 # assign [class="Pcmanfm"] $ws3
 # assign [class="Skype"] $ws5
 
 # Enable window icons for all windows
-#for_window [all] title_window_icon on
+for_window [all] title_window_icon on
+{% if os != 'lmde' %}
 for_window [all] title_window_icon padding 5px
+{% endif %}
 
 # Open these applications in floating mode
 # Options are
 #   floating enable
 #   sticky enable
 #   border pixel 5
 #   border normal
@@ -64,26 +66,26 @@
 for_window [class="(?i)systemsettings"] floating enable
 for_window [class="(?i)ksysguard"] floating enable
 for_window [class="(?i)plasma-systemmonitor"] floating enable
 for_window [class="(?i)spectacle"] floating enable border normal
 for_window [class="(?i)manjaro-hello"] floating enable
 for_window [class="(?i)manjaro settings manager"] floating enable
 for_window [class="(?i)pamac-manager"] floating enable
-for_window [class="(?i)kcalc"] floating enable sticky enable border none
+for_window [class="(?i)kcalc"] floating enable sticky enable border normal
 
 # CLI Apps
 for_window [title="(?i)alsamixer"] floating enable
 
 # Other
 for_window [class="(?i)lxappearance"] floating enable border normal
 for_window [class="(?i)nitrogen"] floating enable border normal
 for_window [class="(?i)pavucontrol"] floating enable border normal
 for_window [class="(?i)qt5ct"] floating enable border normal
 for_window [class="(?i)virtualbox"] floating enable border normal
-#for_window [class="(?i)zoom" window_type="dialog"] floating enable border normal
+for_window [class="(?i)zoom" window_type="dialog"] floating enable border normal
 for_window [class="(?i)zoom"] floating enable border normal
 for_window [class="(?i)arandr"] floating enable border normal
 for_window [class="(?i)firefox" title="About Mozilla Firefox"] floating enable border normal
 #for_window [class="(?i)virt-manager" title="Virtual Machine Manager"] floating enable
 for_window [class="(?i)virt-manager"] floating enable
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/config.d/90-gaps.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/config.d/90-gaps.conf`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 ################################################################################
 # i3-gaps configuration
 ################################################################################
 
+{% if i3_gaps %}
+
 # Set inner/outer gaps
 # Inner gaps are space between two adjacent windows (or split containers).
 # Outer gaps are space along the screen edges. You can configure each side (left, right, top, bottom) separately.
 
 # Inner gaps for all windows: space between two adjacent windows (or split containers).
 # gaps inner <gap_size>[px]
+# Favorite is 15 or 25
 gaps inner 15
 
 # Outer gaps for all windows: space along the screen edges.
 ##gaps outer|horizontal|vertical|top|left|bottom|right <gap_size>[px]
 
 # Inner and outer gaps for all windows on a specific workspace.
 # <ws> can be a workspace number or name.
@@ -67,7 +70,9 @@
         bindsym Shift+plus  gaps outer all plus 5
         bindsym Shift+minus gaps outer all minus 5
         bindsym Shift+0     gaps outer all set 0
 
         bindsym Return mode "default"
         bindsym Escape mode "default"
 }
+
+{% endif %}
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/plugins/archey3/archey3.py` & `ohmyi3-0.1.2/ohmyi3/stubs/plugins/archey3/archey3.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import uvicore
 from ohmyi3 import util
 from uvicore.support.dumper import dump, dd
 
 class Archey3:
     """
-    Archey3 Plugin
+    Ohmyi3 Archey3 Plugin
     Copyright (c) 2023 Matthew Reschke License http://mreschke.com/license/mit
     """
 
-    def __init__(self, configurator):
-        # User Configurator Instance
-        self.configurator = configurator
-
+    def __init__(self, config):
+        """Instantiate Plugin with User Configuration"""
+        self.config = config
 
     def set_archey(self):
         """Set ~/.zshrc archey3 color based on theme"""
-        themes = self.configurator.themes
-        theme = self.configurator.theme
+        themes = self.config.themes
+        theme = self.config.theme
         color = themes.dotget(f"{theme}.archey3")
+
         if not color: return
         if util.exists('~/.zshrc'):
             cmd = f"sed -i 's/archey3.*/archey3 -c {color}/g' ~/.zshrc"
             uvicore.log.item4(f"Plugin Archey3: {cmd}")
             util.shell(cmd)
         if util.exists('~/.bashrc'):
             cmd = f"sed -i 's/archey3.*/archey3 -c {color}/g' ~/.bashrc"
             uvicore.log.item4(f"Plugin Archey3: {cmd}")
             util.shell(cmd)
-
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/plugins/nitrogen/nitrogen.py` & `ohmyi3-0.1.2/ohmyi3/stubs/plugins/nitrogen/nitrogen.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 import uvicore
 from uvicore.support.dumper import dump, dd
 from ohmyi3.util import path, exists, shell
 
 class Nitrogen:
     """
-    Nitrogen Wallpaper Plugin
+    Ohmyi3 Nitrogen Wallpaper Plugin
     Copyright (c) 2023 Matthew Reschke License http://mreschke.com/license/mit
     """
 
-    def __init__(self, configurator, test):
-        # User Configurator Instance
-        self.configurator = configurator
-
+    def __init__(self, config):
+        """Instantiate Plugin with User Configuration"""
+        self.config = config
 
     def set_wallpaper(self):
         """Set nitrogen wallpaper based on selected theme"""
-
-        # Shortcuts
-        configurator = self.configurator
-        app = configurator.app
-        theme = configurator.theme
-        themes = configurator.themes
-        wallpaper_base = configurator.wallpaper_base
+        theme = self.config.theme
+        themes = self.config.themes
+        themes_path = self.config.paths.ohmyi3_themes
+        wallpaper_base = self.config.wallpaper_base
 
         # Get theme background file (jpg or png)
         background = None
-        theme_folder = path([app.themes_folder, theme])
-        jpg = path([theme_folder, 'background.jpg'])
-        png = path([theme_folder, 'background.jpg'])
+        theme_path = path([self.config.paths.ohmyi3_themes, self.config.theme])
+        jpg = path([theme_path, 'background.jpg'])
+        png = path([theme_path, 'background.jpg'])
         if exists(jpg): background = jpg
         if exists(png): background = png
 
         # Check for background override
         override = themes.dotget(f"{theme}.wallpaper")
         if override: background = path(f"{wallpaper_base}/{override}")
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/amber/background.jpg` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/amber/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/amber/theme.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/amber/theme.conf`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Palette Designed for Wallpaper/Abstract/artistic_colors.jpg
 #1E2229 - Main grey everywhere (taken from my konsole grey)
 #2F3D44 - always on border
 #595B5B - ligher borders
 #FDF6E3 - light gray/white
 #EF5B1A - main theme color
 
+{% if bar.enabled %}
 # Start i3bar to display a workspace bar (plus the system information i3status if available)
 bar {
     i3bar_command {{ bar.cmd }}
     status_command {{ bar.status_cmd }}
     position {{ bar.position }}
 
     #mode dock|hide|invisible
@@ -31,14 +32,15 @@
 
         # class             border   backgr.  text
         focused_workspace   #595B5B  #EF5B1A  #292F34
         active_workspace    #595B5B  #1E2229  #EF5B1A
         inactive_workspace  #595B5B  #1E2229  #666666
     }
 }
+{% endif %}
 
 # class                  border   backgr.  text     indic.   child_border
 client.focused           #EF5B1A  #1E2229  #EF5B1A  #B00500  #EF5B1A
 client.focused_inactive  #2F3D44  #0E2229  #EF5B1A  #2F3D44  #2F3D44
 client.unfocused         #2F3D44  #0E2229  #595B5B  #2F3D44  #2F3D44
 
 # Background color which will be used to paint the background of the client window
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/archlinux/background.jpg` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/archlinux/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/archlinux/theme.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/archlinux/theme.conf`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #1E2229 - Main grey everywhere (taken from my konsole grey)
 #2F3D44 - always on border
 #595B5B - ligher borders
 #FDF6E3 - light gray/white
 #1793D1 - main theme color (archlinux blue)
 #106E5C - manjaro green
 
+{% if bar.enabled %}
 # Start i3bar to display a workspace bar (plus the system information i3status if available)
 bar {
     i3bar_command {{ bar.cmd }}
     status_command {{ bar.status_cmd }}
     position {{ bar.position }}
 
     #mode dock|hide|invisible
@@ -32,14 +33,15 @@
 
         # class             border   backgr.  text
         focused_workspace   #595B5B  #1793D1  #292F34
         active_workspace    #595B5B  #1E2229  #1793D1
         inactive_workspace  #595B5B  #1E2229  #666666
     }
 }
+{% endif %}
 
 # class                  border   backgr.  text     indic.   child_border
 client.focused           #1793D1  #1E2229  #1793D1  #106E5C  #1793D1
 client.focused_inactive  #2F3D44  #0E2229  #1793D1  #2F3D44  #2F3D44
 client.unfocused         #2F3D44  #0E2229  #595B5B  #2F3D44  #2F3D44
 
 # Background color which will be used to paint the background of the client window
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/i3status.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/i3status.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/manjaro/background.jpg` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/manjaro/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/manjaro/theme.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/manjaro/theme.conf`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #2F3D44 - always on border
 #595B5B - ligher borders
 #FDF6E3 - light gray/white
 #106E5C - main theme color (manjaro green)
 #1793D1 - archlinux blue
 
 
+
+{% if bar.enabled %}
 # Start i3bar to display a workspace bar (plus the system information i3status if available)
 bar {
     i3bar_command {{ bar.cmd }}
     status_command {{ bar.status_cmd }}
     position {{ bar.position }}
 
     #mode dock|hide|invisible
@@ -33,14 +35,15 @@
 
         # class             border   backgr.  text
         focused_workspace   #595B5B  #106E5C  #292F34
         active_workspace    #595B5B  #1E2229  #106E5C
         inactive_workspace  #595B5B  #1E2229  #666666
     }
 }
+{% endif %}
 
 # class                  border   backgr.  text     indic.   child_border
 client.focused           #106E5C  #1E2229  #106E5C  #1793D1  #106E5C
 client.focused_inactive  #2F3D44  #0E2229  #106E5C  #2F3D44  #2F3D44
 client.unfocused         #2F3D44  #0E2229  #595B5B  #2F3D44  #2F3D44
 
 # Background color which will be used to paint the background of the client window
```

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/pink/background.jpg` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/pink/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.1/ohmyi3/stubs/themes/pink/theme.conf` & `ohmyi3-0.1.2/ohmyi3/stubs/themes/pink/theme.conf`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #6c0509
 #cf5500
 #ae0000
 #07989d
 #008b86
 
 
+{% if bar.enabled %}
 # Start i3bar to display a workspace bar (plus the system information i3status if available)
 bar {
     i3bar_command {{ bar.cmd }}
     status_command {{ bar.status_cmd }}
     position {{ bar.position }}
 
     #mode dock|hide|invisible
@@ -44,14 +45,15 @@
 
         # class             border   backgr.  text
         focused_workspace   #595B5B  #07989d  #292F34
         active_workspace    #595B5B  #1E2229  #b41474
         inactive_workspace  #595B5B  #1E2229  #666666
     }
 }
+{% endif %}
 
 # If you want PINK backgorund tabs
 # class                  border   backgr.  text     indic.   child_border
 # client.focused           #b41474  #b41474  #1E2229  #cf5500  #b41474
 # client.focused_inactive  #b41474  #0E2229  #b41474  #2F3D44  #2F3D44
 # client.unfocused         #b41474  #0E2229  #595B5B  #2F3D44  #2F3D44
```

### Comparing `ohmyi3-0.1.1/pyproject.toml` & `ohmyi3-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ohmyi3"
-version = "0.1.1"
+version = "0.1.2"
 license = "MIT"
 authors = ["Matthew Reschke <mail@mreschke.com>"]
 description = "Dynamic i3 Configuration Manager "
 homepage = "https://github.com/ohmyi3/ohmyi3"
 documentation = "https://github.com/ohmyi3/ohmyi3"
 repository = "https://github.com/ohmyi3/ohmyi3"
 readme = "README.md"
```

### Comparing `ohmyi3-0.1.1/PKG-INFO` & `ohmyi3-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmyi3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dynamic i3 Configuration Manager 
 Home-page: https://github.com/ohmyi3/ohmyi3
 License: MIT
 Author: Matthew Reschke
 Author-email: mail@mreschke.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

