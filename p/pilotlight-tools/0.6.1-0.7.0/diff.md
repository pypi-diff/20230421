# Comparing `tmp/pilotlight_tools-0.6.1.tar.gz` & `tmp/pilotlight_tools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilotlight_tools-0.6.1.tar", last modified: Thu Feb 16 06:15:58 2023, max compression
+gzip compressed data, was "pilotlight_tools-0.7.0.tar", last modified: Fri Apr 21 03:53:16 2023, max compression
```

## Comparing `pilotlight_tools-0.6.1.tar` & `pilotlight_tools-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 06:15:58.100088 pilotlight_tools-0.6.1/
--rw-rw-rw-   0        0        0     1087 2023-02-16 06:15:06.000000 pilotlight_tools-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     3576 2023-02-16 06:15:58.100088 pilotlight_tools-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2532 2023-02-16 06:15:06.000000 pilotlight_tools-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-16 06:15:58.100088 pilotlight_tools-0.6.1/pilotlight_tools/
--rw-rw-rw-   0        0        0        7 2023-02-16 06:15:41.000000 pilotlight_tools-0.6.1/pilotlight_tools/__init__.py
--rw-rw-rw-   0        0        0   103588 2023-02-16 06:15:06.000000 pilotlight_tools-0.6.1/pilotlight_tools/pl_build.py
-drwxrwxrwx   0        0        0        0 2023-02-16 06:15:58.100088 pilotlight_tools-0.6.1/pilotlight_tools.egg-info/
--rw-rw-rw-   0        0        0     3576 2023-02-16 06:15:58.000000 pilotlight_tools-0.6.1/pilotlight_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-02-16 06:15:58.000000 pilotlight_tools-0.6.1/pilotlight_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 06:15:58.000000 pilotlight_tools-0.6.1/pilotlight_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-02-16 06:15:58.000000 pilotlight_tools-0.6.1/pilotlight_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       96 2023-02-16 06:15:41.000000 pilotlight_tools-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-16 06:15:58.100088 pilotlight_tools-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1811 2023-02-16 06:15:06.000000 pilotlight_tools-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-21 03:52:28.000000 pilotlight_tools-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     3766 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2721 2023-04-21 03:52:28.000000 pilotlight_tools-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/pilotlight_tools/
+-rw-rw-rw-   0        0        0        7 2023-04-21 03:52:55.000000 pilotlight_tools-0.7.0/pilotlight_tools/__init__.py
+-rw-rw-rw-   0        0        0   103746 2023-04-21 03:52:28.000000 pilotlight_tools-0.7.0/pilotlight_tools/pl_build.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/
+-rw-rw-rw-   0        0        0     3766 2023-04-21 03:53:16.000000 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-21 03:53:16.000000 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 03:53:16.000000 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 03:53:16.000000 pilotlight_tools-0.7.0/pilotlight_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       96 2023-04-21 03:52:55.000000 pilotlight_tools-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 03:53:16.367242 pilotlight_tools-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1811 2023-04-21 03:52:28.000000 pilotlight_tools-0.7.0/setup.py
```

### Comparing `pilotlight_tools-0.6.1/LICENSE` & `pilotlight_tools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pilotlight_tools-0.6.1/PKG-INFO` & `pilotlight_tools-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilotlight_tools
-Version: 0.6.1
+Version: 0.7.0
 Summary: Pilot Light Tools
 Home-page: https://github.com/pilot-light/pilotlight
 Author: Jonathan Hoffstadt
 Author-email: pilot_light@yahoo.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -31,14 +31,15 @@
 <p align="center">A lightweight game engine with minimal dependencies.</p>
 
 <h1></h1>
 
 <p align="center">
    <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Build"><img src="https://github.com/pilot-light/pilotlight/workflows/Build/badge.svg?branch=master" alt="build"></a>
    <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Static%20Analysis"><img src="https://github.com/pilot-light/pilotlight/workflows/Static%20Analysis/badge.svg?branch=master" alt="static-analysis"></a>
+   <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Tests"><img src="https://github.com/pilot-light/pilotlight/workflows/Tests/badge.svg?branch=master" alt="tests"></a>
 </p>
 
 <p align="center">
   <a href="#information">Information</a> •
   <a href="#developer-notes">Developer Notes</a> • 
   <a href="#license">License</a> •
   <a href="#gallery">Gallery</a> •
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pilotlight_tools Version: 0.6.1 Summary: Pilot
+Metadata-Version: 2.1 Name: pilotlight_tools Version: 0.7.0 Summary: Pilot
 Light Tools Home-page: https://github.com/pilot-light/pilotlight Author:
 Jonathan Hoffstadt Author-email: pilot_light@yahoo.com License: MIT Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows :: Windows 10 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE
                            ****** Pilot Light ******
              A lightweight game engine with minimal dependencies.
-                           [build] [static-analysis]
+                       [build] [static-analysis] [tests]
     Information â¢ Developer_Notes â¢ License â¢ Gallery â¢ Inspiration
 ## Information The plan for _Pilot Light_ is to be collection of "[stb](https:/
 /github.com/nothings/stb) style" libraries that culminate into a lightweight
 game engine. Ideally all of the libraries would be completely standalone but
 this isn't practical for the larger systems so some will rely on others. Once a
 library is completely standalone, it is moved in the _libs_ directory. Beware,
 this project is still in the early stages. ## Developer Notes Information for
```

### Comparing `pilotlight_tools-0.6.1/README.md` & `pilotlight_tools-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 <p align="center">A lightweight game engine with minimal dependencies.</p>
 
 <h1></h1>
 
 <p align="center">
    <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Build"><img src="https://github.com/pilot-light/pilotlight/workflows/Build/badge.svg?branch=master" alt="build"></a>
    <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Static%20Analysis"><img src="https://github.com/pilot-light/pilotlight/workflows/Static%20Analysis/badge.svg?branch=master" alt="static-analysis"></a>
+   <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Tests"><img src="https://github.com/pilot-light/pilotlight/workflows/Tests/badge.svg?branch=master" alt="tests"></a>
 </p>
 
 <p align="center">
   <a href="#information">Information</a> •
   <a href="#developer-notes">Developer Notes</a> • 
   <a href="#license">License</a> •
   <a href="#gallery">Gallery</a> •
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                            ****** Pilot Light ******
              A lightweight game engine with minimal dependencies.
-                           [build] [static-analysis]
+                       [build] [static-analysis] [tests]
     Information â¢ Developer_Notes â¢ License â¢ Gallery â¢ Inspiration
 ## Information The plan for _Pilot Light_ is to be collection of "[stb](https:/
 /github.com/nothings/stb) style" libraries that culminate into a lightweight
 game engine. Ideally all of the libraries would be completely standalone but
 this isn't practical for the larger systems so some will rely on others. Once a
 library is completely standalone, it is moved in the _libs_ directory. Beware,
 this project is still in the early stages. ## Developer Notes Information for
```

### Comparing `pilotlight_tools-0.6.1/pilotlight_tools/pl_build.py` & `pilotlight_tools-0.7.0/pilotlight_tools/pl_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.1"
+__version__ = "0.7.0"
 
 ###############################################################################
 #                                  Info                                       #
 ###############################################################################
 
 # very poorly written & dirty system, to be cleaned up later
 
@@ -593,15 +593,15 @@
                 add_compiler_flags("--debug", "-g")
                 add_linker_flags("dl", "m")
                 set_output_directory(None)
                 set_output_binary(None)
 
         with platform(PlatformType.MACOS):
             with compiler("clang", CompilerType.CLANG):
-                add_compiler_flags("-std=c++17", "--debug", "-g", "-fmodules", "-ObjC")
+                add_compiler_flags("-std=c++17", "--debug", "-g", "-fmodules")
                 add_frameworks("Metal", "MetalKit", "Cocoa", "IOKit", "CoreVideo", "QuartzCore")
                 set_output_directory(None)
                 set_output_binary(None)
 
 ###############################################################################
 #                               Generation                                    #
 ###############################################################################
@@ -632,14 +632,16 @@
                                 if settings._compiler_type == CompilerType.MSVC:
                                     settings._output_binary_extension = ".lib"
                                 else :
                                     settings._output_binary_extension = ".o"
                             elif target._target_type == TargetType.DYNAMIC_LIBRARY:
                                 if settings._compiler_type == CompilerType.MSVC:
                                     settings._output_binary_extension = ".dll"
+                                elif settings._compiler_type == CompilerType.CLANG:
+                                    settings._output_binary_extension = ".dylib"
                                 else :
                                     settings._output_binary_extension = ".so"
                             elif target._target_type == TargetType.EXECUTABLE:
                                 if settings._compiler_type == CompilerType.MSVC:
                                     settings._output_binary_extension = ".exe"
                                 else :
                                     settings._output_binary_extension = ""
```

### Comparing `pilotlight_tools-0.6.1/pilotlight_tools.egg-info/PKG-INFO` & `pilotlight_tools-0.7.0/pilotlight_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilotlight-tools
-Version: 0.6.1
+Version: 0.7.0
 Summary: Pilot Light Tools
 Home-page: https://github.com/pilot-light/pilotlight
 Author: Jonathan Hoffstadt
 Author-email: pilot_light@yahoo.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -31,14 +31,15 @@
 <p align="center">A lightweight game engine with minimal dependencies.</p>
 
 <h1></h1>
 
 <p align="center">
    <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Build"><img src="https://github.com/pilot-light/pilotlight/workflows/Build/badge.svg?branch=master" alt="build"></a>
    <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Static%20Analysis"><img src="https://github.com/pilot-light/pilotlight/workflows/Static%20Analysis/badge.svg?branch=master" alt="static-analysis"></a>
+   <a href="https://github.com/pilot-light/pilotlight/actions?workflow=Tests"><img src="https://github.com/pilot-light/pilotlight/workflows/Tests/badge.svg?branch=master" alt="tests"></a>
 </p>
 
 <p align="center">
   <a href="#information">Information</a> •
   <a href="#developer-notes">Developer Notes</a> • 
   <a href="#license">License</a> •
   <a href="#gallery">Gallery</a> •
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pilotlight-tools Version: 0.6.1 Summary: Pilot
+Metadata-Version: 2.1 Name: pilotlight-tools Version: 0.7.0 Summary: Pilot
 Light Tools Home-page: https://github.com/pilot-light/pilotlight Author:
 Jonathan Hoffstadt Author-email: pilot_light@yahoo.com License: MIT Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows :: Windows 10 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE
                            ****** Pilot Light ******
              A lightweight game engine with minimal dependencies.
-                           [build] [static-analysis]
+                       [build] [static-analysis] [tests]
     Information â¢ Developer_Notes â¢ License â¢ Gallery â¢ Inspiration
 ## Information The plan for _Pilot Light_ is to be collection of "[stb](https:/
 /github.com/nothings/stb) style" libraries that culminate into a lightweight
 game engine. Ideally all of the libraries would be completely standalone but
 this isn't practical for the larger systems so some will rely on others. Once a
 library is completely standalone, it is moved in the _libs_ directory. Beware,
 this project is still in the early stages. ## Developer Notes Information for
```

### Comparing `pilotlight_tools-0.6.1/setup.py` & `pilotlight_tools-0.7.0/setup.py`

 * *Files identical despite different names*

