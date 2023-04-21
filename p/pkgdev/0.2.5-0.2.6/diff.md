# Comparing `tmp/pkgdev-0.2.5.tar.gz` & `tmp/pkgdev-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgdev-0.2.5.tar", last modified: Sat Mar 11 17:35:13 2023, max compression
+gzip compressed data, was "pkgdev-0.2.6.tar", last modified: Fri Apr 21 07:47:49 2023, max compression
```

## Comparing `pkgdev-0.2.5.tar` & `pkgdev-0.2.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1493 2023-03-11 17:34:25.225924 pkgdev-0.2.5/LICENSE
--rw-r--r--   0        0        0      325 2023-03-11 17:34:25.225924 pkgdev-0.2.5/Makefile
--rw-r--r--   0        0        0     6593 2023-03-11 17:34:25.225924 pkgdev-0.2.5/NEWS.rst
--rw-r--r--   0        0        0     1442 2023-03-11 17:34:25.225924 pkgdev-0.2.5/README.rst
--rw-r--r--   0        0        0    23010 2023-03-11 17:35:07.298920 pkgdev-0.2.5/build/sphinx/man/pkgdev.1
--rw-r--r--   0        0        0     7107 2023-03-11 17:34:25.225924 pkgdev-0.2.5/data/share/bash-completion/completions/pkgdev
--rw-r--r--   0        0        0     4044 2023-03-11 17:34:25.225924 pkgdev-0.2.5/data/share/zsh/site-functions/_pkgdev
--rw-r--r--   0        0        0    10034 2023-03-11 17:34:25.225924 pkgdev-0.2.5/doc/conf.py
--rw-r--r--   0        0        0      380 2023-03-11 17:34:25.225924 pkgdev-0.2.5/doc/index.rst
--rw-r--r--   0        0        0     1953 2023-03-11 17:34:25.225924 pkgdev-0.2.5/doc/man/config.rst
--rw-r--r--   0        0        0      297 2023-03-11 17:34:25.225924 pkgdev-0.2.5/doc/man/pkgdev.rst
--rw-r--r--   0        0        0     1494 2023-03-11 17:34:25.225924 pkgdev-0.2.5/py_build.py
--rw-r--r--   0        0        0     1541 2023-03-11 17:34:25.225924 pkgdev-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       43 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/__init__.py
--rw-r--r--   0        0        0       71 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/__main__.py
--rw-r--r--   0        0        0       52 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/_vendor/__init__.py
--rw-r--r--   0        0        0    59090 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/_vendor/tabulate.py
--rw-r--r--   0        0        0       17 2023-03-11 17:35:13.035061 pkgdev-0.2.5/src/pkgdev/_verinfo.py
--rw-r--r--   0        0        0     5912 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/cli.py
--rw-r--r--   0        0        0     1243 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/const.py
--rw-r--r--   0        0        0      741 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/git.py
--rw-r--r--   0        0        0     5948 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/mangle.py
--rwxr-xr-x   0        0        0     1527 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/__init__.py
--rw-r--r--   0        0        0     1230 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/argparsers.py
--rw-r--r--   0        0        0      273 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev.py
--rw-r--r--   0        0        0    15135 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_bugs.py
--rw-r--r--   0        0        0    33449 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_commit.py
--rw-r--r--   0        0        0     4473 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_manifest.py
--rw-r--r--   0        0        0    10261 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_mask.py
--rw-r--r--   0        0        0     2445 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_push.py
--rw-r--r--   0        0        0     9314 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_showkw.py
--rw-r--r--   0        0        0    11822 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_tatt.py
--rw-r--r--   0        0        0        0 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/tatt/__init__.py
--rw-r--r--   0        0        0     4099 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/tatt/template.sh.jinja
--rw-r--r--   0        0        0        0 2023-03-11 17:34:25.225924 pkgdev-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      521 2023-03-11 17:34:25.225924 pkgdev-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/__init__.py
--rw-r--r--   0        0        0     3885 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_cli.py
--rw-r--r--   0        0        0     1888 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev.py
--rw-r--r--   0        0        0     3957 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_bugs.py
--rw-r--r--   0        0        0    45229 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_commit.py
--rw-r--r--   0        0        0     7585 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_manifest.py
--rw-r--r--   0        0        0    13461 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_mask.py
--rw-r--r--   0        0        0     4939 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_push.py
--rw-r--r--   0        0        0     8963 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_showkw.py
--rw-r--r--   0        0        0      908 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/test_git.py
--rw-r--r--   0        0        0     3454 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/test_mangle.py
--rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 pkgdev-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1493 2023-04-21 07:46:41.650615 pkgdev-0.2.6/LICENSE
+-rw-r--r--   0        0        0      325 2023-04-21 07:46:41.650615 pkgdev-0.2.6/Makefile
+-rw-r--r--   0        0        0     6593 2023-04-21 07:46:41.650615 pkgdev-0.2.6/NEWS.rst
+-rw-r--r--   0        0        0     1442 2023-04-21 07:46:41.650615 pkgdev-0.2.6/README.rst
+-rw-r--r--   0        0        0    23009 2023-04-21 07:47:41.538933 pkgdev-0.2.6/build/sphinx/man/pkgdev.1
+-rw-r--r--   0        0        0     7107 2023-04-21 07:46:41.650615 pkgdev-0.2.6/data/share/bash-completion/completions/pkgdev
+-rw-r--r--   0        0        0     4044 2023-04-21 07:46:41.650615 pkgdev-0.2.6/data/share/zsh/site-functions/_pkgdev
+-rw-r--r--   0        0        0    10034 2023-04-21 07:46:41.650615 pkgdev-0.2.6/doc/conf.py
+-rw-r--r--   0        0        0      380 2023-04-21 07:46:41.650615 pkgdev-0.2.6/doc/index.rst
+-rw-r--r--   0        0        0     1953 2023-04-21 07:46:41.650615 pkgdev-0.2.6/doc/man/config.rst
+-rw-r--r--   0        0        0      297 2023-04-21 07:46:41.650615 pkgdev-0.2.6/doc/man/pkgdev.rst
+-rw-r--r--   0        0        0     1494 2023-04-21 07:46:41.650615 pkgdev-0.2.6/py_build.py
+-rw-r--r--   0        0        0     1541 2023-04-21 07:46:41.650615 pkgdev-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-04-21 07:46:41.650615 pkgdev-0.2.6/src/pkgdev/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-21 07:46:41.650615 pkgdev-0.2.6/src/pkgdev/__main__.py
+-rw-r--r--   0        0        0       52 2023-04-21 07:46:41.650615 pkgdev-0.2.6/src/pkgdev/_vendor/__init__.py
+-rw-r--r--   0        0        0    59090 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/_vendor/tabulate.py
+-rw-r--r--   0        0        0       17 2023-04-21 07:47:49.626973 pkgdev-0.2.6/src/pkgdev/_verinfo.py
+-rw-r--r--   0        0        0     5912 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/cli.py
+-rw-r--r--   0        0        0     1243 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/const.py
+-rw-r--r--   0        0        0      741 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/git.py
+-rw-r--r--   0        0        0     5948 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/mangle.py
+-rwxr-xr-x   0        0        0     1527 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/__init__.py
+-rw-r--r--   0        0        0     1230 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/argparsers.py
+-rw-r--r--   0        0        0      273 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/pkgdev.py
+-rw-r--r--   0        0        0    17375 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_bugs.py
+-rw-r--r--   0        0        0    33449 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_commit.py
+-rw-r--r--   0        0        0     4473 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_manifest.py
+-rw-r--r--   0        0        0    10261 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_mask.py
+-rw-r--r--   0        0        0     2445 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_push.py
+-rw-r--r--   0        0        0     9314 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_showkw.py
+-rw-r--r--   0        0        0    11822 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_tatt.py
+-rw-r--r--   0        0        0        0 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/tatt/__init__.py
+-rw-r--r--   0        0        0     4099 2023-04-21 07:46:41.654615 pkgdev-0.2.6/src/pkgdev/tatt/template.sh.jinja
+-rw-r--r--   0        0        0        0 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     3885 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/scripts/test_cli.py
+-rw-r--r--   0        0        0     1888 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/scripts/test_pkgdev.py
+-rw-r--r--   0        0        0     3957 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/scripts/test_pkgdev_bugs.py
+-rw-r--r--   0        0        0    45229 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/scripts/test_pkgdev_commit.py
+-rw-r--r--   0        0        0     7585 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/scripts/test_pkgdev_manifest.py
+-rw-r--r--   0        0        0    13461 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/scripts/test_pkgdev_mask.py
+-rw-r--r--   0        0        0     4939 2023-04-21 07:46:41.654615 pkgdev-0.2.6/tests/scripts/test_pkgdev_push.py
+-rw-r--r--   0        0        0     8963 2023-04-21 07:46:41.658615 pkgdev-0.2.6/tests/scripts/test_pkgdev_showkw.py
+-rw-r--r--   0        0        0      908 2023-04-21 07:46:41.658615 pkgdev-0.2.6/tests/test_git.py
+-rw-r--r--   0        0        0     3454 2023-04-21 07:46:41.658615 pkgdev-0.2.6/tests/test_mangle.py
+-rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 pkgdev-0.2.6/PKG-INFO
```

### Comparing `pkgdev-0.2.5/LICENSE` & `pkgdev-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/NEWS.rst` & `pkgdev-0.2.6/NEWS.rst`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/README.rst` & `pkgdev-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/build/sphinx/man/pkgdev.1` & `pkgdev-0.2.6/build/sphinx/man/pkgdev.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PKGDEV" "1" "Mar 11, 2023" "0.2.5" "pkgdev"
+.TH "PKGDEV" "1" "Apr 21, 2023" "0.2.6" "pkgdev"
 .SH NAME
 pkgdev \- Wrapper for running commandline scripts.
 .SH SYNOPSIS
 .sp
 pkgdev [\-h] [\-\-version] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] {bugs,commit,manifest,mask,push,showkw,tatt} ...
 .SH BASE OPTIONS
 .INDENT 0.0
@@ -51,15 +51,15 @@
 .B \fB\-v, \-\-verbose\fP
 show verbose output
 .TP
 .B \fB\-\-color BOOLEAN\fP
 enable/disable color support
 .UNINDENT
 .SH SUBCOMMANDS
-.SS pkgdev bugs \- Automatic bugs filler
+.SS pkgdev bugs \- Automatic bugs filer
 .SS Synopsis
 .sp
 pkgdev bugs [\-\-config CONFIG_FILE] [\-\-domain DOMAIN] [\-h] [\-\-debug] [\-\-color BOOLEAN] [\-\-api\-key KEY] [\-\-dot DOT] [\-\-auto\-cc\-arches AUTO_CC_ARCHES] [\-s | \-k] [\-a ARCH] [\-p PROFILE] target [target ...]
 .SS Positional Arguments
 .INDENT 0.0
 .TP
 .B \fBtarget\fP
```

### Comparing `pkgdev-0.2.5/data/share/bash-completion/completions/pkgdev` & `pkgdev-0.2.6/data/share/bash-completion/completions/pkgdev`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/data/share/zsh/site-functions/_pkgdev` & `pkgdev-0.2.6/data/share/zsh/site-functions/_pkgdev`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/doc/conf.py` & `pkgdev-0.2.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/doc/man/config.rst` & `pkgdev-0.2.6/doc/man/config.rst`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/py_build.py` & `pkgdev-0.2.6/py_build.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/pyproject.toml` & `pkgdev-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/_vendor/tabulate.py` & `pkgdev-0.2.6/src/pkgdev/_vendor/tabulate.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/cli.py` & `pkgdev-0.2.6/src/pkgdev/cli.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/const.py` & `pkgdev-0.2.6/src/pkgdev/const.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/git.py` & `pkgdev-0.2.6/src/pkgdev/git.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/mangle.py` & `pkgdev-0.2.6/src/pkgdev/mangle.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/__init__.py` & `pkgdev-0.2.6/src/pkgdev/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/argparsers.py` & `pkgdev-0.2.6/src/pkgdev/scripts/argparsers.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_bugs.py` & `pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_bugs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-"""Automatic bugs filler"""
+"""Automatic bugs filer"""
 
 import json
 import urllib.request as urllib
 from collections import defaultdict
 from functools import partial
 from itertools import chain
+from urllib.parse import urlencode
 
 from pkgcheck import const as pkgcheck_const
 from pkgcheck.addons import ArchesAddon, init_addon
 from pkgcheck.addons.profiles import ProfileAddon
 from pkgcheck.checks import visibility
 from pkgcheck.scripts import argparse_actions
 from pkgcore.ebuild.atom import atom
 from pkgcore.ebuild.ebuild_src import package
+from pkgcore.ebuild.errors import MalformedAtom
 from pkgcore.ebuild.misc import sort_keywords
 from pkgcore.repository import multiplex
 from pkgcore.restrictions import boolean, packages, values
 from pkgcore.test.misc import FakePkg
 from pkgcore.util import commandline
 from snakeoil.cli import arghparse
 from snakeoil.cli.input import userquery
@@ -123,14 +125,24 @@
 
     # limit stablereq to whatever is ~arch right now
     match_keywords.intersection_update(x.lstrip("~") for x in pkg.keywords if x[0] == "~")
 
     return frozenset({x for x in match_keywords if "-" not in x})
 
 
+def parse_atom(pkg: str):
+    try:
+        return atom(pkg)
+    except MalformedAtom as exc:
+        try:
+            return atom(f"={pkg}")
+        except MalformedAtom:
+            raise exc
+
+
 class GraphNode:
     __slots__ = ("pkgs", "edges", "bugno")
 
     def __init__(self, pkgs: tuple[tuple[package, set[str]], ...], bugno=None):
         self.pkgs = pkgs
         self.edges: set[GraphNode] = set()
         self.bugno = bugno
@@ -263,15 +275,15 @@
 
         for pkgname, problems in issues.items():
             pkgset: list[package] = self.options.repo.match(atom(pkgname))
             try:
                 combined = boolean.AndRestriction(*set().union(*problems.values()))
                 match = self.find_best_match(combined, pkgset)
                 yield match, set(problems.keys())
-            except ValueError:
+            except (ValueError, IndexError):
                 results: dict[package, set[str]] = defaultdict(set)
                 for keyword, deps in problems.items():
                     match = self.find_best_match(deps, pkgset)
                     results[match].add(keyword)
                 yield from results.items()
 
     def build_full_graph(self, targets: list[package]):
@@ -306,34 +318,39 @@
 
     def output_dot(self, dot_file):
         with open(dot_file, "w") as dot:
             dot.write("digraph {\n")
             dot.write("\trankdir=LR;\n")
             for node in self.nodes:
                 node_text = "\\n".join(node.lines())
+                if node.bugno is not None:
+                    node_text += f"\\nbug #{node.bugno}"
                 dot.write(f'\t{node.dot_edge}[label="{node_text}"];\n')
                 for other in node.edges:
                     dot.write(f"\t{node.dot_edge} -> {other.dot_edge};\n")
             dot.write("}\n")
             dot.close()
 
     def merge_nodes(self, nodes: tuple[GraphNode, ...]) -> GraphNode:
         self.nodes.difference_update(nodes)
+        is_start = bool(self.starting_nodes.intersection(nodes))
         self.starting_nodes.difference_update(nodes)
         new_node = GraphNode(list(chain.from_iterable(n.pkgs for n in nodes)))
 
         for node in nodes:
             new_node.edges.update(node.edges.difference(nodes))
 
         for node in self.nodes:
             if node.edges.intersection(nodes):
                 node.edges.difference_update(nodes)
                 node.edges.add(new_node)
 
         self.nodes.add(new_node)
+        if is_start:
+            self.starting_nodes.add(new_node)
         return new_node
 
     @staticmethod
     def _find_cycles(nodes: tuple[GraphNode, ...], stack: list[GraphNode]) -> tuple[GraphNode, ...]:
         node = stack[-1]
         for edge in node.edges:
             if edge in stack:
@@ -341,25 +358,23 @@
             stack.append(edge)
             if cycle := DependencyGraph._find_cycles(nodes, stack):
                 return cycle
             stack.pop()
         return ()
 
     def merge_cycles(self):
-        new_starts = set()
-        while self.starting_nodes:
-            starting_node = self.starting_nodes.pop()
+        start_nodes = set(self.starting_nodes)
+        while start_nodes:
+            starting_node = start_nodes.pop()
             assert starting_node in self.nodes
             while cycle := self._find_cycles(tuple(self.nodes), [starting_node]):
-                print("Found cycle:", " -> ".join(str(n) for n in cycle))
+                self.out.write("Found cycle: ", " -> ".join(str(n) for n in cycle))
                 new_node = self.merge_nodes(cycle)
                 if starting_node not in self.nodes:
                     starting_node = new_node
-            new_starts.add(starting_node)
-        self.starting_nodes.update(new_starts)
 
     def merge_new_keywords_children(self):
         repo = self.options.search_repo
         found_someone = True
         while found_someone:
             reverse_edges: dict[GraphNode, set[GraphNode]] = defaultdict(set)
             for node in self.nodes:
@@ -375,19 +390,59 @@
                         for pkg in node.pkgs
                         for pkgver in repo.match(pkg[0].unversioned_atom)
                     )
                 )
                 if existing_keywords & frozenset().union(*(pkg[1] for pkg in node.pkgs)):
                     continue  # not fully new keywords
                 orig = next(iter(origs))
-                print(f"Merging {node} into {orig}")
+                self.out.write(f"Merging {node} into {orig}")
                 self.merge_nodes((orig, node))
                 found_someone = True
                 break
 
+    def scan_existing_bugs(self, api_key: str):
+        params = urlencode(
+            {
+                "Bugzilla_api_key": api_key,
+                "include_fields": "id,cf_stabilisation_atoms",
+                "component": "Stabilization",
+                "resolution": "---",
+                "f1": "cf_stabilisation_atoms",
+                "o1": "anywords",
+                "v1": {pkg[0].unversioned_atom for node in self.nodes for pkg in node.pkgs},
+            },
+            doseq=True,
+        )
+        request = urllib.Request(
+            url="https://bugs.gentoo.org/rest/bug?" + params,
+            method="GET",
+            headers={
+                "Content-Type": "application/json",
+                "Accept": "application/json",
+            },
+        )
+        with urllib.urlopen(request, timeout=30) as response:
+            reply = json.loads(response.read().decode("utf-8"))
+        for bug in reply["bugs"]:
+            bug_atoms = (
+                parse_atom(line.split(" ", 1)[0]).unversioned_atom
+                for line in map(str.strip, bug["cf_stabilisation_atoms"].splitlines())
+                if line
+            )
+            bug_match = boolean.OrRestriction(*bug_atoms)
+            for node in self.nodes:
+                if node.bugno is None and all(bug_match.match(pkg[0]) for pkg in node.pkgs):
+                    node.bugno = bug["id"]
+                    self.out.write(
+                        self.out.fg("yellow"),
+                        f"Found https://bugs.gentoo.org/{node.bugno} for node {node}",
+                        self.out.reset,
+                    )
+                    break
+
     def file_bugs(self, api_key: str, auto_cc_arches: frozenset[str]):
         def observe(node: GraphNode):
             self.out.write(
                 f"https://bugs.gentoo.org/{node.bugno} ",
                 " | ".join(node.lines()),
                 " depends on bugs ",
                 {dep.bugno for dep in node.edges},
@@ -406,14 +461,17 @@
     d.build_full_graph(targets)
     d.merge_cycles()
     d.merge_new_keywords_children()
 
     for node in d.nodes:
         node.cleanup_keywords(search_repo)
 
+    if userquery("Check for open bugs matching current graph?", out, err, default_answer=False):
+        d.scan_existing_bugs(options.api_key)
+
     if options.dot is not None:
         d.output_dot(options.dot)
         out.write(out.fg("green"), f"Dot file written to {options.dot}", out.reset)
 
     if not userquery(
         f"Continue and create {len(d.nodes)} stablereq bugs?", out, err, default_answer=False
     ):
```

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_commit.py` & `pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_commit.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_manifest.py` & `pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_manifest.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_mask.py` & `pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_mask.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_push.py` & `pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_push.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_showkw.py` & `pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_showkw.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_tatt.py` & `pkgdev-0.2.6/src/pkgdev/scripts/pkgdev_tatt.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/src/pkgdev/tatt/template.sh.jinja` & `pkgdev-0.2.6/src/pkgdev/tatt/template.sh.jinja`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/conftest.py` & `pkgdev-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/scripts/test_cli.py` & `pkgdev-0.2.6/tests/scripts/test_cli.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/scripts/test_pkgdev.py` & `pkgdev-0.2.6/tests/scripts/test_pkgdev.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/scripts/test_pkgdev_bugs.py` & `pkgdev-0.2.6/tests/scripts/test_pkgdev_bugs.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/scripts/test_pkgdev_commit.py` & `pkgdev-0.2.6/tests/scripts/test_pkgdev_commit.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/scripts/test_pkgdev_manifest.py` & `pkgdev-0.2.6/tests/scripts/test_pkgdev_manifest.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/scripts/test_pkgdev_mask.py` & `pkgdev-0.2.6/tests/scripts/test_pkgdev_mask.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/scripts/test_pkgdev_push.py` & `pkgdev-0.2.6/tests/scripts/test_pkgdev_push.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/scripts/test_pkgdev_showkw.py` & `pkgdev-0.2.6/tests/scripts/test_pkgdev_showkw.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/test_git.py` & `pkgdev-0.2.6/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/tests/test_mangle.py` & `pkgdev-0.2.6/tests/test_mangle.py`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.5/PKG-INFO` & `pkgdev-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgdev
-Version: 0.2.5
+Version: 0.2.6
 Summary: collection of tools for Gentoo development
 Author-email: Tim Harder <radhermit@gmail.com>, Arthur Zamarin <arthurzam@gentoo.org>
 Maintainer-email: Arthur Zamarin <arthurzam@gentoo.org>
 Requires-Python: ~=3.9
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
```

