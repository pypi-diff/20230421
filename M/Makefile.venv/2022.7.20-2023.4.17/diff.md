# Comparing `tmp/Makefile.venv-2022.7.20.tar.gz` & `tmp/Makefile.venv-2023.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Public\.prj\Makefile.venv\pypi\dist\tmpfbdl2mdh\Makefile.venv-2022.7.20.tar", last modified: Thu Jul 21 09:27:54 2022, max compression
+gzip compressed data, was "C:\Users\Public\...\projects\Makefile.venv\pypi\dist\.tmp-fgrukuex\Makefile.venv-2023.4.17.tar", last modified: Fri Apr 21 14:19:21 2023, max compression
```

## Comparing `Makefile.venv-2022.7.20.tar` & `Makefile.venv-2023.4.17.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-07-21 09:27:54.000000 Makefile.venv-2022.7.20/
--rw-rw-rw-   0        0        0      683 2022-07-20 11:57:19.000000 Makefile.venv-2022.7.20/Makefile
--rw-rw-rw-   0        0        0    11287 2022-07-21 09:27:54.000000 Makefile.venv-2022.7.20/PKG-INFO
--rw-rw-rw-   0        0        0      544 2022-07-20 11:57:19.000000 Makefile.venv-2022.7.20/README.md
--rw-rw-rw-   0        0        0      179 2022-07-20 11:57:19.000000 Makefile.venv-2022.7.20/pyproject.toml
--rw-rw-rw-   0        0        0      816 2022-07-21 09:27:54.000000 Makefile.venv-2022.7.20/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-21 09:27:54.000000 Makefile.venv-2022.7.20/src/
-drwxrwxrwx   0        0        0        0 2022-07-21 09:27:54.000000 Makefile.venv-2022.7.20/src/Makefile.venv.egg-info/
--rw-rw-rw-   0        0        0    11287 2022-07-21 09:27:53.000000 Makefile.venv-2022.7.20/src/Makefile.venv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2022-07-21 09:27:54.000000 Makefile.venv-2022.7.20/src/Makefile.venv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-21 09:27:53.000000 Makefile.venv-2022.7.20/src/Makefile.venv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-07-21 09:27:53.000000 Makefile.venv-2022.7.20/src/Makefile.venv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-07-21 09:27:53.000000 Makefile.venv-2022.7.20/src/Makefile.venv.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2022-07-21 09:27:53.000000 Makefile.venv-2022.7.20/src/Makefile.venv.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-21 09:27:54.000000 Makefile.venv-2022.7.20/src/Makefile_venv/
--rw-rw-rw-   0        0        0    11558 2022-07-21 09:27:37.000000 Makefile.venv-2022.7.20/src/Makefile_venv/LICENSE
--rw-rw-rw-   0        0        0     7159 2022-07-21 09:27:37.000000 Makefile.venv-2022.7.20/src/Makefile_venv/Makefile.venv
--rw-rw-rw-   0        0        0    10762 2022-07-21 09:27:38.000000 Makefile.venv-2022.7.20/src/Makefile_venv/README.md
--rw-rw-rw-   0        0        0      328 2022-07-20 11:57:19.000000 Makefile.venv-2022.7.20/src/Makefile_venv/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-21 09:27:54.000000 Makefile.venv-2022.7.20/tests/
--rw-rw-rw-   0        0        0      589 2022-07-20 11:57:19.000000 Makefile.venv-2022.7.20/tests/test_installable.py
--rw-rw-rw-   0        0        0      137 2022-07-20 11:57:19.000000 Makefile.venv-2022.7.20/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-21 14:19:21.000000 Makefile.venv-2023.4.17/
+-rw-rw-rw-   0        0        0      643 2023-04-10 07:12:28.000000 Makefile.venv-2023.4.17/Makefile
+-rw-rw-rw-   0        0        0    11425 2023-04-21 14:19:21.000000 Makefile.venv-2023.4.17/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-04-10 07:12:28.000000 Makefile.venv-2023.4.17/README.md
+-rw-rw-rw-   0        0        0      168 2023-04-10 07:12:28.000000 Makefile.venv-2023.4.17/pyproject.toml
+-rw-rw-rw-   0        0        0      816 2023-04-21 14:19:21.000000 Makefile.venv-2023.4.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 14:19:21.000000 Makefile.venv-2023.4.17/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:19:21.000000 Makefile.venv-2023.4.17/src/Makefile.venv.egg-info/
+-rw-rw-rw-   0        0        0    11425 2023-04-21 14:19:20.000000 Makefile.venv-2023.4.17/src/Makefile.venv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-04-21 14:19:21.000000 Makefile.venv-2023.4.17/src/Makefile.venv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:19:20.000000 Makefile.venv-2023.4.17/src/Makefile.venv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-21 14:19:20.000000 Makefile.venv-2023.4.17/src/Makefile.venv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 14:19:03.000000 Makefile.venv-2023.4.17/src/Makefile.venv.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-21 14:19:20.000000 Makefile.venv-2023.4.17/src/Makefile.venv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:19:21.000000 Makefile.venv-2023.4.17/src/Makefile_venv/
+-rw-rw-rw-   0        0        0    11357 2023-04-21 14:19:08.000000 Makefile.venv-2023.4.17/src/Makefile_venv/LICENSE
+-rw-rw-rw-   0        0        0     7378 2023-04-21 14:19:08.000000 Makefile.venv-2023.4.17/src/Makefile_venv/Makefile.venv
+-rw-rw-rw-   0        0        0    10580 2023-04-21 14:19:08.000000 Makefile.venv-2023.4.17/src/Makefile_venv/README.md
+-rw-rw-rw-   0        0        0      312 2023-04-10 07:12:28.000000 Makefile.venv-2023.4.17/src/Makefile_venv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:19:21.000000 Makefile.venv-2023.4.17/tests/
+-rw-rw-rw-   0        0        0      569 2023-04-10 07:12:28.000000 Makefile.venv-2023.4.17/tests/test_installable.py
+-rw-rw-rw-   0        0        0      126 2023-04-10 07:12:28.000000 Makefile.venv-2023.4.17/tox.ini
```

### Comparing `Makefile.venv-2022.7.20/PKG-INFO` & `Makefile.venv-2023.4.17/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Makefile.venv
-Version: 2022.7.20
+Version: 2023.4.17
 Summary: Seamlessly manage Python virtual environment with a Makefile
 Home-page: https://github.com/sio/Makefile.venv
 License: Apache-2.0
 Keywords: makefile,virtualenv,env
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -50,16 +50,16 @@
 > to shell](https://0x46.net/thoughts/2019/04/27/piping-curl-to-shell/)!
 
 ```make
 include Makefile.venv
 Makefile.venv:
 	curl \
 		-o Makefile.fetched \
-		-L "https://github.com/sio/Makefile.venv/raw/v2022.07.20/Makefile.venv"
-	echo "147b164f0cbbbe4a2740dcca6c9adb6e9d8d15b895be3998697aa6a821a277d8 *Makefile.fetched" \
+		-L "https://github.com/sio/Makefile.venv/raw/v2023.04.17/Makefile.venv"
+	echo "fb48375ed1fd19e41e0cdcf51a4a0c6d1010dfe03b672ffc4c26a91878544f82 *Makefile.fetched" \
 		| sha256sum --check - \
 		&& mv Makefile.fetched Makefile.venv
 ```
 
 > Notes:
 >
 > * *curl* and/or *sha256sum* may not be available by default depending on what
@@ -192,19 +192,20 @@
 Non-existent files are treated as hard dependencies, recipes for creating such
 files must be provided by the main Makefile (sample usage: [pip-compile]).
 Providing empty value (`REQUIREMENTS_TXT=`) turns off processing of
 requirements.txt even when the file exists.
 
 [pip-compile]: docs/howto-pip-compile.md
 
-##### SETUP_PY
+##### SETUP_PY, SETUP_CFG, PYPROJECT_TOML, VENV_LOCAL_PACKAGE
 
-Space separated list of paths to setup․py files. Corresponding packages will
-be installed into venv in [editable mode] along with all their dependencies.
-*Default: setup․py*
+Space separated list of paths to files that contain build instructions
+for local Python packages. Corresponding packages will be installed
+into venv in [editable mode] along with all their dependencies.
+*Default: setup.py setup.cfg pyproject.toml (whichever present)*
 
 Non-existent and empty values are treated in the same way as for REQUIREMENTS_TXT.
 
 [editable mode]: https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs
 
 ##### WORKDIR
 
@@ -314,15 +315,15 @@
 log.
 
 [issues]: https://github.com/sio/Makefile.venv/issues
 
 
 ## License and copyright
 
-Copyright 2019-2022 Vitaly Potyarkin
+Copyright 2019-2023 Vitaly Potyarkin
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Makefile.venv Version: 2022.7.20 Summary:
+Metadata-Version: 2.1 Name: Makefile.venv Version: 2023.4.17 Summary:
 Seamlessly manage Python virtual environment with a Makefile Home-page: https:/
 /github.com/sio/Makefile.venv License: Apache-2.0 Keywords:
 makefile,virtualenv,env Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Description-
 Content-Type: text/markdown License-File: src/Makefile_venv/LICENSE #
 Seamlessly manage Python virtual environment with a Makefile *Makefile.venv*
@@ -19,17 +19,17 @@
 some configuration. ## Installation ### Recommended method Copy
 [*Makefile.venv*](Makefile.venv) to your project directory and add include
 statement to the bottom of your `Makefile`: ```make include Makefile.venv ```
 ### Alternative method Alternatively, you can add installation actions as the
 Makefile recipe: > **Note the checksum step!** Do not skip it, it would be as
 bad as [piping curl > to shell](https://0x46.net/thoughts/2019/04/27/piping-
 curl-to-shell/)! ```make include Makefile.venv Makefile.venv: curl \ -
-o Makefile.fetched \ -L "https://github.com/sio/Makefile.venv/raw/v2022.07.20/
+o Makefile.fetched \ -L "https://github.com/sio/Makefile.venv/raw/v2023.04.17/
 Makefile.venv" echo
-"147b164f0cbbbe4a2740dcca6c9adb6e9d8d15b895be3998697aa6a821a277d8
+"fb48375ed1fd19e41e0cdcf51a4a0c6d1010dfe03b672ffc4c26a91878544f82
 *Makefile.fetched" \ | sha256sum --check - \ && mv Makefile.fetched
 Makefile.venv ``` > Notes: > > * *curl* and/or *sha256sum* may not be available
 by default depending on what > OS and configuration is used > * To install
 *sha256sum* on macOS use `brew install coreutils` > * You can use Perl's
 *shasum -a 256* instead of *sha256sum*, as described > [here](https://
 github.com/sio/Makefile.venv/issues/11). ### Another alternative method If you
 want to use *Makefile.venv* in multiple projects and to be able to conveniently
@@ -80,63 +80,65 @@
 initially to create the virtual environment. *Default: python3* #####
 REQUIREMENTS_TXT Space separated list of paths to requirements.txt files. Paths
 are resolved relative to current working directory. *Default: requirements.txt*
 Non-existent files are treated as hard dependencies, recipes for creating such
 files must be provided by the main Makefile (sample usage: [pip-compile]).
 Providing empty value (`REQUIREMENTS_TXT=`) turns off processing of
 requirements.txt even when the file exists. [pip-compile]: docs/howto-pip-
-compile.md ##### SETUP_PY Space separated list of paths to setupâ¤py files.
-Corresponding packages will be installed into venv in [editable mode] along
-with all their dependencies. *Default: setupâ¤py* Non-existent and empty
-values are treated in the same way as for REQUIREMENTS_TXT. [editable mode]:
-https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs ##### WORKDIR
-Parent directory for the virtual environment. *Default: current working
-directory* ##### VENVDIR Python virtual environment directory. *Default: $
-(WORKDIR)/.venv* ##### PIP_* Variables named starting with `PIP_` are not
-processed by *Makefile.venv* in any way and are passed to underlying pip calls
-as is. See [pip documentation](https://pip.pypa.io/en/stable/user_guide/
-#environment-variables) for more information. Use these variables to customize
-pip invocation, for example to provide custom package index url: ```
-PIP_EXTRA_INDEX_URL="https://your.index/url" ``` ## Samples Makefile: ```make
-.PHONY: test test: venv $(VENV)/python -m unittest include Makefile.venv ```
-Larger sample from a real project can be seen [here](https://github.com/sio/
-issyours/blob/master/Makefile). Also see [an introductory blog post](https://
-potyarkin.ml/posts/2019/manage-python-virtual-environment-from-your-makefile/
-) from project author. Command line: ``` $ make test ...Skipped: creating and
-updating virtual environment... ... -------------------------------------------
---------------------------- Ran 3 tests in 0.000s OK ``` ``` $ make show-venv
-Python 3.5.4 (v3.5.4:3f56838, Aug 8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)]
-pip 19.2.3 from c:\users\99e7~1\appdata\local\temp\.venv\lib\site-packages\pip
-(python 3.5) venv: C:\Users\99E7~1\AppData\Local\Temp\.venv ``` ``` $ make
-python C:/Users/99E7~1/AppData/Local/Temp/.venv/Scripts/python Python 3.5.4
-(v3.5.4:3f56838, Aug 8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)] on win32
-Type "help", "copyright", "credits" or "license" for more information. >>> _
-``` ## Compatibility *Makefile.venv* was written for GNU Make and may not work
-with other make implementations. Please be aware that GNU Make [can not
-correctly handle][spaces] whitespace characters in file paths. Such filepaths
-therefore are considered unsupported by *Makefile.venv* [spaces]: https://
-stackoverflow.com/questions/9838384/can-gnu-make-handle-filenames-with-spaces
-*Makefile.venv* is being [continuously tested][tests] on Linux, Windows and
-macOS. Any inconsistency encountered when running on Windows should be
-considered a bug and should be reported via [issues]. ## Support and
-contributing If you need help with using this Makefile or including it into
-your project, please create **[an issue][issues]**. Issues are also the primary
-venue for reporting bugs and posting feature requests. General discussion
-related to this project is also acceptable and very welcome! In case you wish
-to contribute code or documentation, feel free to open **[a pull request]
-(https://github.com/sio/Makefile.venv/pulls)**. That would certainly make my
-day! I'm open to dialog and I promise to behave responsibly and treat all
-contributors with respect. Please try to do the same, and treat others the way
-you want to be treated. If for some reason you'd rather not use the issue
-tracker, contacting me via email is OK too. Please use a descriptive subject
-line to enhance visibility of your message. Also please keep in mind that
-public discussion channels are preferable because that way many other people
-may benefit from reading past conversations. My email is visible under the
-GitHub profile and in the commit log. [issues]: https://github.com/sio/
-Makefile.venv/issues ## License and copyright Copyright 2019-2022 Vitaly
-Potyarkin Licensed under the Apache License, Version 2.0 (the "License"); you
-may not use this file except in compliance with the License. You may obtain a
-copy of the License at http://www.apache.org/licenses/LICENSE-2.0 Unless
-required by applicable law or agreed to in writing, software distributed under
-the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-CONDITIONS OF ANY KIND, either express or implied. See the License for the
-specific language governing permissions and limitations under the License.
+compile.md ##### SETUP_PY, SETUP_CFG, PYPROJECT_TOML, VENV_LOCAL_PACKAGE Space
+separated list of paths to files that contain build instructions for local
+Python packages. Corresponding packages will be installed into venv in
+[editable mode] along with all their dependencies. *Default: setup.py setup.cfg
+pyproject.toml (whichever present)* Non-existent and empty values are treated
+in the same way as for REQUIREMENTS_TXT. [editable mode]: https://pip.pypa.io/
+en/stable/cli/pip_install/#editable-installs ##### WORKDIR Parent directory for
+the virtual environment. *Default: current working directory* ##### VENVDIR
+Python virtual environment directory. *Default: $(WORKDIR)/.venv* ##### PIP_*
+Variables named starting with `PIP_` are not processed by *Makefile.venv* in
+any way and are passed to underlying pip calls as is. See [pip documentation]
+(https://pip.pypa.io/en/stable/user_guide/#environment-variables) for more
+information. Use these variables to customize pip invocation, for example to
+provide custom package index url: ``` PIP_EXTRA_INDEX_URL="https://your.index/
+url" ``` ## Samples Makefile: ```make .PHONY: test test: venv $(VENV)/python -
+m unittest include Makefile.venv ``` Larger sample from a real project can be
+seen [here](https://github.com/sio/issyours/blob/master/Makefile). Also see [an
+introductory blog post](https://potyarkin.ml/posts/2019/manage-python-virtual-
+environment-from-your-makefile/) from project author. Command line: ``` $ make
+test ...Skipped: creating and updating virtual environment... ... -------------
+--------------------------------------------------------- Ran 3 tests in 0.000s
+OK ``` ``` $ make show-venv Python 3.5.4 (v3.5.4:3f56838, Aug 8 2017, 02:07:06)
+[MSC v.1900 32 bit (Intel)] pip 19.2.3 from c:
+\users\99e7~1\appdata\local\temp\.venv\lib\site-packages\pip (python 3.5) venv:
+C:\Users\99E7~1\AppData\Local\Temp\.venv ``` ``` $ make python C:/Users/99E7~1/
+AppData/Local/Temp/.venv/Scripts/python Python 3.5.4 (v3.5.4:3f56838, Aug 8
+2017, 02:07:06) [MSC v.1900 32 bit (Intel)] on win32 Type "help", "copyright",
+"credits" or "license" for more information. >>> _ ``` ## Compatibility
+*Makefile.venv* was written for GNU Make and may not work with other make
+implementations. Please be aware that GNU Make [can not correctly handle]
+[spaces] whitespace characters in file paths. Such filepaths therefore are
+considered unsupported by *Makefile.venv* [spaces]: https://stackoverflow.com/
+questions/9838384/can-gnu-make-handle-filenames-with-spaces *Makefile.venv* is
+being [continuously tested][tests] on Linux, Windows and macOS. Any
+inconsistency encountered when running on Windows should be considered a bug
+and should be reported via [issues]. ## Support and contributing If you need
+help with using this Makefile or including it into your project, please create
+**[an issue][issues]**. Issues are also the primary venue for reporting bugs
+and posting feature requests. General discussion related to this project is
+also acceptable and very welcome! In case you wish to contribute code or
+documentation, feel free to open **[a pull request](https://github.com/sio/
+Makefile.venv/pulls)**. That would certainly make my day! I'm open to dialog
+and I promise to behave responsibly and treat all contributors with respect.
+Please try to do the same, and treat others the way you want to be treated. If
+for some reason you'd rather not use the issue tracker, contacting me via email
+is OK too. Please use a descriptive subject line to enhance visibility of your
+message. Also please keep in mind that public discussion channels are
+preferable because that way many other people may benefit from reading past
+conversations. My email is visible under the GitHub profile and in the commit
+log. [issues]: https://github.com/sio/Makefile.venv/issues ## License and
+copyright Copyright 2019-2023 Vitaly Potyarkin Licensed under the Apache
+License, Version 2.0 (the "License"); you may not use this file except in
+compliance with the License. You may obtain a copy of the License at http://
+www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
+to in writing, software distributed under the License is distributed on an "AS
+IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+implied. See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `Makefile.venv-2022.7.20/README.md` & `Makefile.venv-2023.4.17/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Packaging Makefile.venv for PyPI
-
-This directory contains helper code and configuration files used to build a
-Python package for *Makefile.venv* and to upload that package to PyPI.
-
-It is assumed that *Makefile.venv* itself is in a working state when working
-on packaging, so we depend on it in multiple places here.
-
-This is also the reason why packaging tests are stored separately from the
-rest of test suite: we can not depend on *Makefile.venv* in the main test
-suite, but it's too useful to forego when doing auxiliary work.
+# Packaging Makefile.venv for PyPI
+
+This directory contains helper code and configuration files used to build a
+Python package for *Makefile.venv* and to upload that package to PyPI.
+
+It is assumed that *Makefile.venv* itself is in a working state when working
+on packaging, so we depend on it in multiple places here.
+
+This is also the reason why packaging tests are stored separately from the
+rest of test suite: we can not depend on *Makefile.venv* in the main test
+suite, but it's too useful to forego when doing auxiliary work.
```

### Comparing `Makefile.venv-2022.7.20/setup.cfg` & `Makefile.venv-2023.4.17/setup.cfg`

 * *Files identical despite different names*

### Comparing `Makefile.venv-2022.7.20/src/Makefile.venv.egg-info/PKG-INFO` & `Makefile.venv-2023.4.17/src/Makefile.venv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Makefile.venv
-Version: 2022.7.20
+Version: 2023.4.17
 Summary: Seamlessly manage Python virtual environment with a Makefile
 Home-page: https://github.com/sio/Makefile.venv
 License: Apache-2.0
 Keywords: makefile,virtualenv,env
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -50,16 +50,16 @@
 > to shell](https://0x46.net/thoughts/2019/04/27/piping-curl-to-shell/)!
 
 ```make
 include Makefile.venv
 Makefile.venv:
 	curl \
 		-o Makefile.fetched \
-		-L "https://github.com/sio/Makefile.venv/raw/v2022.07.20/Makefile.venv"
-	echo "147b164f0cbbbe4a2740dcca6c9adb6e9d8d15b895be3998697aa6a821a277d8 *Makefile.fetched" \
+		-L "https://github.com/sio/Makefile.venv/raw/v2023.04.17/Makefile.venv"
+	echo "fb48375ed1fd19e41e0cdcf51a4a0c6d1010dfe03b672ffc4c26a91878544f82 *Makefile.fetched" \
 		| sha256sum --check - \
 		&& mv Makefile.fetched Makefile.venv
 ```
 
 > Notes:
 >
 > * *curl* and/or *sha256sum* may not be available by default depending on what
@@ -192,19 +192,20 @@
 Non-existent files are treated as hard dependencies, recipes for creating such
 files must be provided by the main Makefile (sample usage: [pip-compile]).
 Providing empty value (`REQUIREMENTS_TXT=`) turns off processing of
 requirements.txt even when the file exists.
 
 [pip-compile]: docs/howto-pip-compile.md
 
-##### SETUP_PY
+##### SETUP_PY, SETUP_CFG, PYPROJECT_TOML, VENV_LOCAL_PACKAGE
 
-Space separated list of paths to setup․py files. Corresponding packages will
-be installed into venv in [editable mode] along with all their dependencies.
-*Default: setup․py*
+Space separated list of paths to files that contain build instructions
+for local Python packages. Corresponding packages will be installed
+into venv in [editable mode] along with all their dependencies.
+*Default: setup.py setup.cfg pyproject.toml (whichever present)*
 
 Non-existent and empty values are treated in the same way as for REQUIREMENTS_TXT.
 
 [editable mode]: https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs
 
 ##### WORKDIR
 
@@ -314,15 +315,15 @@
 log.
 
 [issues]: https://github.com/sio/Makefile.venv/issues
 
 
 ## License and copyright
 
-Copyright 2019-2022 Vitaly Potyarkin
+Copyright 2019-2023 Vitaly Potyarkin
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Makefile.venv Version: 2022.7.20 Summary:
+Metadata-Version: 2.1 Name: Makefile.venv Version: 2023.4.17 Summary:
 Seamlessly manage Python virtual environment with a Makefile Home-page: https:/
 /github.com/sio/Makefile.venv License: Apache-2.0 Keywords:
 makefile,virtualenv,env Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Description-
 Content-Type: text/markdown License-File: src/Makefile_venv/LICENSE #
 Seamlessly manage Python virtual environment with a Makefile *Makefile.venv*
@@ -19,17 +19,17 @@
 some configuration. ## Installation ### Recommended method Copy
 [*Makefile.venv*](Makefile.venv) to your project directory and add include
 statement to the bottom of your `Makefile`: ```make include Makefile.venv ```
 ### Alternative method Alternatively, you can add installation actions as the
 Makefile recipe: > **Note the checksum step!** Do not skip it, it would be as
 bad as [piping curl > to shell](https://0x46.net/thoughts/2019/04/27/piping-
 curl-to-shell/)! ```make include Makefile.venv Makefile.venv: curl \ -
-o Makefile.fetched \ -L "https://github.com/sio/Makefile.venv/raw/v2022.07.20/
+o Makefile.fetched \ -L "https://github.com/sio/Makefile.venv/raw/v2023.04.17/
 Makefile.venv" echo
-"147b164f0cbbbe4a2740dcca6c9adb6e9d8d15b895be3998697aa6a821a277d8
+"fb48375ed1fd19e41e0cdcf51a4a0c6d1010dfe03b672ffc4c26a91878544f82
 *Makefile.fetched" \ | sha256sum --check - \ && mv Makefile.fetched
 Makefile.venv ``` > Notes: > > * *curl* and/or *sha256sum* may not be available
 by default depending on what > OS and configuration is used > * To install
 *sha256sum* on macOS use `brew install coreutils` > * You can use Perl's
 *shasum -a 256* instead of *sha256sum*, as described > [here](https://
 github.com/sio/Makefile.venv/issues/11). ### Another alternative method If you
 want to use *Makefile.venv* in multiple projects and to be able to conveniently
@@ -80,63 +80,65 @@
 initially to create the virtual environment. *Default: python3* #####
 REQUIREMENTS_TXT Space separated list of paths to requirements.txt files. Paths
 are resolved relative to current working directory. *Default: requirements.txt*
 Non-existent files are treated as hard dependencies, recipes for creating such
 files must be provided by the main Makefile (sample usage: [pip-compile]).
 Providing empty value (`REQUIREMENTS_TXT=`) turns off processing of
 requirements.txt even when the file exists. [pip-compile]: docs/howto-pip-
-compile.md ##### SETUP_PY Space separated list of paths to setupâ¤py files.
-Corresponding packages will be installed into venv in [editable mode] along
-with all their dependencies. *Default: setupâ¤py* Non-existent and empty
-values are treated in the same way as for REQUIREMENTS_TXT. [editable mode]:
-https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs ##### WORKDIR
-Parent directory for the virtual environment. *Default: current working
-directory* ##### VENVDIR Python virtual environment directory. *Default: $
-(WORKDIR)/.venv* ##### PIP_* Variables named starting with `PIP_` are not
-processed by *Makefile.venv* in any way and are passed to underlying pip calls
-as is. See [pip documentation](https://pip.pypa.io/en/stable/user_guide/
-#environment-variables) for more information. Use these variables to customize
-pip invocation, for example to provide custom package index url: ```
-PIP_EXTRA_INDEX_URL="https://your.index/url" ``` ## Samples Makefile: ```make
-.PHONY: test test: venv $(VENV)/python -m unittest include Makefile.venv ```
-Larger sample from a real project can be seen [here](https://github.com/sio/
-issyours/blob/master/Makefile). Also see [an introductory blog post](https://
-potyarkin.ml/posts/2019/manage-python-virtual-environment-from-your-makefile/
-) from project author. Command line: ``` $ make test ...Skipped: creating and
-updating virtual environment... ... -------------------------------------------
---------------------------- Ran 3 tests in 0.000s OK ``` ``` $ make show-venv
-Python 3.5.4 (v3.5.4:3f56838, Aug 8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)]
-pip 19.2.3 from c:\users\99e7~1\appdata\local\temp\.venv\lib\site-packages\pip
-(python 3.5) venv: C:\Users\99E7~1\AppData\Local\Temp\.venv ``` ``` $ make
-python C:/Users/99E7~1/AppData/Local/Temp/.venv/Scripts/python Python 3.5.4
-(v3.5.4:3f56838, Aug 8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)] on win32
-Type "help", "copyright", "credits" or "license" for more information. >>> _
-``` ## Compatibility *Makefile.venv* was written for GNU Make and may not work
-with other make implementations. Please be aware that GNU Make [can not
-correctly handle][spaces] whitespace characters in file paths. Such filepaths
-therefore are considered unsupported by *Makefile.venv* [spaces]: https://
-stackoverflow.com/questions/9838384/can-gnu-make-handle-filenames-with-spaces
-*Makefile.venv* is being [continuously tested][tests] on Linux, Windows and
-macOS. Any inconsistency encountered when running on Windows should be
-considered a bug and should be reported via [issues]. ## Support and
-contributing If you need help with using this Makefile or including it into
-your project, please create **[an issue][issues]**. Issues are also the primary
-venue for reporting bugs and posting feature requests. General discussion
-related to this project is also acceptable and very welcome! In case you wish
-to contribute code or documentation, feel free to open **[a pull request]
-(https://github.com/sio/Makefile.venv/pulls)**. That would certainly make my
-day! I'm open to dialog and I promise to behave responsibly and treat all
-contributors with respect. Please try to do the same, and treat others the way
-you want to be treated. If for some reason you'd rather not use the issue
-tracker, contacting me via email is OK too. Please use a descriptive subject
-line to enhance visibility of your message. Also please keep in mind that
-public discussion channels are preferable because that way many other people
-may benefit from reading past conversations. My email is visible under the
-GitHub profile and in the commit log. [issues]: https://github.com/sio/
-Makefile.venv/issues ## License and copyright Copyright 2019-2022 Vitaly
-Potyarkin Licensed under the Apache License, Version 2.0 (the "License"); you
-may not use this file except in compliance with the License. You may obtain a
-copy of the License at http://www.apache.org/licenses/LICENSE-2.0 Unless
-required by applicable law or agreed to in writing, software distributed under
-the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-CONDITIONS OF ANY KIND, either express or implied. See the License for the
-specific language governing permissions and limitations under the License.
+compile.md ##### SETUP_PY, SETUP_CFG, PYPROJECT_TOML, VENV_LOCAL_PACKAGE Space
+separated list of paths to files that contain build instructions for local
+Python packages. Corresponding packages will be installed into venv in
+[editable mode] along with all their dependencies. *Default: setup.py setup.cfg
+pyproject.toml (whichever present)* Non-existent and empty values are treated
+in the same way as for REQUIREMENTS_TXT. [editable mode]: https://pip.pypa.io/
+en/stable/cli/pip_install/#editable-installs ##### WORKDIR Parent directory for
+the virtual environment. *Default: current working directory* ##### VENVDIR
+Python virtual environment directory. *Default: $(WORKDIR)/.venv* ##### PIP_*
+Variables named starting with `PIP_` are not processed by *Makefile.venv* in
+any way and are passed to underlying pip calls as is. See [pip documentation]
+(https://pip.pypa.io/en/stable/user_guide/#environment-variables) for more
+information. Use these variables to customize pip invocation, for example to
+provide custom package index url: ``` PIP_EXTRA_INDEX_URL="https://your.index/
+url" ``` ## Samples Makefile: ```make .PHONY: test test: venv $(VENV)/python -
+m unittest include Makefile.venv ``` Larger sample from a real project can be
+seen [here](https://github.com/sio/issyours/blob/master/Makefile). Also see [an
+introductory blog post](https://potyarkin.ml/posts/2019/manage-python-virtual-
+environment-from-your-makefile/) from project author. Command line: ``` $ make
+test ...Skipped: creating and updating virtual environment... ... -------------
+--------------------------------------------------------- Ran 3 tests in 0.000s
+OK ``` ``` $ make show-venv Python 3.5.4 (v3.5.4:3f56838, Aug 8 2017, 02:07:06)
+[MSC v.1900 32 bit (Intel)] pip 19.2.3 from c:
+\users\99e7~1\appdata\local\temp\.venv\lib\site-packages\pip (python 3.5) venv:
+C:\Users\99E7~1\AppData\Local\Temp\.venv ``` ``` $ make python C:/Users/99E7~1/
+AppData/Local/Temp/.venv/Scripts/python Python 3.5.4 (v3.5.4:3f56838, Aug 8
+2017, 02:07:06) [MSC v.1900 32 bit (Intel)] on win32 Type "help", "copyright",
+"credits" or "license" for more information. >>> _ ``` ## Compatibility
+*Makefile.venv* was written for GNU Make and may not work with other make
+implementations. Please be aware that GNU Make [can not correctly handle]
+[spaces] whitespace characters in file paths. Such filepaths therefore are
+considered unsupported by *Makefile.venv* [spaces]: https://stackoverflow.com/
+questions/9838384/can-gnu-make-handle-filenames-with-spaces *Makefile.venv* is
+being [continuously tested][tests] on Linux, Windows and macOS. Any
+inconsistency encountered when running on Windows should be considered a bug
+and should be reported via [issues]. ## Support and contributing If you need
+help with using this Makefile or including it into your project, please create
+**[an issue][issues]**. Issues are also the primary venue for reporting bugs
+and posting feature requests. General discussion related to this project is
+also acceptable and very welcome! In case you wish to contribute code or
+documentation, feel free to open **[a pull request](https://github.com/sio/
+Makefile.venv/pulls)**. That would certainly make my day! I'm open to dialog
+and I promise to behave responsibly and treat all contributors with respect.
+Please try to do the same, and treat others the way you want to be treated. If
+for some reason you'd rather not use the issue tracker, contacting me via email
+is OK too. Please use a descriptive subject line to enhance visibility of your
+message. Also please keep in mind that public discussion channels are
+preferable because that way many other people may benefit from reading past
+conversations. My email is visible under the GitHub profile and in the commit
+log. [issues]: https://github.com/sio/Makefile.venv/issues ## License and
+copyright Copyright 2019-2023 Vitaly Potyarkin Licensed under the Apache
+License, Version 2.0 (the "License"); you may not use this file except in
+compliance with the License. You may obtain a copy of the License at http://
+www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
+to in writing, software distributed under the License is distributed on an "AS
+IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+implied. See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `Makefile.venv-2022.7.20/src/Makefile_venv/LICENSE` & `Makefile.venv-2023.4.17/src/Makefile_venv/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright {yyyy} {name of copyright owner}
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "{}"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright {yyyy} {name of copyright owner}
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `Makefile.venv-2022.7.20/src/Makefile_venv/Makefile.venv` & `Makefile.venv-2023.4.17/src/Makefile_venv/Makefile.venv`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # SEAMLESSLY MANAGE PYTHON VIRTUAL ENVIRONMENT WITH A MAKEFILE
 #
-# https://github.com/sio/Makefile.venv             v2022.07.20
+# https://github.com/sio/Makefile.venv             v2023.04.17
 #
 #
 # Insert `include Makefile.venv` at the bottom of your Makefile to enable these
 # rules.
 #
 # When writing your Makefile use '$(VENV)/python' to refer to the Python
 # interpreter within virtual environment and '$(VENV)/executablename' for any
@@ -50,33 +50,33 @@
 #       Paths are resolved relative to current working directory.
 #       Default: requirements.txt
 #
 #       Non-existent files are treated as hard dependencies,
 #       recipes for creating such files must be provided by the main Makefile.
 #       Providing empty value (REQUIREMENTS_TXT=) turns off processing of
 #       requirements.txt even when the file exists.
-#   SETUP_PY
-#       Space separated list of paths to setup.py files.
-#       Corresponding packages will be installed into venv in editable mode
-#       along with all their dependencies
-#       Default: setup.py
+#   SETUP_PY, SETUP_CFG, PYPROJECT_TOML, VENV_LOCAL_PACKAGE
+#       Space separated list of paths to files that contain build instructions
+#       for local Python packages. Corresponding packages will be installed
+#       into venv in editable mode along with all their dependencies.
+#       Default: setup.py setup.cfg pyproject.toml (whichever present)
 #
 #       Non-existent and empty values are treated in the same way as for REQUIREMENTS_TXT.
 #   WORKDIR
 #       Parent directory for the virtual environment.
 #       Default: current working directory.
 #   VENVDIR
 #       Python virtual environment directory.
 #       Default: $(WORKDIR)/.venv
 #
 # This Makefile was written for GNU Make and may not work with other make
 # implementations.
 #
 #
-# Copyright (c) 2019-2020 Vitaly Potyarkin
+# Copyright (c) 2019-2023 Vitaly Potyarkin
 #
 # Licensed under the Apache License, Version 2.0
 #    <http://www.apache.org/licenses/LICENSE-2.0>
 #
 
 
 #
@@ -84,14 +84,16 @@
 #
 
 WORKDIR?=.
 VENVDIR?=$(WORKDIR)/.venv
 REQUIREMENTS_TXT?=$(wildcard requirements.txt)  # Multiple paths are supported (space separated)
 SETUP_PY?=$(wildcard setup.py)                  # Multiple paths are supported (space separated)
 SETUP_CFG?=$(foreach s,$(SETUP_PY),$(wildcard $(patsubst %setup.py,%setup.cfg,$(s))))
+PYPROJECT_TOML?=$(wildcard pyproject.toml)
+VENV_LOCAL_PACKAGE?=$(SETUP_PY) $(SETUP_CFG) $(PYPROJECT_TOML)
 MARKER=.initialized-with-Makefile.venv
 
 
 #
 # Python interpreter detection
 #
 
@@ -198,46 +200,42 @@
 debug-venv:
 	@echo "PATH (Shell)=$$PATH"
 	@$(MAKE) --version
 	$(info PATH (GNU Make)="$(PATH)")
 	$(info SHELL="$(SHELL)")
 	$(info PY="$(PY)")
 	$(info REQUIREMENTS_TXT="$(REQUIREMENTS_TXT)")
-	$(info SETUP_PY="$(SETUP_PY)")
-	$(info SETUP_CFG="$(SETUP_CFG)")
+	$(info VENV_LOCAL_PACKAGE="$(VENV_LOCAL_PACKAGE)")
 	$(info VENVDIR="$(VENVDIR)")
 	$(info VENVDEPENDS="$(VENVDEPENDS)")
 	$(info WORKDIR="$(WORKDIR)")
 
 
 #
 # Dependencies
 #
 
 ifneq ($(strip $(REQUIREMENTS_TXT)),)
 VENVDEPENDS+=$(REQUIREMENTS_TXT)
 endif
 
-ifneq ($(strip $(SETUP_PY)),)
-VENVDEPENDS+=$(SETUP_PY)
-endif
-ifneq ($(strip $(SETUP_CFG)),)
-VENVDEPENDS+=$(SETUP_CFG)
+ifneq ($(strip $(VENV_LOCAL_PACKAGE)),)
+VENVDEPENDS+=$(VENV_LOCAL_PACKAGE)
 endif
 
 $(VENV):
 	$(PY) -m venv $(VENVDIR)
 	$(VENV)/python -m pip install --upgrade pip setuptools wheel
 
 $(VENV)/$(MARKER): $(VENVDEPENDS) | $(VENV)
 ifneq ($(strip $(REQUIREMENTS_TXT)),)
 	$(VENV)/pip install $(foreach path,$(REQUIREMENTS_TXT),-r $(path))
 endif
-ifneq ($(strip $(SETUP_PY)),)
-	$(VENV)/pip install $(foreach path,$(SETUP_PY),-e $(dir $(path)))
+ifneq ($(strip $(VENV_LOCAL_PACKAGE)),)
+	$(VENV)/pip install $(foreach path,$(sort $(VENV_LOCAL_PACKAGE)),-e $(dir $(path)))
 endif
 	$(call touch,$(VENV)/$(MARKER))
 
 
 #
 # Interactive shells
 #
```

### Comparing `Makefile.venv-2022.7.20/src/Makefile_venv/README.md` & `Makefile.venv-2023.4.17/src/Makefile_venv/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,319 +1,320 @@
-# Seamlessly manage Python virtual environment with a Makefile
-
-*Makefile.venv* takes care of creating, updating and invoking Python virtual
-environment that you can use in your Makefiles. It will allow you to reduce
-venv related routines to almost zero!
-
-[![test status][badge]][tests]
-
-[badge]: https://github.com/sio/Makefile.venv/workflows/Run%20automated%20tests/badge.svg
-[tests]: https://github.com/sio/Makefile.venv/actions?query=branch%3Amaster+
-
-*Makefile.venv* aims to be an one-stop solution for Python virtual environment
-management, regardless of the format used to define the venv: requirements.txt
-and setup․py are supported out of the box because they have become de-facto
-standards, but if anything else will take their place - Makefile.venv will
-support that too. [Pip-compile], pipenv and poetry are compatible but require
-some configuration.
-
-
-## Installation
-
-### Recommended method
-
-Copy [*Makefile.venv*](Makefile.venv) to your project directory and add
-include statement to the bottom of your `Makefile`:
-
-```make
-include Makefile.venv
-```
-
-### Alternative method
-
-Alternatively, you can add installation actions as the Makefile recipe:
-
-> **Note the checksum step!** Do not skip it, it would be as bad as [piping curl
-> to shell](https://0x46.net/thoughts/2019/04/27/piping-curl-to-shell/)!
-
-```make
-include Makefile.venv
-Makefile.venv:
-	curl \
-		-o Makefile.fetched \
-		-L "https://github.com/sio/Makefile.venv/raw/v2022.07.20/Makefile.venv"
-	echo "147b164f0cbbbe4a2740dcca6c9adb6e9d8d15b895be3998697aa6a821a277d8 *Makefile.fetched" \
-		| sha256sum --check - \
-		&& mv Makefile.fetched Makefile.venv
-```
-
-> Notes:
->
-> * *curl* and/or *sha256sum* may not be available by default depending on what
->   OS and configuration is used
-> * To install *sha256sum* on macOS use `brew install coreutils`
-> * You can use Perl's *shasum -a 256* instead of *sha256sum*, as described
->   [here](https://github.com/sio/Makefile.venv/issues/11).
-
-### Another alternative method
-
-If you want to use *Makefile.venv* in multiple projects and to be able to
-conveniently manage *Makefile.venv* version from one place you might find this
-[pip package] useful:
-
-- Install globally: `pip install Makefile.venv` or
-- Install for current user: `pip install --user Makefile.venv`
-
-This package will install *Makefile.venv* into your `site-packages/` and will
-add a command-line entrypoint which prints the full path to *Makefile.venv*.
-Include it it in your makefiles like this:
-
-```make
-include $(shell Makefile.venv)
-```
-
-[pip package]: https://pypi.org/project/Makefile.venv/
-
-
-## Usage
-
-When writing your Makefile use `$(VENV)/python` to refer to the Python
-interpreter within virtual environment and `$(VENV)/executablename` for any
-other executable in venv.
-
-*Makefile.venv* is not meant to be used as a standalone tool, think of it more
-like a library that enables extra functionality.
-
-
-## Demo screencast
-
-<a href="https://asciinema.org/a/279646" target="_blank">
-<img src="https://asciinema.org/a/279646.svg" title="Demo screencast"/>
-</a>
-
-
-## Targets
-
-*Makefile.venv* provides the following targets. Some are meant to be executed
-directly via `make $target`, some are meant to be dependencies for other
-targets written by you.
-
-##### venv
-
-Use this as a dependency for any target that requires virtual environment to
-be created and configured.
-
-*venv* is a .PHONY target and rules that depend on it will be executed every
-time make is run. This behavior is sensible as default because most Python
-projects use Makefiles for running development chores, not for artifact
-building. In cases where that is not desirable use [order-only prerequisite]
-syntax:
-
-```make
-artifacts.tar.gz: | venv
-	...
-```
-
-[order-only prerequisite]: https://www.gnu.org/software/make/manual/html_node/Prerequisite-Types.html
-
-##### python, ipython
-
-Execute these targets to launch interactive Python shell within virtual
-environment. Ipython is not installed by default when creating the virtual
-environment but will be installed automatically when called for the first
-time.
-
-##### shell, bash, zsh
-
-Execute these targets to launch interactive command line shell. `shell` target
-launches the default shell Makefile executes its rules in (usually /bin/sh).
-`bash` and `zsh` can be used to refer to the specific desired shell (if it's
-installed).
-
-##### show-venv
-
-Execute this target to show versions of Python and pip, and the path to the
-virtual environment. Use this for debugging purposes.
-
-##### clean-venv
-
-Execute this target to remove virtual environment. You can add this as a
-dependency to the `clean` target in your main Makefile.
-
-##### $(VENV)/executablename
-
-Use this target as a dependency for tasks that need `executablename` to be
-installed if `executablename` is not listed as project's dependency neither in
-`requirements.txt` nor in `setup.py`. Only packages with names matching the
-name of the corresponding executable are supported.
-
-This can be a lightweight mechanism for development dependencies tracking.
-E.g. for one-off tools that are not required in every developer's
-environment, therefore are not included in formal dependency lists.
-
-**Note:** Rules using such dependency MUST be defined below
-`include` directive to make use of correct $(VENV) value.
-
-Example (see `ipython` target for another example):
-
-```Makefile
-codestyle: $(VENV)/pyflakes  # `venv` dependency is assumed and may be omitted
-	$(VENV)/pyflakes .
-```
-
-## Variables
-
-*Makefile.venv* can be configured via following variables:
-
-##### PY
-
-Command name for system Python interpreter. It is used only initially to
-create the virtual environment. *Default: python3*
-
-##### REQUIREMENTS_TXT
-
-Space separated list of paths to requirements.txt files.
-Paths are resolved relative to current working directory.
-*Default: requirements.txt*
-
-Non-existent files are treated as hard dependencies, recipes for creating such
-files must be provided by the main Makefile (sample usage: [pip-compile]).
-Providing empty value (`REQUIREMENTS_TXT=`) turns off processing of
-requirements.txt even when the file exists.
-
-[pip-compile]: docs/howto-pip-compile.md
-
-##### SETUP_PY
-
-Space separated list of paths to setup․py files. Corresponding packages will
-be installed into venv in [editable mode] along with all their dependencies.
-*Default: setup․py*
-
-Non-existent and empty values are treated in the same way as for REQUIREMENTS_TXT.
-
-[editable mode]: https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs
-
-##### WORKDIR
-
-Parent directory for the virtual environment. *Default: current working
-directory*
-
-##### VENVDIR
-
-Python virtual environment directory. *Default: $(WORKDIR)/.venv*
-
-##### PIP_*
-
-Variables named starting with `PIP_` are not processed by *Makefile.venv* in
-any way and are passed to underlying pip calls as is. See [pip
-documentation](https://pip.pypa.io/en/stable/user_guide/#environment-variables)
-for more information.
-
-Use these variables to customize pip invocation, for example to provide custom
-package index url:
-
-```
-PIP_EXTRA_INDEX_URL="https://your.index/url"
-```
-
-
-## Samples
-
-Makefile:
-
-```make
-.PHONY: test
-test: venv
-	$(VENV)/python -m unittest
-
-include Makefile.venv
-```
-
-Larger sample from a real project can be seen
-[here](https://github.com/sio/issyours/blob/master/Makefile).
-Also see [an introductory blog
-post](https://potyarkin.ml/posts/2019/manage-python-virtual-environment-from-your-makefile/)
-from project author.
-
-Command line:
-
-```
-$ make test
-
-...Skipped: creating and updating virtual environment...
-
-...
-----------------------------------------------------------------------
-Ran 3 tests in 0.000s
-
-OK
-```
-```
-$ make show-venv
-Python 3.5.4 (v3.5.4:3f56838, Aug  8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)]
-pip 19.2.3 from c:\users\99e7~1\appdata\local\temp\.venv\lib\site-packages\pip (python 3.5)
-venv: C:\Users\99E7~1\AppData\Local\Temp\.venv
-```
-```
-$ make python
-C:/Users/99E7~1/AppData/Local/Temp/.venv/Scripts/python
-Python 3.5.4 (v3.5.4:3f56838, Aug  8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)] on win32
-Type "help", "copyright", "credits" or "license" for more information.
->>> _
-```
-
-
-## Compatibility
-
-*Makefile.venv* was written for GNU Make and may not work with other make
-implementations. Please be aware that GNU Make [can not correctly handle][spaces]
-whitespace characters in file paths. Such filepaths therefore are
-considered unsupported by *Makefile.venv*
-
-[spaces]: https://stackoverflow.com/questions/9838384/can-gnu-make-handle-filenames-with-spaces
-
-*Makefile.venv* is being [continuously tested][tests] on Linux, Windows and macOS. Any
-inconsistency encountered when running on Windows should be considered a bug
-and should be reported via [issues].
-
-
-## Support and contributing
-
-If you need help with using this Makefile or including it into your project,
-please create **[an issue][issues]**.
-Issues are also the primary venue for reporting bugs and posting feature
-requests. General discussion related to this project is also acceptable and
-very welcome!
-
-In case you wish to contribute code or documentation, feel free to open
-**[a pull request](https://github.com/sio/Makefile.venv/pulls)**. That would
-certainly make my day!
-
-I'm open to dialog and I promise to behave responsibly and treat all
-contributors with respect. Please try to do the same, and treat others the way
-you want to be treated.
-
-If for some reason you'd rather not use the issue tracker, contacting me via
-email is OK too. Please use a descriptive subject line to enhance visibility
-of your message. Also please keep in mind that public discussion channels are
-preferable because that way many other people may benefit from reading past
-conversations. My email is visible under the GitHub profile and in the commit
-log.
-
-[issues]: https://github.com/sio/Makefile.venv/issues
-
-
-## License and copyright
-
-Copyright 2019-2022 Vitaly Potyarkin
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
+# Seamlessly manage Python virtual environment with a Makefile
+
+*Makefile.venv* takes care of creating, updating and invoking Python virtual
+environment that you can use in your Makefiles. It will allow you to reduce
+venv related routines to almost zero!
+
+[![test status][badge]][tests]
+
+[badge]: https://github.com/sio/Makefile.venv/workflows/Run%20automated%20tests/badge.svg
+[tests]: https://github.com/sio/Makefile.venv/actions?query=branch%3Amaster+
+
+*Makefile.venv* aims to be an one-stop solution for Python virtual environment
+management, regardless of the format used to define the venv: requirements.txt
+and setup․py are supported out of the box because they have become de-facto
+standards, but if anything else will take their place - Makefile.venv will
+support that too. [Pip-compile], pipenv and poetry are compatible but require
+some configuration.
+
+
+## Installation
+
+### Recommended method
+
+Copy [*Makefile.venv*](Makefile.venv) to your project directory and add
+include statement to the bottom of your `Makefile`:
+
+```make
+include Makefile.venv
+```
+
+### Alternative method
+
+Alternatively, you can add installation actions as the Makefile recipe:
+
+> **Note the checksum step!** Do not skip it, it would be as bad as [piping curl
+> to shell](https://0x46.net/thoughts/2019/04/27/piping-curl-to-shell/)!
+
+```make
+include Makefile.venv
+Makefile.venv:
+	curl \
+		-o Makefile.fetched \
+		-L "https://github.com/sio/Makefile.venv/raw/v2023.04.17/Makefile.venv"
+	echo "fb48375ed1fd19e41e0cdcf51a4a0c6d1010dfe03b672ffc4c26a91878544f82 *Makefile.fetched" \
+		| sha256sum --check - \
+		&& mv Makefile.fetched Makefile.venv
+```
+
+> Notes:
+>
+> * *curl* and/or *sha256sum* may not be available by default depending on what
+>   OS and configuration is used
+> * To install *sha256sum* on macOS use `brew install coreutils`
+> * You can use Perl's *shasum -a 256* instead of *sha256sum*, as described
+>   [here](https://github.com/sio/Makefile.venv/issues/11).
+
+### Another alternative method
+
+If you want to use *Makefile.venv* in multiple projects and to be able to
+conveniently manage *Makefile.venv* version from one place you might find this
+[pip package] useful:
+
+- Install globally: `pip install Makefile.venv` or
+- Install for current user: `pip install --user Makefile.venv`
+
+This package will install *Makefile.venv* into your `site-packages/` and will
+add a command-line entrypoint which prints the full path to *Makefile.venv*.
+Include it it in your makefiles like this:
+
+```make
+include $(shell Makefile.venv)
+```
+
+[pip package]: https://pypi.org/project/Makefile.venv/
+
+
+## Usage
+
+When writing your Makefile use `$(VENV)/python` to refer to the Python
+interpreter within virtual environment and `$(VENV)/executablename` for any
+other executable in venv.
+
+*Makefile.venv* is not meant to be used as a standalone tool, think of it more
+like a library that enables extra functionality.
+
+
+## Demo screencast
+
+<a href="https://asciinema.org/a/279646" target="_blank">
+<img src="https://asciinema.org/a/279646.svg" title="Demo screencast"/>
+</a>
+
+
+## Targets
+
+*Makefile.venv* provides the following targets. Some are meant to be executed
+directly via `make $target`, some are meant to be dependencies for other
+targets written by you.
+
+##### venv
+
+Use this as a dependency for any target that requires virtual environment to
+be created and configured.
+
+*venv* is a .PHONY target and rules that depend on it will be executed every
+time make is run. This behavior is sensible as default because most Python
+projects use Makefiles for running development chores, not for artifact
+building. In cases where that is not desirable use [order-only prerequisite]
+syntax:
+
+```make
+artifacts.tar.gz: | venv
+	...
+```
+
+[order-only prerequisite]: https://www.gnu.org/software/make/manual/html_node/Prerequisite-Types.html
+
+##### python, ipython
+
+Execute these targets to launch interactive Python shell within virtual
+environment. Ipython is not installed by default when creating the virtual
+environment but will be installed automatically when called for the first
+time.
+
+##### shell, bash, zsh
+
+Execute these targets to launch interactive command line shell. `shell` target
+launches the default shell Makefile executes its rules in (usually /bin/sh).
+`bash` and `zsh` can be used to refer to the specific desired shell (if it's
+installed).
+
+##### show-venv
+
+Execute this target to show versions of Python and pip, and the path to the
+virtual environment. Use this for debugging purposes.
+
+##### clean-venv
+
+Execute this target to remove virtual environment. You can add this as a
+dependency to the `clean` target in your main Makefile.
+
+##### $(VENV)/executablename
+
+Use this target as a dependency for tasks that need `executablename` to be
+installed if `executablename` is not listed as project's dependency neither in
+`requirements.txt` nor in `setup.py`. Only packages with names matching the
+name of the corresponding executable are supported.
+
+This can be a lightweight mechanism for development dependencies tracking.
+E.g. for one-off tools that are not required in every developer's
+environment, therefore are not included in formal dependency lists.
+
+**Note:** Rules using such dependency MUST be defined below
+`include` directive to make use of correct $(VENV) value.
+
+Example (see `ipython` target for another example):
+
+```Makefile
+codestyle: $(VENV)/pyflakes  # `venv` dependency is assumed and may be omitted
+	$(VENV)/pyflakes .
+```
+
+## Variables
+
+*Makefile.venv* can be configured via following variables:
+
+##### PY
+
+Command name for system Python interpreter. It is used only initially to
+create the virtual environment. *Default: python3*
+
+##### REQUIREMENTS_TXT
+
+Space separated list of paths to requirements.txt files.
+Paths are resolved relative to current working directory.
+*Default: requirements.txt*
+
+Non-existent files are treated as hard dependencies, recipes for creating such
+files must be provided by the main Makefile (sample usage: [pip-compile]).
+Providing empty value (`REQUIREMENTS_TXT=`) turns off processing of
+requirements.txt even when the file exists.
+
+[pip-compile]: docs/howto-pip-compile.md
+
+##### SETUP_PY, SETUP_CFG, PYPROJECT_TOML, VENV_LOCAL_PACKAGE
+
+Space separated list of paths to files that contain build instructions
+for local Python packages. Corresponding packages will be installed
+into venv in [editable mode] along with all their dependencies.
+*Default: setup.py setup.cfg pyproject.toml (whichever present)*
+
+Non-existent and empty values are treated in the same way as for REQUIREMENTS_TXT.
+
+[editable mode]: https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs
+
+##### WORKDIR
+
+Parent directory for the virtual environment. *Default: current working
+directory*
+
+##### VENVDIR
+
+Python virtual environment directory. *Default: $(WORKDIR)/.venv*
+
+##### PIP_*
+
+Variables named starting with `PIP_` are not processed by *Makefile.venv* in
+any way and are passed to underlying pip calls as is. See [pip
+documentation](https://pip.pypa.io/en/stable/user_guide/#environment-variables)
+for more information.
+
+Use these variables to customize pip invocation, for example to provide custom
+package index url:
+
+```
+PIP_EXTRA_INDEX_URL="https://your.index/url"
+```
+
+
+## Samples
+
+Makefile:
+
+```make
+.PHONY: test
+test: venv
+	$(VENV)/python -m unittest
+
+include Makefile.venv
+```
+
+Larger sample from a real project can be seen
+[here](https://github.com/sio/issyours/blob/master/Makefile).
+Also see [an introductory blog
+post](https://potyarkin.ml/posts/2019/manage-python-virtual-environment-from-your-makefile/)
+from project author.
+
+Command line:
+
+```
+$ make test
+
+...Skipped: creating and updating virtual environment...
+
+...
+----------------------------------------------------------------------
+Ran 3 tests in 0.000s
+
+OK
+```
+```
+$ make show-venv
+Python 3.5.4 (v3.5.4:3f56838, Aug  8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)]
+pip 19.2.3 from c:\users\99e7~1\appdata\local\temp\.venv\lib\site-packages\pip (python 3.5)
+venv: C:\Users\99E7~1\AppData\Local\Temp\.venv
+```
+```
+$ make python
+C:/Users/99E7~1/AppData/Local/Temp/.venv/Scripts/python
+Python 3.5.4 (v3.5.4:3f56838, Aug  8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)] on win32
+Type "help", "copyright", "credits" or "license" for more information.
+>>> _
+```
+
+
+## Compatibility
+
+*Makefile.venv* was written for GNU Make and may not work with other make
+implementations. Please be aware that GNU Make [can not correctly handle][spaces]
+whitespace characters in file paths. Such filepaths therefore are
+considered unsupported by *Makefile.venv*
+
+[spaces]: https://stackoverflow.com/questions/9838384/can-gnu-make-handle-filenames-with-spaces
+
+*Makefile.venv* is being [continuously tested][tests] on Linux, Windows and macOS. Any
+inconsistency encountered when running on Windows should be considered a bug
+and should be reported via [issues].
+
+
+## Support and contributing
+
+If you need help with using this Makefile or including it into your project,
+please create **[an issue][issues]**.
+Issues are also the primary venue for reporting bugs and posting feature
+requests. General discussion related to this project is also acceptable and
+very welcome!
+
+In case you wish to contribute code or documentation, feel free to open
+**[a pull request](https://github.com/sio/Makefile.venv/pulls)**. That would
+certainly make my day!
+
+I'm open to dialog and I promise to behave responsibly and treat all
+contributors with respect. Please try to do the same, and treat others the way
+you want to be treated.
+
+If for some reason you'd rather not use the issue tracker, contacting me via
+email is OK too. Please use a descriptive subject line to enhance visibility
+of your message. Also please keep in mind that public discussion channels are
+preferable because that way many other people may benefit from reading past
+conversations. My email is visible under the GitHub profile and in the commit
+log.
+
+[issues]: https://github.com/sio/Makefile.venv/issues
+
+
+## License and copyright
+
+Copyright 2019-2023 Vitaly Potyarkin
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
```

#### html2text {}

```diff
@@ -12,17 +12,17 @@
 some configuration. ## Installation ### Recommended method Copy
 [*Makefile.venv*](Makefile.venv) to your project directory and add include
 statement to the bottom of your `Makefile`: ```make include Makefile.venv ```
 ### Alternative method Alternatively, you can add installation actions as the
 Makefile recipe: > **Note the checksum step!** Do not skip it, it would be as
 bad as [piping curl > to shell](https://0x46.net/thoughts/2019/04/27/piping-
 curl-to-shell/)! ```make include Makefile.venv Makefile.venv: curl \ -
-o Makefile.fetched \ -L "https://github.com/sio/Makefile.venv/raw/v2022.07.20/
+o Makefile.fetched \ -L "https://github.com/sio/Makefile.venv/raw/v2023.04.17/
 Makefile.venv" echo
-"147b164f0cbbbe4a2740dcca6c9adb6e9d8d15b895be3998697aa6a821a277d8
+"fb48375ed1fd19e41e0cdcf51a4a0c6d1010dfe03b672ffc4c26a91878544f82
 *Makefile.fetched" \ | sha256sum --check - \ && mv Makefile.fetched
 Makefile.venv ``` > Notes: > > * *curl* and/or *sha256sum* may not be available
 by default depending on what > OS and configuration is used > * To install
 *sha256sum* on macOS use `brew install coreutils` > * You can use Perl's
 *shasum -a 256* instead of *sha256sum*, as described > [here](https://
 github.com/sio/Makefile.venv/issues/11). ### Another alternative method If you
 want to use *Makefile.venv* in multiple projects and to be able to conveniently
@@ -73,63 +73,65 @@
 initially to create the virtual environment. *Default: python3* #####
 REQUIREMENTS_TXT Space separated list of paths to requirements.txt files. Paths
 are resolved relative to current working directory. *Default: requirements.txt*
 Non-existent files are treated as hard dependencies, recipes for creating such
 files must be provided by the main Makefile (sample usage: [pip-compile]).
 Providing empty value (`REQUIREMENTS_TXT=`) turns off processing of
 requirements.txt even when the file exists. [pip-compile]: docs/howto-pip-
-compile.md ##### SETUP_PY Space separated list of paths to setupâ¤py files.
-Corresponding packages will be installed into venv in [editable mode] along
-with all their dependencies. *Default: setupâ¤py* Non-existent and empty
-values are treated in the same way as for REQUIREMENTS_TXT. [editable mode]:
-https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs ##### WORKDIR
-Parent directory for the virtual environment. *Default: current working
-directory* ##### VENVDIR Python virtual environment directory. *Default: $
-(WORKDIR)/.venv* ##### PIP_* Variables named starting with `PIP_` are not
-processed by *Makefile.venv* in any way and are passed to underlying pip calls
-as is. See [pip documentation](https://pip.pypa.io/en/stable/user_guide/
-#environment-variables) for more information. Use these variables to customize
-pip invocation, for example to provide custom package index url: ```
-PIP_EXTRA_INDEX_URL="https://your.index/url" ``` ## Samples Makefile: ```make
-.PHONY: test test: venv $(VENV)/python -m unittest include Makefile.venv ```
-Larger sample from a real project can be seen [here](https://github.com/sio/
-issyours/blob/master/Makefile). Also see [an introductory blog post](https://
-potyarkin.ml/posts/2019/manage-python-virtual-environment-from-your-makefile/
-) from project author. Command line: ``` $ make test ...Skipped: creating and
-updating virtual environment... ... -------------------------------------------
---------------------------- Ran 3 tests in 0.000s OK ``` ``` $ make show-venv
-Python 3.5.4 (v3.5.4:3f56838, Aug 8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)]
-pip 19.2.3 from c:\users\99e7~1\appdata\local\temp\.venv\lib\site-packages\pip
-(python 3.5) venv: C:\Users\99E7~1\AppData\Local\Temp\.venv ``` ``` $ make
-python C:/Users/99E7~1/AppData/Local/Temp/.venv/Scripts/python Python 3.5.4
-(v3.5.4:3f56838, Aug 8 2017, 02:07:06) [MSC v.1900 32 bit (Intel)] on win32
-Type "help", "copyright", "credits" or "license" for more information. >>> _
-``` ## Compatibility *Makefile.venv* was written for GNU Make and may not work
-with other make implementations. Please be aware that GNU Make [can not
-correctly handle][spaces] whitespace characters in file paths. Such filepaths
-therefore are considered unsupported by *Makefile.venv* [spaces]: https://
-stackoverflow.com/questions/9838384/can-gnu-make-handle-filenames-with-spaces
-*Makefile.venv* is being [continuously tested][tests] on Linux, Windows and
-macOS. Any inconsistency encountered when running on Windows should be
-considered a bug and should be reported via [issues]. ## Support and
-contributing If you need help with using this Makefile or including it into
-your project, please create **[an issue][issues]**. Issues are also the primary
-venue for reporting bugs and posting feature requests. General discussion
-related to this project is also acceptable and very welcome! In case you wish
-to contribute code or documentation, feel free to open **[a pull request]
-(https://github.com/sio/Makefile.venv/pulls)**. That would certainly make my
-day! I'm open to dialog and I promise to behave responsibly and treat all
-contributors with respect. Please try to do the same, and treat others the way
-you want to be treated. If for some reason you'd rather not use the issue
-tracker, contacting me via email is OK too. Please use a descriptive subject
-line to enhance visibility of your message. Also please keep in mind that
-public discussion channels are preferable because that way many other people
-may benefit from reading past conversations. My email is visible under the
-GitHub profile and in the commit log. [issues]: https://github.com/sio/
-Makefile.venv/issues ## License and copyright Copyright 2019-2022 Vitaly
-Potyarkin Licensed under the Apache License, Version 2.0 (the "License"); you
-may not use this file except in compliance with the License. You may obtain a
-copy of the License at http://www.apache.org/licenses/LICENSE-2.0 Unless
-required by applicable law or agreed to in writing, software distributed under
-the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-CONDITIONS OF ANY KIND, either express or implied. See the License for the
-specific language governing permissions and limitations under the License.
+compile.md ##### SETUP_PY, SETUP_CFG, PYPROJECT_TOML, VENV_LOCAL_PACKAGE Space
+separated list of paths to files that contain build instructions for local
+Python packages. Corresponding packages will be installed into venv in
+[editable mode] along with all their dependencies. *Default: setup.py setup.cfg
+pyproject.toml (whichever present)* Non-existent and empty values are treated
+in the same way as for REQUIREMENTS_TXT. [editable mode]: https://pip.pypa.io/
+en/stable/cli/pip_install/#editable-installs ##### WORKDIR Parent directory for
+the virtual environment. *Default: current working directory* ##### VENVDIR
+Python virtual environment directory. *Default: $(WORKDIR)/.venv* ##### PIP_*
+Variables named starting with `PIP_` are not processed by *Makefile.venv* in
+any way and are passed to underlying pip calls as is. See [pip documentation]
+(https://pip.pypa.io/en/stable/user_guide/#environment-variables) for more
+information. Use these variables to customize pip invocation, for example to
+provide custom package index url: ``` PIP_EXTRA_INDEX_URL="https://your.index/
+url" ``` ## Samples Makefile: ```make .PHONY: test test: venv $(VENV)/python -
+m unittest include Makefile.venv ``` Larger sample from a real project can be
+seen [here](https://github.com/sio/issyours/blob/master/Makefile). Also see [an
+introductory blog post](https://potyarkin.ml/posts/2019/manage-python-virtual-
+environment-from-your-makefile/) from project author. Command line: ``` $ make
+test ...Skipped: creating and updating virtual environment... ... -------------
+--------------------------------------------------------- Ran 3 tests in 0.000s
+OK ``` ``` $ make show-venv Python 3.5.4 (v3.5.4:3f56838, Aug 8 2017, 02:07:06)
+[MSC v.1900 32 bit (Intel)] pip 19.2.3 from c:
+\users\99e7~1\appdata\local\temp\.venv\lib\site-packages\pip (python 3.5) venv:
+C:\Users\99E7~1\AppData\Local\Temp\.venv ``` ``` $ make python C:/Users/99E7~1/
+AppData/Local/Temp/.venv/Scripts/python Python 3.5.4 (v3.5.4:3f56838, Aug 8
+2017, 02:07:06) [MSC v.1900 32 bit (Intel)] on win32 Type "help", "copyright",
+"credits" or "license" for more information. >>> _ ``` ## Compatibility
+*Makefile.venv* was written for GNU Make and may not work with other make
+implementations. Please be aware that GNU Make [can not correctly handle]
+[spaces] whitespace characters in file paths. Such filepaths therefore are
+considered unsupported by *Makefile.venv* [spaces]: https://stackoverflow.com/
+questions/9838384/can-gnu-make-handle-filenames-with-spaces *Makefile.venv* is
+being [continuously tested][tests] on Linux, Windows and macOS. Any
+inconsistency encountered when running on Windows should be considered a bug
+and should be reported via [issues]. ## Support and contributing If you need
+help with using this Makefile or including it into your project, please create
+**[an issue][issues]**. Issues are also the primary venue for reporting bugs
+and posting feature requests. General discussion related to this project is
+also acceptable and very welcome! In case you wish to contribute code or
+documentation, feel free to open **[a pull request](https://github.com/sio/
+Makefile.venv/pulls)**. That would certainly make my day! I'm open to dialog
+and I promise to behave responsibly and treat all contributors with respect.
+Please try to do the same, and treat others the way you want to be treated. If
+for some reason you'd rather not use the issue tracker, contacting me via email
+is OK too. Please use a descriptive subject line to enhance visibility of your
+message. Also please keep in mind that public discussion channels are
+preferable because that way many other people may benefit from reading past
+conversations. My email is visible under the GitHub profile and in the commit
+log. [issues]: https://github.com/sio/Makefile.venv/issues ## License and
+copyright Copyright 2019-2023 Vitaly Potyarkin Licensed under the Apache
+License, Version 2.0 (the "License"); you may not use this file except in
+compliance with the License. You may obtain a copy of the License at http://
+www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
+to in writing, software distributed under the License is distributed on an "AS
+IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+implied. See the License for the specific language governing permissions and
+limitations under the License.
```

