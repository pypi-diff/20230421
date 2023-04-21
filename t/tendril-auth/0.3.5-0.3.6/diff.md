# Comparing `tmp/tendril-auth-0.3.5.tar.gz` & `tmp/tendril-auth-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-auth-0.3.5.tar", last modified: Wed Apr 19 18:12:48 2023, max compression
+gzip compressed data, was "tendril-auth-0.3.6.tar", last modified: Thu Apr 20 18:26:51 2023, max compression
```

## Comparing `tendril-auth-0.3.5.tar` & `tendril-auth-0.3.6.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.532154 tendril-auth-0.3.5/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2023-04-19 18:12:48.532154 tendril-auth-0.3.5/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.492155 tendril-auth-0.3.5/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.500155 tendril-auth-0.3.5/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.500155 tendril-auth-0.3.5/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-auth-0.3.5/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.500155 tendril-auth-0.3.5/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.504155 tendril-auth-0.3.5/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-19 18:12:48.536154 tendril-auth-0.3.5/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3253 2023-03-15 16:03:53.000000 tendril-auth-0.3.5/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.468155 tendril-auth-0.3.5/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.504155 tendril-auth-0.3.5/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.504155 tendril-auth-0.3.5/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.5/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.508155 tendril-auth-0.3.5/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.5/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-02-18 10:30:44.000000 tendril-auth-0.3.5/src/tendril/apiserver/routers/authn.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.512155 tendril-auth-0.3.5/src/tendril/authn/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:59:41.000000 tendril-auth-0.3.5/src/tendril/authn/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5999 2023-03-15 16:03:53.000000 tendril-auth-0.3.5/src/tendril/authn/auth0.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.516155 tendril-auth-0.3.5/src/tendril/authn/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.5/src/tendril/authn/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril-auth-0.3.5/src/tendril/authn/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril-auth-0.3.5/src/tendril/authn/db/mixins.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril-auth-0.3.5/src/tendril/authn/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1193 2023-04-19 17:58:24.000000 tendril-auth-0.3.5/src/tendril/authn/pydantic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2800 2023-04-19 15:44:25.000000 tendril-auth-0.3.5/src/tendril/authn/users.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.520155 tendril-auth-0.3.5/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril-auth-0.3.5/src/tendril/authz/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1508 2023-02-28 00:23:46.000000 tendril-auth-0.3.5/src/tendril/authz/auth0.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril-auth-0.3.5/src/tendril/authz/connector.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.524155 tendril-auth-0.3.5/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril-auth-0.3.5/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril-auth-0.3.5/src/tendril/authz/scopes/common.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1357 2023-02-28 00:59:55.000000 tendril-auth-0.3.5/src/tendril/authz/scopes/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.524155 tendril-auth-0.3.5/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-auth-0.3.5/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2708 2023-03-28 18:07:23.000000 tendril-auth-0.3.5/src/tendril/config/auth.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.528154 tendril-auth-0.3.5/src/tendril_auth.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2023-04-19 18:12:47.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1242 2023-04-19 18:12:48.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-19 18:12:47.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2023-04-19 18:12:47.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-19 18:12:47.000000 tendril-auth-0.3.5/src/tendril_auth.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-19 18:12:48.532154 tendril-auth-0.3.5/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril-auth-0.3.5/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.929500 tendril-auth-0.3.6/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2023-04-20 18:26:51.929500 tendril-auth-0.3.6/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2144 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.753503 tendril-auth-0.3.6/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.777503 tendril-auth-0.3.6/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.781503 tendril-auth-0.3.6/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-auth-0.3.6/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.781503 tendril-auth-0.3.6/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13454 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      937 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1518 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.801502 tendril-auth-0.3.6/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-20 18:26:51.933499 tendril-auth-0.3.6/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3253 2023-03-15 16:03:53.000000 tendril-auth-0.3.6/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.693505 tendril-auth-0.3.6/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.817502 tendril-auth-0.3.6/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.825502 tendril-auth-0.3.6/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.6/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.837502 tendril-auth-0.3.6/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.6/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-02-18 10:30:44.000000 tendril-auth-0.3.6/src/tendril/apiserver/routers/authn.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.861501 tendril-auth-0.3.6/src/tendril/authn/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:59:41.000000 tendril-auth-0.3.6/src/tendril/authn/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5999 2023-03-15 16:03:53.000000 tendril-auth-0.3.6/src/tendril/authn/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1837 2023-04-20 18:25:16.000000 tendril-auth-0.3.6/src/tendril/authn/client.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.877501 tendril-auth-0.3.6/src/tendril/authn/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:58:03.000000 tendril-auth-0.3.6/src/tendril/authn/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2890 2023-02-28 04:21:34.000000 tendril-auth-0.3.6/src/tendril/authn/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      405 2022-12-10 17:21:52.000000 tendril-auth-0.3.6/src/tendril/authn/db/mixins.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1486 2022-12-09 17:58:03.000000 tendril-auth-0.3.6/src/tendril/authn/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1193 2023-04-19 17:58:24.000000 tendril-auth-0.3.6/src/tendril/authn/pydantic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2800 2023-04-19 15:44:25.000000 tendril-auth-0.3.6/src/tendril/authn/users.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.897500 tendril-auth-0.3.6/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril-auth-0.3.6/src/tendril/authz/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1508 2023-02-28 00:23:46.000000 tendril-auth-0.3.6/src/tendril/authz/auth0.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      795 2023-02-28 00:24:44.000000 tendril-auth-0.3.6/src/tendril/authz/connector.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.905500 tendril-auth-0.3.6/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:54:27.000000 tendril-auth-0.3.6/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      111 2023-02-28 00:52:46.000000 tendril-auth-0.3.6/src/tendril/authz/scopes/common.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1357 2023-02-28 00:59:55.000000 tendril-auth-0.3.6/src/tendril/authz/scopes/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.909500 tendril-auth-0.3.6/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-auth-0.3.6/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2708 2023-03-28 18:07:23.000000 tendril-auth-0.3.6/src/tendril/config/auth.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.921500 tendril-auth-0.3.6/src/tendril_auth.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3435 2023-04-20 18:26:50.000000 tendril-auth-0.3.6/src/tendril_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1270 2023-04-20 18:26:51.000000 tendril-auth-0.3.6/src/tendril_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-20 18:26:50.000000 tendril-auth-0.3.6/src/tendril_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      585 2023-04-20 18:26:50.000000 tendril-auth-0.3.6/src/tendril_auth.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-20 18:26:50.000000 tendril-auth-0.3.6/src/tendril_auth.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-20 18:26:51.925500 tendril-auth-0.3.6/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2021-08-13 17:52:37.000000 tendril-auth-0.3.6/tox.ini
```

### Comparing `tendril-auth-0.3.5/.gitignore` & `tendril-auth-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/.readthedocs.yml` & `tendril-auth-0.3.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/.travis.yml` & `tendril-auth-0.3.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/LICENSE` & `tendril-auth-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/PKG-INFO` & `tendril-auth-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-auth
-Version: 0.3.5
+Version: 0.3.6
 Summary: Authentication and User Management Core for Tendril
 Home-page: https://github.com/tendril-framework/tendril-auth
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-auth.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-auth/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-auth
```

### Comparing `tendril-auth-0.3.5/README.rst` & `tendril-auth-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/Makefile` & `tendril-auth-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/_static/custom.css` & `tendril-auth-0.3.6/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/_static/favicon.ico` & `tendril-auth-0.3.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/_static/logo.png` & `tendril-auth-0.3.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/_static/logo_packed.png` & `tendril-auth-0.3.6/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/_templates/about.html` & `tendril-auth-0.3.6/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/conf.py` & `tendril-auth-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/index.rst` & `tendril-auth-0.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/docs/installation.rst` & `tendril-auth-0.3.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/setup.py` & `tendril-auth-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/apiserver/routers/authn.py` & `tendril-auth-0.3.6/src/tendril/apiserver/routers/authn.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/authn/auth0.py` & `tendril-auth-0.3.6/src/tendril/authn/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/authn/db/controller.py` & `tendril-auth-0.3.6/src/tendril/authn/db/controller.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/authn/db/model.py` & `tendril-auth-0.3.6/src/tendril/authn/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/authn/pydantic.py` & `tendril-auth-0.3.6/src/tendril/authn/pydantic.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/authn/users.py` & `tendril-auth-0.3.6/src/tendril/authn/users.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/authz/auth0.py` & `tendril-auth-0.3.6/src/tendril/authz/auth0.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/authz/connector.py` & `tendril-auth-0.3.6/src/tendril/authz/connector.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/authz/scopes/manager.py` & `tendril-auth-0.3.6/src/tendril/authz/scopes/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/config/__init__.py` & `tendril-auth-0.3.6/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril/config/auth.py` & `tendril-auth-0.3.6/src/tendril/config/auth.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/src/tendril_auth.egg-info/PKG-INFO` & `tendril-auth-0.3.6/src/tendril_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-auth
-Version: 0.3.5
+Version: 0.3.6
 Summary: Authentication and User Management Core for Tendril
 Home-page: https://github.com/tendril-framework/tendril-auth
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-auth.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-auth/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-auth
```

### Comparing `tendril-auth-0.3.5/src/tendril_auth.egg-info/SOURCES.txt` & `tendril-auth-0.3.6/src/tendril_auth.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 docs/usage/tendril.rst
 src/tendril/__init__.py
 src/tendril/apiserver/__init__.py
 src/tendril/apiserver/routers/__init__.py
 src/tendril/apiserver/routers/authn.py
 src/tendril/authn/__init__.py
 src/tendril/authn/auth0.py
+src/tendril/authn/client.py
 src/tendril/authn/pydantic.py
 src/tendril/authn/users.py
 src/tendril/authn/db/__init__.py
 src/tendril/authn/db/controller.py
 src/tendril/authn/db/mixins.py
 src/tendril/authn/db/model.py
 src/tendril/authz/__init__.py
```

### Comparing `tendril-auth-0.3.5/src/tendril_auth.egg-info/requires.txt` & `tendril-auth-0.3.6/src/tendril_auth.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/tests/coveralls.py` & `tendril-auth-0.3.6/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-auth-0.3.5/tox.ini` & `tendril-auth-0.3.6/tox.ini`

 * *Files identical despite different names*

