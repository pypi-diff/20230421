# Comparing `tmp/python_poppler-0.4.0.tar.gz` & `tmp/python_poppler-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_poppler-0.4.0.tar", last modified: Wed Mar 22 02:19:24 2023, max compression
+gzip compressed data, was "python_poppler-0.4.1.tar", last modified: Fri Apr 21 20:40:54 2023, max compression
```

## Comparing `python_poppler-0.4.0.tar` & `python_poppler-0.4.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 python_poppler-0.4.0/.github/workflows/build_and_test.yml
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 python_poppler-0.4.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 python_poppler-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      158 1970-01-01 00:00:00.000000 python_poppler-0.4.0/.gitignore
--rw-r--r--   0        0        0    18092 1970-01-01 00:00:00.000000 python_poppler-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0       87 1970-01-01 00:00:00.000000 python_poppler-0.4.0/NEWS.txt
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 python_poppler-0.4.0/README.md
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 python_poppler-0.4.0/TODO
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/Makefile
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/_static/.do_not_delete
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/_templates/.do_not_delete
--rw-r--r--   0        0        0       86 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/api/modules.rst
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/changelog.rst
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/conf.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/contribution.rst
--rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/index.rst
--rw-r--r--   0        0        0     4095 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/installation.rst
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/make.bat
--rw-r--r--   0        0        0     8720 1970-01-01 00:00:00.000000 python_poppler-0.4.0/docs/usage.rst
--rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 python_poppler-0.4.0/meson.build
--rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 python_poppler-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/destination.cpp
--rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/document.cpp
--rw-r--r--   0        0        0     1984 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/embedded_file.cpp
--rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/font.cpp
--rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/global.cpp
--rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/image.cpp
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/meson.build
--rw-r--r--   0        0        0     4856 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/page.cpp
--rw-r--r--   0        0        0     3020 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/page_renderer.cpp
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/page_transition.cpp
--rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/rectangle.cpp
--rw-r--r--   0        0        0     1564 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/toc.cpp
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/version.cpp
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/cpp/version.h
--rw-r--r--   0        0        0       32 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/meson.build
--rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/__init__.py
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/_version.py.in
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/cpp/__init__.py
--rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/destination.py
--rw-r--r--   0        0        0     8678 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/document.py
--rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/embeddedfile.py
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/font.py
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/image.py
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/meson.build
--rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/page.py
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/pagerenderer.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/pagetransition.py
--rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/rectangle.py
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/toc.py
--rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 python_poppler-0.4.0/src/poppler/utilities.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 python_poppler-0.4.0/subprojects/pybind11.wrap
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0       36 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/data/.gitignore
--rw-r--r--   0        0        0     8516 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/data/document.pdf
--rw-r--r--   0        0        0    17873 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/data/error_log.pdf
--rw-r--r--   0        0        0    78233 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/data/sample.pdf
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/data/sample.tex
--rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_destination.py
--rw-r--r--   0        0        0    16232 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_document.py
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_font.py
--rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_image.py
--rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_page.py
--rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_pagerenderer.py
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_pagetransition.py
--rw-r--r--   0        0        0     2109 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_rectangle.py
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_toc.py
--rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tests/test_version.py
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 python_poppler-0.4.0/tox.ini
--rw-r--r--   0        0        0    24079 1970-01-01 00:00:00.000000 python_poppler-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 python_poppler-0.4.1/.github/workflows/build_and_test.yml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 python_poppler-0.4.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 python_poppler-0.4.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      158 1970-01-01 00:00:00.000000 python_poppler-0.4.1/.gitignore
+-rw-r--r--   0        0        0    18092 1970-01-01 00:00:00.000000 python_poppler-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0       87 1970-01-01 00:00:00.000000 python_poppler-0.4.1/NEWS.txt
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 python_poppler-0.4.1/README.md
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 python_poppler-0.4.1/TODO
+-rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/Makefile
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/_static/.do_not_delete
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/_templates/.do_not_delete
+-rw-r--r--   0        0        0       86 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/api/modules.rst
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/changelog.rst
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/conf.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/contribution.rst
+-rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/index.rst
+-rw-r--r--   0        0        0     4095 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/installation.rst
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/make.bat
+-rw-r--r--   0        0        0     8720 1970-01-01 00:00:00.000000 python_poppler-0.4.1/docs/usage.rst
+-rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 python_poppler-0.4.1/meson.build
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 python_poppler-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/destination.cpp
+-rw-r--r--   0        0        0     7485 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/document.cpp
+-rw-r--r--   0        0        0     1984 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/embedded_file.cpp
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/font.cpp
+-rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/global.cpp
+-rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/image.cpp
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/meson.build
+-rw-r--r--   0        0        0     4856 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/page.cpp
+-rw-r--r--   0        0        0     3020 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/page_renderer.cpp
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/page_transition.cpp
+-rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/rectangle.cpp
+-rw-r--r--   0        0        0     1564 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/toc.cpp
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/version.cpp
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/cpp/version.h
+-rw-r--r--   0        0        0       32 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/meson.build
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/__init__.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/_version.py.in
+-rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/cpp/__init__.py
+-rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/destination.py
+-rw-r--r--   0        0        0     8678 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/document.py
+-rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/embeddedfile.py
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/font.py
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/image.py
+-rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/meson.build
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/page.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/pagerenderer.py
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/pagetransition.py
+-rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/rectangle.py
+-rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/toc.py
+-rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 python_poppler-0.4.1/src/poppler/utilities.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 python_poppler-0.4.1/subprojects/pybind11.wrap
+-rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0       36 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/data/.gitignore
+-rw-r--r--   0        0        0     8516 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/data/document.pdf
+-rw-r--r--   0        0        0    17873 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/data/error_log.pdf
+-rw-r--r--   0        0        0    78233 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/data/sample.pdf
+-rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/data/sample.tex
+-rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_destination.py
+-rw-r--r--   0        0        0    16232 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_document.py
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_font.py
+-rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_image.py
+-rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_page.py
+-rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_pagerenderer.py
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_pagetransition.py
+-rw-r--r--   0        0        0     2109 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_rectangle.py
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_toc.py
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tests/test_version.py
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 python_poppler-0.4.1/tox.ini
+-rw-r--r--   0        0        0    24079 1970-01-01 00:00:00.000000 python_poppler-0.4.1/PKG-INFO
```

### Comparing `python_poppler-0.4.0/.github/workflows/build_and_test.yml` & `python_poppler-0.4.1/.github/workflows/build_and_test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 jobs:
 
   build_poppler:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
-        poppler-version: [poppler-0.26.0, poppler-22.04.0, poppler-23.03.0]  #, master]
+        poppler-version: [poppler-0.26.0, poppler-22.04.0, poppler-23.04.0]  #, master]
     steps:
       - name: Install dependencies
         run: sudo apt-get install libopenjp2-7-dev libboost-dev
       - name: clone poppler
         run: |
           git clone https://gitlab.freedesktop.org/poppler/poppler.git
           cd poppler
@@ -57,15 +57,15 @@
   build:
     needs: build_poppler
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04]
         python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
-        poppler-version: [poppler-0.26.0, poppler-22.04.0, poppler-23.03.0]  #, master]
+        poppler-version: [poppler-0.26.0, poppler-22.04.0, poppler-23.04.0]  #, master]
         include:
           - python-version: '3.8'
             poppler-version: system
             os: ubuntu-20.04
           - python-version: '3.10'
             poppler-version: system
             os: ubuntu-22.04
```

### Comparing `python_poppler-0.4.0/.github/workflows/documentation.yml` & `python_poppler-0.4.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/.github/workflows/publish.yml` & `python_poppler-0.4.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/LICENSE.txt` & `python_poppler-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/README.md` & `python_poppler-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/docs/Makefile` & `python_poppler-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/docs/changelog.rst` & `python_poppler-0.4.1/docs/changelog.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 .. _changelog:
 
 Changelog
 =========
 
-0.4.0 (2023-04-21)
+0.4.1 (2023-04-21)
+------------------
+
+- Fix non-pure build for meson-python (:issue:`74` / :pr:`75`)
+- Fix build on Mac OS (:issue:`76` / :pr:`77`)
+- Tested with Python 3.11 and Poppler 23.04.0
+
+0.4.0 (2023-03-21)
 ------------------
 
 - Minimal supported Python version is now 3.7
 - Tested with Python 3.11 and Poppler 23.03.0
 - Build system is now ``meson``, and package is PEP-517 compliant (:pr:`70`)
 
 0.3.0 (2022-04-12)
```

### Comparing `python_poppler-0.4.0/docs/conf.py` & `python_poppler-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/docs/contribution.rst` & `python_poppler-0.4.1/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/docs/index.rst` & `python_poppler-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/docs/installation.rst` & `python_poppler-0.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/docs/make.bat` & `python_poppler-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/docs/usage.rst` & `python_poppler-0.4.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/pyproject.toml` & `python_poppler-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/destination.cpp` & `python_poppler-0.4.1/src/cpp/destination.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/document.cpp` & `python_poppler-0.4.1/src/cpp/document.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/embedded_file.cpp` & `python_poppler-0.4.1/src/cpp/embedded_file.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/font.cpp` & `python_poppler-0.4.1/src/cpp/font.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/global.cpp` & `python_poppler-0.4.1/src/cpp/global.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/image.cpp` & `python_poppler-0.4.1/src/cpp/image.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/meson.build` & `python_poppler-0.4.1/src/cpp/meson.build`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/page.cpp` & `python_poppler-0.4.1/src/cpp/page.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/page_renderer.cpp` & `python_poppler-0.4.1/src/cpp/page_renderer.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/page_transition.cpp` & `python_poppler-0.4.1/src/cpp/page_transition.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/rectangle.cpp` & `python_poppler-0.4.1/src/cpp/rectangle.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/toc.cpp` & `python_poppler-0.4.1/src/cpp/toc.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/version.cpp` & `python_poppler-0.4.1/src/cpp/version.cpp`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/cpp/version.h` & `python_poppler-0.4.1/src/cpp/version.h`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/__init__.py` & `python_poppler-0.4.1/src/poppler/__init__.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/_version.py.in` & `python_poppler-0.4.1/src/poppler/_version.py.in`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/cpp/__init__.py` & `python_poppler-0.4.1/src/poppler/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/destination.py` & `python_poppler-0.4.1/src/poppler/destination.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/document.py` & `python_poppler-0.4.1/src/poppler/document.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/embeddedfile.py` & `python_poppler-0.4.1/src/poppler/embeddedfile.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/font.py` & `python_poppler-0.4.1/src/poppler/font.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/image.py` & `python_poppler-0.4.1/src/poppler/image.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/meson.build` & `python_poppler-0.4.1/src/poppler/meson.build`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/page.py` & `python_poppler-0.4.1/src/poppler/page.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/pagerenderer.py` & `python_poppler-0.4.1/src/poppler/pagerenderer.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/pagetransition.py` & `python_poppler-0.4.1/src/poppler/pagetransition.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/rectangle.py` & `python_poppler-0.4.1/src/poppler/rectangle.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/toc.py` & `python_poppler-0.4.1/src/poppler/toc.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/src/poppler/utilities.py` & `python_poppler-0.4.1/src/poppler/utilities.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/__init__.py` & `python_poppler-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/conftest.py` & `python_poppler-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/data/document.pdf` & `python_poppler-0.4.1/tests/data/document.pdf`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/data/error_log.pdf` & `python_poppler-0.4.1/tests/data/error_log.pdf`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/data/sample.pdf` & `python_poppler-0.4.1/tests/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/data/sample.tex` & `python_poppler-0.4.1/tests/data/sample.tex`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_destination.py` & `python_poppler-0.4.1/tests/test_destination.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_document.py` & `python_poppler-0.4.1/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_font.py` & `python_poppler-0.4.1/tests/test_font.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_image.py` & `python_poppler-0.4.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_page.py` & `python_poppler-0.4.1/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_pagerenderer.py` & `python_poppler-0.4.1/tests/test_pagerenderer.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_pagetransition.py` & `python_poppler-0.4.1/tests/test_pagetransition.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_rectangle.py` & `python_poppler-0.4.1/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_toc.py` & `python_poppler-0.4.1/tests/test_toc.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tests/test_version.py` & `python_poppler-0.4.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/tox.ini` & `python_poppler-0.4.1/tox.ini`

 * *Files identical despite different names*

### Comparing `python_poppler-0.4.0/PKG-INFO` & `python_poppler-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-poppler
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python binding to poppler-cpp
 Keywords: pdf poppler
 Author-Email: Charles Brunet <charles@cbrunet.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
```

