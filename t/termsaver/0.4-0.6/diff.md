# Comparing `tmp/termsaver-0.4.tar.gz` & `tmp/termsaver-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/termsaver-0.4.tar", last modified: Wed Jul 18 23:41:21 2018, max compression
+gzip compressed data, was "termsaver-0.6.tar", last modified: Fri Apr 21 00:44:25 2023, max compression
```

## Comparing `termsaver-0.4.tar` & `termsaver-0.6.tar`

### file list

```diff
@@ -1,59 +1,49 @@
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/doc/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3252 2018-07-18 04:20:19.000000 termsaver-0.4/doc/termsaver.1
--rw-r--r--   0 bruno     (1000) bruno     (1000)      839 2018-07-18 23:41:21.000000 termsaver-0.4/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1083 2018-07-18 03:26:50.000000 termsaver-0.4/MANIFEST.in
--rwxr-xr-x   0 bruno     (1000) bruno     (1000)     3499 2018-07-18 23:17:19.000000 termsaver-0.4/setup.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/locale/
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/locale/ja/
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/locale/ja/LC_MESSAGES/
--rw-r--r--   0 bruno     (1000) bruno     (1000)      528 2018-07-18 03:26:50.000000 termsaver-0.4/locale/ja/LC_MESSAGES/termsaver.mo
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/locale/en/
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/locale/en/LC_MESSAGES/
--rw-r--r--   0 bruno     (1000) bruno     (1000)    12747 2018-07-18 03:26:50.000000 termsaver-0.4/locale/en/LC_MESSAGES/termsaver.mo
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/locale/pt/
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/locale/pt/LC_MESSAGES/
--rw-r--r--   0 bruno     (1000) bruno     (1000)      378 2018-07-18 03:26:50.000000 termsaver-0.4/locale/pt/LC_MESSAGES/termsaver.mo
--rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2018-07-18 23:41:21.000000 termsaver-0.4/setup.cfg
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/termsaver.egg-info/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       13 2018-07-18 23:41:21.000000 termsaver-0.4/termsaver.egg-info/top_level.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)      839 2018-07-18 23:41:21.000000 termsaver-0.4/termsaver.egg-info/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1232 2018-07-18 23:41:21.000000 termsaver-0.4/termsaver.egg-info/SOURCES.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2018-07-18 23:41:21.000000 termsaver-0.4/termsaver.egg-info/dependency_links.txt
--rwxr-xr-x   0 bruno     (1000) bruno     (1000)     8008 2018-07-18 03:26:50.000000 termsaver-0.4/termsaver
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/completion/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2861 2018-07-18 03:26:50.000000 termsaver-0.4/completion/_termsaver
--rw-r--r--   0 bruno     (1000) bruno     (1000)      408 2018-07-18 03:26:50.000000 termsaver-0.4/completion/termsaver-completion.bash
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/termsaverlib/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     8038 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/common.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/termsaverlib/screen/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3052 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/asciiartfarts.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     6346 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/randtxt.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3035 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/jokes4all.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2181 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/urlfetcher.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4209 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/rfc.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    13704 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/sysmon.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3523 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/rssfeed.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     8053 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/clock.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3140 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/quotes4all.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/termsaverlib/screen/base/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     8456 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/base/urlfetcher.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    13186 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/base/filereader.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    11889 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/base/rssfeed.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    12282 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/base/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3177 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/programmer.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/termsaverlib/screen/helper/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     6680 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/helper/urlfetcher.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    11484 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/helper/position.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3939 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/helper/typing.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2518 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/helper/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     6975 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/helper/xmlreader.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3795 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    14019 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/screen/matrix.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5539 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/exception.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2018-07-18 23:41:21.000000 termsaver-0.4/termsaverlib/plugins/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4249 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/plugins/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3477 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/constants.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1902 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/i18n.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1638 2018-07-18 03:26:50.000000 termsaver-0.4/termsaverlib/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     8076 2018-07-18 04:32:08.000000 termsaver-0.4/README
+-rw-r--r--   0        0        0    11609 2023-02-06 15:23:26.427148 termsaver-0.6/LICENSE
+-rw-r--r--   0        0        0     7934 2023-02-08 01:13:09.696063 termsaver-0.6/README.md
+-rw-r--r--   0        0        0      750 2023-04-21 00:44:25.645660 termsaver-0.6/pyproject.toml
+-rw-r--r--   0        0        0    11248 2023-04-21 00:05:45.797612 termsaver-0.6/termsaver/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-08 01:47:38.876905 termsaver-0.6/termsaver/__main__.py
+-rw-r--r--   0        0        0  2046847 2023-02-08 01:13:09.713067 termsaver-0.6/termsaver/data/sw1.txt
+-rw-r--r--   0        0        0     1682 2023-02-08 01:13:09.699063 termsaver-0.6/termsaver/termsaverlib/__init__.py
+-rw-r--r--   0        0        0     8477 2023-02-08 01:13:09.700063 termsaver-0.6/termsaver/termsaverlib/common.py
+-rw-r--r--   0        0        0     3647 2023-02-08 01:13:09.700063 termsaver-0.6/termsaver/termsaverlib/constants.py
+-rw-r--r--   0        0        0     5889 2023-02-08 01:13:09.702064 termsaver-0.6/termsaver/termsaverlib/exception.py
+-rw-r--r--   0        0        0     1211 2023-02-08 01:13:09.701063 termsaver-0.6/termsaver/termsaverlib/helper/__init__.py
+-rw-r--r--   0        0        0     1397 2023-02-08 01:13:09.702064 termsaver-0.6/termsaver/termsaverlib/helper/smartformatter.py
+-rw-r--r--   0        0        0     1375 2023-02-08 01:13:09.701063 termsaver-0.6/termsaver/termsaverlib/helper/utilities.py
+-rw-r--r--   0        0        0     1985 2023-02-08 01:13:09.702064 termsaver-0.6/termsaver/termsaverlib/i18n.py
+-rw-r--r--   0        0        0     4614 2023-04-21 00:05:00.093614 termsaver-0.6/termsaver/termsaverlib/plugins/__init__.py
+-rw-r--r--   0        0        0     2994 2023-02-08 01:13:09.704063 termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/constants.py
+-rw-r--r--   0        0        0     1064 2023-02-08 01:13:09.703064 termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/__init__.py
+-rw-r--r--   0        0        0     2077 2023-02-08 01:13:09.703064 termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/base/__init__.py
+-rw-r--r--   0        0        0     3012 2023-02-08 01:13:09.703064 termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/eps.py
+-rw-r--r--   0        0        0     4100 2023-02-13 17:17:10.128732 termsaver-0.6/termsaver/termsaverlib/screen/__init__.py
+-rw-r--r--   0        0        0     4101 2023-02-08 01:13:09.705063 termsaver-0.6/termsaver/termsaverlib/screen/asciiartfarts.py
+-rw-r--r--   0        0        0    12567 2023-04-21 00:05:45.795615 termsaver-0.6/termsaver/termsaverlib/screen/base/__init__.py
+-rw-r--r--   0        0        0    13235 2023-02-08 01:13:09.704063 termsaver-0.6/termsaver/termsaverlib/screen/base/filereader.py
+-rw-r--r--   0        0        0     9617 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/base/rssfeed.py
+-rw-r--r--   0        0        0     5945 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/base/urlfetcher.py
+-rw-r--r--   0        0        0    14623 2023-04-21 00:05:45.794614 termsaver-0.6/termsaver/termsaverlib/screen/clock.py
+-rw-r--r--   0        0        0    53820 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/clocknumber for tremsaver.xlsm
+-rw-r--r--   0        0        0     2608 2023-02-08 01:13:09.705063 termsaver-0.6/termsaver/termsaverlib/screen/helper/__init__.py
+-rw-r--r--   0        0        0     4134 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/helper/imageconverter.py
+-rw-r--r--   0        0        0    12002 2023-04-21 00:05:45.796613 termsaver-0.6/termsaver/termsaverlib/screen/helper/position.py
+-rw-r--r--   0        0        0     4081 2023-02-08 01:13:09.706063 termsaver-0.6/termsaver/termsaverlib/screen/helper/typing.py
+-rw-r--r--   0        0        0     7322 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/helper/urlfetcher.py
+-rw-r--r--   0        0        0     7204 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/helper/xmlreader.py
+-rw-r--r--   0        0        0    16945 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/img2ascii.py
+-rw-r--r--   0        0        0     4643 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/jokes4all.py
+-rw-r--r--   0        0        0    13137 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/matrix.py
+-rw-r--r--   0        0        0     4642 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/programmer.py
+-rw-r--r--   0        0        0     4694 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/quotes4all.py
+-rw-r--r--   0        0        0     6242 2023-02-08 01:13:09.709064 termsaver-0.6/termsaver/termsaverlib/screen/randtxt.py
+-rw-r--r--   0        0        0     4629 2023-02-08 01:13:09.711067 termsaver-0.6/termsaver/termsaverlib/screen/rfc.py
+-rw-r--r--   0        0        0     4217 2023-02-08 01:13:09.711067 termsaver-0.6/termsaver/termsaverlib/screen/rssfeed.py
+-rw-r--r--   0        0        0     4725 2023-02-08 01:13:09.711067 termsaver-0.6/termsaver/termsaverlib/screen/starwars.py
+-rw-r--r--   0        0        0    15328 2023-02-08 01:13:09.711067 termsaver-0.6/termsaver/termsaverlib/screen/sysmon.py
+-rw-r--r--   0        0        0     3307 2023-02-08 01:13:09.709064 termsaver-0.6/termsaver/termsaverlib/screen/urlfetcher.py
+-rw-r--r--   0        0        0     3987 2023-02-08 01:13:09.710066 termsaver-0.6/termsaver/termsaverlib/screen/wttr.py
+-rw-r--r--   0        0        0       20 2023-02-06 15:23:26.441441 termsaver-0.6/tests/empty-for-tests/testfile.txt
+-rw-r--r--   0        0        0    12237 2023-02-08 01:13:09.710066 termsaver-0.6/tests/screentests.py
+-rw-r--r--   0        0        0     6540 2023-02-08 01:13:09.710066 termsaver-0.6/tests/test.py
+-rw-r--r--   0        0        0     8188 1970-01-01 00:00:00.000000 termsaver-0.6/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `termsaver-0.4/MANIFEST.in` & `termsaver-0.6/termsaver/termsaverlib/helper/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-###############################################################################
-#
-# file:     MANIFEST.in
-#
-# Purpose:  required for python packaging
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-
-#
-# Add l10n files to package
-#
-recursive-include locale/ completion/ *.mo
-
+###############################################################################
+#
+# file:     __init__.py
+#
+# Purpose:  refer to package documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+This package holds all helper classes used by termsaverlib, to add
+reusable functionality to them, and help maintain consistency throughout all
+of them.
+"""
```

### Comparing `termsaver-0.4/termsaverlib/common.py` & `termsaver-0.6/termsaver/termsaverlib/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,276 +1,281 @@
-###############################################################################
-#
-# file:     common.py
-#
-# Purpose:  holds common helper functions used by termsaver code.
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-Holds common functionality used by termsaver screens.
-"""
-
-#
-# Python build-in modules
-#
-import os
-import sys
-import traceback
-import HTMLParser
-import subprocess
-import re
-import time
-
-
-def is_windows():
-    """
-    Returns True if the environment is Microsoft Windows.
-    """
-    return sys.platform == "win32"
-
-
-def is_macos():
-    """
-    Returns True if the environment is Microsoft Windows.
-    """
-    return sys.platform == "darwin"
-
-
-def prettify_exception(ex):
-    """
-    Outputs the exception with its stack trace within separator lines.
-    """
-    print """
-===================================
-Exception: (%s) %s
-%s
-===================================
-""" % (ex.__class__.__name__, ex.message, traceback.format_exc())
-
-
-def get_app_dir():
-    """
-    Retrieves the termsaver main directory based on current operating system.
-
-    For Windows machines, this should be something like:
-
-        <root>\Documents and Settings\<user>\Application Data\termsaver
-
-    For Unix machines, it will be:
-
-        /home/<user>/.termsaver/
-    """
-    if is_windows():
-        path = os.path.join(os.environ['APPDATA'], "termsaver")
-    else:
-        path = os.path.join(os.environ['HOME'], ".termsaver")
-
-    # create if applicable
-    if not os.path.exists(path):
-        # permission errors here will just propagate error
-        os.mkdir(path)
-
-    return path
-
-
-def get_temp_dir():
-    """
-    Retrieves the temporary based on current operating system.
-
-    For Windows machines, this should be something like:
-
-        <root>\Documents and Settings\<user>\Local Settings\Temp
-
-    For Unix machines, it will be:
-
-        /tmp/
-
-    """
-    if is_windows():
-        path = os.environ['TMP']
-    else:
-        path = "/tmp"
-
-    return path
-
-
-def unescape_string(escaped_text):
-    """
-    Unescape strings. This is useful for cases when data that needs to be
-    displayed on screen is escaped for HTML or database stuff.
-
-    Additional replacing is taken here, such as some HTML tags:
-
-        * <br>, replaced to \n
-    """
-    unescaped = escaped_text
-    try:
-        unescaped = HTMLParser.HTMLParser().unescape(escaped_text)
-        # replace most common HTML data
-        unescaped = unescaped.replace('<br>', '\n')
-        unescaped = unescaped.replace('<br/>', '\n')
-        unescaped = unescaped.replace('<br />', '\n')
-        unescaped = unescaped.decode('string_escape')
-    except:
-        #
-        # If there were errors here, just ignore them and try to give back
-        # the string the best it could do
-        #
-        pass
-    return unescaped
-
-
-def get_day_suffix(day):
-    """
-    Returns the suffix of the day, such as in 1st, 2nd, ...
-    """
-    if day in (1, 21, 31):
-        return 'st'
-    elif day in (2, 12, 22):
-        return 'nd'
-    elif day in (3, 23):
-        return 'rd'
-    else:
-        return 'th'
-
-
-def execute_shell(cmd, ignore_errors=False):
-    """
-    Simple routine to execute shell commands.
-    If `ignore_errors` is false (default) errors here will be thrown, and
-    must be treated individually, to ensure proper message to end-user.
-
-    The `cmd` argument must be an array, formatted for subprocess.Popen.
-    If you are not sure on how to do that, just use:  shlex.split(string).
-    """
-    try:
-        p = subprocess.Popen(cmd, stdin=subprocess.PIPE,
-                stdout=subprocess.PIPE, close_fds=True)
-        out, __ = p.communicate()
-    except Exception, e:
-        if not ignore_errors:
-            raise e
-    return out.rstrip()
-
-
-def strip_html(text):
-    """
-    Simple regex that cleans a string of any HTML tags (for terminal output,
-    there isn't much sense to have them printed anyway).
-    """
-    return re.sub('<[^<]+?>', '', text)
-
-
-def get_cpu_usage(sleep_delay, ignore_errors=False):
-    """
-    """
-    try:    
-        if is_windows():
-            raise Exception(_("Functionality not available for Windows. See --help for details."))
-            
-        elif is_macos():
-            ps = subprocess.Popen(['ps', '-A', '-o %cpu'], stdout=subprocess.PIPE)
-            cpu = subprocess.check_output(('awk', '{s+=$1} END {print s "%"}'), stdin=ps.stdout)
-            ps.wait()
-            time.sleep(sleep_delay) # required to simulate same in linux
-            return float(cpu.strip()[:-1])
-
-        else:
-            # linux
-            def getTimeList():
-                statFile = file("/proc/stat", "r")
-                timeList = statFile.readline().split(" ")[2:6]
-                statFile.close()
-                for i in range(len(timeList))  :
-                    timeList[i] = int(timeList[i])
-                return timeList
-            def deltaTime()  :
-                x = getTimeList()
-                time.sleep(sleep_delay)
-                y = getTimeList()
-                for i in range(len(x))  :
-                    y[i] -= x[i]
-                return y
-            dt = deltaTime()
-            if sum(dt) > 0:
-                cpu = 100 - (dt[len(dt) - 1] * 100.00 / sum(dt))
-            else:
-                cpu = 0
-
-            return cpu
-
-    except Exception, e:
-        if not ignore_errors:
-            raise e
-        else:
-            return 0
-
-
-def get_mem_usage(ignore_errors=False):
-    """
-    """
-    try:    
-        if is_windows():
-            raise Exception(_("Functionality not available for Windows. See --help for details."))
-            
-        elif is_macos():
-
-            vm = subprocess.Popen(['vm_stat'], stdout=subprocess.PIPE).communicate()[0].decode()
-            vmLines = vm.split('\n')
-            sep = re.compile(':[\s]+')
-            vmStats = {}
-            for row in range(1,len(vmLines)-2):
-                rowText = vmLines[row].strip()
-                rowElements = sep.split(rowText)
-                vmStats[(rowElements[0])] = int(rowElements[1].strip('\.')) * 4096
-
-            total_mem = (vmStats["Pages wired down"]+vmStats["Pages active"]+vmStats["Pages inactive"]+vmStats["Pages free"])/1024/1024
-            curr_mem = (vmStats["Pages inactive"]+vmStats["Pages free"]) * 100 / (vmStats["Pages wired down"]+vmStats["Pages active"]+vmStats["Pages inactive"]+vmStats["Pages free"])
-
-            return (curr_mem, total_mem)
-
-        else:
-            # linux
-            re_parser = re.compile(r'^(?P<key>\S*):\s*(?P<value>\d*)\s*kB')
-            mem_info = {}
-            for line in open('/proc/meminfo'):
-                match = re_parser.match(line)
-                if not match:
-                    continue # skip lines that don't parse
-                key, value = match.groups(['key', 'value'])
-                if key not in ('MemTotal', 'MemFree'):
-                    continue
-                mem_info[key] = int(value)
-
-            total_mem = mem_info['MemTotal'] / 1024
-            curr_mem = (mem_info['MemTotal'] - mem_info['MemFree']) * 100 / mem_info['MemTotal']
-
-            return (curr_mem, total_mem)
-
-    except Exception, e:
-        if not ignore_errors:
-            raise e
-        else:
-            return (0,0)
-
-
-
-
+###############################################################################
+#
+# file:     common.py
+#
+# Purpose:  holds common helper functions used by termsaver code.
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+Holds common functionality used by termsaver screens.
+"""
+
+#
+# Python build-in modules
+#
+import os
+import sys
+import traceback
+from html.parser import HTMLParser
+import subprocess
+import re
+import time
+
+
+def is_windows():
+    """
+    Returns True if the environment is Microsoft Windows.
+    """
+    return sys.platform == "win32"
+
+
+def is_macos():
+    """
+    Returns True if the environment is Microsoft Windows.
+    """
+    return sys.platform == "darwin"
+
+
+def prettify_exception(ex):
+    """
+    Outputs the exception with its stack trace within separator lines.
+    """
+    error_message = ""
+    if hasattr(ex, 'message'):
+        error_message = ex.message
+    else:
+        error_message = ex
+    print ("""
+===================================
+Exception: (%s) %s
+%s
+===================================
+""" % (ex.__class__.__name__, error_message, traceback.format_exc()))
+
+
+def get_app_dir():
+    """
+    Retrieves the termsaver main directory based on current operating system.
+
+    For Windows machines, this should be something like:
+
+        <root>\Documents and Settings\<user>\Application Data\termsaver
+
+    For Unix machines, it will be:
+
+        /home/<user>/.termsaver/
+    """
+    if is_windows():
+        path = os.path.join(os.environ['APPDATA'], "termsaver")
+    else:
+        path = os.path.join(os.environ['HOME'], ".termsaver")
+
+    # create if applicable
+    if not os.path.exists(path):
+        # permission errors here will just propagate error
+        os.mkdir(path)
+
+    return path
+
+
+def get_temp_dir():
+    """
+    Retrieves the temporary based on current operating system.
+
+    For Windows machines, this should be something like:
+
+        <root>\Documents and Settings\<user>\Local Settings\Temp
+
+    For Unix machines, it will be:
+
+        /tmp/
+
+    """
+    if is_windows():
+        path = os.environ['TMP']
+    else:
+        path = "/tmp"
+
+    return path
+
+
+def unescape_string(escaped_text):
+    """
+    Unescape strings. This is useful for cases when data that needs to be
+    displayed on screen is escaped for HTML or database stuff.
+
+    Additional replacing is taken here, such as some HTML tags:
+
+        * <br>, replaced to \n
+    """
+    unescaped = escaped_text
+    try:
+        unescaped = HTMLParser.HTMLParser().unescape(escaped_text)
+        # replace most common HTML data
+        unescaped = unescaped.replace('<br>', '\n')
+        unescaped = unescaped.replace('<br/>', '\n')
+        unescaped = unescaped.replace('<br />', '\n')
+        # unescaped = unescaped.decode('string_escape')
+    except:
+        #
+        # If there were errors here, just ignore them and try to give back
+        # the string the best it could do
+        #
+        pass
+    return unescaped
+
+
+def get_day_suffix(day):
+    """
+    Returns the suffix of the day, such as in 1st, 2nd, ...
+    """
+    if day in (1, 21, 31):
+        return 'st'
+    elif day in (2, 12, 22):
+        return 'nd'
+    elif day in (3, 23):
+        return 'rd'
+    else:
+        return 'th'
+
+
+def execute_shell(cmd, ignore_errors=False):
+    """
+    Simple routine to execute shell commands.
+    If `ignore_errors` is false (default) errors here will be thrown, and
+    must be treated individually, to ensure proper message to end-user.
+
+    The `cmd` argument must be an array, formatted for subprocess.Popen.
+    If you are not sure on how to do that, just use:  shlex.split(string).
+    """
+    try:
+        p = subprocess.Popen(cmd, stdin=subprocess.PIPE,
+                stdout=subprocess.PIPE, close_fds=True)
+        out, __ = p.communicate()
+    except Exception as e:
+        if not ignore_errors:
+            raise e
+    return out.rstrip()
+
+
+def strip_html(text):
+    """
+    Simple regex that cleans a string of any HTML tags (for terminal output,
+    there isn't much sense to have them printed anyway).
+    """
+    return re.sub('<[^<]+?>', '', text)
+
+
+def get_cpu_usage(sleep_delay, ignore_errors=False):
+    """
+    """
+    try:    
+        if is_windows():
+            raise Exception(_("Functionality not available for Windows. See --help for details."))
+            
+        elif is_macos():
+            ps = subprocess.Popen(['ps', '-A', '-o %cpu'], stdout=subprocess.PIPE)
+            cpu = subprocess.check_output(('awk', '{s+=$1} END {print s "%"}'), stdin=ps.stdout)
+            ps.wait()
+            time.sleep(sleep_delay) # required to simulate same in linux
+            return float(cpu.strip()[:-1])
+
+        else:
+            # linux
+            def getTimeList():
+                statFile = open("/proc/stat", "r")
+                timeList = statFile.readline().split(" ")[2:6]
+                statFile.close()
+                for i in range(len(timeList))  :
+                    timeList[i] = int(timeList[i])
+                return timeList
+            def deltaTime()  :
+                x = getTimeList()
+                time.sleep(sleep_delay)
+                y = getTimeList()
+                for i in range(len(x))  :
+                    y[i] -= x[i]
+                return y
+            dt = deltaTime()
+            if sum(dt) > 0:
+                cpu = 100 - (dt[len(dt) - 1] * 100.00 / sum(dt))
+            else:
+                cpu = 0
+
+            return cpu
+
+    except Exception as e:
+        if not ignore_errors:
+            raise e
+        else:
+            return 0
+
+
+def get_mem_usage(ignore_errors=False):
+    """
+    """
+    try:    
+        if is_windows():
+            raise Exception(_("Functionality not available for Windows. See --help for details."))
+            
+        elif is_macos():
+
+            vm = subprocess.Popen(['vm_stat'], stdout=subprocess.PIPE).communicate()[0] #.decode()
+            vmLines = vm.split('\n')
+            sep = re.compile(':[\s]+')
+            vmStats = {}
+            for row in range(1,len(vmLines)-2):
+                rowText = vmLines[row].strip()
+                rowElements = sep.split(rowText)
+                vmStats[(rowElements[0])] = int(rowElements[1].strip('\.')) * 4096
+
+            total_mem = (vmStats["Pages wired down"]+vmStats["Pages active"]+vmStats["Pages inactive"]+vmStats["Pages free"])/1024/1024
+            curr_mem = (vmStats["Pages inactive"]+vmStats["Pages free"]) * 100 / (vmStats["Pages wired down"]+vmStats["Pages active"]+vmStats["Pages inactive"]+vmStats["Pages free"])
+
+            return (curr_mem, total_mem)
+
+        else:
+            # linux
+            re_parser = re.compile(r'^(?P<key>\S*):\s*(?P<value>\d*)\s*kB')
+            mem_info = {}
+            for line in open('/proc/meminfo'):
+                match = re_parser.match(line)
+                if not match:
+                    continue # skip lines that don't parse
+                key, value = match.groups(['key', 'value'])
+                if key not in ('MemTotal', 'MemFree'):
+                    continue
+                mem_info[key] = int(value)
+
+            total_mem = mem_info['MemTotal'] / 1024
+            curr_mem = (mem_info['MemTotal'] - mem_info['MemFree']) * 100 / mem_info['MemTotal']
+
+            return (curr_mem, total_mem)
+
+    except Exception as e:
+        if not ignore_errors:
+            raise e
+        else:
+            return (0,0)
+
+
+
+
```

### Comparing `termsaver-0.4/termsaverlib/screen/randtxt.py` & `termsaver-0.6/termsaver/termsaverlib/screen/randtxt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,182 +1,174 @@
-###############################################################################
-#
-# file:     randtxt.py
-#
-# Purpose:  holds base classes used by screens in termsaver
-#           refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-Simple screensaver that displays a text in random position on screen.
-
-See additional information in the class itself.
-
-The screen class available here is:
-
-    * `RandTxtScreen`
-"""
-
-import time
-
-from termsaverlib.screen.base import ScreenBase
-from termsaverlib.screen.helper.typing import TypingHelperBase
-from termsaverlib.screen.helper.position import PositionHelperBase
-from termsaverlib import constants, exception
-from termsaverlib.i18n import _
-
-
-class RandTxtScreen(ScreenBase,
-                    TypingHelperBase,
-                    PositionHelperBase):
-    """
-    Simple screensaver that displays a text in random position on screen.
-
-    This screen offers the additional options to customize its behavior:
-
-        * `delay`: Defines the freezing time for a word to be displayed on
-          screen, before a next randomization (cycle). If never changed by
-          command-line options, it will assume the value of `FREEZE_WORD_DELAY`
-
-        * `word`: defines the word to be displayed on screen
-          for files
-    """
-
-    word = ''
-    """
-    Holds the word to be displayed on screen
-    """
-
-    freeze_delay = 0
-    """
-    Defines the freezing time for a word to be displayed on screen, before a
-    next randomization (cycle). If never changed by command-line options,
-    it will assume the value of `FREEZE_WORD_DELAY`.
-    """
-
-    FREEZE_WORD_DELAY = 3
-    """
-    A default freezing time for a word to be displayed on screen, before a
-    next randomization (cycle). Its value is set to 3 seconds.
-    """
-
-    def __init__(self):
-        """
-        Creates a new instance of this class.
-        """
-        ScreenBase.__init__(self,
-            "randtxt",
-            _("displays word in random places on screen"),
-            {'opts': 'hw:d:', 'long_opts': ['help', 'word=', 'delay=']},
-        )
-        self.word = constants.App.TITLE
-        self.delay = 0.01
-        self.line_delay = 0
-        self.cleanup_per_cycle = True
-        self.freeze_delay = self.FREEZE_WORD_DELAY
-
-    def _run_cycle(self):
-        """
-        Executes a cycle of this screen.
-
-        The actions taken here, for each cycle, are as follows:
-
-            * randomize text position vertically and horizontally
-            * print using `typing_print`
-        """
-        # calculate random position based on screen size
-        self.get_terminal_size()
-
-        txt = self.randomize_text_vertically(
-            self.randomize_text_horizontally(self.word))
-
-        self.typing_print(txt)
-
-        time.sleep(self.freeze_delay)
-
-    def _usage_options_example(self):
-        """
-        Describe here the options and examples of this screen.
-
-        The method `_parse_args` will be handling the parsing of the options
-        documented here.
-
-        Additionally, this is dependent on the values exposed in `cli_opts`,
-        passed to this class during its instantiation. Only values properly
-        configured there will be accepted here.
-        """
-        print _("""
-Options:
-
- -w, --word   Sets the word to be displayed
-              default is the name of this application (if you need to use
-              spaces, don't forget to place the word with quotes)
- -d, --delay  Sets how long the word will be displayed before
-              randomized again. Default is %(default_delay)s second(s)
- -h, --help   Displays this help message
-
-Example:
-
-    $ %(app_name)s %(screen)s
-    This will trigger the screensaver to display the default word %(app_title)s
-    in random locations of the screen
-
-    $ %(app_name)s %(screen)s -w FooBar
-    This will trigger the screensaver to display the default word FooBar
-    in random locations of the screen
-""") % {
-        'app_name': constants.App.NAME,
-        'app_title': constants.App.TITLE,
-        'screen': self.name,
-        'default_delay': self.FREEZE_WORD_DELAY,
-       }
-
-    def _parse_args(self, prepared_args):
-        """
-        Handles the special command-line arguments available for this screen.
-        Although this is a base screen, having these options prepared here
-        can save coding for screens that will not change the default options.
-
-        See `_usage_options_example` method for documentation on each of the
-        options being parsed here.
-
-        Additionally, this is dependent on the values exposed in `cli_opts`,
-        passed to this class during its instantiation. Only values properly
-        configured there will be accepted here.
-        """
-        for o, a in prepared_args[0]:  # optlist, args
-            if o in ("-h", "--help"):
-                self.usage()
-                self.screen_exit()
-            elif o in ("-d", "--delay"):
-                try:
-                    # make sure argument is a valid value (float)
-                    self.freeze_delay = float(a)
-                except:
-                    raise exception.InvalidOptionException("delay")
-            elif o in ("-w", "--word"):
-                # make sure argument is a valid value
-                if a in (None, ''):
-                    raise exception.InvalidOptionException("word")
-                self.word = a
-            else:
-                # this should never happen!
-                raise Exception(_("Unhandled option. See --help for details."))
+###############################################################################
+#
+# file:     randtxt.py
+#
+# Purpose:  holds base classes used by screens in termsaver
+#           refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+Simple screensaver that displays a text in random position on screen.
+
+See additional information in the class itself.
+
+The screen class available here is:
+
+    * `RandTxtScreen`
+"""
+
+import time
+
+from termsaver.termsaverlib import constants, exception
+from termsaver.termsaverlib.i18n import _
+from termsaver.termsaverlib.screen.base import ScreenBase
+from termsaver.termsaverlib.screen.helper.position import PositionHelperBase
+from termsaver.termsaverlib.screen.helper.typing import TypingHelperBase
+
+
+class RandTxtScreen(ScreenBase,
+                    TypingHelperBase,
+                    PositionHelperBase):
+    """
+    Simple screensaver that displays a text in random position on screen.
+
+    This screen offers the additional options to customize its behavior:
+
+        * `delay`: Defines the freezing time for a word to be displayed on
+          screen, before a next randomization (cycle). If never changed by
+          command-line options, it will assume the value of `FREEZE_WORD_DELAY`
+
+        * `word`: defines the word to be displayed on screen
+          for files
+    """
+
+    word = ''
+    """
+    Holds the word to be displayed on screen
+    """
+
+    freeze_delay = 0
+    """
+    Defines the freezing time for a word to be displayed on screen, before a
+    next randomization (cycle). If never changed by command-line options,
+    it will assume the value of `FREEZE_WORD_DELAY`.
+    """
+
+    FREEZE_WORD_DELAY = 3
+    """
+    A default freezing time for a word to be displayed on screen, before a
+    next randomization (cycle). Its value is set to 3 seconds.
+    """
+
+    def __init__(self, parser = None):
+        """
+        Creates a new instance of this class.
+        """
+        ScreenBase.__init__(self,
+            "randtxt",
+            _("displays word in random places on screen"),
+            parser
+        )
+        if self.parser:
+            self.parser.add_argument("-w", "--word", type=str, required=False, help="The words to randomly display on screen.")
+            self.parser.add_argument("-d", "--delay", type=float, required=False, default=self.freeze_delay, help="The delay between changing words.")
+        self.word = constants.App.TITLE
+        self.delay = 0.01
+        self.line_delay = 0
+        self.cleanup_per_cycle = True
+        self.freeze_delay = self.FREEZE_WORD_DELAY
+
+    def _run_cycle(self):
+        """
+        Executes a cycle of this screen.
+
+        The actions taken here, for each cycle, are as follows:
+
+            * randomize text position vertically and horizontally
+            * print using `typing_print`
+        """
+        # calculate random position based on screen size
+        self.get_terminal_size()
+
+        txt = self.randomize_text_vertically(
+            self.randomize_text_horizontally(self.word))
+
+        self.typing_print(txt)
+
+        time.sleep(self.freeze_delay)
+
+    def _usage_options_example(self):
+        """
+        Describe here the options and examples of this screen.
+
+        The method `_parse_args` will be handling the parsing of the options
+        documented here.
+
+        Additionally, this is dependent on the values exposed in `cli_opts`,
+        passed to this class during its instantiation. Only values properly
+        configured there will be accepted here.
+        """
+        print (_("""
+Example:
+
+    $ %(app_name)s %(screen)s
+    This will trigger the screensaver to display the default word %(app_title)s
+    in random locations of the screen
+
+    $ %(app_name)s %(screen)s -w FooBar
+    This will trigger the screensaver to display the default word FooBar
+    in random locations of the screen
+""") % {
+        'app_name': constants.App.NAME,
+        'app_title': constants.App.TITLE,
+        'screen': self.name,
+        'default_delay': self.FREEZE_WORD_DELAY,
+       })
+
+    def _parse_args(self, launchScreenImmediately=True):
+        """
+        Handles the special command-line arguments available for this screen.
+        Although this is a base screen, having these options prepared here
+        can save coding for screens that will not change the default options.
+
+        See `_usage_options_example` method for documentation on each of the
+        options being parsed here.
+
+        Additionally, this is dependent on the values exposed in `cli_opts`,
+        passed to this class during its instantiation. Only values properly
+        configured there will be accepted here.
+        """
+        args,unknown = self.parser.parse_known_args()
+        if args.delay:
+            try:
+                # make sure argument is a valid value (float)
+                self.freeze_delay = float(args.delay)
+            except:
+                raise exception.InvalidOptionException("delay")
+        if args.word:
+            if args.word in (None, ''):
+                raise exception.InvalidOptionException("word")
+            self.word = args.word
+
+        if launchScreenImmediately:
+            self.autorun()
+        else:
+            return self
```

### Comparing `termsaver-0.4/termsaverlib/screen/jokes4all.py` & `termsaver-0.6/termsaver/termsaverlib/screen/urlfetcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,105 @@
-###############################################################################
-#
-# file:     jokes4all.py
-#
-# Purpose:  refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-Simple screensaver that displays recent jokes from http://jokes4all.net
-website, from its hourly updated RSS feed.
-
-See additional information in the class itself.
-
-The screen class available here is:
-
-    * `Jokes4AllRSSFeedScreen`
-"""
-
-#
-# Internal modules
-#
-from termsaverlib.screen.base.rssfeed import SimpleRSSFeedScreenBase
-from termsaverlib.i18n import _
-
-
-class Jokes4AllRSSFeedScreen(SimpleRSSFeedScreenBase):
-    """
-    Simple screensaver that displays recent jokes from http://jokes4all.net
-    website, from its hourly updated RSS feed.
-
-    RSS Feed Screen configuration:
-
-      * sleep between items: 30 seconds
-        this is to allow people enough time for them to read the joke
-
-      * clean up each cycle: True
-        this will force the screen to be cleaned (cleared) before each joke
-        is displayed
-
-      * character display delay: 0.015
-        a bit faster than traditional speeds, because users are not
-        interested in the char print animation as much.
-
-      * clean up each item: True
-        this will force the screen to be cleaned (cleared) before each image
-        is displayed
-
-      * display format:
-
-          '\n%(description)s\n\n%(pubDate)s %(link)s\n'
-
-      * center in vertical
-    """
-
-    def __init__(self):
-        """
-        The constructor of this class, using most default values from its super
-        class, `SimpleRSSFeedScreenBase`.
-
-        NOTE: Maybe NSFW (Not Safe For Work)
-        """
-        SimpleRSSFeedScreenBase.__init__(self,
-            "jokes4all",
-            _("displays recent jokes from jokes4all.net (NSFW)"),
-            "http://jokes4all.net/rss/360010113/jokes.xml",
-            ["pubDate", "link", "description"],
-            '\n%(description)s\n\n%(pubDate)s %(link)s\n',
-            0.015
-        )
-
-        # set defaults for this screen
-        self.sleep_between_items = 30
-        self.line_delay = 0
-        self.cleanup_per_item = True
-        self.cleanup_per_cycle = True
-        self.center_vertically = True
+###############################################################################
+#
+# file:     urlfetcher.py
+#
+# Purpose:  refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+Simple screensaver that displays data from a URL.
+
+See additional information in the class itself.
+
+The screen class available here is:
+
+    * `UrlFetcherScreen`
+"""
+
+from termsaver.termsaverlib import constants
+from termsaver.termsaverlib.i18n import _
+#
+# Internal modules
+#
+from termsaver.termsaverlib.screen.base.urlfetcher import SimpleUrlFetcherBase
+
+
+class UrlFetcherScreen(SimpleUrlFetcherBase):
+    """
+    Simple screensaver that displays data from a URL.
+    """
+
+    def __init__(self, parser = None):
+        """
+        Creates a new instance of this class.
+        """
+
+        SimpleUrlFetcherBase.__init__(self,
+            "urlfetcher",
+            _("displays url contents with typing animation"),
+            parser,
+            ''
+        )
+
+        if self.parser:
+            self.parser.add_argument("-u", "--url",
+                help="Defines the URL location from where the information should be fetched, then displayed.",
+                required=True
+            )
+            self.parser.add_argument("-d","--delay",
+                help="Sets the speed of the displaying characters default is 0.003 of a second (advised to keep)",
+                default=0.0003
+        )
+
+    def _parse_args(self, launchScreenImmediately=True):
+        args, unknown = self.parser.parse_known_args()
+
+        if args.delay:
+            self.sleep_between_items = args.delay
+    
+        if args.url:
+            self.url = args.url
+            self.url = self.url.replace('https://', 'http://') # Fetched URL returns 405 on https. Investigate later.
+      
+        if launchScreenImmediately:
+            self.autorun()
+        else:
+            return self
+
+    def _message_no_url(self):
+        """
+        """
+        return _("""
+You just need to provide the URL from where %(app_title)s will read and
+display on screen.
+
+If you do not have any idea which URL to use, check out some examples here:
+
+    RFC
+        RFC-1034 - http://tools.ietf.org/rfc/rfc1034.txt
+
+        See a RFC list from Wikipedia:
+            http://en.wikipedia.org/wiki/List_of_RFCs
+        (remember to use the txt version)
+
+""") % {
+       'app_title': constants.App.TITLE,
+    }
```

### Comparing `termsaver-0.4/termsaverlib/screen/rfc.py` & `termsaver-0.6/termsaver/termsaverlib/screen/rfc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,113 +1,122 @@
-###############################################################################
-#
-# file:     rfc.py
-#
-# Purpose:  refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-A simple screen that fetches documents from RFC (Request for Comments).
-
-The screen class available here is:
-
-    * `RFCScreen`
-"""
-
-#
-# Python built-in modules
-#
-import random
-
-#
-# Internal modules
-#
-from termsaverlib.screen.base.urlfetcher import SimpleUrlFetcherBase
-from termsaverlib.i18n import _
-
-
-class RFCScreen(SimpleUrlFetcherBase):
-    """
-    A simple screen that fetches documents from RFC (Request for Comments).
-
-    Request for Comments (RFC) is a memorandum published by the Internet
-    Engineering Task Force (IETF) describing methods, behaviors, research, or
-    innovations applicable to the working of the Internet and Internet-
-    connected systems.
-
-    More information about RFC at Wikipedia:
-    http://en.wikipedia.org/wiki/Request_for_Comments
-
-    This screen basically does the same as its super class,
-    `SimpleUrlFetcherBase`, with a simple difference that it must randomize
-    the URL to be fetched in every screen cycle. This is done by overriding
-    the `run` command.
-
-    The list of valid RFCs, according to Wikipedia, are listed in `valid_rfc`.
-    Although this may vary in time, small out-of-date information will still
-    not affect the main purpose of this screen.
-    """
-
-    valid_rfc = [
-         768, 791, 792, 793, 826, 854, 855, 862, 863, 864, 868, 903,
-        1034, 1035, 1036, 1058, 1059, 1087, 1112, 1119, 1149, 1157, 1176, 1294,
-        1305, 1321, 1350, 1436, 1441, 1459, 1730, 1777, 1855, 1889, 1918, 1939,
-        1945, 1948, 1950, 1951, 1952, 1964, 1991, 2080, 2119, 2131, 2177, 2195,
-        2228, 2246, 2251, 2252, 2253, 2254, 2255, 2256, 2326, 2327, 2328, 2351,
-        2362, 2397, 2407, 2408, 2409, 2440, 2445, 2453, 2460, 2549, 2570, 2606,
-        2616, 2740, 2743, 2744, 2810, 2811, 2812, 2813, 2821, 2822, 2853, 2865,
-        2866, 2965, 2974, 3022, 3031, 3056, 3080, 3162, 3261, 3284, 3286, 3315,
-        3339, 3376, 3401, 3402, 3403, 3404, 3405, 3501, 3530, 3720, 3783, 3801,
-        3977, 4213, 4217, 4271, 4287, 4251, 4291, 4353, 4408, 4422, 4541, 4575,
-        4579, 4634, 4646, 4787, 4960, 5023, 5533, 5969, 6455, 937, 951, 959,
-    ]
-    """
-    Extracted from Wikipedia: http://en.wikipedia.org/wiki/List_of_RFCs
-    on 2012-02-28, 02:11 AM
-    """
-
-    url_format = "http://tools.ietf.org/rfc/rfc%d.txt"
-    """
-    The URL format that can return a text version of a specific RFC number.
-    """
-
-    def __init__(self):
-        """
-        The constructor of this class, using most default values from its super
-        class, `SimpleUrlFetcherBase`.
-        """
-        SimpleUrlFetcherBase.__init__(self,
-            "rfc",
-            _("randomly displays RFC contents"),
-            "localhost")  # base class require a URL
-
-    def _run_cycle(self):
-        """
-        Executes a cycle of this screen. Overriden from its superclass because
-        it needs to must randomize the URL to be fetched in every screen cycle.
-        """
-        # Randomize next URL to fetch from one of the valid list
-        self.url = self.url_format % self.valid_rfc[
-            random.randint(0, len(self.valid_rfc) - 1)]
-
-        data = self.fetch(self.url)
-        self.clear_screen()
-        self.typing_print(data)
+###############################################################################
+#
+# file:     rfc.py
+#
+# Purpose:  refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+A simple screen that fetches documents from RFC (Request for Comments).
+
+The screen class available here is:
+
+    * `RFCScreen`
+"""
+
+#
+# Python built-in modules
+#
+import random
+
+from termsaver.termsaverlib.i18n import _
+from termsaver.termsaverlib.screen.base import ScreenBase
+#
+# Internal modules
+#
+from termsaver.termsaverlib.screen.base.urlfetcher import SimpleUrlFetcherBase
+
+
+class RFCScreen(SimpleUrlFetcherBase):
+    """
+    A simple screen that fetches documents from RFC (Request for Comments).
+
+    Request for Comments (RFC) is a memorandum published by the Internet
+    Engineering Task Force (IETF) describing methods, behaviors, research, or
+    innovations applicable to the working of the Internet and Internet-
+    connected systems.
+
+    More information about RFC at Wikipedia:
+    http://en.wikipedia.org/wiki/Request_for_Comments
+
+    This screen basically does the same as its super class,
+    `SimpleUrlFetcherBase`, with a simple difference that it must randomize
+    the URL to be fetched in every screen cycle. This is done by overriding
+    the `run` command.
+
+    The list of valid RFCs, according to Wikipedia, are listed in `valid_rfc`.
+    Although this may vary in time, small out-of-date information will still
+    not affect the main purpose of this screen.
+    """
+
+    valid_rfc = [
+         768, 791, 792, 793, 826, 854, 855, 862, 863, 864, 868, 903,
+        1034, 1035, 1036, 1058, 1059, 1087, 1112, 1119, 1149, 1157, 1176, 1294,
+        1305, 1321, 1350, 1436, 1441, 1459, 1730, 1777, 1855, 1889, 1918, 1939,
+        1945, 1948, 1950, 1951, 1952, 1964, 1991, 2080, 2119, 2131, 2177, 2195,
+        2228, 2246, 2251, 2252, 2253, 2254, 2255, 2256, 2326, 2327, 2328, 2351,
+        2362, 2397, 2407, 2408, 2409, 2440, 2445, 2453, 2460, 2549, 2570, 2606,
+        2616, 2740, 2743, 2744, 2810, 2811, 2812, 2813, 2821, 2822, 2853, 2865,
+        2866, 2965, 2974, 3022, 3031, 3056, 3080, 3162, 3261, 3284, 3286, 3315,
+        3339, 3376, 3401, 3402, 3403, 3404, 3405, 3501, 3530, 3720, 3783, 3801,
+        3977, 4213, 4217, 4271, 4287, 4251, 4291, 4353, 4408, 4422, 4541, 4575,
+        4579, 4634, 4646, 4787, 4960, 5023, 5533, 5969, 6455, 937, 951, 959,
+    ]
+    """
+    Extracted from Wikipedia: http://en.wikipedia.org/wiki/List_of_RFCs
+    on 2012-02-28, 02:11 AM
+    """
+
+    url_format = "http://tools.ietf.org/rfc/rfc%d.txt"
+    """
+    The URL format that can return a text version of a specific RFC number.
+    """
+
+    def __init__(self, parser = None):
+        """
+        The constructor of this class, using most default values from its super
+        class, `SimpleUrlFetcherBase`.
+        """
+        SimpleUrlFetcherBase.__init__(self,
+            "rfc",
+            _("randomly displays RFC contents"),
+            parser,
+            "localhost",
+        )  # base class require a URL
+
+    def _run_cycle(self):
+        """
+        Executes a cycle of this screen. Overriden from its superclass because
+        it needs to must randomize the URL to be fetched in every screen cycle.
+        """
+        # Randomize next URL to fetch from one of the valid list
+        self.url = self.url_format % self.valid_rfc[
+            random.randint(0, len(self.valid_rfc) - 1)]
+
+        data = self.fetch(self.url)
+        self.clear_screen()
+        self.typing_print(data.decode("utf-8"))
+
+    def _parse_args(self, launchScreenImmediately=True):
+        if launchScreenImmediately:
+            self.autorun()
+        else:
+            return self
```

### Comparing `termsaver-0.4/termsaverlib/screen/sysmon.py` & `termsaver-0.6/termsaver/termsaverlib/screen/sysmon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,432 +1,453 @@
-# -*- coding: utf-8 -*-
-###############################################################################
-#
-# file:     sysmon.py
-#
-# Purpose:  refer to python doc for documentation details.
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-This module contains a simple screen that displays CPU/MEM charts.
-See additional information in the class itself.
-
-The screen class available here is:
-
-    * `SysmonScreen`
-"""
-
-#
-# Python mobdules
-#
-import time
-import re
-import os
-
-#
-# Internal modules
-#
-from termsaverlib.screen.base import ScreenBase
-from termsaverlib.screen.helper.position import PositionHelperBase
-from termsaverlib import constants, exception, common
-from termsaverlib.i18n import _
-
-
-class SysmonScreen(ScreenBase, PositionHelperBase):
-    """
-    Simple screen that displays CPU/MEM usage charts on a terminal window.
-
-    From its base classes, the functionality provided here bases on the
-    settings defined below:
-
-        * clean up each cycle: False
-          The screen will be cleared manually after the CPU calculation
-          is completed (it requires a sleep)
-
-    """
-
-    path = None
-    """
-    Defines the path of the file containing a monitoring value, from 0 to 100.
-    """
-
-    info = {
-            'db': [
-                #
-                # store data in format: 
-                # {'time': ??, 'cpu': ??, 'mem': ??, 'extra': ??}
-                #
-            ],
-            'total_mem': 0,
-            'max_cpu': 0,
-            'max_mem': 0,
-            'max_extra': 0, # for an external path
-    }
-    """
-    Registers the history of CPU/MEM usage, used to build the charts
-    """
-
-    delay = None
-    """
-    Defines the printing delay, to give a cool visual of a
-    moving screen. This value is measured in seconds, and default is 0.5.
-    """
-
-
-    #
-    # Graphical elements
-    #
-
-    pie_chart = ['○', '◔', '◑', '◕', '●']
-    """
-    Holds the unicode symbols for pie chart representation of percentage
-    """
-    block = [' ', '▁', '▂', '▃', '▄', '▅', '▆', '▇', '█', '█']
-    """
-    Holds the block unicode symbolds used to draw the charts
-    """
-    axis_corner = "└"
-    """
-    Represents the unicode symbol for the axis corner in the xy chart
-    """
-    axis_h = "─"
-    """
-    Represents the unicode symbol for the horizontal axis in the xy chart
-    """
-    axis_v = "│"
-    """
-    Represents the unicode symbol for the vertical axis in the xy chart
-    """
-
-    adjust = True
-    """
-    Defines if the graphics should hold a 0-100 count or adjust to the highest
-    value available
-    """
-
-
-    def __init__(self):
-        """
-        The constructor of this class.
-        """
-        ScreenBase.__init__(self,
-            "sysmon",
-            _("displays a graphical system monitor"),
-            {'opts': 'hd:np:', 'long_opts': ['help', 'delay=', 'no-adjust', 'path=']},
-        )
-        if self.delay is None:
-            self.delay = 0.5
-
-        #
-        # Due to a time delay to calculate CPU usage
-        # we need to clear the screen manually
-        #
-        self.cleanup_per_cycle = False
-
-
-    def _run_cycle(self):
-        """
-        Executes a cycle of this screen.
-        """
-
-        # calculate random position based on screen size
-        self.get_terminal_size()
-
-        # update info data
-        if self.path:
-            #
-            # run the flow for external path
-            #
-            self.update_stats_extra()
-            
-            if self.geometry['x'] > 16: # just to avoid unexpected exceptions
-                title = "%s: %s" % (_('Monitoring'), (self.path[:(self.geometry['x'] - 16)] 
-                        + (self.path[(self.geometry['x'] - 16):] and '...')))
-            else:
-                title = _("Monitoring file")
-                
-            txt = self.get_xy_chart(title, 'extra')
-            
-            txt += self.center_text_horizontally(
-                "\n  Load: %s%%   %s " % (
-                ("%02d" % self.info['db'][-1]['extra']),
-                self.get_chart(self.info['db'][-1]['extra']),
-                )
-            ) 
-            
-        else:
-            #
-            # run the flow for CPU/Mem as default
-            #
-            self.update_stats()
-
-            txt = self.get_xy_chart("CPU Monitor", 'cpu')
-    
-            txt += "\n"
-    
-            txt += self.get_xy_chart("MEM Monitor", 'mem')
-    
-            txt += self.center_text_horizontally(
-                "\n%s  CPU: %s%%   %s  MEM: %s%% (total %sMB)" % (
-                self.get_chart(self.info['db'][-1]['cpu']),
-                ('%.1f' % self.info['db'][-1]['cpu']),
-                self.get_chart(self.info['db'][-1]['mem']),
-                self.info['db'][-1]['mem'],
-                int(self.info['total_mem'])
-            ))
-
-        #
-        # Due to a time delay to calculate CPU usage
-        # we need to clear the screen manually
-        #
-        self.clear_screen()
-
-        # just print the whole text
-        print txt
-
-        #
-        # The sleep happens here in the CPU calculation instead
-        #
-        #time.sleep(self.delay)
-
-    def update_stats_extra(self):
-        """
-        Updates the info property with latest information on an extra path, 
-        defined by --path argument option
-
-        Note: This also takes care of sleep (defined by delay property)
-        """
-        
-        f = open(self.path, 'r')
-        try:
-            val = int(f.read())
-        except:
-            raise exception.TermSaverException(
-               _('The file does not contain an integer as expected.'))
-        if val < 0 or val > 100:
-            raise exception.TermSaverException(
-                _('The file contains invalid data (must be between 0 and 100).'))
-        f.close()
-
-        # cut the data to keep only recent values
-        self.info['db'] = self.info['db'][-(self.geometry['x'] - 5):]
-
-        max_extra = 0
-        for item in self.info['db']:
-            if item['extra'] > max_extra:
-                max_extra = item['extra']
-        self.info['max_extra'] = max_extra
-        self.info['db'].append( {
-                'time': time.time(),
-                'extra': val,
-             }
-        )
-        time.sleep(self.delay)
-        
-        
-    def update_stats(self):
-        """
-        Updates the info property with latest information on CPU and MEM usage.
-
-        Note: This also takes care of sleep (defined by delay property)
-        """
-        
-        # TODO - Implement similar features for Windows/Mac OS
-        #        maybe consider psutil package
-        if os.name != "posix":
-            raise exception.TermSaverException(help_msg="OS is not supported!")
-
-        # memory info
-        mem_info = common.get_mem_usage()
-        
-        # cpu info
-        cpu = common.get_cpu_usage(self.delay)
-
-        self.info['total_mem'] = mem_info[1]
-
-        # insert into history data
-        self.info['db'].append( {
-                'time': time.time(),
-                'cpu': cpu,
-                'mem': mem_info[0]
-             }
-        )
-        # cut the data to keep only recent values
-        self.info['db'] = self.info['db'][-(self.geometry['x'] - 5):]
-
-        # recalculate the cpu ceiling value
-        max_cpu, max_mem = 0, 0
-        for item in self.info['db']:
-            if item['cpu'] > max_cpu:
-                max_cpu = item['cpu']
-            if item['mem'] > max_mem:
-                max_mem = item['mem']
-        self.info['max_cpu'] = max_cpu
-        self.info['max_mem'] = max_mem
-
-
-    def format_time(self, epoch):
-        """
-        Formats a given epoch time into a very simplistic form compared to
-        current time (eg. 1h meaning 1 hour ago).
-        """
-        elapsed = time.time() - epoch
-        if elapsed > 3600:
-            return "%.1fh" % (elapsed/3600.0)
-        elif elapsed > 60:
-            return "%.1fm" % (elapsed/60.0)
-        elif elapsed > 1:
-            return "%.1fs" % elapsed
-        else:
-            return ""
-
-    def get_chart(self, perc):
-        """
-        returns a pie chart unicode depending on the percentage (eg. 100%)
-        given.
-        """
-        pos = int(perc * 5 / 100)
-        if pos < len(self.pie_chart) and pos >= 0:
-            return self.pie_chart[pos]
-        else:
-            return ""
-
-    def get_xy_chart(self, title, key):
-
-        ceiling = 100
-        if self.adjust:
-            ceiling = self.info['max_' + key]
-
-        ysize = int((self.geometry['y'] - 13)/2) # remove lines used
-        current_position = 0
-
-        txt = self.align_text_right(title) + "\n" \
-            + ('%.0f' % ceiling) + "%\n"
-        # create output (11 lines)
-        for y in range(ysize - 1, -1, -1):
-            current_position = 0
-            txt += " " + self.axis_v
-            for x in range(self.geometry['x'] - 5): # padding
-                if len(self.info['db']) - 1 < x:
-                    txt += " "
-                else:
-                    current_position += 1
-
-                    # to keep proportions
-                    ratio = 1
-                    if ceiling > 0:
-                        ratio = int(self.info['db'][x][key] * ysize / ceiling)
-
-                    # based on number of blocks (10)
-                    if ratio >= y + 1:
-                        txt += self.block[-1]
-                    elif y > 0 and ratio > y:
-                        txt += self.block[ratio - y]
-                    elif y > 0:
-                        txt += self.block[0]
-                    else:
-                        txt += self.block[1]
-
-            txt += "\n"
-
-        txt += " " + self.axis_corner + self.axis_h * (self.geometry['x'] - 5) + "\n"
-
-        txt += "%s%s%s\n" % (self.format_time(self.info['db'][0]['time']),
-                " " * (current_position - 5), _("now"))
-
-        return txt
-
-    def _usage_options_example(self):
-        """
-        Describe here the options and examples of this screen.
-
-        The method `_parse_args` will be handling the parsing of the options
-        documented here.
-
-        Additionally, this is dependent on the values exposed in `cli_opts`,
-        passed to this class during its instantiation. Only values properly
-        configured there will be accepted here.
-        """
-        print _("""
-Options:
-
- -d, --delay  Sets the speed of the displaying characters
-              default is 0.5 seconds (advised to keep at least above 0.1).
- -n, --no-adjust
-              Forces the charts to displays 0 ~ 100%% values, instead of
-              dynamically adjusted values based on current maximum.
- -p, --path   Sets the location of a file to be monitored. The file must only
-              contain a number from 0 to 100, or the screen will not start.
-              This option is optional.               
- -h, --help   Displays this help message
-
-Example:
-
-    $ %(app_name)s %(screen)s
-    This will trigger the screensaver to display a dot on screen, with random
-    size increase.
-
-    $ %(app_name)s %(screen)s -d 5
-    Overrides the default delay to 5 seconds
-
-""") % {
-        'app_name': constants.App.NAME,
-        'screen': self.name,
-       }
-
-    def _parse_args(self, prepared_args):
-        """
-        Handles the special command-line arguments available for this screen.
-        Although this is a base screen, having these options prepared here
-        can save coding for screens that will not change the default options.
-
-        See `_usage_options_example` method for documentation on each of the
-        options being parsed here.
-
-        Additionally, this is dependent on the values exposed in `cli_opts`,
-        passed to this class during its instantiation. Only values properly
-        configured there will be accepted here.
-        """
-        for o, a in prepared_args[0]:  # optlist, args
-            if o in ("-h", "--help"):
-                self.usage()
-                self.screen_exit()
-            elif o in ("-n", "--no-adjust"):
-                self.adjust = False
-            elif o in ("-p", "--path"):
-                # make sure argument is a valid value (existing path)
-                self.path = a
-                if not os.path.exists(self.path):
-                    raise exception.PathNotFoundException(self.path,
-                        _("Make sure the file exists."))
-                if not os.path.isfile(self.path):
-                    raise exception.InvalidOptionException("--path",
-                        _("Make sure it is a file"))
-                    
-            elif o in ("-d", "--delay"):
-                try:
-                    # make sure argument is a valid value (float)
-                    self.delay = float(a)
-                except:
-                    raise exception.InvalidOptionException("delay")
-            else:
-                # this should never happen!
-                raise Exception(_("Unhandled option. See --help for details."))
+# -*- coding: utf-8 -*-
+###############################################################################
+#
+# file:     sysmon.py
+#
+# Purpose:  refer to python doc for documentation details.
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+This module contains a simple screen that displays CPU/MEM charts.
+See additional information in the class itself.
+
+The screen class available here is:
+
+    * `SysmonScreen`
+"""
+
+import os
+import re
+#
+# Python mobdules
+#
+import time
+
+from termsaver.termsaverlib import common, constants, exception
+from termsaver.termsaverlib.i18n import _
+#
+# Internal modules
+#
+from termsaver.termsaverlib.screen.base import ScreenBase
+from termsaver.termsaverlib.screen.helper.position import PositionHelperBase
+
+
+class SysmonScreen(ScreenBase, PositionHelperBase):
+    """
+    Simple screen that displays CPU/MEM usage charts on a terminal window.
+
+    From its base classes, the functionality provided here bases on the
+    settings defined below:
+
+        * clean up each cycle: False
+          The screen will be cleared manually after the CPU calculation
+          is completed (it requires a sleep)
+
+    """
+
+    path = None
+    """
+    Defines the path of the file containing a monitoring value, from 0 to 100.
+    """
+
+    info = {
+            'db': [
+                #
+                # store data in format: 
+                # {'time': ??, 'cpu': ??, 'mem': ??, 'extra': ??}
+                #
+            ],
+            'total_mem': 0,
+            'max_cpu': 0,
+            'max_mem': 0,
+            'max_extra': 0, # for an external path
+    }
+    """
+    Registers the history of CPU/MEM usage, used to build the charts
+    """
+
+    delay = None
+    """
+    Defines the printing delay, to give a cool visual of a
+    moving screen. This value is measured in seconds, and default is 0.5.
+    """
+
+
+    #
+    # Graphical elements
+    #
+
+    pie_chart = [
+        ['○', '◔', '◑', '◕', '●'],
+        [' ', '|', '(', 'C', 'O'],
+        [' ', '|', '(', 'C', 'O']
+    ]
+    """
+    Holds the unicode symbols for pie chart representation of percentage
+    """
+    block = [
+        [' ', '▁', '▂', '▃', '▄', '▅', '▆', '▇', '█', '█'],
+        [' ', '\033(0s\033(B', '\033(0s\033(B', '\033(0s\033(B', '\033(0s\033(B', '\033[7m \033[27m', '\033[7m \033[27m', '\033[7m \033[27m', '\033[7m \033[27m', '\033[7m \033[27m'],
+        [' ', '_', '_', 'm', 'm', 'm', '#', '#', '#', '#']
+    ]
+    """
+    Holds the block unicode symbolds used to draw the charts
+    """
+    axis_corner = ["└","\033(0m\033(B","+"]
+    """
+    Represents the unicode symbol for the axis corner in the xy chart
+    """
+    axis_h = ["─","\033(0q\033(B","-"]
+    """
+    Represents the unicode symbol for the horizontal axis in the xy chart
+    """
+    axis_v = ["│","\033(0x\033(B","|"]
+    """
+    Represents the unicode symbol for the vertical axis in the xy chart
+    """
+
+    adjust = True
+    """
+    Defines if the graphics should hold a 0-100 count or adjust to the highest
+    value available
+    """
+
+    symbol_index = 0
+    """
+    Holds the index of the symbol set we're using.
+    """
+
+
+    def __init__(self, parser = None):
+        """
+        The constructor of this class.
+        """
+        ScreenBase.__init__(self,
+            "sysmon",
+            _("displays a graphical system monitor"),
+            parser
+        )
+        if self.delay is None:
+            self.delay = 0.5
+
+        if self.parser:
+            self.parser.add_argument("-d","--delay", help="""
+            Sets the speed of the displaying characters
+            Default is 0.5 seconds (advised to keep at least above 0.1).""", default=0.5)
+            self.parser.add_argument("-n","--no-adjust", dest="adjust", action="store_true", help="""
+            Forces the charts to displays 0 ~ 100%% values, instead of dynamically adjusted values based on current maximum.
+            """)
+            self.parser.add_argument("-p","--path", help="""
+            Sets the location of a file to be monitored. The file must only contain a number from 0 to 100, or the screen will not start.
+            This option is optional.
+            """)
+            self.parser.add_argument("-v", "--variant",  action="store_true", default="False", help="""
+            Sets the alternative mode, which uses a different set of unicode symbols to draw the charts.
+            Will not work with -a / -ascii option.
+            """)
+            self.parser.add_argument("-a", "--ascii", action="store_true", default=False, help="""
+            Sets the ASCII mode, which uses only ASCII characters to draw the charts.
+            Will not work with -v / -variant option.
+            """)
+        #
+        # Due to a time delay to calculate CPU usage
+        # we need to clear the screen manually
+        #
+        self.cleanup_per_cycle = False
+
+    def _run_cycle(self):
+        """
+        Executes a cycle of this screen.
+        """
+
+        # calculate random position based on screen size
+        self.get_terminal_size()
+
+        # update info data
+        if self.path:
+            #
+            # run the flow for external path
+            #
+            self.update_stats_extra()
+            
+            if self.geometry['x'] > 16: # just to avoid unexpected exceptions
+                title = "%s: %s" % (_('Monitoring'), (self.path[:(self.geometry['x'] - 16)] 
+                        + (self.path[(self.geometry['x'] - 16):] and '...')))
+            else:
+                title = _("Monitoring file")
+                
+            txt = self.get_xy_chart(title, 'extra')
+            
+            txt += self.center_text_horizontally(
+                "\n  Load: %s%%   %s " % (
+                ("%02d" % self.info['db'][-1]['extra']),
+                self.get_chart(self.info['db'][-1]['extra']),
+                )
+            ) 
+            
+        else:
+            #
+            # run the flow for CPU/Mem as default
+            #
+            self.update_stats()
+
+            txt = self.get_xy_chart("CPU Monitor", 'cpu')
+    
+            txt += "\n"
+    
+            txt += self.get_xy_chart("MEM Monitor", 'mem')
+    
+            txt += self.center_text_horizontally(
+                "\n%s  CPU: %s%%   %s  MEM: %s%% (total %sMB)" % (
+                self.get_chart(self.info['db'][-1]['cpu']),
+                ('%.1f' % self.info['db'][-1]['cpu']),
+                self.get_chart(self.info['db'][-1]['mem']),
+                self.info['db'][-1]['mem'],
+                int(self.info['total_mem'])
+            ))
+
+        #
+        # Due to a time delay to calculate CPU usage
+        # we need to clear the screen manually
+        #
+        self.clear_screen()
+
+        # just print the whole text
+        print(txt)
+
+        #
+        # The sleep happens here in the CPU calculation instead
+        #
+        #time.sleep(self.delay)
+
+    def update_stats_extra(self):
+        """
+        Updates the info property with latest information on an extra path, 
+        defined by --path argument option
+
+        Note: This also takes care of sleep (defined by delay property)
+        """
+        
+        f = open(self.path, 'r')
+        try:
+            val = int(f.read())
+        except:
+            raise exception.TermSaverException(
+               _('The file does not contain an integer as expected.'))
+        if val < 0 or val > 100:
+            raise exception.TermSaverException(
+                _('The file contains invalid data (must be between 0 and 100).'))
+        f.close()
+
+        # cut the data to keep only recent values
+        self.info['db'] = self.info['db'][-(self.geometry['x'] - 5):]
+
+        max_extra = 0
+        for item in self.info['db']:
+            if item['extra'] > max_extra:
+                max_extra = item['extra']
+        self.info['max_extra'] = max_extra
+        self.info['db'].append( {
+                'time': time.time(),
+                'extra': val,
+             }
+        )
+        time.sleep(self.delay)
+        
+        
+    def update_stats(self):
+        """
+        Updates the info property with latest information on CPU and MEM usage.
+
+        Note: This also takes care of sleep (defined by delay property)
+        """
+        
+        # TODO - Implement similar features for Windows/Mac OS
+        #        maybe consider psutil package
+        if os.name != "posix":
+            raise exception.TermSaverException(help_msg="OS is not supported!")
+
+        # memory info
+        mem_info = common.get_mem_usage()
+        
+        # cpu info
+        cpu = common.get_cpu_usage(self.delay)
+
+        self.info['total_mem'] = mem_info[1]
+
+        # insert into history data
+        self.info['db'].append( {
+                'time': time.time(),
+                'cpu': cpu,
+                'mem': mem_info[0]
+             }
+        )
+        # cut the data to keep only recent values
+        self.info['db'] = self.info['db'][-(self.geometry['x'] - 5):]
+
+        # recalculate the cpu ceiling value
+        max_cpu, max_mem = 0, 0
+        for item in self.info['db']:
+            if item['cpu'] > max_cpu:
+                max_cpu = item['cpu']
+            if item['mem'] > max_mem:
+                max_mem = item['mem']
+        self.info['max_cpu'] = max_cpu
+        self.info['max_mem'] = max_mem
+
+
+    def format_time(self, epoch):
+        """
+        Formats a given epoch time into a very simplistic form compared to
+        current time (eg. 1h meaning 1 hour ago).
+        """
+        elapsed = time.time() - epoch
+        if elapsed > 3600:
+            return "%.1fh" % (elapsed/3600.0)
+        elif elapsed > 60:
+            return "%.1fm" % (elapsed/60.0)
+        elif elapsed > 1:
+            return "%.1fs" % elapsed
+        else:
+            return ""
+
+    def get_chart(self, perc):
+        """
+        returns a pie chart unicode depending on the percentage (eg. 100%)
+        given.
+        """
+        pos = int(perc * 5 / 100)
+        if pos < len(self.pie_chart[self.symbol_index]) and pos >= 0:
+            return self.pie_chart[self.symbol_index][pos]
+        else:
+            return ""
+
+    def get_xy_chart(self, title, key):
+
+        ceiling = 100
+        if self.adjust:
+            ceiling = self.info['max_' + key]
+
+        ysize = int((self.geometry['y'] - 13)/2) # remove lines used
+        current_position = 0
+
+        txt = self.align_text_right(title) + "\n" \
+            + ('%.0f' % ceiling) + "%\n"
+        # create output (11 lines)
+        for y in range(ysize - 1, -1, -1):
+            current_position = 0
+            txt += " " + self.axis_v[self.symbol_index]
+            for x in range(self.geometry['x'] - 5): # padding
+                if len(self.info['db']) - 1 < x:
+                    txt += " "
+                else:
+                    current_position += 1
+
+                    # to keep proportions
+                    ratio = 1
+                    if ceiling > 0:
+                        ratio = int(self.info['db'][x][key] * ysize / ceiling)
+
+                    # based on number of blocks (10)
+                    if ratio >= y + 1:
+                        txt += self.block[self.symbol_index][-1]
+                    elif y > 0 and ratio > y:
+                        txt += self.block[self.symbol_index][ratio - y]
+                    elif y > 0:
+                        txt += self.block[self.symbol_index][0]
+                    else:
+                        txt += self.block[self.symbol_index][1]
+
+            txt += "\n"
+
+        txt += " " + self.axis_corner[self.symbol_index] + self.axis_h[self.symbol_index] * (self.geometry['x'] - 5) + "\n"
+
+        txt += "%s%s%s\n" % (self.format_time(self.info['db'][0]['time']),
+                " " * (current_position - 5), _("now"))
+
+        return txt
+
+    def _usage_options_example(self):
+        """
+        Describe here the options and examples of this screen.
+
+        The method `_parse_args` will be handling the parsing of the options
+        documented here.
+
+        Additionally, this is dependent on the values exposed in `cli_opts`,
+        passed to this class during its instantiation. Only values properly
+        configured there will be accepted here.
+        """
+        return (_("""
+    $ %(app_name)s %(screen)s
+    This will trigger the screensaver to display a dot on screen, with random
+    size increase.
+
+    $ %(app_name)s %(screen)s -d 5
+    Overrides the default delay to 5 seconds
+
+""") % {
+        'app_name': constants.App.NAME,
+        'screen': self.name,
+       })
+
+    def _parse_args(self, launchScreenImmediately=True):
+        """
+        Handles the special command-line arguments available for this screen.
+        Although this is a base screen, having these options prepared here
+        can save coding for screens that will not change the default options.
+
+        See `_usage_options_example` method for documentation on each of the
+        options being parsed here.
+
+        Additionally, this is dependent on the values exposed in `cli_opts`,
+        passed to this class during its instantiation. Only values properly
+        configured there will be accepted here.
+        """
+        args,unknown = self.parser.parse_known_args()
+
+        if args.adjust:
+            self.adjust = False
+
+        if args.path:
+            self.path = args.path
+            if not os.path.exists(self.path):
+                raise exception.PathNotFoundException(self.path,
+                    _("Make sure the file exists."))
+            if not os.path.isfile(self.path):
+                raise exception.InvalidOptionException("--path",
+                    _("Make sure it is a file"))
+        if args.delay:
+            try:
+                # make sure argument is a valid value (float)
+                self.delay = float(args.delay)
+            except:
+                raise exception.InvalidOptionException("delay")
+
+        if args.variant:
+            self.symbol_index = 1
+        elif args.ascii:
+            self.symbol_index = 2
+
+        if launchScreenImmediately:
+            self.autorun()
+        else:
+            return self
```

### Comparing `termsaver-0.4/termsaverlib/screen/base/filereader.py` & `termsaver-0.6/termsaver/termsaverlib/screen/base/filereader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,338 +1,327 @@
-###############################################################################
-#
-# file:     filereader.py
-#
-# Purpose:  refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-This module contains a screen base class that handles screens that require
-recursive directory scanning for files to be printed out.
-See additional information in the class itself.
-
-The helper class available here is:
-
-    * `FileReaderBase`
-"""
-
-#
-# Python built-in modules
-#
-import os
-import Queue as queue
-from threading import Thread
-
-#
-# Internal modules
-#
-from termsaverlib.screen.base import ScreenBase
-from termsaverlib import exception, constants
-from termsaverlib.screen.helper.typing import TypingHelperBase
-from termsaverlib.i18n import _
-
-
-class FileReaderBase(ScreenBase, TypingHelperBase):
-    """
-    A base class used to handle file reading, more specifically, multiple files
-    retrieved from a `path` recursively. This also uses the `TypingHelperBase`
-    helper class to add functionality of typing writer display.
-
-    The instantiation of this class takes two additional arguments, compared
-    with its base class:
-
-        * `delay`: Defines the speed of the typing writer. See more details
-          of this in `TypingHelperBase` class documentation. Its value is
-          defined by `TypingHelperBase`'s default, if none is informed.
-
-        * `path`: Defines the path to be recursively checked for text
-                  files to be displayed on terminal screen.
-
-    When inheriting from this screen, you can also take advantage of the
-    following properties and functionalities:
-
-        * `cleanup_per_file`: forces to clean up the screen for each file in
-          the looping. The alternative, available in
-          `ScreenBase.cleanup_per_cycle`, only handles a cycle action.
-
-    """
-
-    path = ''
-
-    cleanup_per_file = False
-
-    def __init__(self, name, description, path=None, delay=None, cli_opts=None):
-        """
-        Creates a new instance of this class.
-
-        This constructor has two additional arguments, compared with its base
-        class:
-
-            * delay: defines the speed of the typing writer. See more details
-              of this in `TypingHelperBase` class documentation.
-
-            * path: defines the path from where this screen should scan
-              for files
-        """
-        ScreenBase.__init__(self, name, description, cli_opts)
-        # define default cli options, if none are informed
-        if not cli_opts:
-            self.cli_opts = {
-                             'opts': 'hd:p:',
-                             'long_opts': ['help', 'delay=', 'path='],
-            }
-        self.delay = delay
-        self.path = path
-        self.cleanup_per_cycle = False
-
-    def _run_cycle(self):
-        """
-        Executes a \"cycle\" of this screen.
-            * The concept of \"cycle\" is no longer accurate, and is misleading.
-              this function will not return.
-        New threaded implementation:
-            * Checks if self.path is a valid path, using `os.path.exists`
-            * Assigns a new Queue to `queue_of_valid_files`
-            * Appends a new `FileScannerThread` object to a list of threads
-            * `start()`s the `FileScannerThread`
-                * `FileScannerThread` will put paths in the queue as valid
-                   file paths are found
-            * `clear_screen()`s
-            * Gets a file from `queue_of_valid_files`, removing item from queue
-            * While nextFile (empty sequences are false)
-                * As long as there is something in the queue - that is, as long
-                  as `queue.queue.get()` is able to get an object from (the)
-                  `queue_of_valid_files`, this test evaluates True.
-                * I imagine that this behaves unpredictably given a computer
-                  with __REALLY__ slow I/O
-            * Opens `nextFile` with handle-auto-closing `with` statement and
-              `typing_print()`s it
-            * Clears screen if `self.cleanup_per_file`
-            * Puts `nextFile` ON the queue
-                * Because `queue_of_valid_files.get()` REMOVES a file path
-                  from the queue, `_run_cycle()` will never reach that path
-                  again, and eventually will exhaust the queue
-                  (failing silently, with a blank screen)
-                    * A static blank screen is the antithesis of a screensaver
-                * Therefore, `queue_of_valid_files.put(nextFile)` puts the file
-                  path at the last spot in the queue
-            * Finally, another call to `queue_of_valid_files.get()` sets up
-              the next iteration in the while loop.
-        """
-        # validate path
-        if not os.path.exists(self.path):
-            raise exception.PathNotFoundException(self.path)
-
-        queue_of_valid_files = queue.Queue()
-
-        threads = [FileReaderBase.FileScannerThread(self, queue_of_valid_files, self.path)]
-        threads[-1].daemon = True
-        threads[-1].start()
-        #self.clear_screen() hides any error message produced before it!
-        self.clear_screen()
-        nextFile = queue_of_valid_files.get()
-        while nextFile:
-            with open(nextFile, 'r') as f:
-                file_data = f.read()
-                self.typing_print(file_data)
-            if self.cleanup_per_file:
-                self.clear_screen()
-            queue_of_valid_files.put(nextFile)
-            nextFile = queue_of_valid_files.get()
-    def _usage_options_example(self):
-        """
-        Describe here the options and examples of this screen.
-
-        The method `_parse_args` will be handling the parsing of the options
-        documented here.
-
-        Additionally, this is dependent on the values exposed in `cli_opts`,
-        passed to this class during its instantiation. Only values properly
-        configured there will be accepted here.
-        """
-        print _("""
-Options:
-
- -p, --path   Sets the location to search for text-based source files.
-              this option is mandatory.
- -d, --delay  Sets the speed of the displaying characters
-              default is%(default_delay)s of a second
- -h, --help   Displays this help message
-
-Examples:
-
-    $ %(app_name)s %(screen)s -p /path/to/my/code
-    This will trigger the screensaver to read all files in the path selected
-
-    $ %(app_name)s %(screen)s -p /path/to/my/code -d 0
-    This will trigger the screensaver to read all files in the path selected
-    with no delay (too fast for a screensaver, but it's your choice that
-    matters!)
-""") % {
-        'screen': self.name,
-        'app_name': constants.App.NAME,
-        'default_delay': constants.Settings.CHAR_DELAY_SECONDS,
-    }
-
-    def _parse_args(self, prepared_args):
-        """
-        Handles the special command-line arguments available for this screen.
-        Although this is a base screen, having these options prepared here
-        can save coding for screens that will not change the default options.
-
-        See `_usage_options_example` method for documentation on each of the
-        options being parsed here.
-
-        Additionally, this is dependent on the values exposed in `cli_opts`,
-        passed to this class during its instantiation. Only values properly
-        configured there will be accepted here.
-        """
-        for o, a in prepared_args[0]:  # optlist, args
-            if o in ("-h", "--help"):
-                self.usage()
-                self.screen_exit()
-            elif o in ("-d", "--delay"):
-                try:
-                    # make sure argument is a valid value (float)
-                    self.delay = float(a)
-                except:
-                    raise exception.InvalidOptionException("delay")
-            elif o in ("-p", "--path"):
-                # make sure argument is a valid value (existing path)
-                self.path = a
-                if not os.path.exists(self.path):
-                    raise exception.PathNotFoundException(self.path,
-                        _("Make sure the file or directory exists."))
-            else:
-                # this should never happen!
-                raise Exception(_("Unhandled option. See --help for details."))
-
-        # last validations
-        if self.path in (None, ''):
-            raise exception.InvalidOptionException("path",
-                _("It is mandatory option"), help=self._message_no_path())
-
-    def _recurse_to_exec(self, path, func, filetype=''):
-        """
-        Executes a function for each file found recursively within the
-        specified path.
-
-        Arguments:
-
-            * path: the path to be recursively checked (directory)
-
-            * func: the function to be executed with the file(s)
-
-            * filetype: to filter for a specific filetype
-        """
-        try:
-            if os.path.isdir(path):
-                for item in os.listdir(path):
-                    f = os.path.join(path, item)
-                    if os.path.isdir(f):
-                        if not item.startswith('.'):
-                            self._recurse_to_exec(f, func, filetype)
-                    elif f.endswith(filetype) and not self._is_path_binary(f):
-                        func(f)
-            elif path.endswith(filetype) and not self._is_path_binary(path):
-                func(path)
-        except:
-            # If IOError, don't put on queue, as the path might throw
-            # another IOError during screen saver operations.
-            return
-
-    @staticmethod
-    def recursively_populate_queue(self, queue_of_valid_files, path, filetype=''):
-        """
-        Populates an (empty) queue of all files within directory
-        in "path", with the paths to said files.
-
-        MUST be a staticmethod for threaded implementation to function.
-
-        Arguments:
-            * queue_of_valid_files
-
-            * path: the path to be recursively checked (directory)
-
-            * filetype: to filter for a specific filetype
-        """
-        self._recurse_to_exec(path, queue_of_valid_files.put, filetype)
-
-    def _is_path_binary(self, path):
-        """
-        Returns True if the given path corresponds to a binary, or, if for any
-        reason, the file can not be accessed or opened.
-
-        For the merit of being a binary file (i.e., termsaver will not be able
-        to handle it), it is safe enough to consider the above True, as any
-        files in this situation will be simply skipped, avoiding weird errors
-        being thrown to the end-user.
-
-        Arguments:
-
-            * path: the file location
-        """
-        CHUNKSIZE = 1024
-
-        f = None
-        try:
-            f = open(path, 'rb')
-        except:
-            # If IOError, don't even bother, as the path might throw
-            # another IOError during screen saver operations.
-            return True
-        try:
-            while True:
-                chunk = f.read(CHUNKSIZE)
-                if '\0' in chunk:  # found null byte
-                    return True
-                if len(chunk) < CHUNKSIZE:
-                    break  # done
-        except:
-            # If IOError, don't even bother, as the path might throw
-            # another IOError during screen saver operations.
-            return True
-        finally:
-            if f:
-                f.close()
-        return False
-
-    def _message_no_path(self):
-        """
-        Defines a method to be overriden by inheriting classes, with the
-        purpose to display extra help information for specific errors.
-        """
-        return ""
-
-    class FileScannerThread(Thread):
-        """Screen-animation independent thread for path scanning.
-           Allows animation to begin prior to completion of path scanning.
-        """
-        def __init__(self, fileReaderInstance, queue_of_valid_files, path_to_scan):
-            Thread.__init__(self)
-            self.__queue_of_valid_files = queue_of_valid_files
-            self.__path_to_scan         = path_to_scan
-            self.__file_reader_instance = fileReaderInstance
-        def run(self):
-            """Thread begins executing this function on
-               call to `aThreadObject.start()`.
-            """
-            FileReaderBase.recursively_populate_queue(self.__file_reader_instance, self.__queue_of_valid_files, self.__path_to_scan)
+###############################################################################
+#
+# file:     filereader.py
+#
+# Purpose:  refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+This module contains a screen base class that handles screens that require
+recursive directory scanning for files to be printed out.
+See additional information in the class itself.
+
+The helper class available here is:
+
+    * `FileReaderBase`
+"""
+
+import importlib
+#
+# Python built-in modules
+#
+import os
+import queue  # as queue
+from threading import Thread
+
+from termsaver.termsaverlib import constants, exception
+from termsaver.termsaverlib.i18n import _
+#
+# Internal modules
+#
+from termsaver.termsaverlib.screen.base import ScreenBase
+from termsaver.termsaverlib.screen.helper.typing import TypingHelperBase
+
+
+class FileReaderBase(ScreenBase, TypingHelperBase):
+    """
+    A base class used to handle file reading, more specifically, multiple files
+    retrieved from a `path` recursively. This also uses the `TypingHelperBase`
+    helper class to add functionality of typing writer display.
+
+    The instantiation of this class takes two additional arguments, compared
+    with its base class:
+
+        * `delay`: Defines the speed of the typing writer. See more details
+          of this in `TypingHelperBase` class documentation. Its value is
+          defined by `TypingHelperBase`'s default, if none is informed.
+
+        * `path`: Defines the path to be recursively checked for text
+                  files to be displayed on terminal screen.
+
+    When inheriting from this screen, you can also take advantage of the
+    following properties and functionalities:
+
+        * `cleanup_per_file`: forces to clean up the screen for each file in
+          the looping. The alternative, available in
+          `ScreenBase.cleanup_per_cycle`, only handles a cycle action.
+
+    """
+
+    path = ''
+
+    cleanup_per_file = False
+
+    def __init__(self, name, description, parser, path=None, delay=None):
+        """
+        Creates a new instance of this class.
+
+        This constructor has two additional arguments, compared with its base
+        class:
+
+            * delay: defines the speed of the typing writer. See more details
+              of this in `TypingHelperBase` class documentation.
+
+            * path: defines the path from where this screen should scan
+              for files
+        """
+        ScreenBase.__init__(self, name, description, parser)
+
+        if self.parser != None:
+            self.parser.add_argument("-p","--path",required=True, action="store", type=str, help="""Sets the location to search for text-based source files.
+                this option is mandatory.""")
+            
+            self.parser.add_argument("-d","--delay", action="store", type=int, help="""Sets the speed of the displaying characters
+                default is%(default_delay)s of a second""" % {'default_delay': constants.Settings.CHAR_DELAY_SECONDS})
+
+        self.delay = delay
+        self.path = path
+        self.ignore_binary = False
+        self.cleanup_per_cycle = False
+        self.colorize = False
+        self.pygments_installed = False
+        self.is_initalized = False
+
+    def _run_cycle(self):
+        if self.is_initalized is False:
+            #if 'pygments' in sys.modules:
+            pygments_spec = importlib.util.find_spec('pygments')
+            found = pygments_spec is not None
+            if found is True:
+                from pygments import highlight
+                from pygments.formatters import TerminalFormatter
+                from pygments.lexers import guess_lexer
+                self.pygments_installed = True
+            self.is_initalized = True
+        """
+        Executes a \"cycle\" of this screen.
+            * The concept of \"cycle\" is no longer accurate, and is misleading.
+              this function will not return.
+        New threaded implementation:
+            * Checks if self.path is a valid path, using `os.path.exists`
+            * Assigns a new Queue to `queue_of_valid_files`
+            * Appends a new `FileScannerThread` object to a list of threads
+            * `start()`s the `FileScannerThread`
+                * `FileScannerThread` will put paths in the queue as valid
+                   file paths are found
+            * `clear_screen()`s
+            * Gets a file from `queue_of_valid_files`, removing item from queue
+            * While nextFile (empty sequences are false)
+                * As long as there is something in the queue - that is, as long
+                  as `queue.queue.get()` is able to get an object from (the)
+                  `queue_of_valid_files`, this test evaluates True.
+                * I imagine that this behaves unpredictably given a computer
+                  with __REALLY__ slow I/O
+            * Opens `nextFile` with handle-auto-closing `with` statement and
+              `typing_print()`s it
+            * Clears screen if `self.cleanup_per_file`
+            * Puts `nextFile` ON the queue
+                * Because `queue_of_valid_files.get()` REMOVES a file path
+                  from the queue, `_run_cycle()` will never reach that path
+                  again, and eventually will exhaust the queue
+                  (failing silently, with a blank screen)
+                    * A static blank screen is the antithesis of a screensaver
+                * Therefore, `queue_of_valid_files.put(nextFile)` puts the file
+                  path at the last spot in the queue
+            * Finally, another call to `queue_of_valid_files.get()` sets up
+              the next iteration in the while loop.
+        """
+        # validate path
+        if not os.path.exists(self.path):
+            raise exception.PathNotFoundException(self.path)
+        
+        if os.path.isdir(self.path):            
+            queue_of_valid_files = queue.Queue()
+
+            threads = [FileReaderBase.FileScannerThread(self, queue_of_valid_files, self.path)]
+            threads[-1].daemon = True
+            threads[-1].start()
+            
+            print(_("""
+    Scanning path for supported files.
+    If this message does not disappear then there are no supported file types in the given path."""))
+
+            nextFile = queue_of_valid_files.get()
+        else:
+            nextFile = self.path
+    
+        #self.clear_screen() hides any error message produced before it!
+        self.clear_screen()
+
+        while nextFile:
+            with open(nextFile, 'r') as f:
+                file_data = f.read()
+                if self.pygments_installed is True:
+                    if self.colorize is True:
+                        lexer = guess_lexer(file_data)
+                        formatter = TerminalFormatter
+                        file_data = highlight(file_data,lexer,formatter())
+                self.typing_print(file_data)
+            if self.cleanup_per_file:
+                self.clear_screen()
+            queue_of_valid_files.put(nextFile)
+            nextFile = queue_of_valid_files.get()
+    def _usage_options_example(self):
+        """
+        Describe here the options and examples of this screen.
+
+        The method `_parse_args` will be handling the parsing of the options
+        documented here.
+
+        Additionally, this is dependent on the values exposed in `cli_opts`,
+        passed to this class during its instantiation. Only values properly
+        configured there will be accepted here.
+        """
+        print (_("""
+Examples:
+
+    $ %(app_name)s %(screen)s -p /path/to/my/code
+    This will trigger the screensaver to read all files in the path selected
+
+    $ %(app_name)s %(screen)s -p /path/to/my/code -d 0
+    This will trigger the screensaver to read all files in the path selected
+    with no delay (too fast for a screensaver, but it's your choice that
+    matters!)
+""") % {
+        'screen': self.name,
+        'app_name': constants.App.NAME,
+        'default_delay': constants.Settings.CHAR_DELAY_SECONDS,
+    })
+
+    def _recurse_to_exec(self, path, func, filetype=''):
+        """
+        Executes a function for each file found recursively within the
+        specified path.
+
+        Arguments:
+
+            * path: the path to be recursively checked (directory)
+
+            * func: the function to be executed with the file(s)
+
+            * filetype: to filter for a specific filetype
+        """
+        try:
+            if os.path.isdir(path):
+                for item in os.listdir(path):
+                    f = os.path.join(path, item)
+                    if os.path.isdir(f):
+                        if not item.startswith('.'):
+                            self._recurse_to_exec(f, func, filetype)
+                    elif f.endswith(filetype):
+                        if self.ignore_binary is False and not self._is_path_binary(f):
+                            func(f)
+                        elif self.ignore_binary is True and self._is_path_binary(f):
+                            func(f)
+            elif path.endswith(filetype) and not self._is_path_binary(path):
+                func(path)
+        except:
+            # If IOError, don't put on queue, as the path might throw
+            # another IOError during screen saver operations.
+            return
+
+    @staticmethod
+    def recursively_populate_queue(self, queue_of_valid_files, path, filetype=''):
+        """
+        Populates an (empty) queue of all files within directory
+        in "path", with the paths to said files.
+
+        MUST be a staticmethod for threaded implementation to function.
+
+        Arguments:
+            * queue_of_valid_files
+
+            * path: the path to be recursively checked (directory)
+
+            * filetype: to filter for a specific filetype
+        """
+        self._recurse_to_exec(path, queue_of_valid_files.put, filetype)
+
+    def _is_path_binary(self, path):
+        """
+        Returns True if the given path corresponds to a binary, or, if for any
+        reason, the file can not be accessed or opened.
+
+        For the merit of being a binary file (i.e., termsaver will not be able
+        to handle it), it is safe enough to consider the above True, as any
+        files in this situation will be simply skipped, avoiding weird errors
+        being thrown to the end-user.
+
+        Arguments:
+
+            * path: the file location
+        """
+        CHUNKSIZE = 1024
+
+        f = None
+        try:
+            f = open(path, 'rb')
+        except:
+            # If IOError, don't even bother, as the path might throw
+            # another IOError during screen saver operations.
+            return True
+        try:
+            while True:
+                chunk = f.read(CHUNKSIZE)
+                if '\0' in chunk:  # found null byte
+                    return True
+                if len(chunk) < CHUNKSIZE:
+                    break  # done
+        except:
+            # If IOError, don't even bother, as the path might throw
+            # another IOError during screen saver operations.
+            return True
+        finally:
+            if f:
+                f.close()
+        return False
+
+    def _message_no_path(self):
+        """
+        Defines a method to be overriden by inheriting classes, with the
+        purpose to display extra help information for specific errors.
+        """
+        return ""
+
+    class FileScannerThread(Thread):
+        """Screen-animation independent thread for path scanning.
+           Allows animation to begin prior to completion of path scanning.
+        """
+        def __init__(self, fileReaderInstance, queue_of_valid_files, path_to_scan):
+            Thread.__init__(self)
+            self.__queue_of_valid_files = queue_of_valid_files
+            self.__path_to_scan         = path_to_scan
+            self.__file_reader_instance = fileReaderInstance
+        def run(self):
+            """Thread begins executing this function on
+               call to `aThreadObject.start()`.
+            """
+            FileReaderBase.recursively_populate_queue(self.__file_reader_instance, self.__queue_of_valid_files, self.__path_to_scan)
```

### Comparing `termsaver-0.4/termsaverlib/screen/base/__init__.py` & `termsaver-0.6/termsaver/termsaverlib/screen/base/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,351 +1,357 @@
-###############################################################################
-#
-# file:     __init__.py
-#
-# Purpose:  refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-This module holds base classes that are used by all screens within termsaver
-application. Each individual "screen" represents a unique screensaver that can
-be triggered by termsaver.
-
-The base classes available in this package are:
-
-  * `ScreenBase`: the most basic screen class, which will handle simple
-                  interaction with the terminal.
-
-  * `filereader.FileReaderBase`: handles screens that require recursive
-     directory scanning for files to be printed out
-
-  * `urlfetcher.UrlFetcherBase`: handles screens that require Internet
-     connectivity.
-
-  * `urlfetcher.SimpleUrlFetcherBase`: similar as `UrlFetcherBase`,
-     with simpler options (to avoid overhead to build your own argument
-     parsing, and usage documentation)
-
-  * `rssfeed.RSSFeedScreenBase`: handles RSS parsing from Internet.
-
-  * `rssfeed.SimpleRSSFeedScreenBase`: similar as `RSSFeedScreenBase`,
-     with simpler options (to avoid overhead to build your own argument
-     parsing, and usage documentation)
-
-
-Build your own screen
-=====================
-
-It is very simple to inherit from these base classes and create your own
-screen. See some of the examples implemented here already. Basically, you will
-need to:
-
-    * define a name and description for your screen (class instantiation)
-      and keep them as short as possible (avoid too much typing)
-
-    * if applicable, define your command-line usage guidelines and options
-      (see `cli_opts`), if appropriate and override `_parse_args` method.
-      Create your help/usage text by overriding the `_usage_options_example`
-      method.
-
-    * build your action by overriding the `_run_cycle` method, if applicable
-      (the base class will be triggered by the `autorun` method that loops
-      indefinitely or until there is a keyboard interruption (ctrl+C).
-
-Before you start, though, I strongly advise you to check out the code here
-thoroughly, to avoid reinventing the wheel in parts that are already covered.
-Additionally, consistency is important, so try to keep the same concept of how
-things are done here... Well, if you have better idea, I am very opened to
-adapt (but then instead of making a mess, we would change it all to be still
-consistent).
-
-"""
-
-#
-# Python built-in modules
-#
-import os
-import getopt
-import sys
-
-#
-# Internal modules
-#
-from termsaverlib import common, constants, exception
-from termsaverlib.screen.helper import ScreenHelperBase
-from termsaverlib.i18n import _
-
-
-class ScreenBase(ScreenHelperBase):
-    """
-    This is the main screen that all screens must inherit in order to be part
-    of the screensaver list, accessible with termsaver command-line options.
-
-    When inheriting this to your own screen, remember to override the
-    following methods:
-
-        * `_run_cycle`: define here the algorithm to display a text-based
-           look-alike screensaver. See other classes for example on how to
-           use this.
-
-        * `_usage_options_example`: print out here the options and examples
-           on how to use your screen. See other classes for examples on how
-           to use this.
-
-        * `_parse_args`: from a properly parsed (using getopt) argument list,
-           customize the configuration of your screen accordingly
-
-    That's all you need to do!
-
-    Additionally, you can also call the following helper methods:
-
-        * `screen_exit`: if by any reason you need to close the application
-          (remember, in most cases, you can just rely on throwing exceptions
-          that are understood by termsaver application, available in
-          `termsaverlib.exception` module)
-
-        * `log` : if you need to write anything on screen before or after a
-           screen cycle, you can do it in style by calling this method, which
-           will inform the screen as a prefix to the message being displayed
-           on screen.
-
-    You can also use the following optional property:
-
-        * `cleanup_per_cycle`:  Defines if the screen should be cleaned up for
-           every rotation cycle (new file).
-
-    IMPORTANT:
-               All other methods are not to be tempered with!
-    """
-
-    name = ''
-    """
-    Defines the name of the screen.
-    """
-
-    description = ''
-    """
-    Defines the description (short) of the screen.
-    """
-
-    cli_opts = {}
-    """
-    Defines the getopt format command-line options of the screen. It should be
-    an object in the following structure:
-
-    cli_opts = {
-                 'opts': 'h',
-                 'long_opts': ['help',],
-    }
-    """
-
-    cleanup_per_cycle = False
-    """
-    Defines if the screen should be cleaned up for every rotation cycle
-    (new file).
-    """
-
-    def __init__(self, name, description, cli_opts):
-        """
-        The basic constructor of this class. You need to inform basic
-        information about your screen:
-
-           * `name`: describes the name of the screen (try to keep it short,
-                     and/or abbreviated, as much as possible)
-
-           * `description`: a brief (very brief) description of what the screen
-                            does (if you need to write more documentation about
-                            it, you can rely on man docs for that)
-
-           * `cli_opts`: the command line options that will be available for
-                         your screen (use getopt formatting)
-        """
-        self.name = name
-        self.description = description
-        self.cli_opts = cli_opts
-
-    def autorun(self, args, loop=True):
-        """
-        The accessible method for dynamically running a screen.
-        This method will basically parse the arguments, prepare them with
-        the method `_parse_args` that is inherited in sub-classes, and with
-        the property `cli_opts` that holds the formatting of the arguments.
-
-        Once all is ready to go, this will call the `_run_cycle` method, which
-        is filled in the sub-classes with the algorithms to display text on
-        screen to behave as a screensaver.
-
-        The arguments of this method are:
-
-            * args: (MANDATORY) the arguments passed when termsaver is executed
-                    from command-line. See `termsaver` script for details.
-
-            * loop: (OPTIONAL) defines if termsaver should be executing on an
-                    infinite looping (goes on until the keyboard interrupt
-                    (Ctrl+C) is pressed), or not. This is up to the screen
-                    action (or end-user through configuable setting) to decide.
-        """
-
-        # prepare values and validate
-        if not args:
-            args = ''
-        if not self.cli_opts \
-            or 'opts' not in self.cli_opts.keys() \
-                or not self.cli_opts['opts']:
-            self.cli_opts['opts'] = ''
-        if not self.cli_opts['long_opts']:
-            self.cli_opts['long_opts'] = []
-        else:
-            if not type(self.cli_opts['long_opts']) is list or \
-                [type(i) == str for i in self.cli_opts['long_opts']] \
-                    != [True for __ in range(len(self.cli_opts['long_opts']))]:
-                #
-                # Don't worry too much about errors here. This is supposed to
-                # help developers while programming screens for this app.
-                #
-                raise Exception("Value of 'long_opts' in cli_opts dict MUST "\
-                                "be a list of strings.")
-
-        try:
-            self._parse_args(getopt.getopt(args, self.cli_opts['opts'],
-                                     self.cli_opts['long_opts']))
-        except getopt.GetoptError, e:
-            raise exception.InvalidOptionException("", str(e))
-
-        # execute the cycle
-        self.clear_screen()
-
-        while(loop):
-            try:
-                self._run_cycle()
-            except KeyboardInterrupt, e:
-                #
-                # do some cleanup if applicable
-                #
-                self._on_keyboard_interrupt()
-                raise e
-
-            # Clear screen if appropriate
-            if self.cleanup_per_cycle:
-                self.clear_screen()
-
-    def _run_cycle(self):
-        """
-        Executes a cycle of this screen. This base class actually does not hold
-        any special actions to begin with, but executing it from inheriting
-        classes is also a good practice, to allow future implementations that
-        must be taken from a base class.
-        """
-        pass
-
-    @staticmethod
-    def usage_header():
-        """
-        Simply prints a header information, used with the `usage` method.
-
-        See also `usage` method for details.
-        """
-        print """%(app_title)s v.%(app_version)s - %(app_description)s.
-""" % {
-               'app_title': constants.App.TITLE,
-               'app_version': constants.App.VERSION,
-               'app_description': constants.App.DESCRIPTION,
-        }
-
-    @staticmethod
-    def usage_footer():
-        """
-        Simply prints a footer information, used with the `usage` method.
-
-        See also `usage` method for details.
-        """
-        print """--
-See more information about this project at:
-%(url)s
-
-Report bugs to authors at:
-%(source_url)s
-""" % {
-        'url': constants.App.URL,
-        'source_url': constants.App.SOURCE_URL,
-       }
-
-    def _usage_options_example(self):
-        """
-        Describe here the options and examples of your screen.
-        See some examples of already implemented base screens so you can
-        write similar stuff on your own, and keep consistency.
-        """
-        pass
-
-    def usage(self):
-        """
-        Defines the usage information that is presented when a user hits the
-        help option.You should not directly override this method, instead, just
-        override the protected method `_usage_options_example`, created for
-        this purpose. All other stuff will be defined by the `usage_header` and
-        `usage_footer` methods.
-        """
-
-        # header
-        self.usage_header()
-
-        print _("""Screen: %(screen)s
-Description: %(description)s
-
-Usage: %(app_name)s %(screen)s [options]""") % {
-               'app_name': constants.App.NAME,
-               'screen': self.name,
-               'description': self.description,
-        }
-        # any additional info in between (see other classes for reference)
-        self._usage_options_example()
-
-        #footer
-        self.usage_footer()
-
-    def _parse_args(self, prepared_args):
-        """
-        (protected) MUST be overriden in inheriting classes, to deal with
-        special arguments that will customize values for them.
-        """
-        pass
-
-    def screen_exit(self, error=0):
-        """
-        Exits the screen (and finishes the application) with a specific error.
-        If none is informed, it exits as successful (error 0).
-        """
-        sys.exit(error)
-
-    def log(self, text):
-        """
-        Prints a log message on screen in the format:
-            %(app_name)s.%(screen)s: %(message)s
-        """
-        print "%s.%s: %s" % (constants.App.NAME, self.name, text)
-
-    def _on_keyboard_interrupt(self):
-        """
-        Executes extra commands if the keyboard interrupt exception happened
-        while running a cycle. 
-        """
+###############################################################################
+#
+# file:     __init__.py
+#
+# Purpose:  refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+This module holds base classes that are used by all screens within termsaver
+application. Each individual "screen" represents a unique screensaver that can
+be triggered by termsaver.
+
+The base classes available in this package are:
+
+  * `ScreenBase`: the most basic screen class, which will handle simple
+                  interaction with the terminal.
+
+  * `filereader.FileReaderBase`: handles screens that require recursive
+     directory scanning for files to be printed out
+
+  * `urlfetcher.UrlFetcherBase`: handles screens that require Internet
+     connectivity.
+
+  * `urlfetcher.SimpleUrlFetcherBase`: similar as `UrlFetcherBase`,
+     with simpler options (to avoid overhead to build your own argument
+     parsing, and usage documentation)
+
+  * `rssfeed.RSSFeedScreenBase`: handles RSS parsing from Internet.
+
+  * `rssfeed.SimpleRSSFeedScreenBase`: similar as `RSSFeedScreenBase`,
+     with simpler options (to avoid overhead to build your own argument
+     parsing, and usage documentation)
+
+
+Build your own screen
+=====================
+
+It is very simple to inherit from these base classes and create your own
+screen. See some of the examples implemented here already. Basically, you will
+need to:
+
+    * define a name and description for your screen (class instantiation)
+      and keep them as short as possible (avoid too much typing)
+
+    * if applicable, define your command-line usage guidelines and options
+      (see `cli_opts`), if appropriate and override `_parse_args` method.
+      Create your help/usage text by overriding the `_usage_options_example`
+      method.
+
+    * build your action by overriding the `_run_cycle` method, if applicable
+      (the base class will be triggered by the `autorun` method that loops
+      indefinitely or until there is a keyboard interruption (ctrl+C).
+
+Before you start, though, I strongly advise you to check out the code here
+thoroughly, to avoid reinventing the wheel in parts that are already covered.
+Additionally, consistency is important, so try to keep the same concept of how
+things are done here... Well, if you have better idea, I am very opened to
+adapt (but then instead of making a mess, we would change it all to be still
+consistent).
+
+"""
+
+#
+# Python built-in modules
+#
+import subprocess
+import sys
+
+from termsaver.termsaverlib.helper.utilities import show_stdout_cursor
+
+pynput_installed = None
+reqs = subprocess.check_output([sys.executable, '-m', 'pip', 'freeze'])
+installed_packages = [r.decode().split('==')[0] for r in reqs.split()]
+if 'pynput' in installed_packages:
+    pynput_installed = True
+    from pynput import keyboard
+
+#
+# Internal modules
+#
+from termsaver.termsaverlib import constants
+from termsaver.termsaverlib.i18n import _
+from termsaver.termsaverlib.screen.helper import ScreenHelperBase
+
+
+class ScreenBase(ScreenHelperBase):
+    """
+    This is the main screen that all screens must inherit in order to be part
+    of the screensaver list, accessible with termsaver command-line options.
+
+    When inheriting this to your own screen, remember to override the
+    following methods:
+
+        * `_run_cycle`: define here the algorithm to display a text-based
+           look-alike screensaver. See other classes for example on how to
+           use this.
+
+        * `_usage_options_example`: print out here the options and examples
+           on how to use your screen. See other classes for examples on how
+           to use this.
+
+        * `_parse_args`: from a properly parsed (using getopt) argument list,
+           customize the configuration of your screen accordingly
+
+    That's all you need to do!
+
+    Additionally, you can also call the following helper methods:
+
+        * `screen_exit`: if by any reason you need to close the application
+          (remember, in most cases, you can just rely on throwing exceptions
+          that are understood by termsaver application, available in
+          `termsaverlib.exception` module)
+
+        * `log` : if you need to write anything on screen before or after a
+           screen cycle, you can do it in style by calling this method, which
+           will inform the screen as a prefix to the message being displayed
+           on screen.
+
+    You can also use the following optional property:
+
+        * `cleanup_per_cycle`:  Defines if the screen should be cleaned up for
+           every rotation cycle (new file).
+
+    IMPORTANT:
+               All other methods are not to be tempered with!
+    """
+
+    name = ''
+    """
+    Defines the name of the screen.
+    """
+
+    parser = None
+    """
+    The argument parser for the screen
+    """
+
+    description = ''
+    """
+    Defines the description (short) of the screen.
+    """
+
+    cleanup_per_cycle = False
+    """
+    Defines if the screen should be cleaned up for every rotation cycle
+    (new file).
+    """
+
+    def __init__(self, name, description, parser=None):
+        """
+        The basic constructor of this class. You need to inform basic
+        information about your screen:
+
+           * `name`: describes the name of the screen (try to keep it short,
+                     and/or abbreviated, as much as possible)
+
+           * `description`: a brief (very brief) description of what the screen
+                            does (if you need to write more documentation about
+                            it, you can rely on man docs for that)
+        """
+        self.parser = parser
+        if self.parser:
+            self.parser.prog = "termsaver " + name
+
+        self.name = name
+        self.description = description
+        
+        if pynput_installed is not None:
+            self.listener = keyboard.Listener(
+                on_press=self.on_press,
+                on_release=self.on_release
+            )
+    
+    def on_press(self, key):
+        """
+        This method is called when a key is pressed.
+        """
+        if pynput_installed is not None:
+            self.listener.stop()
+    
+    def on_release(self, key):
+        """
+        This method is called when a key is released.
+        Unused for now, but leaving it in so we have options in the future.
+        """
+        pass
+
+    def autorun(self, loop=True):
+        """
+        The accessible method for dynamically running a screen.
+        This method will basically parse the arguments, prepare them with
+        the method `_parse_args` that is inherited in sub-classes, and with
+        the property `cli_opts` that holds the formatting of the arguments.
+
+        Once all is ready to go, this will call the `_run_cycle` method, which
+        is filled in the sub-classes with the algorithms to display text on
+        screen to behave as a screensaver.
+
+        The arguments of this method are:
+
+            * args: (MANDATORY) the arguments passed when termsaver is executed
+                    from command-line. See `termsaver` script for details.
+
+            * loop: (OPTIONAL) defines if termsaver should be executing on an
+                    infinite looping (goes on until the keyboard interrupt
+                    (Ctrl+C) is pressed), or not. This is up to the screen
+                    action (or end-user through configuable setting) to decide.
+        """
+        # execute the cycle
+        self.clear_screen()
+
+        if pynput_installed is not None:
+            self.listener.start()
+        while(
+            (loop and pynput_installed is None)
+            or
+            (loop and pynput_installed is not None and self.listener.is_alive())
+        ):
+            try:
+                self._run_cycle()
+            except KeyboardInterrupt as e:
+                #
+                # do some cleanup if applicable
+                #
+                self._on_keyboard_interrupt()
+                raise e
+
+            # Clear screen if appropriate
+            if self.cleanup_per_cycle:
+                self.clear_screen()
+        show_stdout_cursor()
+
+    def _run_cycle(self):
+        """
+        Executes a cycle of this screen. This base class actually does not hold
+        any special actions to begin with, but executing it from inheriting
+        classes is also a good practice, to allow future implementations that
+        must be taken from a base class.
+        """
+        pass
+
+    @staticmethod
+    def usage_header():
+        """
+        Simply prints a header information, used with the `usage` method.
+
+        See also `usage` method for details.
+        """
+        print ("""%(app_title)s v.%(app_version)s - %(app_description)s.
+""" % {
+               'app_title': constants.App.TITLE,
+               'app_version': constants.App.VERSION,
+               'app_description': constants.App.DESCRIPTION,
+        })
+
+    @staticmethod
+    def usage_footer():
+        """
+        Simply prints a footer information, used with the `usage` method.
+
+        See also `usage` method for details.
+        """
+        print ("""--
+See more information about this project at:
+%(url)s
+
+Report bugs to authors at:
+%(source_url)s
+""" % {
+        'url': constants.App.URL,
+        'source_url': constants.App.SOURCE_URL,
+       })
+
+    def _usage_options_example(self):
+        """
+        Describe here the examples of your screen.
+        See some examples of already implemented base screens so you can
+        write similar stuff on your own, and keep consistency.
+        """
+        pass
+
+    def usage(self):
+        """
+        Defines the usage information that is presented when a user hits the
+        help option.You should not directly override this method, instead, just
+        override the protected method `_usage_options_example`, created for
+        this purpose. All other stuff will be defined by the `usage_header` and
+        `usage_footer` methods.
+        """
+
+        # header
+        self.usage_header()
+
+        print (_("""Screen: %(screen)s
+Description: %(description)s""") % {
+               'app_name': constants.App.NAME,
+               'screen': self.name,
+               'description': self.description,
+        })
+        # any additional info in between (see other classes for reference)
+        if self.parser:
+            self.parser.print_help()
+
+        usage = self._usage_options_example()
+        if usage != None and usage != '':
+            print(_("\r\nExamples:"))
+            print(usage)
+
+        #footer
+        self.usage_footer()
+
+    def _parse_args(self, launchScreenImmediately=True):
+        """
+        (protected) MUST be overriden in inheriting classes, to deal with
+        special arguments that will customize values for them.
+        """
+        pass
+
+    def screen_exit(self, error=0):
+        """
+        Exits the screen (and finishes the application) with a specific error.
+        If none is informed, it exits as successful (error 0).
+        """
+        sys.exit(error)
+
+    def log(self, text):
+        """
+        Prints a log message on screen in the format:
+            %(app_name)s.%(screen)s: %(message)s
+        """
+        print ("%s.%s: %s" % (constants.App.NAME, self.name, text))
+
+    def _on_keyboard_interrupt(self):
+        """
+        Executes extra commands if the keyboard interrupt exception happened
+        while running a cycle. 
+        """
         pass
```

### Comparing `termsaver-0.4/termsaverlib/screen/helper/position.py` & `termsaver-0.6/termsaver/termsaverlib/screen/helper/position.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,342 +1,346 @@
-###############################################################################
-#
-# file:     position.py
-#
-# Purpose:  refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-A helper class that provides positioning functionality to screens, such as
-defining a terminal size, and centering information (horizontally or
-vertically).
-
-See additional information in the class itself.
-
-The helper class available here is:
-
-    * `PositionHelperBase`
-
-"""
-#
-# Python built-in modules
-#
-import sys
-import time
-import platform
-import math
-import random
-import textwrap
-
-#
-# Internal modules
-#
-from termsaverlib.screen.helper import ScreenHelperBase
-
-
-class PositionHelperBase(ScreenHelperBase):
-    """
-    This helper class provides positioning functionality to the screens,
-    by dealing with the current dimensions of the terminal.
-
-    There are main methods available here:
-
-        * `get_terminal_size`: retrieves the current terminal dimensions, width
-           and height, to be stored in local propertiy `geometry`.
-
-        * `center_text_vertically`: centers a specified text in vertical
-
-        * `center_text_horizontally`: centers a specified text in horizontal
-
-        * `randomize_text_vertically`: randomizes a specified text in vertical
-
-        * `randomize_text_horizontally`: randomizes a specified text in 
-           horizontal
-
-    If the method `get_terminal_size` is never called, all other functionality,
-    relying on terminal dimensions, will just based on a default size, set as
-    80x25.
-
-    The main properties available are:
-
-        * `geometry`: defines the size of the terminal (populated by the
-          `get_terminal_size` method, whenever called.
-
-        * `position`: defines the current position of the text to be printed,
-           based on usage of other methods that temper with text positioning
-           (eg. `randomize_text_horizontally`)
-
-        * `changed_geometry`: for every call to `get_terminal_size` method,
-           holds the information if the terminal has changed size or not.
-    """
-    
-    geometry = {
-        'x' : 0,
-        'y' : 0,
-    }
-    """
-    Defines the current terminal width and height.
-    Its default value is set as 80x25.
-    """
-
-    __old_geometry = {
-        'x' : 0,
-        'y' : 0,
-    }
-    """
-    Private property to track changes in the geometry. Refer to
-    `changed_geometry` to identify any terminal size changes.
-    """
-    
-    changed_geometry = False
-    """
-    A simple boolean that identifies if the terminal has changed size since the
-    last check with `get_terminal_size`. This is handy to decide what to do
-    with a particular screen (eg: clear and redraw again?).
-    """
-    
-    position = {
-        'x' : 0,
-        'y' : 0,
-    }
-    """
-    Stores the latest position X-Y axis (width and height) position value after
-    calling the randomizing methods of this class (useful to allow you to know
-    the previous location of the text in the window) 
-    """
-    
-    def fix_text_wrap(self, text):
-        """
-        Wraps the text to the geometry size, maintaining existing new lines.
-        """
-
-        # fail safe if the screen does not properly set geometry
-        if self.geometry['x'] == 0:
-            return text
-
-        temp = text.split("\n")
-        longest_line = max([len(x) for x in temp])
-        new_text = []
-        for l in temp:
-            t = "\n".join(textwrap.wrap(l, width=self.geometry['x']))
-            
-            # fill in trailing blanks
-            t += " " * (min(longest_line, self.geometry['x']) - min(len(t), self.geometry['x']))
-            new_text.append(t)
-        return "\n".join(new_text)
-    
-    def center_text_vertically(self, text):
-        """
-        Returns the text argument with additional new lines, calculated to
-        display the text in the vertical center of the screen.
-
-        Arguments:
-
-            * text: the text to be vertically centered
-        """
-
-        temp = self.fix_text_wrap(text).split("\n")
-        self.position['y'] = int(math.floor(
-                (self.geometry['y'] - len(temp)) / 2))
-        return "\n" * self.position['y'] + text
-        
-    def center_text_horizontally(self, text):
-        """
-        Returns the text argument with additional blank spaces, calculated to
-        display the text in the horizontal center of the screen.
-
-        Arguments:
-
-            * text: the text to be horizontally centered
-        """
-
-        temp = self.fix_text_wrap(text).split("\n")
-        new_text = ""
-        for t in temp:
-            self.position['x'] = int(math.ceil(
-                    (self.geometry['x'] - len(t)) / 2))
-            new_text += " " * self.position['x'] + t
-            if len(temp) > 1:
-                new_text += "\n"
-
-        return new_text
-
-    def align_text_right(self, text):
-        """
-        Returns the text argument with additional blank spaces, calculated to
-        display the text in the right.
-
-        Arguments:
-
-            * text: the text to be aligned
-        """
-        return " " * (self.geometry['x'] - len(text)) + text
-
-    def randomize_text_horizontally(self, text):
-        """
-        Returns the text argument with additional blank spaces, calculated to
-        display the text in a random position of the screen.
-
-        Arguments:
-
-            * text: the text to be horizontally randomized
-        """
-
-        # find longest line
-        temp = self.fix_text_wrap(text).split("\n")
-        longest_line = max([len(x) for x in temp])
-
-        self.position['x'] = random.randint(0, 
-                self.geometry['x'] - longest_line)
-        
-        new_text = ""
-        for t in temp:
-            new_text += " " * self.position['x'] + t
-            if len(temp) > 0:
-                new_text += "\n"
-
-        return new_text
-
-    def randomize_text_vertically(self, text):
-        """
-        Returns the text argument with additional new lines, calculated to
-        display the text in a random position of the screen.
-
-        Arguments:
-
-            * text: the text to be vertically randomized
-        """
-        total_lines = len(self.fix_text_wrap(text).split("\n"))
-        self.position['y'] = random.randint(0, 
-                max(0, self.geometry['y'] - total_lines))
-        
-        return "\n" * self.position['y'] + text
-
-    def get_terminal_size(self):
-        """ 
-        Retrieves the screen terminal dimensions, returning a tuple
-        (width, height), and will also store them in internal property 
-        `geometry`.
-        
-        Copyright note:
-        This code has been adapted from:
-        http://stackoverflow.com/questions/566746/\
-            how-to-get-console-window-width-in-python
-
-        posted by Harco Kuppens, at Jul 1 '11 at 16:23.
-
-        """
-        
-        # This is required if you are programming from non-windows platforms
-        # more on this at: http://pydev.org/manual_adv_assistants.html
-        #@PydevCodeAnalysisIgnore
-        def _get_terminal_size_windows():
-            res = None
-            try:
-                from ctypes import windll, create_string_buffer
-        
-                # stdin handle is -10
-                # stdout handle is -11
-                # stderr handle is -12
-                h = windll.kernel32.GetStdHandle(-12)
-                csbi = create_string_buffer(22)
-                res = windll.kernel32.GetConsoleScreenBufferInfo(h, csbi)
-            except:
-                return None
-            if res:
-                import struct
-                (_, _, _, _, _,
-                 left, top, right, bottom, _, _) = struct.unpack("hhhhHhhhhhh",
-                                                                 csbi.raw)
-                sizex = right - left + 1
-                sizey = bottom - top + 1
-                return sizex, sizey
-            else:
-                return None
-        
-        def _get_terminal_size_tput():
-            try:
-                import subprocess
-                proc = subprocess.Popen(["tput", "cols"], 
-                                        stdin = subprocess.PIPE, 
-                                        stdout = subprocess.PIPE)
-                output = proc.communicate(input = None)
-                cols = int(output[0])
-                proc = subprocess.Popen(["tput", "lines"], 
-                                        stdin = subprocess.PIPE, 
-                                        stdout = subprocess.PIPE)
-                output = proc.communicate(input = None)
-                rows = int(output[0])
-                return (cols, rows)
-            except:
-                return None
-        
-        
-        def _get_terminal_size_linux():
-            def ioctl_GWINSZ(fd):
-                try:
-                    import fcntl, termios, struct
-                    cr = struct.unpack('hh', fcntl.ioctl(fd, 
-                                                         termios.TIOCGWINSZ, 
-                                                         '1234'))
-                except:
-                    return None
-                return cr
-            cr = ioctl_GWINSZ(0) or ioctl_GWINSZ(1) or ioctl_GWINSZ(2)
-            if not cr:
-                try:
-                    fd = os.open(os.ctermid(), os.O_RDONLY)
-                    cr = ioctl_GWINSZ(fd)
-                    os.close(fd)
-                except:
-                    pass
-            if not cr:
-                try:
-                    cr = (os.environ['LINES'], os.environ['COLUMNS'])
-                except:
-                    return None
-            return int(cr[1]), int(cr[0])
-        
-        current_os = platform.system()
-        tuple_xy = None
-        if current_os == 'Windows':
-            tuple_xy = _get_terminal_size_windows()
-            if tuple_xy is None:
-                tuple_xy = _get_terminal_size_tput()
-                # needed for window's python in cygwin's xterm!
-        if current_os == 'Linux' or current_os == 'Darwin' or \
-                current_os.startswith('CYGWIN'):
-            tuple_xy = _get_terminal_size_linux()
-        if tuple_xy is None:
-            tuple_xy = (80, 25)  # default value
-        
-        self.geometry['x'], self.geometry['y'] = tuple_xy
-
-        # store geometry changes
-        if self.__old_geometry == {'x': 0, 'y': 0}:
-            # first time checking geometry
-            self.__old_geometry = self.geometry.copy()
-            self.changed_geometry = False
-        elif self.__old_geometry != self.geometry:
-            self.__old_geometry = self.geometry.copy()
-            self.changed_geometry = True
-        else:
-            self.changed_geometry = False
+###############################################################################
+#
+# file:     position.py
+#
+# Purpose:  refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+A helper class that provides positioning functionality to screens, such as
+defining a terminal size, and centering information (horizontally or
+vertically).
+
+See additional information in the class itself.
+
+The helper class available here is:
+
+    * `PositionHelperBase`
+
+"""
+import math
+import platform
+import random
+#
+# Python built-in modules
+#
+import sys
+import textwrap
+import time
+
+#
+# Internal modules
+#
+from termsaver.termsaverlib.screen.helper import ScreenHelperBase
+
+
+class PositionHelperBase(ScreenHelperBase):
+    """
+    This helper class provides positioning functionality to the screens,
+    by dealing with the current dimensions of the terminal.
+
+    There are main methods available here:
+
+        * `get_terminal_size`: retrieves the current terminal dimensions, width
+           and height, to be stored in local propertiy `geometry`.
+
+        * `center_text_vertically`: centers a specified text in vertical
+
+        * `center_text_horizontally`: centers a specified text in horizontal
+
+        * `randomize_text_vertically`: randomizes a specified text in vertical
+
+        * `randomize_text_horizontally`: randomizes a specified text in 
+           horizontal
+
+    If the method `get_terminal_size` is never called, all other functionality,
+    relying on terminal dimensions, will just based on a default size, set as
+    80x25.
+
+    The main properties available are:
+
+        * `geometry`: defines the size of the terminal (populated by the
+          `get_terminal_size` method, whenever called.
+
+        * `position`: defines the current position of the text to be printed,
+           based on usage of other methods that temper with text positioning
+           (eg. `randomize_text_horizontally`)
+
+        * `changed_geometry`: for every call to `get_terminal_size` method,
+           holds the information if the terminal has changed size or not.
+    """
+    
+    geometry = {
+        'x' : 0,
+        'y' : 0,
+    }
+    """
+    Defines the current terminal width and height.
+    Its default value is set as 80x25.
+    """
+
+    __old_geometry = {
+        'x' : 0,
+        'y' : 0,
+    }
+    """
+    Private property to track changes in the geometry. Refer to
+    `changed_geometry` to identify any terminal size changes.
+    """
+    
+    changed_geometry = False
+    """
+    A simple boolean that identifies if the terminal has changed size since the
+    last check with `get_terminal_size`. This is handy to decide what to do
+    with a particular screen (eg: clear and redraw again?).
+    """
+    
+    position = {
+        'x' : 0,
+        'y' : 0,
+    }
+    """
+    Stores the latest position X-Y axis (width and height) position value after
+    calling the randomizing methods of this class (useful to allow you to know
+    the previous location of the text in the window) 
+    """
+    
+    def fix_text_wrap(self, text):
+        """
+        Wraps the text to the geometry size, maintaining existing new lines.
+        """
+
+        # fail safe if the screen does not properly set geometry
+        if self.geometry['x'] == 0:
+            return text
+
+        temp = text.split("\n")
+        longest_line = max([len(x) for x in temp])
+        new_text = []
+        for l in temp:
+            # if utf string thwn width must be bigger
+            overlen = len(l)-len(l) #.decode('utf-8)'))
+            t = "\n".join(textwrap.wrap(l, width=self.geometry['x']+overlen))
+            
+            # fill in trailing blanks
+            t += " " * (min(longest_line, self.geometry['x']) - min(len(t), self.geometry['x']))
+            new_text.append(t)
+        return "\n".join(new_text)
+    
+    def center_text_vertically(self, text):
+        """
+        Returns the text argument with additional new lines, calculated to
+        display the text in the vertical center of the screen.
+
+        Arguments:
+
+            * text: the text to be vertically centered
+        """
+
+        temp = self.fix_text_wrap(text).split("\n")
+        self.position['y'] = int(math.floor(
+                (self.geometry['y'] - len(temp)) / 2))
+        return "\n" * self.position['y'] + text
+        
+    def center_text_horizontally(self, text):
+        """
+        Returns the text argument with additional blank spaces, calculated to
+        display the text in the horizontal center of the screen.
+
+        Arguments:
+
+            * text: the text to be horizontally centered
+        """
+
+        temp = self.fix_text_wrap(text).split("\n")
+        new_text = ""
+        for t in temp:
+            self.position['x'] = int(math.ceil(
+                    (self.geometry['x'] - len(t)) / 2))
+            new_text += " " * self.position['x'] + t
+            if len(temp) > 1:
+                new_text += "\n"
+
+        return new_text
+
+    def align_text_right(self, text):
+        """
+        Returns the text argument with additional blank spaces, calculated to
+        display the text in the right.
+
+        Arguments:
+
+            * text: the text to be aligned
+        """
+        return " " * (self.geometry['x'] - len(text)) + text
+
+    def randomize_text_horizontally(self, text):
+        """
+        Returns the text argument with additional blank spaces, calculated to
+        display the text in a random position of the screen.
+
+        Arguments:
+
+            * text: the text to be horizontally randomized
+        """
+
+        # find longest line
+        temp = self.fix_text_wrap(text).split("\n")
+        longest_line = max([len(x) for x in temp])
+
+        self.position['x'] = random.randint(0, 
+                self.geometry['x'] - longest_line)
+        
+        new_text = ""
+        for t in temp:
+            new_text += " " * self.position['x'] + t
+            if len(temp) > 0:
+                new_text += "\n"
+
+        return new_text
+
+    def randomize_text_vertically(self, text):
+        """
+        Returns the text argument with additional new lines, calculated to
+        display the text in a random position of the screen.
+
+        Arguments:
+
+            * text: the text to be vertically randomized
+        """
+        total_lines = len(self.fix_text_wrap(text).split("\n"))
+        self.position['y'] = random.randint(0, 
+                max(0, self.geometry['y'] - total_lines))
+        
+        return "\n" * self.position['y'] + text
+
+    def get_terminal_size(self):
+        """ 
+        Retrieves the screen terminal dimensions, returning a tuple
+        (width, height), and will also store them in internal property 
+        `geometry`.
+        
+        Copyright note:
+        This code has been adapted from:
+        http://stackoverflow.com/questions/566746/\
+            how-to-get-console-window-width-in-python
+
+        posted by Harco Kuppens, at Jul 1 '11 at 16:23.
+
+        """
+        
+        # This is required if you are programming from non-windows platforms
+        # more on this at: http://pydev.org/manual_adv_assistants.html
+        #@PydevCodeAnalysisIgnore
+        def _get_terminal_size_windows():
+            res = None
+            try:
+                from ctypes import create_string_buffer, windll
+
+                # stdin handle is -10
+                # stdout handle is -11
+                # stderr handle is -12
+                h = windll.kernel32.GetStdHandle(-12)
+                csbi = create_string_buffer(22)
+                res = windll.kernel32.GetConsoleScreenBufferInfo(h, csbi)
+            except:
+                return None
+            if res:
+                import struct
+                (_, _, _, _, _,
+                 left, top, right, bottom, _, _) = struct.unpack("hhhhHhhhhhh",
+                                                                 csbi.raw)
+                sizex = right - left + 1
+                sizey = bottom - top + 1
+                return sizex, sizey
+            else:
+                return None
+        
+        def _get_terminal_size_tput():
+            try:
+                import subprocess
+                proc = subprocess.Popen(["tput", "cols"], 
+                                        stdin = subprocess.PIPE, 
+                                        stdout = subprocess.PIPE)
+                output = proc.communicate(input = None)
+                cols = int(output[0])
+                proc = subprocess.Popen(["tput", "lines"], 
+                                        stdin = subprocess.PIPE, 
+                                        stdout = subprocess.PIPE)
+                output = proc.communicate(input = None)
+                rows = int(output[0])
+                return (cols, rows)
+            except:
+                return None
+        
+        
+        def _get_terminal_size_linux():
+            def ioctl_GWINSZ(fd):
+                try:
+                    import fcntl
+                    import struct
+                    import termios
+                    cr = struct.unpack('hh', fcntl.ioctl(fd, 
+                                                         termios.TIOCGWINSZ, 
+                                                         '1234'))
+                except:
+                    return None
+                return cr
+            cr = ioctl_GWINSZ(0) or ioctl_GWINSZ(1) or ioctl_GWINSZ(2)
+            if not cr:
+                try:
+                    fd = os.open(os.ctermid(), os.O_RDONLY)
+                    cr = ioctl_GWINSZ(fd)
+                    os.close(fd)
+                except:
+                    pass
+            if not cr:
+                try:
+                    cr = (os.environ['LINES'], os.environ['COLUMNS'])
+                except:
+                    return None
+            return int(cr[1]), int(cr[0])
+        
+        current_os = platform.system()
+        tuple_xy = None
+        if current_os == 'Windows':
+            tuple_xy = _get_terminal_size_windows()
+            if tuple_xy is None:
+                tuple_xy = _get_terminal_size_tput()
+                # needed for window's python in cygwin's xterm!
+        if current_os == 'Linux' or current_os == 'Darwin' or \
+                current_os.startswith('CYGWIN'):
+            tuple_xy = _get_terminal_size_linux()
+        if tuple_xy is None:
+            tuple_xy = (80, 25)  # default value
+        
+        self.geometry['x'], self.geometry['y'] = tuple_xy
+
+        # store geometry changes
+        if self.__old_geometry == {'x': 0, 'y': 0}:
+            # first time checking geometry
+            self.__old_geometry = self.geometry.copy()
+            self.changed_geometry = False
+        elif self.__old_geometry != self.geometry:
+            self.__old_geometry = self.geometry.copy()
+            self.changed_geometry = True
+        else:
+            self.changed_geometry = False
```

### Comparing `termsaver-0.4/termsaverlib/screen/helper/typing.py` & `termsaver-0.6/termsaver/termsaverlib/screen/helper/typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-###############################################################################
-#
-# file:     typing.py
-#
-# Purpose:  refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-A helper class used for screens that require more dynamic output to users.
-See additional information in the class itself.
-
-The helper class available here is:
-
-    * `TypingHelperBase`
-
-"""
-#
-# Python built-in modules
-#
-import sys
-import time
-
-#
-# Internal modules
-#
-from termsaverlib.screen.helper import ScreenHelperBase
-from termsaverlib import constants
-
-
-class TypingHelperBase(ScreenHelperBase):
-    """
-    This helper class gives functionality to screens to print out information
-    in a more interactive way, simulating a typing writer machine, based on
-    two main speed control properties:
-
-        * `delay`: defines the delay for printing out characters of a string
-
-        * `line_delay`: defines the delay for printing out new lines within a
-          string (sometimes, setting different proportions make a lot of a
-          difference)
-
-    If no values are defined by the screen itself, default values should be
-    used. The `delay` is set in `constants.Settings.CHAR_DELAY_SECONDS`, and
-    the `line_delay` is 10 times the value of delay.
-
-    To use this screen helper is pretty straightforward, just call the method:
-
-        * `typing_print`: this will print the specified text string using the
-           speed controls `delay` and `line_delay`.
-
-    """
-
-    delay = None
-    """
-    Defines the character printing delay, to give a cool visual of a
-    typing machine. This value is measured in seconds, and default marks are
-    defined in `constants.Settings.CHAR_DELAY_SECONDS`.
-    """
-
-    line_delay = None
-    """
-    Defines the delay imposed to every new line prior to char printing. By
-    default, its value is 10x the `delay`.
-    """
-
-    def typing_print(self, text):
-        """
-        Prints text with standard output to allow side-by-side printing, and
-        give the impression of a typing writer machine. The speed is controlled
-        by properties of this class: `delay` and `line_delay`.
-
-        Arguments:
-
-            * text: the text to be printed in typing style
-
-        Notes:
-
-            * This also supports new lines (\n)
-            * blank spaces, due to its lack of meaning, are ignored for speed
-              limiting, so they will be flushed all at once.
-
-        """
-        # set defaults
-        if self.delay is None:
-            self.delay = constants.Settings.CHAR_DELAY_SECONDS
-
-        if self.line_delay is None:
-            self.line_delay = 10 * self.delay
-        splitText = text.split('\n')
-        for line in splitText:
-            for char in line:
-                sys.stdout.write(char)
-
-                # only pause if it is not a blank space
-                if char != ' ':
-                    time.sleep(self.delay)
-
-                sys.stdout.flush()
-
-            # need to re-print the line removed from the split
-            sys.stdout.write('\n')
-
-            time.sleep(self.line_delay)  # specific pause for new lines
+###############################################################################
+#
+# file:     typing.py
+#
+# Purpose:  refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+A helper class used for screens that require more dynamic output to users.
+See additional information in the class itself.
+
+The helper class available here is:
+
+    * `TypingHelperBase`
+
+"""
+#
+# Python built-in modules
+#
+import sys
+import time
+
+from termsaver.termsaverlib import constants
+#
+# Internal modules
+#
+from termsaver.termsaverlib.screen.helper import ScreenHelperBase
+
+
+class TypingHelperBase(ScreenHelperBase):
+    """
+    This helper class gives functionality to screens to print out information
+    in a more interactive way, simulating a typing writer machine, based on
+    two main speed control properties:
+
+        * `delay`: defines the delay for printing out characters of a string
+
+        * `line_delay`: defines the delay for printing out new lines within a
+          string (sometimes, setting different proportions make a lot of a
+          difference)
+
+    If no values are defined by the screen itself, default values should be
+    used. The `delay` is set in `constants.Settings.CHAR_DELAY_SECONDS`, and
+    the `line_delay` is 10 times the value of delay.
+
+    To use this screen helper is pretty straightforward, just call the method:
+
+        * `typing_print`: this will print the specified text string using the
+           speed controls `delay` and `line_delay`.
+
+    """
+
+    delay = None
+    """
+    Defines the character printing delay, to give a cool visual of a
+    typing machine. This value is measured in seconds, and default marks are
+    defined in `constants.Settings.CHAR_DELAY_SECONDS`.
+    """
+
+    line_delay = None
+    """
+    Defines the delay imposed to every new line prior to char printing. By
+    default, its value is 10x the `delay`.
+    """
+
+    def typing_print(self, text):
+        """
+        Prints text with standard output to allow side-by-side printing, and
+        give the impression of a typing writer machine. The speed is controlled
+        by properties of this class: `delay` and `line_delay`.
+
+        Arguments:
+
+            * text: the text to be printed in typing style
+
+        Notes:
+
+            * This also supports new lines (\n)
+            * blank spaces, due to its lack of meaning, are ignored for speed
+              limiting, so they will be flushed all at once.
+
+        """
+        # set defaults
+        if self.delay is None:
+            self.delay = constants.Settings.CHAR_DELAY_SECONDS
+
+        if self.line_delay is None:
+            self.line_delay = 10 * self.delay
+        splitText = text.split("\n")
+        for line in splitText:
+            for char in line:
+                sys.stdout.write(char)
+
+                # only pause if it is not a blank space
+                if char != ' ':
+                    time.sleep(self.delay)
+
+                sys.stdout.flush()
+
+            # need to re-print the line removed from the split
+            sys.stdout.write('\n')
+
+            time.sleep(self.line_delay)  # specific pause for new lines
```

### Comparing `termsaver-0.4/termsaverlib/screen/helper/__init__.py` & `termsaver-0.6/termsaver/termsaverlib/screen/helper/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-###############################################################################
-#
-# file:     __init__.py
-#
-# Purpose:  refer to package documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-This package holds all helper classes used by termsaver screens, to add
-reusable functionality to them, and help maintain consistency throughout all
-of them.
-
-All helper screens should inherit from the base screen helper
-`ScreenHelperBase`, documented below.
-
-The available classes in this package are:
-
-    * `ScreenHelperBase`: the main helper class from which all helper classes
-      will inherit from.
-
-    * `typing.TypingHelperBase`: helper functionality to display typing writer
-      effects for screens.
-
-    * `urlfetcher.URLFetcherHelperBase`: helper functionalities to give
-      Internet connectivity to screens.
-
-    * `xmlreader.XMLReaderHelperBase`: helper functionalities to assist on
-       XML parsing.
-
-"""
-#
-# Python built-in modules
-#
-from os import system
-
-#
-# Internal modules
-#
-from termsaverlib.common import is_windows
-
-
-class ScreenHelperBase(object):
-    """
-    This is the main helper class from which all should inherit from. This
-    will also hold most rudimentary functionalities that can be reused by
-    all screens.
-    """
-
-    @staticmethod
-    def clear_screen():
-        """
-        A simple method that clears the screen.
-
-        This supports both Windows and Unix base systems.
-        """
-        if is_windows():
-            # Execute command for Windows Platform, DOS console
-            __ = system('cls')  # Windows prints the output of this call
-        else:
-            # Execute command for Unix based Platform
-            system('clear')
+###############################################################################
+#
+# file:     __init__.py
+#
+# Purpose:  refer to package documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+This package holds all helper classes used by termsaver screens, to add
+reusable functionality to them, and help maintain consistency throughout all
+of them.
+
+All helper screens should inherit from the base screen helper
+`ScreenHelperBase`, documented below.
+
+The available classes in this package are:
+
+    * `ScreenHelperBase`: the main helper class from which all helper classes
+      will inherit from.
+
+    * `typing.TypingHelperBase`: helper functionality to display typing writer
+      effects for screens.
+
+    * `urlfetcher.URLFetcherHelperBase`: helper functionalities to give
+      Internet connectivity to screens.
+
+    * `xmlreader.XMLReaderHelperBase`: helper functionalities to assist on
+       XML parsing.
+
+"""
+#
+# Python built-in modules
+#
+from os import system
+
+#
+# Internal modules
+#
+from termsaver.termsaverlib.common import is_windows
+
+
+class ScreenHelperBase(object):
+    """
+    This is the main helper class from which all should inherit from. This
+    will also hold most rudimentary functionalities that can be reused by
+    all screens.
+    """
+
+    @staticmethod
+    def clear_screen():
+        """
+        A simple method that clears the screen.
+
+        This supports both Windows and Unix base systems.
+        """
+        if is_windows():
+            # Execute command for Windows Platform, DOS console
+            __ = system('cls')  # Windows prints the output of this call
+        else:
+            # Execute command for Unix based Platform
+            system('clear')
```

### Comparing `termsaver-0.4/termsaverlib/screen/helper/xmlreader.py` & `termsaver-0.6/termsaver/termsaverlib/screen/helper/xmlreader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-###############################################################################
-#
-# file:     xmlreader.py
-#
-# Purpose:  refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-A helper class used for screens that require XML handling. See
-additional information in the class itself.
-
-The helper class available here is:
-
-    * `XMLReaderHelperBase`
-
-"""
-
-#
-# Python built-in modules
-#
-import os
-from xml.dom.minidom import parse, Node, parseString
-
-#
-# Internal modules
-#
-from termsaverlib.screen.helper import ScreenHelperBase
-from termsaverlib import exception
-
-
-class XMLReaderHelperBase(ScreenHelperBase):
-    """
-    This helper class will handle basic XML parsing, not trying to solve all
-    mysteries of the universe here. What we are looking for are main nodes that
-    contain repetitive data, commonly found on a dataset, or RSS feed. More
-    complex handling is not treated at this point, but it might be implemented
-    if the need surfaces.
-
-    The basic instantiation of this class require you to inform 2 arguments:
-
-        * `base_node`: Defines the primary node where the data must be
-           retrieved from.
-
-        * `tags`: Defines which tags within the XML must be parsed to build a
-           list of dictionaries.
-
-    Those two arguments will give the hint about where is the data and which
-    piece of it you are looking for.
-
-    For actually getting the data, you will need to:
-
-        * prepare a raw data (file content, Internet data, etc) into a
-          XML object, named `__doc`; and
-        * parse the XML object into a more convenient list of dictionaries
-          that will be populated in `data` property.
-
-    To prepare the data, you have 2 options:
-
-        * `doc_xml_string`: a method that will create a dom xml document from
-          a text string (obviously it must be a XML)
-
-        * `doc_xml_file`: a method that will create a dom xml document from
-          a file content (obviously it must be a XML)
-
-    Once you have the XML properly prepared, and stored in `__doc`, you can
-    call the parsing method:
-
-        * `parse_data`: this will actually execute the action to extract the
-           information you are looking for based on the arguments passed
-           in the instantiation.
-
-    """
-
-    __doc = None
-    """
-    Holds the xml.dom.minidom document object
-    """
-
-    clean_dirt = []
-    """
-    Holds a list of strings that will be cleaned up from each result in the
-    XML data, when placing them into the `data` property. This can be pretty
-    handy to remove trailing spaces, new lines, or unwanted HTML tags from the
-    data.
-    """
-
-    base_node = None
-    """
-    Defines the primary node where the data must be retrieved from.
-    """
-
-    tags = []
-    """
-    Defines which tags within the XML must be parsed to build a
-    list of dictionaries.
-    """
-
-    data = None
-    """
-    Holds a list, created from properly parsing the dom document object in
-    `__doc`, as specified with `base_node` and `tags` filtering.
-    """
-
-    def __init__(self, base_node, tags):
-        """
-        Creates a new instance of this class.
-
-        Arguments:
-
-        * `base_node`: Defines the primary node where the data must be
-           retrieved from.
-
-        * `tags`: Defines which tags within the XML must be parsed to build a
-           list of dictionaries.
-        """
-        self.base_node = base_node
-        self.tags = tags
-
-    def parse_data(self):
-        """
-        Only call this once you have already created the dom document object,
-        by calling either `doc_xml_file` or `doc_xml_string` methods.
-
-        This will parse the document into a list, much simpler to deal with.
-        On the logic here is done, the list is available in the property `data`
-        """
-        def get_note_value(node, node_type):
-            result = ''
-            for node2 in node:
-                for node3 in node2.childNodes:
-                    if node3.nodeType == node_type:
-                        result += node3.data
-            # clean possible dirt
-            for t in self.clean_dirt:
-                # execute a loop here for dealing with multiple occurrences
-                # (such as multiple spaces)
-                while result.find(t) > -1:
-                    result = result.replace(t, "")
-            return result
-
-        if self.__doc is None:
-            raise Exception("""You must parse the raw data, by calling a \
-doc_xml_* method to populate the dom document object.""")
-
-        result = []
-        for node in self.__doc.getElementsByTagName(self.base_node):
-            temp = {}
-            for tag in self.tags:
-                temp[tag] = get_note_value(node.getElementsByTagName(tag),
-                                           Node.TEXT_NODE)
-                if not temp[tag]:
-                    temp[tag] = get_note_value(node.getElementsByTagName(tag),
-                                               Node.CDATA_SECTION_NODE)
-            result.append(temp)
-        self.data = result
-
-    def doc_xml_file(self, path):
-        """
-        Parses a specified file into a xml.dom.minidom document object, to be
-        used by `parse_data` method later on. This method here will store the
-        result in the private `__doc` property.
-
-        Arguments:
-
-            * path: the XML file path that will be parsed into a dom
-              document object.
-        """
-        if not os.path.exists(path):
-            raise exception.PathNotFoundException(path)
-
-        try:
-            self.__doc = parse(path)
-        except:
-            raise exception.XmlException(path)
-
-    def doc_xml_string(self, text):
-        """
-        Parses a specified string into a xml.dom.minidom document object, to be
-        used by `parse_data` method later on. This method here will store the
-        result in the private `__doc` property.
-
-        Arguments:
-
-            * text: the XML string value that will be parsed into a dom
-              document object.
-        """
-        try:
-            self.__doc = parseString(text)
-        except:
-            raise exception.XmlException(text)
+###############################################################################
+#
+# file:     xmlreader.py
+#
+# Purpose:  refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+A helper class used for screens that require XML handling. See
+additional information in the class itself.
+
+The helper class available here is:
+
+    * `XMLReaderHelperBase`
+
+"""
+
+#
+# Python built-in modules
+#
+import os
+from xml.dom.minidom import Node, parse, parseString
+
+from termsaver.termsaverlib import exception
+#
+# Internal modules
+#
+from termsaver.termsaverlib.screen.helper import ScreenHelperBase
+
+
+class XMLReaderHelperBase(ScreenHelperBase):
+    """
+    This helper class will handle basic XML parsing, not trying to solve all
+    mysteries of the universe here. What we are looking for are main nodes that
+    contain repetitive data, commonly found on a dataset, or RSS feed. More
+    complex handling is not treated at this point, but it might be implemented
+    if the need surfaces.
+
+    The basic instantiation of this class require you to inform 2 arguments:
+
+        * `base_node`: Defines the primary node where the data must be
+           retrieved from.
+
+        * `tags`: Defines which tags within the XML must be parsed to build a
+           list of dictionaries.
+
+    Those two arguments will give the hint about where is the data and which
+    piece of it you are looking for.
+
+    For actually getting the data, you will need to:
+
+        * prepare a raw data (file content, Internet data, etc) into a
+          XML object, named `__doc`; and
+        * parse the XML object into a more convenient list of dictionaries
+          that will be populated in `data` property.
+
+    To prepare the data, you have 2 options:
+
+        * `doc_xml_string`: a method that will create a dom xml document from
+          a text string (obviously it must be a XML)
+
+        * `doc_xml_file`: a method that will create a dom xml document from
+          a file content (obviously it must be a XML)
+
+    Once you have the XML properly prepared, and stored in `__doc`, you can
+    call the parsing method:
+
+        * `parse_data`: this will actually execute the action to extract the
+           information you are looking for based on the arguments passed
+           in the instantiation.
+
+    """
+
+    __doc = None
+    """
+    Holds the xml.dom.minidom document object
+    """
+
+    clean_dirt = []
+    """
+    Holds a list of strings that will be cleaned up from each result in the
+    XML data, when placing them into the `data` property. This can be pretty
+    handy to remove trailing spaces, new lines, or unwanted HTML tags from the
+    data.
+    """
+
+    base_node = None
+    """
+    Defines the primary node where the data must be retrieved from.
+    """
+
+    tags = []
+    """
+    Defines which tags within the XML must be parsed to build a
+    list of dictionaries.
+    """
+
+    data = None
+    """
+    Holds a list, created from properly parsing the dom document object in
+    `__doc`, as specified with `base_node` and `tags` filtering.
+    """
+
+    def __init__(self, base_node, tags):
+        """
+        Creates a new instance of this class.
+
+        Arguments:
+
+        * `base_node`: Defines the primary node where the data must be
+           retrieved from.
+
+        * `tags`: Defines which tags within the XML must be parsed to build a
+           list of dictionaries.
+        """
+        self.base_node = base_node
+        self.tags = tags
+
+    def parse_data(self):
+        """
+        Only call this once you have already created the dom document object,
+        by calling either `doc_xml_file` or `doc_xml_string` methods.
+
+        This will parse the document into a list, much simpler to deal with.
+        On the logic here is done, the list is available in the property `data`
+        """
+        def get_note_value(node, node_type):
+            result = ''
+            for node2 in node:
+                for node3 in node2.childNodes:
+                    if node3.nodeType == node_type:
+                        result += node3.data
+            # clean possible dirt
+            for t in self.clean_dirt:
+                # execute a loop here for dealing with multiple occurrences
+                # (such as multiple spaces)
+                while result.find(t) > -1:
+                    result = result.replace(t, "")
+            return result
+
+        if self.__doc is None:
+            raise Exception("""You must parse the raw data, by calling a \
+doc_xml_* method to populate the dom document object.""")
+
+        result = []
+        for node in self.__doc.getElementsByTagName(self.base_node):
+            temp = {}
+            for tag in self.tags:
+                temp[tag] = get_note_value(node.getElementsByTagName(tag),
+                                           Node.TEXT_NODE)
+                if not temp[tag]:
+                    temp[tag] = get_note_value(node.getElementsByTagName(tag),
+                                               Node.CDATA_SECTION_NODE)
+            result.append(temp)
+        self.data = result
+
+    def doc_xml_file(self, path):
+        """
+        Parses a specified file into a xml.dom.minidom document object, to be
+        used by `parse_data` method later on. This method here will store the
+        result in the private `__doc` property.
+
+        Arguments:
+
+            * path: the XML file path that will be parsed into a dom
+              document object.
+        """
+        if not os.path.exists(path):
+            raise exception.PathNotFoundException(path)
+
+        try:
+            self.__doc = parse(path)
+        except:
+            raise exception.XmlException(path)
+
+    def doc_xml_string(self, text):
+        """
+        Parses a specified string into a xml.dom.minidom document object, to be
+        used by `parse_data` method later on. This method here will store the
+        result in the private `__doc` property.
+
+        Arguments:
+
+            * text: the XML string value that will be parsed into a dom
+              document object.
+        """
+        try:
+            self.__doc = parseString(text)
+        except:
+            raise exception.XmlException(text)
```

### Comparing `termsaver-0.4/termsaverlib/exception.py` & `termsaver-0.6/termsaver/termsaverlib/exception.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,185 +1,188 @@
-###############################################################################
-#
-# file:     exceptions.py
-#
-# Purpose:  holds termsaver special exceptions
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-This module holds special exceptions triggered by termsaver (and handled
-internally as well, but with more human-readable treatment).
-
-The classes available here are:
-
-  * `TermSaverException`
-     A generic exception that implements read-only functionality for its
-     inheriting classes.
-
-  * `ScreenNotFoundException`
-     An exception that happens when termsaver is dealing with non existing
-     screens.
-
-  * `PathNotFoundException`
-     An exception that happens when termsaver is dealing with non existing
-     files.
-
-  * `UrlException`
-     An exception that happens when termsaver is dealing with URL connectvitiy
-     issues.
-
-"""
-
-
-class TermSaverException(Exception):
-    """
-    A base exception class providing additional read-only feature to its
-    inheriting classes. You must fill the `readonly` list to enable a property
-    as read-only.
-    """
-
-    readonly = []
-    """
-    Defines a list to place names of properties that should be read-only.
-    """
-
-    help_msg = ''
-    """
-    An extra string of information to help guide users on exception issues.
-    """
-
-    def __init__(self, *args, **kwargs):
-        """
-        Instantiate a new exception object.
-
-        You may use the extra property `help` when instantiating this.
-        """
-
-        Exception.__init__(self, *args)
-
-        # get the help argument dynamically from kwargs, if applicable
-        if "help" in kwargs:
-            self.help_msg = kwargs['help']
-
-            # mark this property as read-only
-            self.readonly.append("help")
-
-    def __setattr__(self, name, val):
-        """
-        Override of original to check for read-only properties, throwing
-        exception if tempered with.
-        """
-        if name not in self.readonly:
-            self.__dict__[name] = val
-        else:
-            raise Exception("%s.%s is read only!" % (self.__class__.__name__,
-                                                     name))
-
-
-class PathNotFoundException(TermSaverException):
-    """
-    Exception to handle special cases when a path required to run could not be
-    found in the file system.
-    """
-
-    path = ''
-    """
-    The name of the screen that could not be found by termsaver.
-    """
-
-    def __init__(self, path, *args, **kwargs):
-        """
-        Instantiates this exception class, with an additional parameter for the
-        name of the screen not found by termsaver. This value is accessible by
-        """
-        TermSaverException.__init__(self, *args, **kwargs)
-        self.path = path
-
-        # mark this property as read-only
-        self.readonly.append('path')
-
-
-class UrlException(TermSaverException):
-    """
-    Exception to handle special cases when connectivity to a specific URL was
-    not successful.
-    """
-
-    url = ''
-    """
-    The name of the screen that could not be found by termsaver.
-    """
-
-    def __init__(self, url, *args, **kwargs):
-        """
-        Instantiates this exception class, with an additional parameter for the
-        name of the screen not found by termsaver. This value is accessible by
-        """
-        TermSaverException.__init__(self, *args, **kwargs)
-        self.url = url
-
-        # mark this property as read-only
-        self.readonly.append('url')
-
-
-class InvalidOptionException(TermSaverException):
-    """
-    Exception to handle special cases when user uses comman line options
-    wrongfully.
-    """
-
-    option_name = ''
-    """
-    The name of the screen that could not be found by termsaver.
-    """
-
-    def __init__(self, option_name, *args, **kwargs):
-        """
-        Instantiates this exception class, with an additional parameter for the
-        name of the screen not found by termsaver. This value is accessible by
-        """
-        TermSaverException.__init__(self, *args, **kwargs)
-        self.option_name = option_name
-
-        # mark this property as read-only
-        self.readonly.append('option_name')
-
-
-class XmlException(TermSaverException):
-    """
-    Exception to handle XML issues.
-    """
-
-    name = ''
-    """
-    The name of the file path or URL that had issues with parsing
-    """
-
-    def __init__(self, name, *args, **kwargs):
-        """
-        Instantiates this exception class, with an additional parameter for the
-        name of the screen not found by termsaver. This value is accessible by
-        """
-        TermSaverException.__init__(self, *args, **kwargs)
-        self.name = name
-
-        # mark this property as read-only
-        self.readonly.append('name')
+###############################################################################
+#
+# file:     exceptions.py
+#
+# Purpose:  holds termsaver special exceptions
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+This module holds special exceptions triggered by termsaver (and handled
+internally as well, but with more human-readable treatment).
+
+The classes available here are:
+
+  * `TermSaverException`
+     A generic exception that implements read-only functionality for its
+     inheriting classes.
+
+  * `ScreenNotFoundException`
+     An exception that happens when termsaver is dealing with non existing
+     screens.
+
+  * `PathNotFoundException`
+     An exception that happens when termsaver is dealing with non existing
+     files.
+
+  * `UrlException`
+     An exception that happens when termsaver is dealing with URL connectvitiy
+     issues.
+
+"""
+
+
+class TermSaverException(Exception):
+    """
+    A base exception class providing additional read-only feature to its
+    inheriting classes. You must fill the `readonly` list to enable a property
+    as read-only.
+    """
+
+    readonly = []
+    """
+    Defines a list to place names of properties that should be read-only.
+    """
+
+    help_msg = ''
+    """
+    An extra string of information to help guide users on exception issues.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        Instantiate a new exception object.
+
+        You may use the extra property `help` when instantiating this.
+        """
+
+        Exception.__init__(self, *args)
+
+        # get the help argument dynamically from kwargs, if applicable
+        if "help" in kwargs:
+            self.help_msg = kwargs['help']
+
+            # mark this property as read-only
+            self.readonly.append("help")
+
+    def __setattr__(self, name, val):
+        """
+        Override of original to check for read-only properties, throwing
+        exception if tempered with.
+        """
+        if name not in self.readonly:
+            self.__dict__[name] = val
+        else:
+            raise Exception("%s.%s is read only!" % (self.__class__.__name__,
+                                                     name))
+
+
+class PathNotFoundException(TermSaverException):
+    """
+    Exception to handle special cases when a path required to run could not be
+    found in the file system.
+    """
+
+    path = ''
+    """
+    The name of the screen that could not be found by termsaver.
+    """
+
+    def __init__(self, path, *args, **kwargs):
+        """
+        Instantiates this exception class, with an additional parameter for the
+        name of the screen not found by termsaver. This value is accessible by
+        """
+        TermSaverException.__init__(self, *args, **kwargs)
+        if 'path' not in self.readonly:
+            self.path = path
+
+            # mark this property as read-only
+            self.readonly.append('path')
+
+
+class UrlException(TermSaverException):
+    """
+    Exception to handle special cases when connectivity to a specific URL was
+    not successful.
+    """
+
+    url = ''
+    """
+    The name of the screen that could not be found by termsaver.
+    """
+
+    def __init__(self, url, *args, **kwargs):
+        """
+        Instantiates this exception class, with an additional parameter for the
+        name of the screen not found by termsaver. This value is accessible by
+        """
+        TermSaverException.__init__(self, *args, **kwargs)
+        if 'url' not in self.readonly:
+            self.url = url
+
+            # mark this property as read-only
+            self.readonly.append('url')
+
+
+class InvalidOptionException(TermSaverException):
+    """
+    Exception to handle special cases when user uses comman line options
+    wrongfully.
+    """
+
+    option_name = ''
+    """
+    The name of the screen that could not be found by termsaver.
+    """
+
+    def __init__(self, option_name, *args, **kwargs):
+        """
+        Instantiates this exception class, with an additional parameter for the
+        name of the screen not found by termsaver. This value is accessible by
+        """
+        TermSaverException.__init__(self, *args, **kwargs)
+        if 'option_name' not in self.readonly:
+            self.option_name = option_name
+
+            # mark this property as read-only
+            self.readonly.append('option_name')
+
+
+class XmlException(TermSaverException):
+    """
+    Exception to handle XML issues.
+    """
+
+    name = ''
+    """
+    The name of the file path or URL that had issues with parsing
+    """
+
+    def __init__(self, name, *args, **kwargs):
+        """
+        Instantiates this exception class, with an additional parameter for the
+        name of the screen not found by termsaver. This value is accessible by
+        """
+        TermSaverException.__init__(self, *args, **kwargs)
+        self.name = name
+
+        # mark this property as read-only
+        self.readonly.append('name')
```

### Comparing `termsaver-0.4/termsaverlib/plugins/__init__.py` & `termsaver-0.6/termsaver/termsaverlib/plugins/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,131 @@
-###############################################################################
-#
-# file:     __init__.py
-#
-# Purpose:  refer to python doc for documentation details.
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-This module itself holds simple functions to better handle the screens
-available within any plugins installed. Available functions:
-
-    * `get_available_plugin_screens`: Gets the available screens in
-       sub-directories {plugin}/screen/ for dynamic instantiation.
-
-The modules available in this package are installed on-demand, so they are
-not documented here.
-
-How to create plugins
-=====================
-
-The main script termsaver will execute a dynamic search for all screens
-that inherit from the `ScreenBase` class. For plugins, however, screens are
-not placed in the same directory of the built-in screens, but instead into
-their own location.
-
-The directory structure of a plugin should be like:
-
-      plugins/
-         |
-         |---- __init__.py
-         |
-         |---- my_plugin/
-         |         |
-         |         |---- __init__.py
-         |         |
-         |         |---- screen
-         |         |       |
-         |         |       |---- __init__.py
-         |         |       |
-         |         |       |---- my_screen.py
-         |         |       |
-         |         |       |---- ...
-         |         |       |
-
-Additional rules before you begin:
-
-(1) Naming Conventions
-    The application name must be in the format: termsaver-{plugin-name}, and
-    the directory to be created inside the plugins will be {plugin-name}.
-
-    Python does not like dashes for module names, so be careful with names you
-    pick.
-
-(2) Screens
-    Each screen you design (inside the plugins/{plugin-name}/screen directory)
-    must inherit from the `ScreenBase` class, as this is the base for the
-    application to find the screen, and handle input/output accordingly.
-
-
-This sctructure is designed to immitate termsaver's main structure, so once you
-get familiar with it, it should be piece of cake to manage your own "space".
-
-"""
-
-#
-# Python built-in modules
-#
-import os
-import inspect
-
-#
-# Internal modules
-#
-from termsaverlib.screen import base
-
-
-def get_available_plugin_screens():
-    """
-    Gets the available screens in this package for dynamic instantiation.
-    """
-    ignore_list = ['__init__.py']
-    screens = []
-    for plugin in os.listdir(os.path.join(os.path.dirname(__file__))):
-        if (os.path.isdir(os.path.join(os.path.dirname(__file__), plugin))):
-            # we are inside the plugin directory, get screens available in
-            # screens directory
-            for module in os.listdir(os.path.join(os.path.dirname(__file__),
-                    plugin, "screen")):
-                if module in ignore_list or module[-3:] != '.py':
-                    continue
-                module_name = plugin + ".screen." + module[:-3]
-
-                m = __import__(module_name, globals(), locals(),
-                        [module_name.rsplit(".", 1)[-1]])
-
-                # loop module's classes in search for the ones inheriting
-                # Screenbase and ignore name (no need) with underscore variable
-                for name, obj in inspect.getmembers(m):
-                    if inspect.isclass(obj) and issubclass(obj,
-                            base.ScreenBase) and not name.endswith("Base"):
-                        screens.append(obj)
-    return screens
+###############################################################################
+#
+# file:     __init__.py
+#
+# Purpose:  refer to python doc for documentation details.
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+This module itself holds simple functions to better handle the screens
+available within any plugins installed. Available functions:
+
+    * `get_available_plugin_screens`: Gets the available screens in
+       sub-directories {plugin}/screen/ for dynamic instantiation.
+
+The modules available in this package are installed on-demand, so they are
+not documented here.
+
+How to create plugins
+=====================
+
+The main script termsaver will execute a dynamic search for all screens
+that inherit from the `ScreenBase` class. For plugins, however, screens are
+not placed in the same directory of the built-in screens, but instead into
+their own location.
+
+The directory structure of a plugin should be like:
+
+      plugins/
+         |
+         |---- __init__.py
+         |
+         |---- my_plugin/
+         |         |
+         |         |---- __init__.py
+         |         |
+         |         |---- screen
+         |         |       |
+         |         |       |---- __init__.py
+         |         |       |
+         |         |       |---- my_screen.py
+         |         |       |
+         |         |       |---- ...
+         |         |       |
+
+Additional rules before you begin:
+
+(1) Naming Conventions
+    The application name must be in the format: termsaver-{plugin-name}, and
+    the directory to be created inside the plugins will be {plugin-name}.
+
+    Python does not like dashes for module names, so be careful with names you
+    pick.
+
+(2) Screens
+    Each screen you design (inside the plugins/{plugin-name}/screen directory)
+    must inherit from the `ScreenBase` class, as this is the base for the
+    application to find the screen, and handle input/output accordingly.
+
+
+This structure is designed to immitate termsaver's main structure, so once you
+get familiar with it, it should be piece of cake to manage your own "space".
+
+"""
+
+import inspect
+#
+# Python built-in modules
+#
+import os
+import sys
+
+#
+# Internal modules
+#
+from termsaver.termsaverlib.screen import base
+
+
+def get_available_plugin_screens():
+    """
+    Gets the available screens in this package for dynamic instantiation.
+    """
+    ignore_list = ['__init__.py']
+    screens = []
+    for plugin in os.listdir(os.path.join(os.path.dirname(__file__))):
+        
+        if ("__pycache__" in plugin): continue
+
+        if (os.path.isdir(os.path.join(os.path.dirname(__file__), plugin))):
+            # we are inside the plugin directory, get screens available in
+            # screens directory
+
+            for module in os.listdir(os.path.join(os.path.dirname(__file__),
+                    plugin, "screen")):
+
+                if module in ignore_list or module[-3:] != '.py':
+                    continue
+
+                module_name = plugin + ".screen." + module[:-3]
+
+                if os.path.join(os.path.dirname(__file__)) not in sys.path:
+                    sys.path.append(os.path.join(os.path.dirname(__file__)))
+
+                m = __import__(module_name, globals(), locals(),
+                        [module_name.rsplit(".", 1)[-1]])
+
+                # loop module's classes in search for the ones inheriting
+                # Screenbase and ignore name (no need) with underscore variable
+                for name, obj in inspect.getmembers(m):
+                    if inspect.isclass(obj) and issubclass(obj,
+                            base.ScreenBase) and not name.endswith("Base"):
+                        screens.append(obj)
+    return screens
```

### Comparing `termsaver-0.4/termsaverlib/constants.py` & `termsaver-0.6/termsaver/termsaverlib/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,113 +1,114 @@
-###############################################################################
-#
-# file:     constants.py
-#
-# Purpose:  refer to module documentation for details
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-Holds constant values used throughout termsaver application.
-"""
-
-
-class PropertyClass:
-    """
-    A base class that defines a class as a holder for properties only, not to
-    be instantiated in any circumstances.
-    """
-
-    def __init__(self):
-        """
-        This class (and sub-classes) should not be instantiated.
-        """
-        raise NotImplementedError("This class cannot be instantiated!")
-
-
-class App(PropertyClass):
-    """
-    Holds application related properties used by termsaver screens.
-    Refer to each of the available properties for detailed documentation.
-    """
-
-    VERSION = "0.4"
-    """
-    Defines the version of termsaver application. This is accessed during
-    install process, and to any help and usage messages informed by it.
-
-    Refer to CHANGELOG file for a complete history about this project.
-    """
-
-    NAME = 'termsaver'
-    """
-    Defines the termsaver application, as it is executed from command-line.
-    """
-
-    TITLE = 'TermSaver'
-    """
-    Defines the termsaver application's official name as it should appear
-    in documentation.
-    """
-
-    DESCRIPTION = 'A simple text-based terminal screensaver'
-    """
-    Defines the main description of the termsaver application.
-    """
-
-    URL = 'http://termsaver.brunobraga.net'
-    """
-    Defines the termsaver official website address.
-    """
-
-    SOURCE_URL = 'http://github.com/brunobraga/termsaver'
-    """
-    Defines the termsaver official source-code control site, hosted on GitHub.
-    """
-
-    AUTHORS = [
-               'Bruno Braga <bruno.braga@gmail.com>',
-               'Shelby Jueden <shelbyjueden@gmail.com>',
-               'Alexander Riccio <alexander@riccio.com>',
-    ]
-    """
-    Defines a list of all authors contributing to the termsaver application.
-    """
-
-
-class Settings(PropertyClass):
-    """
-    Holds configuration settings used by termsaver application. Refer to each
-    of the available properties for detailed documentation.
-    """
-
-    CHAR_DELAY_SECONDS = 0.003
-    """
-    Defines basically the speed in which the text will be displayed, character
-    by character, giving a cool impression of an automated type writing machine
-    Default value is 0.003 seconds (3 milliseconds). It is advised to use
-    values between 0.01 and 0.001.
-    """
-
-    FETCH_INTERVAL_SECONDS = 3600
-    """
-    Defines the interval between each fetching of data over the Internet.
-    Default value is 1 hour.
-    """
+###############################################################################
+#
+# file:     constants.py
+#
+# Purpose:  refer to module documentation for details
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+Holds constant values used throughout termsaver application.
+"""
+
+
+class PropertyClass:
+    """
+    A base class that defines a class as a holder for properties only, not to
+    be instantiated in any circumstances.
+    """
+
+    def __init__(self):
+        """
+        This class (and sub-classes) should not be instantiated.
+        """
+        raise NotImplementedError("This class cannot be instantiated!")
+
+
+class App(PropertyClass):
+    """
+    Holds application related properties used by termsaver screens.
+    Refer to each of the available properties for detailed documentation.
+    """
+
+    VERSION = "0.6"
+    """
+    Defines the version of termsaver application. This is accessed during
+    install process, and to any help and usage messages informed by it.
+
+    Refer to CHANGELOG file for a complete history about this project.
+    """
+
+    NAME = 'termsaver'
+    """
+    Defines the termsaver application, as it is executed from command-line.
+    """
+
+    TITLE = 'TermSaver'
+    """
+    Defines the termsaver application's official name as it should appear
+    in documentation.
+    """
+
+    DESCRIPTION = 'A simple text-based terminal screensaver'
+    """
+    Defines the main description of the termsaver application.
+    """
+
+    URL = 'http://github.com/brunobraga/termsaver'
+    """
+    Defines the termsaver official website address.
+    """
+
+    SOURCE_URL = 'http://github.com/brunobraga/termsaver'
+    """
+    Defines the termsaver official source-code control site, hosted on GitHub.
+    """
+
+    AUTHORS = [
+               'Bruno Braga <bruno@brunobraga.net>',
+               'Shelby Jueden <shelbyjueden@gmail.com>',
+               'Alexander Riccio <alexander@riccio.com>',
+               'Eddie Dover <ed@eddiedover.dev>',
+    ]
+    """
+    Defines a list of all authors contributing to the termsaver application.
+    """
+
+
+class Settings(PropertyClass):
+    """
+    Holds configuration settings used by termsaver application. Refer to each
+    of the available properties for detailed documentation.
+    """
+
+    CHAR_DELAY_SECONDS = 0.003
+    """
+    Defines basically the speed in which the text will be displayed, character
+    by character, giving a cool impression of an automated type writing machine
+    Default value is 0.003 seconds (3 milliseconds). It is advised to use
+    values between 0.01 and 0.001.
+    """
+
+    FETCH_INTERVAL_SECONDS = 3600
+    """
+    Defines the interval between each fetching of data over the Internet.
+    Default value is 1 hour.
+    """
```

### Comparing `termsaver-0.4/termsaverlib/i18n.py` & `termsaver-0.6/termsaver/termsaverlib/i18n.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-###############################################################################
-#
-# file:     i18n.py
-#
-# Purpose:  refer to python doc for documentation details.
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-Handles all internationalization (i18n) functionality for termsaver application
-"""
-
-#
-# Python build-in modules
-#
-import gettext
-
-#
-# Internal modules
-#
-from termsaverlib import constants
-
-_ = None
-"""
-The unicode text dealer for i18n stuff, renamed as an underscore to keep same
-standards used by gettext.
-"""
-
-
-def set_app(application_name):
-    """
-    Defines the application name for the binding text files.
-    """
-    result = None
-
-    try:
-        gettext.textdomain(application_name)
-        result = gettext.gettext
-    except:
-        #
-        # If we can not handle i18n, just deal with text as it is
-        #
-        result = lambda x: x
-    
-        # For debugging
-        #raise
-
-    return result
-
-#
-# Call the default (termsaver app name)
-#    
-_ = set_app(constants.App.NAME)
-#
-# This should be overriden by plugins, as they can have their own i18n files
+###############################################################################
+#
+# file:     i18n.py
+#
+# Purpose:  refer to python doc for documentation details.
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+Handles all internationalization (i18n) functionality for termsaver application
+"""
+
+#
+# Python build-in modules
+#
+import gettext
+
+#
+# Internal modules
+#
+from termsaver.termsaverlib import constants
+
+_ = None
+"""
+The unicode text dealer for i18n stuff, renamed as an underscore to keep same
+standards used by gettext.
+"""
+
+
+def set_app(application_name):
+    """
+    Defines the application name for the binding text files.
+    """
+    result = None
+
+    try:
+        gettext.textdomain(application_name)
+        result = gettext.gettext
+    except:
+        #
+        # If we can not handle i18n, just deal with text as it is
+        #
+        result = lambda x: x
+    
+        # For debugging
+        #raise
+
+    return result
+
+#
+# Call the default (termsaver app name)
+#    
+_ = set_app(constants.App.NAME)
+#
+# This should be overriden by plugins, as they can have their own i18n files
 #
```

### Comparing `termsaver-0.4/termsaverlib/__init__.py` & `termsaver-0.6/termsaver/termsaverlib/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-###############################################################################
-#
-# file:     __init__.py
-#
-# Purpose:  refer to python doc for documentation details.
-#
-# Note:     This file is part of Termsaver application, and should not be used
-#           or executed separately.
-#
-###############################################################################
-#
-# Copyright 2012 Termsaver
-#
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
-#
-###############################################################################
-"""
-This module holds all stuff required for termsaver application to work properly
-
-The modules available in this package are:
-
-    * `common`: helper functions used by termsaver code
-
-    * `constants`: series of configuration constants used by termsaver code
-
-    * `exceptions`: various exceptions classes to handle termsaver errors
-
-    * `i18n`: handles internationalization for termsaver application
-
-This also contains the following sub-packages:
-
-    * `screen`: holds all screens accessible by termsaver application. Also
-      holds base and helper classes to ease the implementation of new screens.
-"""
+###############################################################################
+#
+# file:     __init__.py
+#
+# Purpose:  refer to python doc for documentation details.
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+"""
+This module holds all stuff required for termsaver application to work properly
+
+The modules available in this package are:
+
+    * `common`: helper functions used by termsaver code
+
+    * `constants`: series of configuration constants used by termsaver code
+
+    * `exceptions`: various exceptions classes to handle termsaver errors
+
+    * `i18n`: handles internationalization for termsaver application
+
+This also contains the following sub-packages:
+
+    * `screen`: holds all screens accessible by termsaver application. Also
+      holds base and helper classes to ease the implementation of new screens.
+"""
```

### Comparing `termsaver-0.4/README` & `termsaver-0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,319 +1,266 @@
-.. ############################################################################
-.. #
-.. # file:     README
-.. #
-.. # Purpose:  holds basic information about termsaver application, 
-.. #           in markdown format for GitHub.
-.. #
-.. # Note:     This file is part of Termsaver application, and should not be 
-.. #           used or executed separately.
-.. #
-.. ############################################################################
-.. #
-.. # Copyright 2012 Termsaver
-.. # 
-.. # Licensed under the Apache License, Version 2.0 (the "License"); you may
-.. # not use this file except in compliance with the License. You may obtain
-.. # a copy of the License at
-.. #
-.. #     http://www.apache.org/licenses/LICENSE-2.0
-.. #
-.. # Unless required by applicable law or agreed to in writing, software
-.. # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-.. # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-.. # License for the specific language governing permissions and limitations
-.. # under the License.
-.. #
-.. ############################################################################
-
-=========
-TermSaver
-=========
-
-*A simple text-based screensaver for terminal windows.*
-
-You may also want to visit our website: http://termsaver.brunobraga.net
-
-
-.. image:: https://github.com/brunobraga/termsaver/raw/master/extras/termsaver-main_medium.jpeg
-
-
-----------
-Background
-----------
-
-The motivation behind this project is basically pure boredom (laughs). 
-Seriously, it may look like nonsense to have a screensaver look-alike program
-running on a terminal window. Nonetheless, sometimes, we still want to see some
-kind of movement, or action on the screen... which invigorates one's state of
-mind and helps concentration back to the black screen (well, some people like 
-it white, meh!).
-
-If you are:
-
-  * looking for some extra display on your main terminal window, to keep the 
-    screen busy while you are up to something else; or
-  * looking for some distractions that may entertain you after too many hours
-    in front of the terminal; or
-  * with plenty of screen space (so long 80x25 default terminal window! long 
-    live 1920px...), and use many terminals on screen; or
-  * just wanting to pretend you are busy with something (this is terrible)
-
-then, TermSaver is the **right** application for you.
-
-
-------------
-Requirements
-------------
-
-  * Linux, or Mac (or Windows too, but you are on your own)
-  * Python 2.5+ (and < 3.x)
-
-
-
-------------
-Installation
-------------
-
-Apt (Advanced Packaging Tool)
------------------------------
-
-For Ubuntu (12.10+) distro, you can use:
-
-::
-
-        sudo apt-get install termsaver
-
-Pip (Pip Installs Packages, for Python Package Index)
------------------------------------------------------
-
-For those using others, and still want to do it the easy way, I recommend:
-
-::
-
-        sudo pip install termsaver
-
-
-From the Source
----------------
-
-1. Download the Source here_: 
-
-.. _here: http://pypi.python.org/pypi/termsaver/
-
-2. Unpack it
-
-::     
-
-        tar -zxvf termsaver-{version}.tar.gz
-
-3. Install it
-
-::
-
-        sudo python setup.py install 
-
-PPA (Advanced Packaging Tool)
------------------------------
-
-If you can't wait for Debian/Ubuntu releases, you can get the latest packages from:
-
-::
-
-
-        sudo add-apt-repository ppa:bruno-braga/termsaver
-        sudo apt-get update
-        sudo apt-get install termsaver
-
-
---------
-Features
---------
-
-The TermSaver is a very simple application, built with the idea to allow more 
-screensavers to be added to its core. Developers, please read the section below. 
-
-The current published screensavers are:
-
-Ascii Art Farts
----------------
-
-This is a screensaver that displays ascii art from asciiartfarts.com 
-RSS feed in an animation format. 
-
-
-Jokes For All
--------------
-
-This is a screensaver that displays recent jokes from http://jokes4all.net
-website, from its hourly updated RSS_ feed.
-
-.. _RSS : http://en.wikipedia.org/wiki/RSS
-
-Programmer
-----------
-
-This is a screensaver that displays source code from a specified path in
-visual animation.
-
-Quotes For All
---------------
-
-This is a screensaver that displays recent quotes from http://quotes4all.net
-website, from its hourly updated RSS_ feed.
-
-.. _RSS : http://en.wikipedia.org/wiki/RSS
-
-Random Text
------------
-
-This is a screensaver that displays a text (your name, or whatever) on a 
- randomized position of the screen, changing position every N seconds.
-
-Request for Change
-------------------
-
-This is a screensaver that fetches documents from RFC (Request for Comments)
-in visual animation, which are documents elaborated by the  Internet 
-Engineering Task Force, available at http://tools.ietf.org/rfc/. This 
-screensaver randomizes documents to display, from a list of latest valid
-documents. See more information about this in Wikipedia_.
-
-.. _Wikipedia : http://en.wikipedia.org/wiki/Request_for_Comments
-
-
-RSS Feeds
----------
-
-This is a screensaver that displays any 
-RSS_ feed you want to show in your terminal, with customizable settings 
-and format.
-
-.. _RSS : http://en.wikipedia.org/wiki/RSS
-
-URL Fetcher
------------
-
-This is a screensaver that displays content from a specified 
-URL_ directly on screen, in visual animation.
-
-.. _URL : http://en.wikipedia.org/wiki/Uniform_resource_locator
-
-Clock
------
-
-This is a screensaver that displays a digital clock using ascii letters.
-
-Matrix
-------
-
-This is a screensaver that displays falling (rising) Japanese characters
-simulating the screen from the movie The_Matrix_
-
-.. _The_Matrix : http://en.wikipedia.org/wiki/The_Matrix
-
-
-Sysmon
-------
-
-(For Linux/Mac systems only) Displays the CPU/Memory usage over time in a graphic
-alike screensaver.
-
-
-------
-
-**Disclaimer Note**: termsaver holds no responsibility for the contents offered 
-by third-parties, nor it has controls to filter them. Use it at your own risk.
-
-
-----------
-Developers
-----------
-
-A more detailed guideline for developers willing to jump in and create 
-screensavers for termsaver is here: https://github.com/brunobraga/termsaver/wiki/Developers
-
-
--------
-Roadmap
--------
-
-There is no current roadmap defined, besides improvement tickets created in
-Issues_ tab in GitHub.
-Refer also to http://github.com/brunobraga/termsaver/wiki/Brainstorming for
-some insights of stuff we are thinking about.
-
-.. _Issues : https://github.com/brunobraga/termsaver/issues
-
-----------
-Contribute
-----------
-
-Translation
------------
-
-The internationalization of this application follows same standards of most
-applications out there, by using *gettext* and MO/PO files.
-
-The translation is still being finished up, and when it is ready for 
-contributor calls, we will post detailed information about the procedure.
-
-
-Screensavers (plugin)
----------------------
-
-As of v0.2, full plugin support is available, find an example here:
-
-https://github.com/brunobraga/termsaver-figlet
-
-
-Submit a bug
-------------
-
-If you find any errors in this application, you are more than welcome to 
-participate. You can:
-
-* report the bug: https://github.com/brunobraga/termsaver/issues
-
-* Fork this project: https://github.com/brunobraga/termsaver/fork
-
-    
----------
-Uninstall
----------
-
-Using Apt (Advanced Packaging Tool)  or PPA (Personal Package Archive)
-----------------------------------------------------------------------
-
-::
-
-        sudo apt-get remove termsaver
-
-
-Using Pip (Pip Install Packages, for Python Package Index)
-----------------------------------------------------------
-
-::
-
-        sudo pip uninstall termsaver
-
-
-Manual Uninstall
-----------------
-
-Just remove manually the following files:
-
-::
-
-    # For Linux boxes
-    rm -rvf /usr/local/bin/termsaver 
-    rm -rvf /usr/local/lib/python2.7/dist-packages/termsaver* 
-    rm -rvf /usr/local/share/man/man1/termsaver.1 
-    find /usr/local/share/locale/ -name "termsaver.mo" -exec rm -rfv {} \; 
-
-If the actuall location differ from the above, it might be worth it to just
-run the find command and look for them yourself (should not be hard):
-
-::
-
-        find /usr/ -name "*termsaver*" 
+<!-- 
+###############################################################################
+#
+# file:     README.md
+#
+# Purpose:  holds basic information about termsaver application, 
+#           in markdown format for GitHub.
+#
+# Note:     This file is part of Termsaver application, and should not be used
+#           or executed separately.
+#
+###############################################################################
+#
+# Copyright 2012 Termsaver
+#
+# Licensed under the Apache License, Version 2.0 (the "License"); you may
+# not use this file except in compliance with the License. You may obtain
+# a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+# License for the specific language governing permissions and limitations
+# under the License.
+#
+###############################################################################
+-->
+
+TermSaver
+=========
+
+*A simple text-based screensaver for terminal windows.*
+
+![termsaver](https://github.com/brunobraga/termsaver/raw/master/extras/termsaver-main_medium.jpeg)
+
+
+Background
+----------
+
+The motivation behind this project is basically pure boredom (laughs). 
+Seriously, it may look like nonsense to have a screensaver look-alike program
+running on a terminal window. Nonetheless, sometimes, we still want to see some
+kind of movement, or action on the screen... which invigorates one's state of
+mind and helps concentration back to the black screen (well, some people like 
+it white, meh!).
+
+If you are:
+
+  * looking for some extra display on your main terminal window, to keep the 
+    screen busy while you are up to something else; or
+  * looking for some distractions that may entertain you after too many hours
+    in front of the terminal; or
+  * with plenty of screen space (so long 80x25 default terminal window! long 
+    live 1920px...), and use many terminals on screen; or
+  * just wanting to pretend you are busy with something (this is terrible)
+
+then, TermSaver is the **right** application for you.
+
+
+Requirements
+------------
+
+  * Linux, or Mac (or Windows too, but you are on your own)
+  * Python 3.x (Python 2.x was deprecated since 08-2020)
+
+
+Installation
+------------
+#### Pip (Pip Installs Packages, for Python Package Index)
+
+For those using others, and still want to do it the easy way, I recommend:
+
+        sudo pip install termsaver
+
+
+#### From the Source
+
+For the brave (laughs), you can compile/install from the source:
+
+1. Download the Source 
+[here](http://pypi.python.org/pypi/termsaver/) or [here](https://github.com/brunobraga/termsaver/)
+
+2. Unpack it
+     
+        tar -zxvf termsaver-{version}.tar.gz
+
+3. Build it
+        cd termsaver-{version}/
+        python -m build
+
+3. Install it
+        cd dist/
+        pip install termsaver-{version}-py3-none-any.whl
+
+
+Features
+--------
+
+The TermSaver is a very simple application, built with the idea to allow more 
+screensavers to be added to its core. Developers, please read the section below. 
+
+The current published screensavers are:
+
+
+#### Ascii Art Farts
+
+This is a screensaver that displays ascii art from asciiartfarts.com 
+RSS feed in an animation format. 
+
+
+#### Clock
+
+This is a screensaver that displays a digital clock using ascii letters.
+
+
+#### Img2Ascii
+
+This is a screensaver that displays images using ascii letters.
+
+
+#### Jokes For All
+
+This is a screensaver that displays recent jokes from <http://jokes4all.net>
+website, from its hourly updated [RSS](http://en.wikipedia.org/wiki/RSS) feed.
+
+
+#### Matrix
+
+This is a screensaver that displays falling (rising) Japanese characters
+simulating the screen from the movie 
+[The Matrix](http://en.wikipedia.org/wiki/The_Matrix).
+
+
+#### Programmer
+
+This is a screensaver that displays source code from a specified path in
+visual animation. If the [pygments](https://pygments.org/) package is installed, this screensaver
+will apply syntax highlighting based on the file type.
+
+#### Quotes For All
+
+This is a screensaver that displays recent quotes from <http://quotes4all.net>
+website, from its hourly updated [RSS](http://en.wikipedia.org/wiki/RSS) feed.
+
+
+#### Random Text
+
+This is a screensaver that displays a text (your name, or whatever) on a 
+ randomized position of the screen, changing position every N seconds.
+
+
+#### Request for Comments
+
+This is a screensaver that fetches documents from RFC (Request for Comments)
+in visual animation, which are documents elaborated by the  Internet 
+Engineering Task Force, available at <http://tools.ietf.org/rfc/>. This 
+screensaver randomizes documents to display, from a list of latest valid
+documents. See more information about this in 
+[Wikipedia](http://en.wikipedia.org/wiki/Request_for_Comments).
+
+
+#### RSS Feeds
+
+This is a screensaver that displays any 
+[RSS](http://en.wikipedia.org/wiki/RSS) feed you want to show in your
+terminal, with customizable settings and format.
+
+
+#### URL Fetcher
+
+This is a screensaver that displays content from a specified 
+[URL](http://en.wikipedia.org/wiki/Uniform_resource_locator) directly
+on screen, in visual animation.
+
+
+#### Star Wars Asciimation
+
+This is a screensaver that displays the Star Wars Asciimation from
+<http://asciimation.co.nz>.
+
+
+#### Sysmon
+
+(For Linux/Mac systems only) Displays the CPU/Memory usage over time in a graphic
+alike screensaver.
+
+#### WWTR.IN
+
+Shows weather information from [wttr.in](https://www.wttr.in/)
+
+ - - -
+
+**Disclaimer Note**: termsaver holds no responsibility for the contents offered 
+by third-parties, nor it has controls to filter them. Use it at your own risk.
+
+
+Developers
+----------
+
+A more detailed guideline for developers willing to jump in and create 
+screensavers for termsaver is here: <https://github.com/brunobraga/termsaver/wiki/Developers>
+
+
+Roadmap
+-------
+
+There is no current roadmap defined, besides improvement tickets created in
+[Issues](https://github.com/brunobraga/termsaver/issues) tab in GitHub.
+Refer also to <http://github.com/brunobraga/termsaver/wiki/Brainstorming> for
+some insights of stuff we are thinking about.
+
+Contribute
+----------
+
+### Translation
+
+The internationalization of this application follows same standards of most
+applications out there, by using *gettext* and MO/PO files.
+
+The translation is still being finished up, and when it is ready for 
+contributor calls, we will post detailed information about the procedure.
+
+
+### Screensavers (plugin)
+
+As of v0.2, full plugin support is available, find an example here:
+
+https://github.com/brunobraga/termsaver-figlet
+
+
+### Submit a bug
+
+If you find any errors in this application, you are more than welcome to 
+participate. You can:
+
+* report the bug: <https://github.com/brunobraga/termsaver/issues>
+
+* Fork this project: <https://github.com/brunobraga/termsaver/fork>
+    
+Uninstall
+----------
+
+### Using Pip (Pip Install Packages, for Python Package Index)
+
+        sudo pip uninstall termsaver
+
+
+### Manual Uninstall
+
+Just remove manually the following files:
+
+        # For Linux boxes
+        rm -rvf /usr/local/bin/termsaver
+        
+        # change your python version/location here
+        rm -rvf /usr/local/lib/python3.x/dist-packages/termsaver* 
+        
+        rm -rvf /usr/local/share/man/man1/termsaver.1 
+        find /usr/local/share/locale/ -name "termsaver.mo" -exec rm -rfv {} \; 
+
+If the actuall location differ from the above, it might be worth it to just
+run the find command and look for them yourself (should not be hard):
+
+        find /usr/ -name "*termsaver*"
```

