# Comparing `tmp/edwh-0.6.6.tar.gz` & `tmp/edwh-0.7.0.tar.gz`

## Comparing `edwh-0.6.6.tar` & `edwh-0.7.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 edwh-0.6.6/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh-0.6.6/config.toml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.6.6/requirements-dev.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 edwh-0.6.6/requirements.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   193690 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57310 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    22378 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66395 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1141227 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134231 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113689 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    63269 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0    66858 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24418 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93277 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    31524 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96592 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48558 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82126 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182939 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30275 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53725 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   173191 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152168 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   248525 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444970 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73973 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    96993 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446284 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140957 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/edwh/__about__.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/edwh/__about__.meta.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/edwh/__init__.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/edwh/__init__.meta.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/edwh/cli.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/edwh/cli.meta.json
--rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    27009 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86512 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33595 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75549 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97916 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12954 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   382607 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/tests/__init__.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 edwh-0.6.6/.mypy_cache/3.10/tests/__init__.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh-0.6.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh-0.6.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh-0.6.6/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.6.6/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.6.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.6.6/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.6.6/src/edwh/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 edwh-0.6.6/src/edwh/cli.py
--rw-r--r--   0        0        0    23388 2020-02-02 00:00:00.000000 edwh-0.6.6/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.6.6/tests/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.6.6/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.6.6/LICENSE.txt
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 edwh-0.6.6/README.md
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 edwh-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 edwh-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 edwh-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh-0.7.0/config.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.7.0/requirements-dev.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 edwh-0.7.0/requirements.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   193690 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57310 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0    22378 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66395 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1141227 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134231 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113689 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    63269 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0    66858 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    24418 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93277 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    31524 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    96592 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48558 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82126 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   182939 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30275 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53725 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   173191 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152168 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0   248525 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444970 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73973 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    96993 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446284 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140957 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/edwh/__about__.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/edwh/__about__.meta.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/edwh/__init__.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/edwh/__init__.meta.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/edwh/cli.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/edwh/cli.meta.json
+-rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    27009 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86512 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33595 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75549 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97916 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12954 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   382607 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/tests/__init__.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 edwh-0.7.0/.mypy_cache/3.10/tests/__init__.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 edwh-0.7.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 edwh-0.7.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 edwh-0.7.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.7.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 edwh-0.7.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.7.0/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.7.0/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 edwh-0.7.0/src/edwh/cli.py
+-rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 edwh-0.7.0/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 edwh-0.7.0/README.md
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 edwh-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 edwh-0.7.0/PKG-INFO
```

### Comparing `edwh-0.6.6/CHANGELOG.md` & `edwh-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.7.0 (2023-04-21)
+### Feature
+* `apply_dotenv_vars_to_yaml_templates` added for traefik. ([`cc65abe`](https://github.com/educationwarehouse/edwh/commit/cc65abe300de0457f0ab464dcfa84cf2c3c981b5))
+
 ## v0.6.6 (2023-04-21)
 
 
 ## v0.6.5 (2023-04-20)
 ### Fix
 * Semver testing + demo plugin re-included ([`3e96848`](https://github.com/educationwarehouse/edwh/commit/3e968480ab67596a961a219bb3f7b900fbe7fa1f))
 * `exec_setup_in_other_task` has changed a little to search further up parent folders, until a `tasks.py` is found. ([`1675d8b`](https://github.com/educationwarehouse/edwh/commit/1675d8b0b83f238839f0d76013e09e412ea01598))
```

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_ast.data.json` & `edwh-0.7.0/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_ast.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_codecs.data.json` & `edwh-0.7.0/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_codecs.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_collections_abc.data.json` & `edwh-0.7.0/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_collections_abc.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_ctypes.data.json` & `edwh-0.7.0/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_ctypes.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/abc.data.json` & `edwh-0.7.0/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/abc.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/array.data.json` & `edwh-0.7.0/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/array.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/builtins.data.json` & `edwh-0.7.0/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/builtins.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/codecs.data.json` & `edwh-0.7.0/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/codecs.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/contextlib.data.json` & `edwh-0.7.0/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/contextlib.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/dataclasses.data.json` & `edwh-0.7.0/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/dataclasses.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/enum.data.json` & `edwh-0.7.0/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/enum.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/genericpath.data.json` & `edwh-0.7.0/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/genericpath.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/io.data.json` & `edwh-0.7.0/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/io.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/mmap.data.json` & `edwh-0.7.0/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/mmap.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/pathlib.data.json` & `edwh-0.7.0/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/pathlib.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/pickle.data.json` & `edwh-0.7.0/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/pickle.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/posixpath.data.json` & `edwh-0.7.0/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/posixpath.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/re.data.json` & `edwh-0.7.0/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/re.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/sre_compile.data.json` & `edwh-0.7.0/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/sre_compile.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/sre_constants.data.json` & `edwh-0.7.0/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/sre_constants.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/sre_parse.data.json` & `edwh-0.7.0/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/sre_parse.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/subprocess.data.json` & `edwh-0.7.0/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/subprocess.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/sys.data.json` & `edwh-0.7.0/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/sys.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/types.data.json` & `edwh-0.7.0/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/types.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/typing.data.json` & `edwh-0.7.0/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/typing.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/typing_extensions.data.json` & `edwh-0.7.0/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/typing_extensions.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_typeshed/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/collections/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/collections/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/collections/abc.data.json` & `edwh-0.7.0/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/collections/abc.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/ctypes/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/ctypes/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/edwh/__about__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/edwh/__about__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/edwh/__about__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/edwh/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/edwh/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/edwh/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/edwh/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/edwh/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/edwh/cli.data.json` & `edwh-0.7.0/.mypy_cache/3.10/edwh/cli.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/edwh/cli.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/edwh/cli.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/charset.data.json` & `edwh-0.7.0/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/charset.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/contentmanager.data.json` & `edwh-0.7.0/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/contentmanager.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/errors.data.json` & `edwh-0.7.0/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/errors.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/header.data.json` & `edwh-0.7.0/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/header.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/message.data.json` & `edwh-0.7.0/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/message.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/policy.data.json` & `edwh-0.7.0/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/email/policy.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/abc.data.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/abc.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/machinery.data.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/machinery.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/os/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/os/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/os/path.data.json` & `edwh-0.7.0/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/os/path.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/tests/__init__.data.json` & `edwh-0.7.0/.mypy_cache/3.10/tests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/.mypy_cache/3.10/tests/__init__.meta.json` & `edwh-0.7.0/.mypy_cache/3.10/tests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/src/edwh/cli.py` & `edwh-0.7.0/src/edwh/cli.py`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/src/edwh/tasks.py` & `edwh-0.7.0/src/edwh/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,62 @@
         allowed.add(" ")
 
     answer = input(prompt).lower().strip()
     answer += " "
 
     return answer[0] in allowed
 
+# used for treafik config
+def apply_dotenv_vars_to_yaml_templates(yaml_path: Path, dotenv_path:Path):
+    """Indention preserving templating of yaml files, uses dotenv_path for variables.
+
+    Pythong formatting is used with a dictionary of environment variables used from os environment variables
+    updated by the dotenv_path parsed .dotenv entries.
+    Templating is found using `# template:`
+    indention is saved, everything after the above indicator is python string formatted and written back.
+
+    Example:
+        |config:
+        |    email: some@one.com # template: {EMAIL}
+
+    assuming dotenv file contains:
+        |EMAIL=yep@thatsme.com
+
+    applying this function will result in:
+        |config:
+        |    email: yep@thatsme.com # template: {EMAIL}
+    """
+    env = os.environ.copy()
+    env.update(edwh.tasks.read_dotenv(dotenv_path))
+    needle = re.compile(r'# *template:')
+    env_variable_re = re.compile(r'\$[A-Z0-9]')
+    with yaml_path.open(mode='r+') as yaml_file:
+        source_lines = yaml_file.read().split('\n')
+        new_lines = []
+        for line in source_lines:
+            if len(needle.findall(line)):
+                # split on template definition:
+                old, template = needle.split(line)
+                template = template.strip()
+                # save the indention part, add an addition if no indention was found
+                indention = (re.findall(r'^[\s]*',old)+[''])[0]
+                if not old.lstrip().startswith('#'):
+                    # skip comment only lines
+                    new = template.format(**env)
+                    # reconstruct the line for the yaml file
+                    line = f'{indention}{new} # template: {template}'
+            new_lines.append(line)
+        # move filepointer to the start of the file
+        yaml_file.seek(0,0)
+        # write all lines and newlines to the file
+        yaml_file.write('\n'.join(new_lines))
+        # and remove any part that might be left over (when the new file is shorter than the old one)
+        yaml_file.truncate()
+
+
 
 @dataclass
 class TomlConfig:
     config: dict
     all_services: list[str]
     celeries: list[str]
     services_minimal: list[str]
```

### Comparing `edwh-0.6.6/LICENSE.txt` & `edwh-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/README.md` & `edwh-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/pyproject.toml` & `edwh-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh-0.6.6/PKG-INFO` & `edwh-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.6.6
+Version: 0.7.0
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

