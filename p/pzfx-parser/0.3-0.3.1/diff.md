# Comparing `tmp/pzfx_parser-0.3.tar.gz` & `tmp/pzfx_parser-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzfx_parser-0.3.tar", last modified: Thu Mar  4 09:24:29 2021, max compression
+gzip compressed data, was "pzfx_parser-0.3.1.tar", last modified: Fri Apr 21 08:20:29 2023, max compression
```

## Comparing `pzfx_parser-0.3.tar` & `pzfx_parser-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,3 @@
--rw-r--r--   0        0        0     1083 2021-03-04 09:23:54.839129 pzfx_parser-0.3/LICENSE
--rw-r--r--   0        0        0      108 2021-03-04 09:23:54.839489 pzfx_parser-0.3/README.md
--rw-r--r--   0        0        0      324 2021-03-04 09:23:54.839805 pzfx_parser-0.3/pyproject.toml
--rw-r--r--   0        0        0     4096 2021-03-04 09:23:54.840301 pzfx_parser-0.3/pzfx_parser.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 pzfx_parser-0.3/setup.py
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pzfx_parser-0.3/PKG-INFO
+-rw-r--r--   0        0        0      324 2023-04-21 08:19:49.373544 pzfx_parser-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4334 2023-04-21 08:19:49.373762 pzfx_parser-0.3.1/pzfx_parser.py
+-rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 pzfx_parser-0.3.1/PKG-INFO
```

### Comparing `pzfx_parser-0.3/pzfx_parser.py` & `pzfx_parser-0.3.1/pzfx_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """Package to load and parse tables in a Prism pzfx file."""
 
 import xml.etree.ElementTree as ET
 import pandas as pd
 from itertools import count, chain, cycle
 import numpy as np
 
-__version__ = '0.3'
+__version__ = '0.3.1'
 
 
 class PrismFileLoadError(Exception):
     pass
 
 
 def _get_all_text(element):
     s = ''
     for c in element.iter():
         if c.text is not None:
             s += c.text
     return s
 
 
-def _subcolumn_to_numpy(subcolumn):
+def _subcolumn_to_numpy(subcolumn, ns):
     try:
         data = []
-        for d in subcolumn.findall('d'):
+        for d in subcolumn.findall('d', ns):
             if not (('Excluded' in d.attrib) and (d.attrib['Excluded'] == '1')):
                 if _get_all_text(d) == '':
                     data.append(None)
                 else:
                     data.append(float(_get_all_text(d)))
             else:
                 data.append(np.nan)
     except Exception as a:  # If data can't be read silently fail
         print("Couldn't Read a column in the file because: %s" % a)
         data = None
 
     return np.array(data)
 
 
-def _parse_xy_table(table):
+def _parse_xy_table(table, ns):
     xformat = table.attrib['XFormat']
     try:
         yformat = table.attrib['YFormat']
     except KeyError:
         yformat = None
     evformat = table.attrib['EVFormat']
 
@@ -55,60 +55,64 @@
         yslist = cycle(['Mean', 'Lower', 'Upper'])
         ysubcolumn_names = lambda: next(yslist)
     else:
         yscounter = count()
         ysubcolumn_names = lambda: str(next(yscounter))
 
     columns = {}
-    for xcolumn in chain(table.findall('XColumn'), table.findall('XAdvancedColumn')):
-        xcolumn_name = _get_all_text(xcolumn.find('Title'))
-        for subcolumn in xcolumn.findall('Subcolumn'):
+    for xcolumn in chain(table.findall('XColumn', ns), table.findall('XAdvancedColumn', ns)):
+        xcolumn_name = _get_all_text(xcolumn.find('Title', ns))
+        for subcolumn in xcolumn.findall('Subcolumn', ns):
             subcolumn_name = xcolumn_name + '_' + xsubcolumn_names()
-            columns[subcolumn_name] = _subcolumn_to_numpy(subcolumn)
-    for ycolumn in chain(table.findall('YColumn'), table.findall('YAdvancedColumn')):
-        ycolumn_name = _get_all_text(ycolumn.find('Title'))
-        for subcolumn in ycolumn.findall('Subcolumn'):
+            columns[subcolumn_name] = _subcolumn_to_numpy(subcolumn, ns)
+    for ycolumn in chain(table.findall('YColumn', ns), table.findall('YAdvancedColumn', ns)):
+        ycolumn_name = _get_all_text(ycolumn.find('Title', ns))
+        for subcolumn in ycolumn.findall('Subcolumn', ns):
             subcolumn_name = ycolumn_name + '_' + ysubcolumn_names()
-            columns[subcolumn_name] = _subcolumn_to_numpy(subcolumn)
+            columns[subcolumn_name] = _subcolumn_to_numpy(subcolumn, ns)
 
     maxlength = max([v.shape[0] if v.shape != () else 0 for v in columns.values()])
     for k, v in columns.items():
         if v.shape != ():
             if v.shape[0] < maxlength:
                 columns[k] = np.pad(v, (0, maxlength - v.shape[0]), mode='constant', constant_values=np.nan)
         else:
             columns[k] = np.pad(v, (0, maxlength - 0), mode='constant', constant_values=np.nan)
 
     return pd.DataFrame(columns)
 
 
-def _parse_table_to_dataframe(table):
+def _parse_table_to_dataframe(table, ns):
     # table_id = table.attrib['ID']
     tabletype = table.attrib['TableType']
 
     if tabletype == 'XY' or tabletype == 'TwoWay' or tabletype == 'OneWay':
-        df = _parse_xy_table(table)
+        df = _parse_xy_table(table, ns)
     else:
         raise PrismFileLoadError('Cannot parse %s tables for now!' % tabletype)
 
     return df
 
 
 def read_pzfx(filename):
     """Open and parse the Prism pzfx file given in `filename`.
     Returns a dictionary containing table names as keys and pandas DataFrames as values."""
     tree = ET.parse(filename)
     root = tree.getroot()
-    if root.tag != 'GraphPadPrismFile':
+    if root.tag == 'GraphPadPrismFile':
+        ns = None
+    elif root.tag == '{http://graphpad.com/prism/Prism.htm}GraphPadPrismFile':
+        ns = {'': 'http://graphpad.com/prism/Prism.htm'}
+    else:
         raise PrismFileLoadError('Not a Prism file!')
     if root.attrib['PrismXMLVersion'] != '5.00':
         raise PrismFileLoadError('Can only load Prism files with XML version 5.00!')
 
-    tables = {_get_all_text(table.find('Title')): _parse_table_to_dataframe(table)
-              for table in root.findall('Table')}
+    tables = {_get_all_text(table.find('Title', ns)): _parse_table_to_dataframe(table, ns)
+              for table in root.findall('Table', ns)}
 
     return tables
 
 
 def convert_pzfx_to_excel(tables, output_filename):
     """Takes a `tables` dict (from `read_pzfx`) and writes to an xlsx file, returns nothing."""
     with pd.ExcelWriter(output_filename, engine='openpyxl') as writer:
```

