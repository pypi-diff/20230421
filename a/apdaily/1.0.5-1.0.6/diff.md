# Comparing `tmp/apdaily-1.0.5.tar.gz` & `tmp/apdaily-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apdaily-1.0.5.tar", last modified: Fri Apr 21 00:42:27 2023, max compression
+gzip compressed data, was "apdaily-1.0.6.tar", last modified: Fri Apr 21 04:05:35 2023, max compression
```

## Comparing `apdaily-1.0.5.tar` & `apdaily-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:27.363017 apdaily-1.0.5/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)     1162 2023-04-21 00:42:27.363017 apdaily-1.0.5/PKG-INFO
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      839 2023-04-21 00:39:50.000000 apdaily-1.0.5/README.md
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      103 2023-04-20 17:56:45.000000 apdaily-1.0.5/pyproject.toml
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      712 2023-04-21 00:42:27.372343 apdaily-1.0.5/setup.cfg
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:26.409519 apdaily-1.0.5/src/
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:26.620464 apdaily-1.0.5/src/apdaily/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.5/src/apdaily/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      143 2023-04-20 17:56:45.000000 apdaily-1.0.5/src/apdaily/main.py
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:26.943417 apdaily-1.0.5/src/apdaily.egg-info/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)     1162 2023-04-21 00:42:25.000000 apdaily-1.0.5/src/apdaily.egg-info/PKG-INFO
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      428 2023-04-21 00:42:26.000000 apdaily-1.0.5/src/apdaily.egg-info/SOURCES.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        1 2023-04-21 00:42:25.000000 apdaily-1.0.5/src/apdaily.egg-info/dependency_links.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)       12 2023-04-21 00:42:25.000000 apdaily-1.0.5/src/apdaily.egg-info/requires.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)       40 2023-04-21 00:42:25.000000 apdaily-1.0.5/src/apdaily.egg-info/top_level.txt
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:27.186131 apdaily-1.0.5/src/apdaily_methods/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.5/src/apdaily_methods/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)     3487 2023-04-21 00:42:10.000000 apdaily-1.0.5/src/apdaily_methods/apdaily_m1.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      334 2023-04-21 00:42:02.000000 apdaily-1.0.5/src/apdaily_methods/mouse_util.py
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:42:27.310748 apdaily-1.0.5/src/apdaily_startup/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.5/src/apdaily_startup/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)     4567 2023-04-21 00:27:23.000000 apdaily-1.0.5/src/apdaily_startup/apdaily_startup_main.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:05:35.751543 apdaily-1.0.6/
+-rw-rw-rw-   0        0        0     1153 2023-04-21 04:05:35.751543 apdaily-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-04-21 00:39:50.000000 apdaily-1.0.6/README.md
+-rw-rw-rw-   0        0        0      103 2023-04-20 17:56:45.000000 apdaily-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      693 2023-04-21 04:05:35.754479 apdaily-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 04:05:35.674878 apdaily-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 04:05:35.692667 apdaily-1.0.6/src/apdaily/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:56:45.000000 apdaily-1.0.6/src/apdaily/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-04-20 17:56:45.000000 apdaily-1.0.6/src/apdaily/main.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:05:35.741464 apdaily-1.0.6/src/apdaily.egg-info/
+-rw-rw-rw-   0        0        0     1153 2023-04-21 04:05:35.000000 apdaily-1.0.6/src/apdaily.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-04-21 04:05:35.000000 apdaily-1.0.6/src/apdaily.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:05:35.000000 apdaily-1.0.6/src/apdaily.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 04:05:35.000000 apdaily-1.0.6/src/apdaily.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       40 2023-04-21 04:05:35.000000 apdaily-1.0.6/src/apdaily.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 04:05:35.746500 apdaily-1.0.6/src/apdaily_methods/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:56:45.000000 apdaily-1.0.6/src/apdaily_methods/__init__.py
+-rw-rw-rw-   0        0        0     3487 2023-04-21 00:42:10.000000 apdaily-1.0.6/src/apdaily_methods/apdaily_m1.py
+-rw-rw-rw-   0        0        0      334 2023-04-21 00:42:02.000000 apdaily-1.0.6/src/apdaily_methods/mouse_util.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:05:35.749508 apdaily-1.0.6/src/apdaily_startup/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:56:45.000000 apdaily-1.0.6/src/apdaily_startup/__init__.py
+-rw-rw-rw-   0        0        0     4567 2023-04-21 00:27:23.000000 apdaily-1.0.6/src/apdaily_startup/apdaily_startup_main.py
```

### Comparing `apdaily-1.0.5/PKG-INFO` & `apdaily-1.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1
-Name: apdaily
-Version: 1.0.5
-Summary: A package that allows you to watch AP Classroom Daily videos automatically.
-Home-page: https://github.com/SarangaR/APDaily-Dev
-Author: Saranga Rajagopalan
-Author-email: sarnga.raj@gmail.com
-License: : OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# APDaily
-This package allows you to watch AP Classroom Videos automatically.
-## Authors
-- [@SarangaR](https://www.github.com/SarangaR)
-## Installation
-- Install the apdaily package with pip
-```bash
-  pip install apdaily
-```
-- Then copy the ```src/scripts``` folder from this repository and run the install script
-#### Linux
-```bash
-  sudo ./scripts/apdaily-setup.sh
-```
-#### Windows
-In an administrator command prompt:
-```cmd
-  scripts/apdaily-setup.bat
-```
-
-## Settings
- - Use the mouse_util script to set the mouse positions in the config file
- ```Python
- import apdaily_methods.mouse_util as mouse_util
- mouse_util.run()
- ```
- - Update the other portions of the config.toml file included in the ```src/scripts``` folder of this repo (same place as the install script)
- - Then re-run the install script
- 
-
+Metadata-Version: 2.1
+Name: apdaily
+Version: 1.0.6
+Summary: A package that allows you to watch AP Classroom Daily videos automatically.
+Home-page: https://github.com/SarangaR/APDaily-Dev
+Author: Fdhsy
+License: : OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# APDaily
+This package allows you to watch AP Classroom Videos automatically.
+## Authors
+- [@SarangaR](https://www.github.com/SarangaR)
+## Installation
+- Install the apdaily package with pip
+```bash
+  pip install apdaily
+```
+- Then copy the ```src/scripts``` folder from this repository and run the install script
+#### Linux
+```bash
+  sudo ./scripts/apdaily-setup.sh
+```
+#### Windows
+In an administrator command prompt:
+```cmd
+  scripts/apdaily-setup.bat
+```
+
+## Settings
+ - Use the mouse_util script to set the mouse positions in the config file
+ ```Python
+ import apdaily_methods.mouse_util as mouse_util
+ mouse_util.run()
+ ```
+ - Update the other portions of the config.toml file included in the ```src/scripts``` folder of this repo (same place as the install script)
+ - Then re-run the install script
+ 
+
```

### Comparing `apdaily-1.0.5/README.md` & `apdaily-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `apdaily-1.0.5/setup.cfg` & `apdaily-1.0.6/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6170 6461 696c 790a 7665 7273 696f  = apdaily.versio
-00000020: 6e20 3d20 312e 302e 350a 6175 7468 6f72  n = 1.0.5.author
-00000030: 203d 2053 6172 616e 6761 2052 616a 6167   = Saranga Rajag
-00000040: 6f70 616c 616e 0a61 7574 686f 725f 656d  opalan.author_em
-00000050: 6169 6c20 3d20 7361 726e 6761 2e72 616a  ail = sarnga.raj
-00000060: 4067 6d61 696c 2e63 6f6d 0a64 6573 6372  @gmail.com.descr
-00000070: 6970 7469 6f6e 203d 2041 2070 6163 6b61  iption = A packa
-00000080: 6765 2074 6861 7420 616c 6c6f 7773 2079  ge that allows y
-00000090: 6f75 2074 6f20 7761 7463 6820 4150 2043  ou to watch AP C
-000000a0: 6c61 7373 726f 6f6d 2044 6169 6c79 2076  lassroom Daily v
-000000b0: 6964 656f 7320 6175 746f 6d61 7469 6361  ideos automatica
-000000c0: 6c6c 792e 0a6c 6f6e 675f 6465 7363 7269  lly..long_descri
-000000d0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-000000e0: 4144 4d45 2e6d 640a 6c6f 6e67 5f64 6573  ADME.md.long_des
-000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000110: 6b64 6f77 6e0a 7572 6c20 3d20 6874 7470  kdown.url = http
-00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-00000130: 6172 616e 6761 522f 4150 4461 696c 792d  arangaR/APDaily-
-00000140: 4465 760a 7072 6f6a 6563 745f 7572 6c73  Dev.project_urls
-00000150: 203d 200a 4275 6720 5472 6163 6b65 7220   = .Bug Tracker 
-00000160: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000170: 2e63 6f6d 2f53 6172 616e 6761 522f 4150  .com/SarangaR/AP
-00000180: 4461 696c 792d 4465 762f 6973 7375 6573  Daily-Dev/issues
-00000190: 0a63 6c61 7373 6966 6965 7273 203d 200a  .classifiers = .
-000001a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001b0: 7561 6765 203d 203a 2050 7974 686f 6e20  uage = : Python 
-000001c0: 3a3a 2033 0a4c 6963 656e 7365 203d 203a  :: 3.License = :
-000001d0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000001e0: 204d 4954 204c 6963 656e 7365 0a4f 7065   MIT License.Ope
-000001f0: 7261 7469 6e67 2053 7973 7465 6d20 3d20  rating System = 
-00000200: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000210: 0a0a 5b6f 7074 696f 6e73 5d0a 7061 636b  ..[options].pack
-00000220: 6167 655f 6469 7220 3d20 0a09 3d73 7263  age_dir = ..=src
-00000230: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000240: 3a0a 7079 7468 6f6e 5f72 6571 7569 7265  :.python_require
-00000250: 7320 3d20 3e3d 332e 360a 696e 7374 616c  s = >=3.6.instal
-00000260: 6c5f 7265 7175 6972 6573 203d 200a 0970  l_requires = ..p
-00000270: 796e 7075 740a 0974 6f6d 6c0a 0a5b 6f70  ynput..toml..[op
-00000280: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000290: 696e 645d 0a77 6865 7265 203d 2073 7263  ind].where = src
-000002a0: 0a0a 5b65 6767 5f69 6e66 6f5d 0a74 6167  ..[egg_info].tag
-000002b0: 5f62 7569 6c64 203d 200a 7461 675f 6461  _build = .tag_da
-000002c0: 7465 203d 2030 0a0a                      te = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2061 7064 6169 6c79 0d0a 7665 7273   = apdaily..vers
+00000020: 696f 6e20 3d20 312e 302e 360d 0a61 7574  ion = 1.0.6..aut
+00000030: 686f 7220 3d20 4664 6873 790d 0a64 6573  hor = Fdhsy..des
+00000040: 6372 6970 7469 6f6e 203d 2041 2070 6163  cription = A pac
+00000050: 6b61 6765 2074 6861 7420 616c 6c6f 7773  kage that allows
+00000060: 2079 6f75 2074 6f20 7761 7463 6820 4150   you to watch AP
+00000070: 2043 6c61 7373 726f 6f6d 2044 6169 6c79   Classroom Daily
+00000080: 2076 6964 656f 7320 6175 746f 6d61 7469   videos automati
+00000090: 6361 6c6c 792e 0d0a 6c6f 6e67 5f64 6573  cally...long_des
+000000a0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000b0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
+000000c0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+000000d0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+000000e0: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
+000000f0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000100: 636f 6d2f 5361 7261 6e67 6152 2f41 5044  com/SarangaR/APD
+00000110: 6169 6c79 2d44 6576 0d0a 7072 6f6a 6563  aily-Dev..projec
+00000120: 745f 7572 6c73 203d 200d 0a42 7567 2054  t_urls = ..Bug T
+00000130: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
+00000140: 2f67 6974 6875 622e 636f 6d2f 5361 7261  /github.com/Sara
+00000150: 6e67 6152 2f41 5044 6169 6c79 2d44 6576  ngaR/APDaily-Dev
+00000160: 2f69 7373 7565 730d 0a63 6c61 7373 6966  /issues..classif
+00000170: 6965 7273 203d 200d 0a50 726f 6772 616d  iers = ..Program
+00000180: 6d69 6e67 204c 616e 6775 6167 6520 3d20  ming Language = 
+00000190: 3a20 5079 7468 6f6e 203a 3a20 330d 0a4c  : Python :: 3..L
+000001a0: 6963 656e 7365 203d 203a 204f 5349 2041  icense = : OSI A
+000001b0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000001c0: 6963 656e 7365 0d0a 4f70 6572 6174 696e  icense..Operatin
+000001d0: 6720 5379 7374 656d 203d 203a 204f 5320  g System = : OS 
+000001e0: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
+000001f0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+00000200: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
+00000210: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000220: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+00000230: 6573 203d 203e 3d33 2e36 0d0a 696e 7374  es = >=3.6..inst
+00000240: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000250: 0a09 7079 6e70 7574 0d0a 0974 6f6d 6c0d  ..pynput...toml.
+00000260: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000270: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000280: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
+00000290: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+000002a0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000002b0: 300d 0a0d 0a                             0....
```

### Comparing `apdaily-1.0.5/src/apdaily.egg-info/PKG-INFO` & `apdaily-1.0.6/src/apdaily.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1
-Name: apdaily
-Version: 1.0.5
-Summary: A package that allows you to watch AP Classroom Daily videos automatically.
-Home-page: https://github.com/SarangaR/APDaily-Dev
-Author: Saranga Rajagopalan
-Author-email: sarnga.raj@gmail.com
-License: : OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# APDaily
-This package allows you to watch AP Classroom Videos automatically.
-## Authors
-- [@SarangaR](https://www.github.com/SarangaR)
-## Installation
-- Install the apdaily package with pip
-```bash
-  pip install apdaily
-```
-- Then copy the ```src/scripts``` folder from this repository and run the install script
-#### Linux
-```bash
-  sudo ./scripts/apdaily-setup.sh
-```
-#### Windows
-In an administrator command prompt:
-```cmd
-  scripts/apdaily-setup.bat
-```
-
-## Settings
- - Use the mouse_util script to set the mouse positions in the config file
- ```Python
- import apdaily_methods.mouse_util as mouse_util
- mouse_util.run()
- ```
- - Update the other portions of the config.toml file included in the ```src/scripts``` folder of this repo (same place as the install script)
- - Then re-run the install script
- 
-
+Metadata-Version: 2.1
+Name: apdaily
+Version: 1.0.6
+Summary: A package that allows you to watch AP Classroom Daily videos automatically.
+Home-page: https://github.com/SarangaR/APDaily-Dev
+Author: Fdhsy
+License: : OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# APDaily
+This package allows you to watch AP Classroom Videos automatically.
+## Authors
+- [@SarangaR](https://www.github.com/SarangaR)
+## Installation
+- Install the apdaily package with pip
+```bash
+  pip install apdaily
+```
+- Then copy the ```src/scripts``` folder from this repository and run the install script
+#### Linux
+```bash
+  sudo ./scripts/apdaily-setup.sh
+```
+#### Windows
+In an administrator command prompt:
+```cmd
+  scripts/apdaily-setup.bat
+```
+
+## Settings
+ - Use the mouse_util script to set the mouse positions in the config file
+ ```Python
+ import apdaily_methods.mouse_util as mouse_util
+ mouse_util.run()
+ ```
+ - Update the other portions of the config.toml file included in the ```src/scripts``` folder of this repo (same place as the install script)
+ - Then re-run the install script
+ 
+
```

### Comparing `apdaily-1.0.5/src/apdaily_methods/apdaily_m1.py` & `apdaily-1.0.6/src/apdaily_methods/apdaily_m1.py`

 * *Files identical despite different names*

### Comparing `apdaily-1.0.5/src/apdaily_startup/apdaily_startup_main.py` & `apdaily-1.0.6/src/apdaily_startup/apdaily_startup_main.py`

 * *Files identical despite different names*

