# Comparing `tmp/py_3rdparty_mediawiki-0.9.4.tar.gz` & `tmp/py_3rdparty_mediawiki-0.9.5.tar.gz`

## Comparing `py_3rdparty_mediawiki-0.9.4.tar` & `py_3rdparty_mediawiki-0.9.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/.pydevproject
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/.readthedocs.yml
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/.travis.yml
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/docs/Makefile
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/docs/requirements.txt
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/docs/source/conf.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/docs/source/index.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/docs/source/modules.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/docs/source/setup.rst
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/docs/source/tests.rst
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/docs/source/wikibot.rst
--rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/scripts/doc
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/scripts/install
--rwxr-xr-x   0        0        0     2621 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/scripts/nightlywikibackup
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/scripts/release
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/basetest.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_MediaWikiTable.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_PageHistory.py
--rw-r--r--   0        0        0    24432 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_SMWApi.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_Selector.py
--rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_WikiPush.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_WikiUser.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_duckinterface.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_lambda.py
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_wikibot.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_wikiclient.py
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_wikiquery.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/tests/test_wikitext.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/__init__.py
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/crypt.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/lambda_action.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/mwTable.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/pagehistory.py
--rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/selector.py
--rw-r--r--   0        0        0    24548 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/smw.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/version.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wiki.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiaction.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikibackup.py
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikibot.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiclient.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiedit.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikinuke.py
--rw-r--r--   0        0        0    39658 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikipush.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiquery.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikitext.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiupload.py
--rw-r--r--   0        0        0    10050 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiuser.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/.gitignore
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/LICENSE
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/README.md
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/.pydevproject
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/.readthedocs.yml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/.travis.yml
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/docs/Makefile
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/docs/requirements.txt
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/docs/source/conf.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/docs/source/index.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/docs/source/modules.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/docs/source/setup.rst
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/docs/source/tests.rst
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/docs/source/wikibot.rst
+-rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/scripts/doc
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/scripts/install
+-rwxr-xr-x   0        0        0     2621 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/scripts/nightlywikibackup
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/scripts/release
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/basetest.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_MediaWikiTable.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_PageHistory.py
+-rw-r--r--   0        0        0    24432 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_SMWApi.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_Selector.py
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_WikiPush.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_WikiUser.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_duckinterface.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_lambda.py
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_wikibot.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_wikiclient.py
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_wikiquery.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/tests/test_wikitext.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/__init__.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/crypt.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/lambda_action.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/mwTable.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/pagehistory.py
+-rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/selector.py
+-rw-r--r--   0        0        0    24548 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/smw.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/version.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wiki.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiaction.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikibackup.py
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikibot.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiclient.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiedit.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikinuke.py
+-rw-r--r--   0        0        0    41607 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikipush.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiquery.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikitext.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiupload.py
+-rw-r--r--   0        0        0    10050 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiuser.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/.gitignore
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/LICENSE
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/README.md
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 py_3rdparty_mediawiki-0.9.5/PKG-INFO
```

### Comparing `py_3rdparty_mediawiki-0.9.4/.readthedocs.yml` & `py_3rdparty_mediawiki-0.9.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/.travis.yml` & `py_3rdparty_mediawiki-0.9.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/.github/workflows/build.yml` & `py_3rdparty_mediawiki-0.9.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/.github/workflows/upload-to-pypi.yml` & `py_3rdparty_mediawiki-0.9.5/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/docs/Makefile` & `py_3rdparty_mediawiki-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/docs/source/conf.py` & `py_3rdparty_mediawiki-0.9.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/docs/source/index.rst` & `py_3rdparty_mediawiki-0.9.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/docs/source/tests.rst` & `py_3rdparty_mediawiki-0.9.5/docs/source/tests.rst`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/docs/source/wikibot.rst` & `py_3rdparty_mediawiki-0.9.5/docs/source/wikibot.rst`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/scripts/nightlywikibackup` & `py_3rdparty_mediawiki-0.9.5/scripts/nightlywikibackup`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/basetest.py` & `py_3rdparty_mediawiki-0.9.5/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_MediaWikiTable.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_MediaWikiTable.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_PageHistory.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_PageHistory.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_SMWApi.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_SMWApi.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_Selector.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_Selector.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_WikiPush.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_WikiPush.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_WikiUser.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_WikiUser.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_duckinterface.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_duckinterface.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_lambda.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_wikibot.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_wikibot.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_wikiclient.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_wikiclient.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_wikiquery.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_wikiquery.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/tests/test_wikitext.py` & `py_3rdparty_mediawiki-0.9.5/tests/test_wikitext.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/crypt.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/crypt.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/lambda_action.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/lambda_action.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/mwTable.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/mwTable.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/pagehistory.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/pagehistory.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/selector.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/selector.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/smw.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/smw.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/version.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/version.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/wiki.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/wiki.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiaction.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiaction.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikibot.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikibot.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiclient.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiclient.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikipush.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikipush.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,24 @@
 
 class WikiPush(object):
     '''
     Push pages from one MediaWiki to another
     '''
     differ=None
     
-    def __init__(self, fromWikiId, toWikiId=None,login=False,verbose=True,debug=False):
+    def __init__(self, fromWikiId:str, toWikiId:str=None,login:bool=False,verbose:bool=True,debug:bool=False):
         '''
         Constructor
+        
+        Args:
+            fromWikiId(str): the id of the wiki to push from (source)
+            toWikiID(str): the id of the wiki to push to (target)
+            login(bool): if True login to source wiki
+            verbose(bool): if True print info messages
+            debug(bool): if True show debugging messages
         '''
         self.verbose=verbose
         self.debug=debug
         self.fromWiki=None
         self.toWiki=None
         
         self.fromWikiId=fromWikiId
@@ -382,74 +389,109 @@
             else:
                 repo=Repo(backupPath)
             self.log("committing to git repository")
             repo.git.add(all=True)
             timestamp=datetime.datetime.now().isoformat()
             repo.index.commit("auto commit by wikibackup at %s" % timestamp)
         
-    def backupImages(self,imageList,imageBackupPath):
-        '''
-        '''
+    def backupImages(self,imageList:list,imageBackupPath:str):
+        """
+        backup the images in the givne imageList
+        
+        Args:
+            imageList(list): the list of images
+            imageBackupPath(str): the path to the backup directory
+        """
         for image in imageList:
             try:
                 imagePath,filename=self.downloadImage(image,imageBackupPath)
             except Exception as ex:
                 self.handleException(ex)
-        
-    def push(self,pageTitles,force=False,ignore=False,withImages=False):
-        '''
-        push the given page titles
+                
+    def work(self,pageTitles:list,activity:str="copying",comment:str="pushed",force:bool=False,ignore:bool=False,withImages:bool=False)->list:
+        """
+        work on the given page titles
         
         Args:
             pageTitles(list): a list of page titles to be transfered from the formWiki to the toWiki
+            activity(str): the activity to perform
+            comment(str): the comment to display 
             force(bool): True if pages should be overwritten if they exist
             ignore(bool): True if warning for images should be ignored (e.g if they exist)
             withImages(bool): True if the image on a page should also be copied
-        '''
+        Returns:
+            list: a list of pageTitles for which the activity failed
+        """
+        failed=[]
         total=len(pageTitles)
-        self.log("copying %d pages from %s to %s" % (total,self.fromWikiId,self.toWikiId))
+        self.log(f"{activity} {total} pages from {self.fromWikiId} to {self.toWikiId}")
         for i,pageTitle in enumerate(pageTitles):
             try:
-                self.log("%d/%d (%4.0f%%): copying %s ..." % (i+1,total,(i+1)/total*100,pageTitle), end='')
+                percent=(i+1)/total*100
+                self.log(f"{i+1}/{total} ({percent:4.0f}%): {activity} ... {pageTitle}", end='')
                 page=self.fromWiki.getPage(pageTitle)
                 if page.exists:
                     # is this an image?
                     if isinstance(page,Image):
                         self.pushImages([page],ignore=ignore)
                     else:
                         newPage=self.toWiki.getPage(pageTitle)
                         if not newPage.exists or force:
                             try:
-                                comment="pushed from %s by wikipush" % self.fromWikiId
                                 newPage.edit(page.text(),comment)
                                 self.log("✅")
                                 pageOk=True
                             except Exception as ex:
                                 pageOk=self.handleException(ex, ignore)
+                                if not pageOk:
+                                    failed.append(pageTitle)
                             if withImages and pageOk:
                                 self.pushImages(page.images(),ignore=ignore)
                         else:
                             self.log("👎")
                 else:
                     self.log("❌")
+                    failed.append(pageTitle)
             except Exception as ex:
-                self.log("❌:%s" % str(ex) )       
+                self.log(f"❌:{str(ex)}")   
+                failed.append(pageTitle)
+        return failed
+        
+    def push(self,pageTitles,force=False,ignore=False,withImages=False)->list:
+        '''
+        push the given page titles
+        
+        Args:
+            pageTitles(list): a list of page titles to be transfered from the formWiki to the toWiki
+            force(bool): True if pages should be overwritten if they exist
+            ignore(bool): True if warning for images should be ignored (e.g if they exist)
+            withImages(bool): True if the image on a page should also be copied
+        Returns:
+            list: a list of pageTitles for which the activity failed
+        '''
+        comment=f"pushed from {self.fromWikiId} by wikipush"  
+        return self.work(pageTitles, activity="copying",comment=comment,force=force, ignore=ignore, withImages=withImages)
                 
-    def ensureParentDirectoryExists(self,filePath):
-        # for pages that have a "/" in the name:
+    def ensureParentDirectoryExists(self,filePath:str):
+        """
+        for pages that have a "/" in the name make sure that the parent Directory exists
+        
+        Args:
+            filePath(str): the filePath to check
+        """
         directory = os.path.dirname(filePath)
         self.ensureDirectoryExists(directory)
         
-    def ensureDirectoryExists(self,directory):
-        '''
+    def ensureDirectoryExists(self,directory:str):
+        """
         make sure the given directory exists
         
         Args: 
             directory(str): the directory to check for existence
-        '''
+        """
         Path(directory).mkdir(parents=True, exist_ok=True)
         
     def getHomePath(self,localPath):
         '''
         get the given home path
         '''
         homePath=f"{Path.home()}/{localPath}"
@@ -457,15 +499,14 @@
         return homePath
                     
     def getDownloadPath(self):
         '''
         get the download path
         '''
         return self.getHomePath("Downloads/mediawiki")
-        
             
     def pushImages(self,imageList,delim="",ignore=False):
         '''
         push the images in the given image List
         
         Args:
             imageList(list): a list of images to be pushed
@@ -583,17 +624,20 @@
             if warnings:
                 raise Exception(warnings)
 
     def restore(self, pageTitles=None, backupPath=None, listFile=None, stdIn=False):
         """
         restore given page titles from local backup
         If no page titles are given the whole backup is restored.
+        
         Args:
             pageTitles(list): a list of pageTitles to be restored to toWiki. If None -> full restore of backup
             backupPath(str): path to backup location
+            listFile:
+            stdIn:
         """
         if stdIn:
             backupPath = os.path.dirname(pageTitles[0].strip())
             pageTitlesfix= []
             for i in pageTitles:
                 pageTitlesfix.append(os.path.basename(i.strip().replace('.wiki','')))
             pageTitles = pageTitlesfix
@@ -601,28 +645,28 @@
             f = open(listFile, 'r')
             allx = f.readlines()
             pageTitles = []
             for i in allx:
                 pageTitles.append(os.path.basename(i.strip()).replace('.wiki',''))
         else:
             if backupPath is None:
-                backupPath=self.getHomePath("wikibackup/%s" % self.toWikiId)
+                backupPath=self.getHomePath(f"wikibackup/{self.toWikiId}")
             if pageTitles is None:
                 pageTitles = []
                 for path, subdirs, files in os.walk(backupPath):
                     for name in files:
                         filename = os.path.join(path, name)[len(backupPath)+1:]
                         if filename.endswith(".wiki"):
                             pageTitles.append(filename[:-len(".wiki")])
         total = len(pageTitles)
         self.log("restoring %d pages from %s to %s" % (total, backupPath, self.toWikiId))
         for i,pageTitle in enumerate(pageTitles):
             try:
                 self.log("%d/%d (%4.0f%%): restore %s ..." % (i + 1, total, (i + 1) / total * 100, pageTitle),end='')
-                wikiFilePath = "%s/%s.wiki" % (backupPath, pageTitle)
+                wikiFilePath = f"{backupPath}/{pageTitle}.wiki"
                 with open(wikiFilePath, mode='r') as wikiFile:
                     page_content = wikiFile.read()
                     page = self.toWiki.getPage(pageTitle)
                     page.edit(page_content, f"modified through wikirestore by {self.toWiki.wikiUser.user}")
                 self.log("✅")
             except Exception as ex:
                 self.log("❌:%s" % str(ex) )
@@ -665,15 +709,15 @@
     program_version_message = '%%(prog)s %s (%s)' % (program_version, program_build_date)
     program_shortdesc = "wikipush"
     user_name="Wolfgang Fahl"
 
     program_license = '''%s
 
   Created by %s on %s.
-  Copyright 2020 Wolfgang Fahl. All rights reserved.
+  Copyright 2020-2023 Wolfgang Fahl. All rights reserved.
 
   Licensed under the Apache License 2.0
   http://www.apache.org/licenses/LICENSE-2.0
 
   Distributed on an "AS IS" basis without warranties
   or conditions of any kind, either express or implied.
```

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikitext.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikitext.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/wikibot3rd/wikiuser.py` & `py_3rdparty_mediawiki-0.9.5/wikibot3rd/wikiuser.py`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/.gitignore` & `py_3rdparty_mediawiki-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/LICENSE` & `py_3rdparty_mediawiki-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/README.md` & `py_3rdparty_mediawiki-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/pyproject.toml` & `py_3rdparty_mediawiki-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_3rdparty_mediawiki-0.9.4/PKG-INFO` & `py_3rdparty_mediawiki-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-3rdparty-mediawiki
-Version: 0.9.4
+Version: 0.9.5
 Summary: Wrapper for mwclient with improvements for 3rd party wikis
 Project-URL: homepage, https://wiki.bitplan.com/index.php/Py-3rdparty-mediawiki
 Project-URL: documentation, https://wiki.bitplan.com/index.php/Py-3rdparty-mediawiki
 Project-URL: repository, https://wiki.bitplan.com/index.php/Py-3rdparty-mediawiki
 Author-email: Wolfgang Fahl <wf@bitplan.com>, Tim Holzheim <tim.holzheim@rwth-aachen.de>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>, Tim Holzheim <tim.holzheim@rwth-aachen.de>
 License-Expression: Apache-2.0
```

