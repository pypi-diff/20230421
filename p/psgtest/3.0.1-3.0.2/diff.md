# Comparing `tmp/psgtest-3.0.1.tar.gz` & `tmp/psgtest-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psgtest-3.0.1.tar", last modified: Fri Apr 21 11:16:55 2023, max compression
+gzip compressed data, was "dist\psgtest-3.0.2.tar", last modified: Fri Apr 21 11:21:40 2023, max compression
```

## Comparing `psgtest-3.0.1.tar` & `psgtest-3.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:16:55.000000 psgtest-3.0.1/
--rw-rw-rw-   0        0        0     8172 2023-04-21 11:16:55.000000 psgtest-3.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 11:16:55.000000 psgtest-3.0.1/psgtest/
--rw-rw-rw-   0        0        0    39475 2023-04-21 10:42:04.000000 psgtest-3.0.1/psgtest/psgtest.py
--rw-rw-rw-   0        0        0    16958 2021-11-04 18:03:39.000000 psgtest-3.0.1/psgtest/psgtest_icon.ico
--rw-rw-rw-   0        0        0    20186 2021-10-30 20:48:11.000000 psgtest-3.0.1/psgtest/psgtest_icon.png
--rw-rw-rw-   0        0        0       23 2021-11-12 18:21:37.000000 psgtest-3.0.1/psgtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:16:55.000000 psgtest-3.0.1/psgtest.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-21 11:16:55.000000 psgtest-3.0.1/psgtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-21 11:16:55.000000 psgtest-3.0.1/psgtest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     8172 2023-04-21 11:16:55.000000 psgtest-3.0.1/psgtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       27 2023-04-21 11:16:55.000000 psgtest-3.0.1/psgtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0      295 2023-04-21 11:16:55.000000 psgtest-3.0.1/psgtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 11:16:55.000000 psgtest-3.0.1/psgtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6056 2023-04-21 10:47:58.000000 psgtest-3.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 11:16:55.000000 psgtest-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1483 2023-04-21 11:16:51.000000 psgtest-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:21:40.000000 psgtest-3.0.2/
+-rw-rw-rw-   0        0        0     8172 2023-04-21 11:21:40.000000 psgtest-3.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 11:21:40.000000 psgtest-3.0.2/psgtest/
+-rw-rw-rw-   0        0        0    39473 2023-04-21 11:20:24.000000 psgtest-3.0.2/psgtest/psgtest.py
+-rw-rw-rw-   0        0        0    16958 2021-11-04 18:03:39.000000 psgtest-3.0.2/psgtest/psgtest_icon.ico
+-rw-rw-rw-   0        0        0    20186 2021-10-30 20:48:11.000000 psgtest-3.0.2/psgtest/psgtest_icon.png
+-rw-rw-rw-   0        0        0       23 2021-11-12 18:21:37.000000 psgtest-3.0.2/psgtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:21:40.000000 psgtest-3.0.2/psgtest.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     8172 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      295 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6056 2023-04-21 10:47:58.000000 psgtest-3.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:21:40.000000 psgtest-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1483 2023-04-21 11:21:17.000000 psgtest-3.0.2/setup.py
```

### Comparing `psgtest-3.0.1/PKG-INFO` & `psgtest-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psgtest
-Version: 3.0.1
+Version: 3.0.2
 Summary: Run your Python programs, capture the output, using your choice of interpreters
 Home-page: https://github.com/PySimpleGUI/psgtest
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Description: 
         <p align="center">
```

### Comparing `psgtest-3.0.1/psgtest/psgtest.py` & `psgtest-3.0.2/psgtest/psgtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
 
 def make_window(sp_to_mline_dict=None, sp_to_filename=None):
     """
     Creates the main window
     :return: The main window object
     :rtype: (sg.Window)
     """
-
+    icon = b'iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAYAAAAeP4ixAAAABmJLR0QA/wD/AP+gvaeTAAADv0lEQVRogd2Zy0tVQRzHP1bkDa1NtCgtolQIKwlcCJYtFRRsX0S7+gPS9tqDFlmLHhi1lhSF8LHQDKQnLYOgiMRF5SbBV6SW3Ra/3+mcbuece+aeOcfsC8O5zuM739/M/GZ+M0I6KAf6gHlN/UBlSn1bQzkwA2Rz0gxQtoa6jNGHCB9EhJcBQ5r3YA11GWMeEe0d/d2aN2urkw22iELwXb9FPmU/UujfGnqQ0R9C/KUcGNa8njXU9RdG+duRTdOTuCL8ptsUWQscEFPLJksioHAhVgYiDWdPBTZnxNYSKwg2ZuSpBY7Yzm4Tzg6UVP1Q/Dc+kqQh6zbi9S6VKBGv1aVlE15hUSLedWFIlIh3XTi7I9BGCJQ6vCPcT3DE2+dT/59BIyJqSv+uAr7g7+wVWmdK8xpTVRqCDPAWEdXuyS9DHHtOUx+uEWjdrLbNpKI0Dy4igt4BxQbtNgNvtG1nArqMcARYAX4CDQW0b9C2K8q1JigGXiMj2h2Dp1s5XmM2o9ZwRQVMAltj8JQA75XrsgVdRqhDXkBWgeMW+Oo9fEct8EVCBtdJr1nk7cLdxbZY5A3EDeK/muRL15M2ogGZ/qQNWaWwXTASMshZkQWuJtWJcjvnUiIH5eWkO1AU4/rgRdvkNcihFbSrHAJGgGVNw0B1jP6OaV8rwOEYPH9gA/AKGaGbPuWHcO8f3jRHPGNuKc9LLF0HzijhR/wPvhEtH0WCwgpgDDeMLxTbgE/KczoGDwClwGclO+lTXgQsafl+T36F5n0j3mieUp5PqqVgXFKiZwGCvIZ4Q/RKgg1pAcaBRWBBfzcH9F8EPFeuSwVZAOwAviJOVxtSz7n5jSEGVAKPcB8fvHBCfr8UFMrXqoavqskYHdrBQJ561Yhj5wqbBQ546rVo/hJwHtipqQ13VoNmZkDLO0yNKMV9l6qPUL8acewlZDkN5hgB8Fj5zvu0d26L4wH89bhX5ZIIen7jnDZ8YdIoD5wteqdP2S4tmw9p/0LrnPUrDHoOatXvvWgaU8F9/baG1srBNGL9HotCxpWzzafsAuFLC2Cv1pk26dRxvlh7dw6acZ29HVlOuxAjlgl3dpAYzGkfGZPaKGzbLQSdmG+/Dg5qvQ8mHd7RRr2mSiOgGVlCC+Q/EL3oVU23TTrbj5y8zguJzSVmilLgrmpZBPaZErQgI5ZFnj+7gCbkBdHmP1FzsUn7aNI+nafXBaLNnC9qgAmSv9rmSxPkuZdEjUzrgBPICVsFbAc2RmxrilXkBH+HBKsPkTtJKH4B042N7RpiCBAAAAAASUVORK5CYII='
     sg.set_options(icon=icon)
     theme = get_theme()
     if not theme:
         theme = sg.OFFICIAL_PYSIMPLEGUI_THEME
     sg.theme(theme)
     # First the window layout...2 columns
 
@@ -753,9 +753,8 @@
         sg.Print('WHOA!  Exception in the main event loop', e, wait=True)
     window.close()
 
 
 
 
 if __name__ == '__main__':
-    icon = b'iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAYAAAAeP4ixAAAABmJLR0QA/wD/AP+gvaeTAAADv0lEQVRogd2Zy0tVQRzHP1bkDa1NtCgtolQIKwlcCJYtFRRsX0S7+gPS9tqDFlmLHhi1lhSF8LHQDKQnLYOgiMRF5SbBV6SW3Ra/3+mcbuece+aeOcfsC8O5zuM739/M/GZ+M0I6KAf6gHlN/UBlSn1bQzkwA2Rz0gxQtoa6jNGHCB9EhJcBQ5r3YA11GWMeEe0d/d2aN2urkw22iELwXb9FPmU/UujfGnqQ0R9C/KUcGNa8njXU9RdG+duRTdOTuCL8ptsUWQscEFPLJksioHAhVgYiDWdPBTZnxNYSKwg2ZuSpBY7Yzm4Tzg6UVP1Q/Dc+kqQh6zbi9S6VKBGv1aVlE15hUSLedWFIlIh3XTi7I9BGCJQ6vCPcT3DE2+dT/59BIyJqSv+uAr7g7+wVWmdK8xpTVRqCDPAWEdXuyS9DHHtOUx+uEWjdrLbNpKI0Dy4igt4BxQbtNgNvtG1nArqMcARYAX4CDQW0b9C2K8q1JigGXiMj2h2Dp1s5XmM2o9ZwRQVMAltj8JQA75XrsgVdRqhDXkBWgeMW+Oo9fEct8EVCBtdJr1nk7cLdxbZY5A3EDeK/muRL15M2ogGZ/qQNWaWwXTASMshZkQWuJtWJcjvnUiIH5eWkO1AU4/rgRdvkNcihFbSrHAJGgGVNw0B1jP6OaV8rwOEYPH9gA/AKGaGbPuWHcO8f3jRHPGNuKc9LLF0HzijhR/wPvhEtH0WCwgpgDDeMLxTbgE/KczoGDwClwGclO+lTXgQsafl+T36F5n0j3mieUp5PqqVgXFKiZwGCvIZ4Q/RKgg1pAcaBRWBBfzcH9F8EPFeuSwVZAOwAviJOVxtSz7n5jSEGVAKPcB8fvHBCfr8UFMrXqoavqskYHdrBQJ561Yhj5wqbBQ546rVo/hJwHtipqQ13VoNmZkDLO0yNKMV9l6qPUL8acewlZDkN5hgB8Fj5zvu0d26L4wH89bhX5ZIIen7jnDZ8YdIoD5wteqdP2S4tmw9p/0LrnPUrDHoOatXvvWgaU8F9/baG1srBNGL9HotCxpWzzafsAuFLC2Cv1pk26dRxvlh7dw6acZ29HVlOuxAjlgl3dpAYzGkfGZPaKGzbLQSdmG+/Dg5qvQ8mHd7RRr2mSiOgGVlCC+Q/EL3oVU23TTrbj5y8zguJzSVmilLgrmpZBPaZErQgI5ZFnj+7gCbkBdHmP1FzsUn7aNI+nafXBaLNnC9qgAmSv9rmSxPkuZdEjUzrgBPICVsFbAc2RmxrilXkBH+HBKsPkTtJKH4B042N7RpiCBAAAAAASUVORK5CYII='
     main()
```

### Comparing `psgtest-3.0.1/psgtest/psgtest_icon.ico` & `psgtest-3.0.2/psgtest/psgtest_icon.ico`

 * *Files identical despite different names*

### Comparing `psgtest-3.0.1/psgtest/psgtest_icon.png` & `psgtest-3.0.2/psgtest/psgtest_icon.png`

 * *Files identical despite different names*

### Comparing `psgtest-3.0.1/psgtest.egg-info/PKG-INFO` & `psgtest-3.0.2/psgtest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psgtest
-Version: 3.0.1
+Version: 3.0.2
 Summary: Run your Python programs, capture the output, using your choice of interpreters
 Home-page: https://github.com/PySimpleGUI/psgtest
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Description: 
         <p align="center">
```

### Comparing `psgtest-3.0.1/README.md` & `psgtest-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `psgtest-3.0.1/setup.py` & `psgtest-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             return f.read()
     except IOError:
         return ''
 
 
 setuptools.setup(
     name="psgtest",
-    version="3.0.1",
+    version="3.0.2",
     author="PySimpleGUI",
     author_email="PySimpleGUI@PySimpleGUI.org",
     description="Run your Python programs, capture the output, using your choice of interpreters",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/PySimpleGUI/psgtest",
     packages=['psgtest'],
```

