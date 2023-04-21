# Comparing `tmp/cmdix-1.0.2.tar.gz` & `tmp/cmdix-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdix-1.0.2.tar", last modified: Wed Nov  2 15:50:38 2022, max compression
+gzip compressed data, was "cmdix-2.0.1.tar", last modified: Fri Apr 21 20:48:33 2023, max compression
```

## Comparing `cmdix-1.0.2.tar` & `cmdix-2.0.1.tar`

### file list

```diff
@@ -1,121 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:50:38.617865 cmdix-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-02 15:49:56.000000 cmdix-1.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-02 15:49:56.000000 cmdix-1.0.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-11-02 15:49:56.000000 cmdix-1.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:50:38.609865 cmdix-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-11-02 15:49:56.000000 cmdix-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:50:38.609865 cmdix-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2022-11-02 15:49:56.000000 cmdix-1.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-02 15:49:56.000000 cmdix-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-11-02 15:49:56.000000 cmdix-1.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-11-02 15:49:56.000000 cmdix-1.0.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-02 15:49:56.000000 cmdix-1.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-11-02 15:49:56.000000 cmdix-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-02 15:50:38.617865 cmdix-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-11-02 15:49:56.000000 cmdix-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:50:38.609865 cmdix-1.0.2/cmdix/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4795 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       53 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:50:38.617865 cmdix-1.0.2/cmdix/command/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/arch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/base64.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/basename.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/bunzip2.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/bzip2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/cal.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/cat.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/chmod.py
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/chown.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/chroot.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/clear.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/cp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3539 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/crond.py
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/diff.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/dirname.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/expand.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/gunzip.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/gzip.py
--rw-r--r--   0 runner    (1001) docker     (121)    11228 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/httpd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/id.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/init.py
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/kill.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/ln.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2145 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/ls.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/md5sum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/mkdir.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/mktemp.py
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/more.py
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/mount.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/mv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/nl.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/pwd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/rm.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/rmdir.py
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sendmail.py
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/seq.py
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sh.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sha1sum.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sha224sum.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sha256sum.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sha384sum.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sha512sum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/shred.py
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/shuf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sleep.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/smtpd.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/sort.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/tail.py
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/tar.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/tee.py
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/touch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4223 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/uname.py
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/uptime.py
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/uuidgen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/watch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/wc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/wget.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/whoami.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/yes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3151 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/command/zip.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/compressor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/hasher.py
--rw-r--r--   0 runner    (1001) docker     (121)     5228 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:50:38.617865 cmdix-1.0.2/cmdix/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_basename.py
--rw-r--r--   0 runner    (1001) docker     (121)     6960 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_cal.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_expand.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_login.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_md5sum.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_nl.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_onlyunix.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_pycoreutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_pycoreutils_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_tail.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_tar.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-11-02 15:49:56.000000 cmdix-1.0.2/cmdix/test/test_uuidgen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:50:38.609865 cmdix-1.0.2/cmdix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-02 15:50:38.000000 cmdix-1.0.2/cmdix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-11-02 15:50:38.000000 cmdix-1.0.2/cmdix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 15:50:38.000000 cmdix-1.0.2/cmdix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-11-02 15:50:38.000000 cmdix-1.0.2/cmdix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-11-02 15:50:38.000000 cmdix-1.0.2/cmdix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-02 15:50:38.000000 cmdix-1.0.2/cmdix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-02 15:49:56.000000 cmdix-1.0.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:50:38.617865 cmdix-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-11-02 15:49:56.000000 cmdix-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-02 15:49:56.000000 cmdix-1.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-11-02 15:49:56.000000 cmdix-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-02 15:49:56.000000 cmdix-1.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-02 15:49:56.000000 cmdix-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-11-02 15:49:56.000000 cmdix-1.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-11-02 15:50:38.617865 cmdix-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-11-02 15:49:56.000000 cmdix-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.640558 cmdix-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 20:48:09.000000 cmdix-2.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 20:48:09.000000 cmdix-2.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 20:48:09.000000 cmdix-2.0.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.612558 cmdix-2.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-21 20:48:09.000000 cmdix-2.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.612558 cmdix-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-21 20:48:09.000000 cmdix-2.0.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 20:48:09.000000 cmdix-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-21 20:48:09.000000 cmdix-2.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-21 20:48:09.000000 cmdix-2.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-21 20:48:09.000000 cmdix-2.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-21 20:48:09.000000 cmdix-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-21 20:48:33.640558 cmdix-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-21 20:48:09.000000 cmdix-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.616558 cmdix-2.0.1/cmdix/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4795 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.632558 cmdix-2.0.1/cmdix/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/bunzip2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/bzip2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/chown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/chroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/crond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/dirname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/gunzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/httpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/ln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/rmdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sendmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha1sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha224sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha256sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha384sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha512sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/shred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/shuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/touch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/uname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/uuidgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/wc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/wget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/yes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.616558 cmdix-2.0.1/cmdix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-21 20:48:09.000000 cmdix-2.0.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.636558 cmdix-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-21 20:48:09.000000 cmdix-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 20:48:09.000000 cmdix-2.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 20:48:09.000000 cmdix-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 20:48:09.000000 cmdix-2.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-21 20:48:09.000000 cmdix-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-21 20:48:09.000000 cmdix-2.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-21 20:48:33.640558 cmdix-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.640558 cmdix-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_onlyunix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_pycoreutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_pycoreutils_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_uuidgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-21 20:48:09.000000 cmdix-2.0.1/tox.ini
```

### Comparing `cmdix-1.0.2/.github/workflows/main.yml` & `cmdix-2.0.1/.github/workflows/main.yml`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 on: [push, pull_request]
 
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient.
-  FORCE_COLOR: -106
+  # to a non-empty value is sufficient. For tox, it must be one of
+  # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
+  # in common is "1".
+  FORCE_COLOR: 1
   # MyPy's color enforcement (must be a non-zero number)
   MYPY_FORCE_COLOR: -42
   # Recognized by the `py` package, dependency of `pytest` (must be "1")
   PY_COLORS: 1
   # Make tox-wrapped tools see color requests
   TOX_TESTENV_PASSENV: >-
     FORCE_COLOR
@@ -34,34 +36,59 @@
 
 jobs:
   test:
     strategy:
       matrix:
         python:
         - "3.7"
-        - "3.10"
         - "3.11"
+        - "3.12"
         # Workaround for actions/setup-python#508
         dev:
         - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
+        include:
+        # tests hang on Python < 3.9
+        #- python: "3.8"
+        #  platform: ubuntu-latest
+        - python: "3.9"
+          platform: ubuntu-latest
+        - python: "3.10"
+          platform: ubuntu-latest
         # disabled for #11
-        #include:
         #- python: pypy3.9
         #  platform: ubuntu-latest
-        # tests hang on Unix on Python < 3.9
+        
+        # tests hang on Python < 3.9
         exclude:
         - python: "3.7"
-          platform: ubuntu-latest
-        - python: "3.7"
           platform: macos-latest
+        - python: "3.7"
+          platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
+    continue-on-error: ${{ matrix.python == '3.12' }}
+    steps:
+      - uses: actions/checkout@v3
+      - name: Setup Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python }}${{ matrix.dev }}
+      - name: Install tox
+        run: |
+          python -m pip install tox
+      - name: Run tests
+        run: tox
+
+  docs:
+    runs-on: ubuntu-latest
+    env:
+      TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
@@ -71,14 +98,15 @@
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
+    - docs
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
```

### Comparing `cmdix-1.0.2/CHANGES.rst` & `cmdix-2.0.1/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v2.0.1
+======
+
+Fixed argument reference in ``cp``.
+
+v2.0.0
+======
+
+Removed smtpd command, incompatible with Python 3.12.
+
 v1.0.2
 ======
 
 #12: Fixed argument reference in ``mv``.
 
 v1.0.1
 ======
```

### Comparing `cmdix-1.0.2/Dockerfile` & `cmdix-2.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/LICENSE` & `cmdix-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/PKG-INFO` & `cmdix-2.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdix
-Version: 1.0.2
+Version: 2.0.1
 Summary: Unix commands in Pure Python
 Home-page: https://github.com/jaraco/cmdix
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,33 +15,30 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/cmdix.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/cmdix
 
 .. image:: https://img.shields.io/pypi/pyversions/cmdix.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/cmdix
 
 .. image:: https://github.com/jaraco/cmdix/workflows/tests/badge.svg
    :target: https://github.com/jaraco/cmdix/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
 ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 cmdix is a pure Python implementation of various standard UNIX commands,
 like 'ls', 'cp' and 'sleep'. It also contains a shell-like environment which
 will make Unix-users feel right at home on the Windows command-prompt.
 
 Forked from the abandoned `pycoreutils project
```

### Comparing `cmdix-1.0.2/README.rst` & `cmdix-2.0.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 .. image:: https://img.shields.io/pypi/v/cmdix.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/cmdix
 
 .. image:: https://img.shields.io/pypi/pyversions/cmdix.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/cmdix
 
 .. image:: https://github.com/jaraco/cmdix/workflows/tests/badge.svg
    :target: https://github.com/jaraco/cmdix/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
 ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 cmdix is a pure Python implementation of various standard UNIX commands,
 like 'ls', 'cp' and 'sleep'. It also contains a shell-like environment which
 will make Unix-users feel right at home on the Windows command-prompt.
 
 Forked from the abandoned `pycoreutils project
```

### Comparing `cmdix-1.0.2/cmdix/__init__.py` & `cmdix-2.0.1/cmdix/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/base64.py` & `cmdix-2.0.1/cmdix/command/base64.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/basename.py` & `cmdix-2.0.1/cmdix/command/basename.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/cal.py` & `cmdix-2.0.1/cmdix/command/cal.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/cat.py` & `cmdix-2.0.1/cmdix/command/cat.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/chmod.py` & `cmdix-2.0.1/cmdix/command/chmod.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/chown.py` & `cmdix-2.0.1/cmdix/command/chown.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/chroot.py` & `cmdix-2.0.1/cmdix/command/chroot.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/cp.py` & `cmdix-2.0.1/cmdix/command/cp.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 def func(args):
     # Set the _copy function
     if args.preserve:
         _copy = shutil.copy2
     else:
         _copy = shutil.copy
 
-    dstbase = args.pop()
+    (dest,) = args.DIRECTORY
     for src in args.SOURCE:
-        handle(_copy, args, dstbase, src)
+        handle(_copy, args, dest, src)
 
 
 def handle(_copy, args, dstbase, src):
     if args.recursive:
         # Create the base destination directory if it does not exists
         if not os.path.exists(dstbase):
             os.mkdir(dstbase)
```

### Comparing `cmdix-1.0.2/cmdix/command/crond.py` & `cmdix-2.0.1/cmdix/command/crond.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/diff.py` & `cmdix-2.0.1/cmdix/command/diff.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/dirname.py` & `cmdix-2.0.1/cmdix/command/dirname.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/env.py` & `cmdix-2.0.1/cmdix/command/env.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/expand.py` & `cmdix-2.0.1/cmdix/command/expand.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/httpd.py` & `cmdix-2.0.1/cmdix/command/httpd.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/id.py` & `cmdix-2.0.1/cmdix/command/id.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/init.py` & `cmdix-2.0.1/cmdix/command/init.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/kill.py` & `cmdix-2.0.1/cmdix/command/kill.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/ln.py` & `cmdix-2.0.1/cmdix/command/ln.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/logger.py` & `cmdix-2.0.1/cmdix/command/logger.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/login.py` & `cmdix-2.0.1/cmdix/command/login.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/ls.py` & `cmdix-2.0.1/cmdix/command/ls.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/mkdir.py` & `cmdix-2.0.1/cmdix/command/mkdir.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/mktemp.py` & `cmdix-2.0.1/cmdix/command/mktemp.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/more.py` & `cmdix-2.0.1/cmdix/command/more.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/mount.py` & `cmdix-2.0.1/cmdix/command/mount.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/mv.py` & `cmdix-2.0.1/cmdix/command/mv.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/nl.py` & `cmdix-2.0.1/cmdix/command/nl.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/pwd.py` & `cmdix-2.0.1/cmdix/command/pwd.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/rm.py` & `cmdix-2.0.1/cmdix/command/rm.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/rmdir.py` & `cmdix-2.0.1/cmdix/command/rmdir.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/sendmail.py` & `cmdix-2.0.1/cmdix/command/sendmail.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/seq.py` & `cmdix-2.0.1/cmdix/command/seq.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/sh.py` & `cmdix-2.0.1/cmdix/command/sh.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/shred.py` & `cmdix-2.0.1/cmdix/command/shred.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/shuf.py` & `cmdix-2.0.1/cmdix/command/shuf.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/sleep.py` & `cmdix-2.0.1/cmdix/command/sleep.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/sort.py` & `cmdix-2.0.1/cmdix/command/sort.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/tail.py` & `cmdix-2.0.1/cmdix/command/tail.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/tar.py` & `cmdix-2.0.1/cmdix/command/tar.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/tee.py` & `cmdix-2.0.1/cmdix/command/tee.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/touch.py` & `cmdix-2.0.1/cmdix/command/touch.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/uname.py` & `cmdix-2.0.1/cmdix/command/uname.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/uptime.py` & `cmdix-2.0.1/cmdix/command/uptime.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/uuidgen.py` & `cmdix-2.0.1/cmdix/command/uuidgen.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/watch.py` & `cmdix-2.0.1/cmdix/command/watch.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/wc.py` & `cmdix-2.0.1/cmdix/command/wc.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/wget.py` & `cmdix-2.0.1/cmdix/command/wget.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/command/zip.py` & `cmdix-2.0.1/cmdix/command/zip.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/compressor.py` & `cmdix-2.0.1/cmdix/compressor.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/exception.py` & `cmdix-2.0.1/cmdix/exception.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/hasher.py` & `cmdix-2.0.1/cmdix/hasher.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/lib.py` & `cmdix-2.0.1/cmdix/lib.py`

 * *Files identical despite different names*

### Comparing `cmdix-1.0.2/cmdix/test/__init__.py` & `cmdix-2.0.1/tests/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import filecmp
 import os
 import os.path
 import sys
 import io
+import pathlib
 
 import pytest
 
 import cmdix
 
 
 class BaseTestCase:
@@ -14,37 +15,30 @@
         assert filecmp.cmp(file1, file2)
 
     def createfile(self, filename, content=None, size=64 * 1024, fill='0'):
         """
         Create a temporary file containing `content`. If `content` is not
         defined, fill file with `size` times `fill`.
         """
-        with open(os.path.join(self.workdir, filename), 'w') as fd:
-            if content:
-                fd.write(content)
-            else:
-                fd.write(size * fill)
+        pathlib.Path(self.workdir, filename).write_text(content or fill * size)
 
     def createrandomfile(self, filename, size):
         """
         Create a temporary file containing random data
         """
-        with open(os.path.join(self.workdir, filename), 'w') as fd:
-            fd.write(os.urandom(size))
+        pathlib.Path(self.workdir, filename).write_text(os.urandom(size))
 
-    def runcommandline(self, commandline, stdin=None):
+    def runcommandline(self, commandline):
         """
         Run commandline as a subprocess.
 
         :param commandline: A string containing the commandline, i.e. 'ls -l X'
         :return:            A tuple containing the unicoded stdout and stderr
         """
-        with CapturedOutput() as output:
-            cmdix.runcommandline(commandline)
-        return output
+        cmdix.runcommandline(commandline)
 
     @pytest.fixture(autouse=True)
     def tmpdir_as_cwd(self, tmpdir):
         with tmpdir.as_cwd():
             self.workdir = str(tmpdir)
             yield tmpdir
 
@@ -86,28 +80,7 @@
         self.createfile('dir1/dir1-1/dir1-1-1/file1-1-1-1', size=55555)
         self.createfile('dir1/dir1-2/file1-2-1', size=66666)
         self.createfile('dir1/dir1-2/file1-2-2', size=77777)
         self.createfile('dir2/dir2-2/file2-2-1', size=88888)
 
     def setStdin(self, string):
         sys.stdin = io.StringIO(string)
-
-
-class CapturedOutput:
-    def __init__(self):
-        self.stdout = io.StringIO()
-        self.stderr = io.StringIO()
-
-    def __enter__(self):
-        sys.stdout = self.stdout
-        sys.stderr = self.stderr
-        return self
-
-    def __exit__(self, *args):
-        sys.stdout = sys.__stdout__
-        sys.stderr = sys.__stderr__
-
-    def __iter__(self):
-        return iter((self.stdout.getvalue(), self.stderr.getvalue()))
-
-    def __getitem__(self, item):
-        return tuple(self)[item]
```

### Comparing `cmdix-1.0.2/cmdix/test/test_base64.py` & `cmdix-2.0.1/tests/test_base64.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from . import BaseTestCase
 
 
 class TestCase(BaseTestCase):
-    def test_base64_decode(self):
+    def test_base64_decode(self, capsys):
         self.createfile('foo', content='SGF2ZSBhIGxvdCBvZiBmdW4uLi4K')
-        output = self.runcommandline('base64 -d foo')[0]
-        assert output == 'Have a lot of fun...\n'
+        self.runcommandline('base64 -d foo')
+        assert capsys.readouterr().out == 'Have a lot of fun...\n'
 
-    def test_base64_encode(self):
+    def test_base64_encode(self, capsys):
         self.createfile('foo', size=50)
-        output = self.runcommandline('base64 -w 30 foo')[0]
+        self.runcommandline('base64 -w 30 foo')
         expected = (
             'MDAwMDAwMDAwMDAwMDAwMDAwMDAwMD\n'
             'AwMDAwMDAwMDAwMDAwMDAwMDAwMDAw\n'
             'MDAwMDA=\n'
         )
-        assert output == expected
+        assert capsys.readouterr().out == expected
```

### Comparing `cmdix-1.0.2/cmdix/test/test_cal.py` & `cmdix-2.0.1/tests/test_cal.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from . import BaseTestCase
 
 
 class TestCase(BaseTestCase):
-    def test_cal_1arg(self):
+    def test_cal_1arg(self, capsys):
         expected = '''\
                                   123
 
       January                   February                   March
 Su Mo Tu We Th Fr Sa      Su Mo Tu We Th Fr Sa      Su Mo Tu We Th Fr Sa
                 1  2          1  2  3  4  5  6          1  2  3  4  5  6
  3  4  5  6  7  8  9       7  8  9 10 11 12 13       7  8  9 10 11 12 13
@@ -37,31 +37,31 @@
                 1  2          1  2  3  4  5  6                1  2  3  4
  3  4  5  6  7  8  9       7  8  9 10 11 12 13       5  6  7  8  9 10 11
 10 11 12 13 14 15 16      14 15 16 17 18 19 20      12 13 14 15 16 17 18
 17 18 19 20 21 22 23      21 22 23 24 25 26 27      19 20 21 22 23 24 25
 24 25 26 27 28 29 30      28 29 30                  26 27 28 29 30 31
 31
 '''
-        out = self.runcommandline('cal -S 123')[0]
-        assert out == expected
+        self.runcommandline('cal -S 123')
+        assert capsys.readouterr().out == expected
 
-    def test_cal_2args(self):
+    def test_cal_2args(self, capsys):
         expected = '''\
    December 4000
 Mo Tu We Th Fr Sa Su
              1  2  3
  4  5  6  7  8  9 10
 11 12 13 14 15 16 17
 18 19 20 21 22 23 24
 25 26 27 28 29 30 31
 '''
-        out = self.runcommandline('cal -M 12 4000')[0]
-        assert out == expected
+        self.runcommandline('cal -M 12 4000')
+        assert capsys.readouterr().out == expected
 
-    def test_cal_y(self):
+    def test_cal_y(self, capsys):
         expected = '''\
                                   2000
 
       January                   February                   March
 Su Mo Tu We Th Fr Sa      Su Mo Tu We Th Fr Sa      Su Mo Tu We Th Fr Sa
                    1             1  2  3  4  5                1  2  3  4
  2  3  4  5  6  7  8       6  7  8  9 10 11 12       5  6  7  8  9 10 11
@@ -129,9 +129,9 @@
           1  2  3  4                         1          1  2  3  4  5  6
  5  6  7  8  9 10 11       2  3  4  5  6  7  8       7  8  9 10 11 12 13
 12 13 14 15 16 17 18       9 10 11 12 13 14 15      14 15 16 17 18 19 20
 19 20 21 22 23 24 25      16 17 18 19 20 21 22      21 22 23 24 25 26 27
 26 27 28 29 30 31         23 24 25 26 27 28 29      28 29 30 31
                           30
 '''
-        out = self.runcommandline('cal -y 2000 3000')[0]
-        assert out == expected
+        self.runcommandline('cal -y 2000 3000')
+        assert capsys.readouterr().out == expected
```

### Comparing `cmdix-1.0.2/cmdix/test/test_login.py` & `cmdix-2.0.1/tests/test_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from . import BaseTestCase
-from ..command import login
+from cmdix.command import login
 
 
 class TestCase(BaseTestCase):
     def test_login_check_password(self):
         # tests disabled (don't work)
         return
         # Password is pycoreutils
```

### Comparing `cmdix-1.0.2/cmdix/test/test_ls.py` & `cmdix-2.0.1/tests/test_ls.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 import textwrap
 import pytest
 
 from . import BaseTestCase
 
 
 class TestCase(BaseTestCase):
-    def test_ls(self):
+    def test_ls(self, capsys):
         self.setup_filesystem()
-        out = self.runcommandline('ls')[0]
-        assert out == 'dir1\ndir2\nfile1\nfile2.txt\nfile3.empty\n'
+        self.runcommandline('ls')
+        assert capsys.readouterr().out == 'dir1\ndir2\nfile1\nfile2.txt\nfile3.empty\n'
 
     @pytest.mark.xfail("platform.system() == 'Windows'")
-    def test_ls_l(self):
+    def test_ls_l(self, capsys):
         os.mkdir('biz', mode=0o755)
         self.createfile('foo', size=100)
         self.createfile('bar', size=999999)
         os.chmod('bar', stat.S_IWUSR + stat.S_IRGRP + stat.S_IWOTH + stat.S_IXOTH)
         os.chmod('foo', 0o644)
 
         dirsize = os.stat('biz').st_size
         uid = os.getuid()
         gid = os.getgid()
         date = time.strftime('%Y-%m-%d %H:%m', time.localtime())
-        out = self.runcommandline('ls -l')[0]
+        self.runcommandline('ls -l')
         expected = (
             textwrap.dedent(
                 """
             --w-r---wx 1 {uid:<5} {gid:<5} 999999 {date} bar
             drwxr-xr-x 2 {uid:<5} {gid:<5} {dirsize:>6} {date} biz
             -rw-r--r-- 1 {uid:<5} {gid:<5}    100 {date} foo
             """
             )
             .lstrip()
             .format(**locals())
         )
-        assert out == expected
+        assert capsys.readouterr().out == expected
```

### Comparing `cmdix-1.0.2/cmdix/test/test_onlyunix.py` & `cmdix-2.0.1/tests/test_onlyunix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import platform
 
 import pytest
 
 import cmdix
-from .. import exception
+from cmdix import exception
 
 
 @pytest.fixture
 def pretend_windows(monkeypatch):
     monkeypatch.setattr(os, 'name', 'nt')
     monkeypatch.setattr(platform, 'system', lambda: 'Windows')
```

### Comparing `cmdix-1.0.2/cmdix/test/test_tar.py` & `cmdix-2.0.1/tests/test_tar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import tarfile
 
 import pytest
 
-from ..exception import StdErrException
+from cmdix.exception import StdErrException
 from . import BaseTestCase
 
 
 class TestCase(BaseTestCase):
     def test_notarfile(self):
         self.createfile('foo', size=100)
         with pytest.raises(StdErrException):
             self.runcommandline('tar -tf foo')
 
-    def test_tar(self):
+    def test_tar(self, capsys):
         self.setup_filesystem()
         good = [
             'dir1/',
             'dir1/dir1-1/',
             'dir1/dir1-1/dir1-1-1/',
             'dir1/dir1-1/dir1-1-1/file1-1-1-1',
             'dir1/dir1-1/dir1-1-2/',
@@ -32,27 +32,28 @@
             'dir2/dir2-2/',
             'dir2/dir2-2/file2-2-1',
             'file1',
         ]
 
         for archive in ('foo.tar', 'foo.tar.bz2', 'foo.tar.gz'):
             # Create an archive
-            res = self.runcommandline('tar -cf {0} dir1 dir2 file1'.format(archive))
-            assert res[0] == ''
+            self.runcommandline('tar -cf {0} dir1 dir2 file1'.format(archive))
+            assert capsys.readouterr().out == ''
             list_ = []
             for tarinfo in tarfile.open(archive):
                 name = tarinfo.name
                 if tarinfo.isdir():
                     name += '/'
                 list_.append(name)
             list_.sort()
             assert list_ == good
 
             # List the archive
-            x = self.runcommandline('tar -tf {0}'.format(archive))[0].split()
+            self.runcommandline('tar -tf {0}'.format(archive))
+            x = capsys.readouterr().out.split()
             x.sort()
             assert x == good
 
             # Extract the archive
             """
             d = os.getcwd()
             os.mkdir('extractdir')
```

### Comparing `cmdix-1.0.2/cmdix/test/test_uuidgen.py` & `cmdix-2.0.1/tests/test_uuidgen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from . import BaseTestCase
 
 
 class TestCase(BaseTestCase):
-    def test_uuidgen(self):
+    def test_uuidgen(self, capsys):
         # Make sure uuid1() generates UUIDs that are actually version 1.
-        for uuid in [self.runcommandline('uuidgen')[0] for i in range(10)]:
+        for iter in range(10):
+            self.runcommandline('uuidgen')
+            uuid = capsys.readouterr().out
             ell = uuid.rstrip().split('-')
 
             # Check uuid-length
             assert len(uuid) == 37
 
             # Check if uuid ends with \n
             assert uuid.endswith('\n')
```

### Comparing `cmdix-1.0.2/cmdix.egg-info/PKG-INFO` & `cmdix-2.0.1/cmdix.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdix
-Version: 1.0.2
+Version: 2.0.1
 Summary: Unix commands in Pure Python
 Home-page: https://github.com/jaraco/cmdix
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,33 +15,30 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/cmdix.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/cmdix
 
 .. image:: https://img.shields.io/pypi/pyversions/cmdix.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/cmdix
 
 .. image:: https://github.com/jaraco/cmdix/workflows/tests/badge.svg
    :target: https://github.com/jaraco/cmdix/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
 ..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 cmdix is a pure Python implementation of various standard UNIX commands,
 like 'ls', 'cp' and 'sleep'. It also contains a shell-like environment which
 will make Unix-users feel right at home on the Windows command-prompt.
 
 Forked from the abandoned `pycoreutils project
```

### Comparing `cmdix-1.0.2/cmdix.egg-info/SOURCES.txt` & `cmdix-2.0.1/cmdix.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -72,41 +72,40 @@
 cmdix/command/sha224sum.py
 cmdix/command/sha256sum.py
 cmdix/command/sha384sum.py
 cmdix/command/sha512sum.py
 cmdix/command/shred.py
 cmdix/command/shuf.py
 cmdix/command/sleep.py
-cmdix/command/smtpd.py
 cmdix/command/sort.py
 cmdix/command/tail.py
 cmdix/command/tar.py
 cmdix/command/tee.py
 cmdix/command/touch.py
 cmdix/command/uname.py
 cmdix/command/uptime.py
 cmdix/command/uuidgen.py
 cmdix/command/watch.py
 cmdix/command/wc.py
 cmdix/command/wget.py
 cmdix/command/whoami.py
 cmdix/command/yes.py
 cmdix/command/zip.py
-cmdix/test/__init__.py
-cmdix/test/test_base64.py
-cmdix/test/test_basename.py
-cmdix/test/test_cal.py
-cmdix/test/test_cat.py
-cmdix/test/test_expand.py
-cmdix/test/test_login.py
-cmdix/test/test_ls.py
-cmdix/test/test_md5sum.py
-cmdix/test/test_nl.py
-cmdix/test/test_onlyunix.py
-cmdix/test/test_pycoreutils.py
-cmdix/test/test_pycoreutils_lib.py
-cmdix/test/test_tail.py
-cmdix/test/test_tar.py
-cmdix/test/test_uuidgen.py
 docs/conf.py
 docs/history.rst
-docs/index.rst
+docs/index.rst
+tests/__init__.py
+tests/test_base64.py
+tests/test_basename.py
+tests/test_cal.py
+tests/test_cat.py
+tests/test_expand.py
+tests/test_login.py
+tests/test_ls.py
+tests/test_md5sum.py
+tests/test_nl.py
+tests/test_onlyunix.py
+tests/test_pycoreutils.py
+tests/test_pycoreutils_lib.py
+tests/test_tail.py
+tests/test_tar.py
+tests/test_uuidgen.py
```

### Comparing `cmdix-1.0.2/cmdix.egg-info/entry_points.txt` & `cmdix-2.0.1/cmdix.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 sha224sum = cmdix:run
 sha256sum = cmdix:run
 sha384sum = cmdix:run
 sha512sum = cmdix:run
 shred = cmdix:run
 shuf = cmdix:run
 sleep = cmdix:run
-smtpd = cmdix:run
 sort = cmdix:run
 tail = cmdix:run
 tar = cmdix:run
 tee = cmdix:run
 touch = cmdix:run
 uname = cmdix:run
 uptime = cmdix:run
```

### Comparing `cmdix-1.0.2/docs/conf.py` & `cmdix-2.0.1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
 extensions = [
     'sphinx.ext.autodoc',
     'jaraco.packaging.sphinx',
 ]
 
 master_doc = "index"
 html_theme = "furo"
```

### Comparing `cmdix-1.0.2/setup.cfg` & `cmdix-2.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,31 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
+	pytest-flake8; \
+	python_version < "3.12"
 	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
 	
 	types-backports
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
+	sphinx-lint
 
 [options.entry_points]
 console_scripts = 
 	gunzip = cmdix:run
 	gzip = cmdix:run
 	uname = cmdix:run
 	tail = cmdix:run
@@ -108,15 +110,14 @@
 	mount = cmdix:run
 	watch = cmdix:run
 	login = cmdix:run
 	shred = cmdix:run
 	md5sum = cmdix:run
 	init = cmdix:run
 	uptime = cmdix:run
-	smtpd = cmdix:run
 	expand = cmdix:run
 	seq = cmdix:run
 	wget = cmdix:run
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cmdix-1.0.2/tox.ini` & `cmdix-2.0.1/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 # https://github.com/jaraco/skeleton/issues/6
 tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
-	# workaround for pytest-dev/pytest#8076
-	pytest >= 6.2.1
+setenv =
+	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
-extras = testing
+extras =
+	testing
 
 [testenv:docs]
 extras =
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
+	python -m sphinxlint
 
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
```

