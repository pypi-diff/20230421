# Comparing `tmp/canopy-viz-0.1.2.tar.gz` & `tmp/canopy_viz-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canopy-viz-0.1.2.tar", max compression
+gzip compressed data, was "canopy_viz-0.2.tar", max compression
```

## Comparing `canopy-viz-0.1.2.tar` & `canopy_viz-0.2.tar`

### file list

```diff
@@ -1,7 +1,3 @@
--rw-r--r--   0        0        0     1063 2021-12-31 19:23:03.330882 canopy-viz-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2021-12-31 20:07:17.857696 canopy-viz-0.1.2/canopy_viz/__init__.py
--rw-r--r--   0        0        0     4838 2021-12-31 20:07:17.857696 canopy-viz-0.1.2/canopy_viz/canopy.py
--rw-r--r--   0        0        0      693 2021-12-31 20:07:17.857696 canopy-viz-0.1.2/canopy_viz/cli.py
--rw-r--r--   0        0        0      481 2021-12-31 20:11:12.877208 canopy-viz-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      804 2021-12-31 20:11:20.389843 canopy-viz-0.1.2/setup.py
--rw-r--r--   0        0        0      700 2021-12-31 20:11:20.390070 canopy-viz-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      158 2023-04-20 21:56:55.680294 canopy_viz-0.2/README.md
+-rw-r--r--   0        0        0      359 2023-04-20 22:02:26.178617 canopy_viz-0.2/pyproject.toml
+-rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 canopy_viz-0.2/PKG-INFO
```

