# Comparing `tmp/excel-sql-engine-1.4.tar.gz` & `tmp/excel-sql-engine-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-sql-engine-1.4.tar", last modified: Thu Apr 20 16:13:29 2023, max compression
+gzip compressed data, was "excel-sql-engine-1.6.tar", last modified: Fri Apr 21 18:46:59 2023, max compression
```

## Comparing `excel-sql-engine-1.4.tar` & `excel-sql-engine-1.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 16:13:29.690418 excel-sql-engine-1.4/
--rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 excel-sql-engine-1.4/LICENCE
--rw-rw-rw-   0        0        0     8280 2023-04-20 16:13:29.688419 excel-sql-engine-1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 16:13:29.631008 excel-sql-engine-1.4/PyxlSql/
--rw-rw-rw-   0        0        0      563 2023-03-13 18:23:44.000000 excel-sql-engine-1.4/PyxlSql/__init__.py
--rw-rw-rw-   0        0        0     7211 2023-04-16 21:00:33.000000 excel-sql-engine-1.4/PyxlSql/pyxlAbstracts.py
--rw-rw-rw-   0        0        0    15468 2023-04-18 13:41:16.000000 excel-sql-engine-1.4/PyxlSql/pyxlArgs.py
--rw-rw-rw-   0        0        0    37187 2023-04-18 13:08:46.000000 excel-sql-engine-1.4/PyxlSql/pyxlEngine.py
--rw-rw-rw-   0        0        0     2934 2023-03-13 18:23:44.000000 excel-sql-engine-1.4/PyxlSql/pyxlErrors.py
--rw-rw-rw-   0        0        0    26449 2023-04-18 13:02:23.000000 excel-sql-engine-1.4/PyxlSql/pyxlGrammar.py
--rw-rw-rw-   0        0        0     9167 2023-04-18 13:57:14.000000 excel-sql-engine-1.4/PyxlSql/pyxlPivot.py
--rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 excel-sql-engine-1.4/PyxlSql/pyxlResults.py
--rw-rw-rw-   0        0        0    17853 2023-04-18 13:44:08.000000 excel-sql-engine-1.4/PyxlSql/pyxlSheets.py
--rw-rw-rw-   0        0        0    14058 2023-04-18 13:52:15.000000 excel-sql-engine-1.4/PyxlSql/pyxlSql.py
--rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 excel-sql-engine-1.4/PyxlSql/pyxlStages.py
--rw-rw-rw-   0        0        0    13451 2023-04-18 13:01:32.000000 excel-sql-engine-1.4/PyxlSql/pyxlWorkbook.py
--rw-rw-rw-   0        0        0     7581 2023-04-20 14:22:23.000000 excel-sql-engine-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 16:13:29.675305 excel-sql-engine-1.4/excel_sql_engine.egg-info/
--rw-rw-rw-   0        0        0     8280 2023-04-20 16:13:29.000000 excel-sql-engine-1.4/excel_sql_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-04-20 16:13:29.000000 excel-sql-engine-1.4/excel_sql_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 16:13:29.000000 excel-sql-engine-1.4/excel_sql_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2023-04-20 15:20:18.000000 excel-sql-engine-1.4/excel_sql_engine.egg-info/setup.cfg
--rw-rw-rw-   0        0        0        8 2023-04-20 16:13:29.000000 excel-sql-engine-1.4/excel_sql_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 16:13:29.690418 excel-sql-engine-1.4/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-04-20 15:27:59.000000 excel-sql-engine-1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:13:29.683555 excel-sql-engine-1.4/tests/
--rw-rw-rw-   0        0        0     7703 2023-04-17 15:39:30.000000 excel-sql-engine-1.4/tests/test_Northwind.py
--rw-rw-rw-   0        0        0     6381 2023-04-18 14:00:43.000000 excel-sql-engine-1.4/tests/test_tooling.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:46:59.830321 excel-sql-engine-1.6/
+-rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 excel-sql-engine-1.6/LICENCE
+-rw-rw-rw-   0        0        0     8284 2023-04-21 18:46:59.826719 excel-sql-engine-1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 18:46:59.764020 excel-sql-engine-1.6/PyxlSql/
+-rw-rw-rw-   0        0        0      563 2023-03-13 18:23:44.000000 excel-sql-engine-1.6/PyxlSql/__init__.py
+-rw-rw-rw-   0        0        0     7211 2023-04-16 21:00:33.000000 excel-sql-engine-1.6/PyxlSql/pyxlAbstracts.py
+-rw-rw-rw-   0        0        0    15468 2023-04-18 13:41:16.000000 excel-sql-engine-1.6/PyxlSql/pyxlArgs.py
+-rw-rw-rw-   0        0        0    37421 2023-04-21 17:35:39.000000 excel-sql-engine-1.6/PyxlSql/pyxlEngine.py
+-rw-rw-rw-   0        0        0     2934 2023-03-13 18:23:44.000000 excel-sql-engine-1.6/PyxlSql/pyxlErrors.py
+-rw-rw-rw-   0        0        0    26449 2023-04-18 13:02:23.000000 excel-sql-engine-1.6/PyxlSql/pyxlGrammar.py
+-rw-rw-rw-   0        0        0     9159 2023-04-21 18:05:53.000000 excel-sql-engine-1.6/PyxlSql/pyxlPivot.py
+-rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 excel-sql-engine-1.6/PyxlSql/pyxlResults.py
+-rw-rw-rw-   0        0        0    14165 2023-04-21 18:17:44.000000 excel-sql-engine-1.6/PyxlSql/pyxlSheets.py
+-rw-rw-rw-   0        0        0    14097 2023-04-20 17:00:21.000000 excel-sql-engine-1.6/PyxlSql/pyxlSql.py
+-rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 excel-sql-engine-1.6/PyxlSql/pyxlStages.py
+-rw-rw-rw-   0        0        0    18944 2023-04-21 15:56:11.000000 excel-sql-engine-1.6/PyxlSql/pyxlWorkbook.py
+-rw-rw-rw-   0        0        0     7585 2023-04-21 09:26:14.000000 excel-sql-engine-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 18:46:59.814466 excel-sql-engine-1.6/excel_sql_engine.egg-info/
+-rw-rw-rw-   0        0        0     8284 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      196 2023-04-20 15:20:18.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/setup.cfg
+-rw-rw-rw-   0        0        0        8 2023-04-21 18:46:59.000000 excel-sql-engine-1.6/excel_sql_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:46:59.830321 excel-sql-engine-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2023-04-21 18:38:21.000000 excel-sql-engine-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:46:59.822717 excel-sql-engine-1.6/tests/
+-rw-rw-rw-   0        0        0     7703 2023-04-17 15:39:30.000000 excel-sql-engine-1.6/tests/test_Northwind.py
+-rw-rw-rw-   0        0        0     6381 2023-04-18 14:00:43.000000 excel-sql-engine-1.6/tests/test_tooling.py
```

### Comparing `excel-sql-engine-1.4/LICENCE` & `excel-sql-engine-1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/PKG-INFO` & `excel-sql-engine-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-sql-engine
-Version: 1.4
+Version: 1.6
 Summary: A tiny SQL engine for Excel files, based on Openpyxl
 Home-page: https://gitlab.com/fabien.battini/pyxlsql
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: excel sql
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -180,10 +180,10 @@
 Documentation is built using Sphinx https://www.sphinx-doc.org/
 
 Documentation is generated in https://fabien_battini.gitlab.io/pyxlsql/html/
 This process is achieved automatically through gitlab CI pipelines.
 
 gitlab repository: https://gitlab.com/fabien_battini/pyxlsql
 
-pypi: https://pypi.org/project/open-pyxl-sql
+pypi: https://pypi.org/project/excel-sql-engine/
 
 LinkedIN: https://www.linkedin.com/in/fabien-battini-supelec/
```

### Comparing `excel-sql-engine-1.4/PyxlSql/__init__.py` & `excel-sql-engine-1.6/PyxlSql/__init__.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlAbstracts.py` & `excel-sql-engine-1.6/PyxlSql/pyxlAbstracts.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlArgs.py` & `excel-sql-engine-1.6/PyxlSql/pyxlArgs.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlEngine.py` & `excel-sql-engine-1.6/PyxlSql/pyxlEngine.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,20 @@
         self.pivot = None
         # dst_sheet_arg.verify_fields(not_in_src=True)  # useless: never a field
         # src_arg.verify_fields(not_in_dst=True)  # useless: never a field
 
     def execute(self):
         print(f"EXECUTE PIVOT '{self.dst_sheet_arg.get_sheet_name()}' FROM '{self.src_sheet_arg.get_sheet_name()}'")
         assert self.dst_sheet_arg is not None, "INTERNAL: PivotCmd::execute "
-        self.pivot = Pivot(self.dst_sheet_arg.get_sheet(),self.src_sheet_arg.get_sheet() , use_formula=True)
+        dst_sheet = self.dst_sheet_arg.get_sheet()
+        src_sheet = self.src_sheet_arg.get_sheet()
+        colors_column = dst_sheet.columns[2]
+        dst_sheet.column_styles[colors_column]=None # otherwise, the color of the 1st rox is copied due to automatic style
+
+        self.pivot = Pivot(dst_sheet,src_sheet , use_formula=True)
 
 
 
 # Example: SAVE OpenTV.xlsx
 class SaveCmd(Cmd):
     name = 'SAVE'
     help = "Saves the workbook in 'Filename'"
```

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlErrors.py` & `excel-sql-engine-1.6/PyxlSql/pyxlErrors.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlGrammar.py` & `excel-sql-engine-1.6/PyxlSql/pyxlGrammar.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlPivot.py` & `excel-sql-engine-1.6/PyxlSql/pyxlPivot.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,17 +169,17 @@
 
         #
         for row_nb in range(2, max_row):
             formula = "= {}/{}".format(dst_sheet.get_reference(row_nb, sums, absolute=False),
                                        dst_sheet.get_reference(max_row, sums))
             dst_sheet.set_value(row_nb, percent, formula)
 
-            formula = "=SUM({}:{})".format(dst_sheet.get_reference(2, percent),
+        formula = "=SUM({}:{})".format(dst_sheet.get_reference(2, percent),
                                        dst_sheet.get_reference(max_row - 1, percent))
-            dst_sheet.set_value(max_row, percent, formula)
+        dst_sheet.set_value(max_row, percent, formula)
 
         #
 
         pie = PieChart()
         label_row = dst_sheet.find_column(labels)
         data_row = dst_sheet.find_column(percent)
```

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlResults.py` & `excel-sql-engine-1.6/PyxlSql/pyxlResults.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlSheets.py` & `excel-sql-engine-1.6/PyxlSql/pyxlSheets.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,35 @@
 # developed by fabien.battini@gmail.com
 # ---------------------------------------------------------------------------------------------------------------
 
 import re
 import inspect
 import openpyxl
 import openpyxl.styles
-from PyxlSql.pyxlErrors import PyxlSqlColumnError, PyxlSqlInternalError
+from PyxlSql.pyxlErrors import PyxlSqlColumnError
+from copy import copy
+
+class PyxlStyle:
+    """Style for columns, limited features"""
+
+    def __init__(self,cell):
+        self.number_format = cell.number_format
+        self.style = cell.style
+        self.fill = copy(cell.fill)
+        self.font = copy(cell.font)
+        self.alignment = copy(cell.alignment)
+
+    def copy_to_cell(self,cell):
+        # for some strange reason, the order of the following statements is important.
+        # probably setting the style resets the number format
+        cell.style = self.style
+        cell.fill = copy(self.fill)
+        cell.font = copy(self.font)
+        cell.number_format = self.number_format
+        cell.alignment = copy(self.alignment)
 
 
 # ---------------------------------------------------------------------------------------------------------------
 # class NamedWS
 # ---------------------------------------------------------------------------------------------------------------
 
 
@@ -72,15 +92,15 @@
             col_name = self.openpyxl_sheet.cell(row=first_row, column=i).value
             if col_name is not None and col_name != "" and col_name != " ":
                 col_name = str(col_name)  # str(), because could be an integer, typically a year
                 self.column_names[col_name] = i
                 self.columns.append(col_name)
                 cell = self.openpyxl_sheet.cell(row=first_row + 1, column=i)
                 if cell is not None:
-                    self.column_styles[col_name] = cell.number_format
+                    self.column_styles[col_name] = PyxlStyle(cell)
         self.data_is_read = True
     def get_name(self):
         return self.openpyxl_sheet.title
 
     def rename(self, new_name:str):
         self.openpyxl_sheet.title = new_name
         self.full_name = self.father.filename + ':[' + new_name + ']'
@@ -136,28 +156,30 @@
 
     def get_string(self, row_nb, column_name):
         cell = self.get_cell(row_nb, column_name)
         if cell is None or cell.value is None or cell.value == "None":
             return ""
         return str(cell.value)
 
-    def get_html_value(self, row_nb, column_name):
-        cell = self.get_cell(row_nb, column_name)
+    @staticmethod
+    def get_html_value_from_cell(cell):
+
         if cell is None or cell.value is None or cell.value == "None":
             return ""
-        if isinstance(cell.value,str) and cell.value[0]=='=':
+        if isinstance(cell.value, str) and (cell.value != '' and cell.value[0] == '='):
             # this is a formula
             return cell.value
 
         if cell.is_date:
             proto = cell.number_format
-            val = proto.replace("mm-dd-yy", "{:02d}/{:02d}/{:04d}".format(cell.value.month,cell.value.day,cell.value.year)) # strange enough
+            val = proto.replace("mm-dd-yy", "{:02d}/{:02d}/{:04d}".format(cell.value.month, cell.value.day,
+                                                                          cell.value.year))  # strange enough
             val = val.replace("yyyy", "{:4d}".format(cell.value.year))
-            val = val.replace("h:mm", "{:d}:{:02d}".format(cell.value.hour,cell.value.minute))
-            val = val.replace("yy", "{:02d}".format(cell.value.year%100))
+            val = val.replace("h:mm", "{:d}:{:02d}".format(cell.value.hour, cell.value.minute))
+            val = val.replace("yy", "{:02d}".format(cell.value.year % 100))
             val = val.replace("y", "{:d}".format(cell.value.year))
             val = val.replace("mm", "{:02d}".format(cell.value.month))
             val = val.replace("m", "{:d}".format(cell.value.month))
             val = val.replace("dd", "{:02d}".format(cell.value.day))
             val = val.replace("d", "{:d}".format(cell.value.day))
             val = val.replace("h", "{:d}".format(cell.value.hour))
             val = val.replace("s", "{:02d}".format(cell.value.second))
@@ -190,169 +212,42 @@
             "0.0000000%": ":.7f",
             "0.00000000%": ":.8f",
             "0.000000000%": ":.9f",
             "0.0000000000%": ":.10f",
         }
 
         if cell.number_format in number_formats.keys():
-            proto = "{"+number_formats[cell.number_format]+'}'
+            proto = "{" + number_formats[cell.number_format] + '}'
             if cell.number_format[-1] == '%':
                 try:
                     val = proto.format(float(cell.value) * 100)
                     return val + "%"
                 except ValueError:
                     # sometimes, the format of the cell is inherited from a previous value,
                     # and therefore is set as %, while the content is indeed a string!
                     return str(cell.value)
 
             val = proto.format(cell.value)
             return val
-
         return str(cell.value)
 
-    @staticmethod
-    def norm(f:float)->int:
-        i = int(f)
-        i = max(0,i)
-        i = min(255,i)
-        return i
-
-    @staticmethod
-    def hex2(i:int):
-        if i < 16:
-            return "0"+hex(i)[2:]
-        return hex(i)[2:]
-    @staticmethod
-    def hsl_to_rgb(t,s,l):
-        lp = l/255
-        c = (1 - abs(2*lp -1))*s
-        tp = t*6/256
-        m = l - c/2
-        x = c*(1-abs(tp % 2 -1))
-        # if t == 0 and False:
-        #     rp,gp,bp=0,0,0
-        if 0 <= tp < 1:
-            rp,gp,bp = c,x,0
-        elif 1 <= tp < 2:
-            rp,gp,bp = x,c,0
-        elif 2 <= tp < 3:
-            rp,gp,bp = 0,c,x
-        elif 3 <= tp < 4:
-            rp,gp,bp = 0,x,c
-        elif 4 <= tp < 5:
-            rp,gp,bp = x,0,c
-        else:
-            rp,gp,bp = c,0,x
-        r = PyxlSheet.norm(rp + m)
-        g = PyxlSheet.norm(gp + m)
-        b = PyxlSheet.norm(bp + m)
-        return PyxlSheet.hex2(r) + PyxlSheet.hex2(g) + PyxlSheet.hex2(b)
-    @staticmethod
-    def rgb_to_hsl(rgb):
-        # see https://fr.wikipedia.org/wiki/Teinte_saturation_luminosité
-        r = int(rgb[0:2],16)
-        g = int(rgb[2:4],16)
-        b = int(rgb[4:6],16)
-        ma = max(r,g,b)
-        mi = min(r,g,b)
-        c = ma - mi
-
-        if c == 0:
-            tp = 0
-        elif ma == r:
-            tp = ((g - b) / c) % 6
-        elif ma == g:
-            tp = ((b - r) / c + 2) % 6
-        else:
-            tp = ((r - g) / c + 4) % 6
-
-
-        t =  (tp * 255)/6 # if rgb != "FFFFFF" else 170
-        l =  ((ma+mi)/2)
-        lp = l / 255
-        s = 0.0 if  lp == 0 or lp == 1 else  (c / (1 - abs(2 * lp - 1)))
-        return t,s,l
-
-    @staticmethod
-    def tint_rgb(rgb, tint) -> str:
-        t, s, l = PyxlSheet.rgb_to_hsl(rgb)
-        if l == 255 or (t == 0 and l != 0):      #   strange behavior, but tests leads to this !
-            l = l * (1+tint)
-        else:
-            l = tint * (255 - l) + l  # retro-engineering of Excel behavior
-        return PyxlSheet.hsl_to_rgb(t, s, l)
-
-    def get_rgb_color(self, color):
-        if color is None:
-            return None
-        if color.type == 'rgb':
-            if color.rgb[0:2] == "00": # alpha = do not use color
-                return None
-            return self.tint_rgb(color.rgb[2:], color.tint)
-
-        if color.type =='theme':
-            rgb = self.father.theme[color.index]
-            return self.tint_rgb(rgb, color.tint)
+    def get_html_value(self, row_nb, column_name):
+        cell = self.get_cell(row_nb, column_name)
+        return self.get_html_value_from_cell(cell)
 
-        raise PyxlSqlInternalError("Excel unknown color not theme nor rgb")
 
     def get_cell_color(self, cell):
-        return self.get_rgb_color(cell.fill.fgColor)
+        return self.father.get_rgb_color(cell.fill.fgColor)
 
 
-    def get_html_style(self, row_nb, column_name):
-        # Manage bold/italic, center/left/right, number formats, date, formula
-
 
+    def get_html_style(self, row_nb, column_name):
         cell = self.get_cell(row_nb, column_name)
-        cell_format = ""
-        cell_style = 'style="'
-        v_align = cell.alignment.vertical
-        if v_align is  None:
-            # excel defaults to bottom
-            # html defaults to top
-            cell_style += " vertical-align: bottom; "
-        elif v_align == 'center':
-            cell_style += " vertical-align: middle; "
-        elif v_align == 'top':
-            cell_style += " vertical-align: top; "
-
-        cell_color = self.get_rgb_color(cell.fill.fgColor)
-        if cell_color is not None:
-            cell_format += f" bgcolor='#{cell_color}' "  # noqa
-
-        h_align = cell.alignment.horizontal
-        if h_align is not None:
-            cell_style += f" text-align: {h_align}; "
-
-
-        cell_font = cell.font
-        if cell_font is not None :
-            # rough font-size computation, from https://www.w3schools.com/css/css_font_size.asp
-            # default html font-size = 16px = 1em
-            # default excel font-size = 11
-            # rough-estimate : html-font-size = excel*16/11 px
-            cell_style += f"font-family:'{cell_font.name}';font-size:{int(cell_font.size*16/11)}px;"
-            font_color = self.get_rgb_color(cell_font.color)
-            if font_color is not None:
-                cell_style += f"color:#{font_color};"
-                # TODO: utiliser mathplotlib pour reconstruire le pie chart
-                # https://matplotlib.org/3.1.1/gallery/pie_and_polar_charts/pie_features
-                # voir https://groups.google.com/g/openpyxl-users/c/v2FDsbDDTqU/m/rQWLAXZFkeUJ
-            if cell_font.b:
-                cell_style += "font-weight: bold; "
-            if cell_font.i:
-                cell_style += 'font-style: italic; '
-            if cell_font.u:
-                cell_style += 'text-decoration: underline; '
+        return self.father.get_html_style_from_cell(cell)
 
-        if cell_style != "":
-           cell_style += '"'
-
-        return cell_format + cell_style
     def get_float(self, row_nb, column_name):
         cell = self.get_cell(row_nb, column_name)
         if cell is None:
             return 0
         val = cell.value
 
         if val is None or val == "":
@@ -363,15 +258,15 @@
             int_val = eval(val)  # a tentative to manage simple cells, such as '=12.56-24.9'
             # print("EVAL", val, intVal)
             # TODO: Track Errors
             return int_val
 
         return float(val)  # ********** CAVEAT! must be Float, because can be less than 1
 
-    def get_style(self, column_name):
+    def get_style(self, column_name)->PyxlStyle :
          lc_column_name = str(column_name)  # .lower()
          if lc_column_name not in self.column_names:
              raise PyxlSqlColumnError(column_name, self.full_name)
          return self.column_styles[lc_column_name]
 
     # def get_index(self, *column_names):
     #     """
@@ -405,18 +300,15 @@
             value = re.sub("^ *", "", value)
             value = re.sub(" *$", "", value)
 
         cell.value = value
         cell.font = self.book_default_font
         style = number_format if number_format is not None else self.get_style(column_name)
         if style is not None:
-            cell.number_format = style
-
-        if number_format:
-            cell.number_format = number_format
+            style.copy_to_cell(cell)
 
         self.current_row = max(self.current_row, row_nb+1)  # current_row is the first FREE cell
 
     # UNUSED, for future PIVOT
     # def create_row(self, init):
     #     for column, value in init.items():
     #         self.set_value(self.current_row, column, value)
```

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlSql.py` & `excel-sql-engine-1.6/PyxlSql/pyxlSql.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # ----------------------- General behavior
 # REQ 0001: PyxlSQL uses openPyxl to read excel files
 # REQ 0002: PyxlSQL statements are stored 'Pyxl SQL' sheet
 # REQ 0003: Sheet are described as 'sheet name' or 'filename.xlsx[sheet name]'
 # REQ 0004: remove start/trailing spaces for Command, Clause, field names, it is a common error, hard to find
 # REQ 0005: Import functools automatically, otherwise MIN/MAX do not work
 # REQ 0006: Requirements and FIX ME should be extracted automatically from the source code and published in doc
-# TODO: Req 0007: Use API token to upload on Pypi. see  https://pyptoxi.org/help/#apitoken and https://pypi.org/manage/account/token/
+# Req 0007: Use API token to upload on Pypi. see  https://pyptoxi.org/help/#apitoken and https://pypi.org/manage/account/token/
 # REQ 0008: Generate to do.rst through tox, using parse_requirements.py
 # REQ 0009: publish also htmlcov on gitlab.io
 # REQ 0010: create a downloadable executable for windows user : python -m pip install PyInstaller #
 # TODO: REQ 0011: create a doc specific to windows user that do not know python
 # REQ 0012: manage also .ods files from LibreOffice: NO, this is NOT possible, OpenPyxl does NOT read .ods format
 # REQ 0013: LAZY reading of sheets: only sheets that are referred by the SQL commands are read.
 
@@ -269,11 +269,13 @@
     def run_first(self):
         """Used for tests with pytest"""
         for existing_file in self.files:
             if os.path.isfile(existing_file) and re.match(r".*\.xls(x|m|)$", existing_file):
                 return SqlWb(self, existing_file, file_path=self.file_path)
         raise PyxlSqlError("No file to process", '{' + self.files[0] + '}')
 
+def run_pyxl_sql():
+    my_runner = PyxlRunner()
+    my_runner.run()
 
 if __name__ == "__main__":
-    cmdline = PyxlRunner()
-    cmdline.run()
+    run_pyxl_sql()
```

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlStages.py` & `excel-sql-engine-1.6/PyxlSql/pyxlStages.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/PyxlSql/pyxlWorkbook.py` & `excel-sql-engine-1.6/PyxlSql/pyxlWorkbook.py`

 * *Files 22% similar despite different names*

```diff
@@ -131,14 +131,19 @@
             theme.append(m.group(1))
         else:
             raise PyxlSqlInternalError("Excel wrong file format for color theme")
 
         m = re.search(r'<a:accent6><a:srgbClr val="([\dABCDEF]*)"/></a:accent6>', theme_desc)
         if m:
             theme.append(m.group(1))
+
+        m = re.search(r'<a:folHlink><a:srgbClr val="([\dABCDEF]*)"/></a:folHlink>', theme_desc)
+        if m:
+            theme.append(m.group(1))
+
         return theme
 
     def find_file(self, filename):
         if filename is None:
             return None
         if os.path.exists(filename):
             return filename
@@ -216,19 +221,167 @@
         try:
             ins = open(file_name, mode)
         except OSError as error:
             raise PyxlSqlExecutionError(f"FATAL ERROR: Cannot open('{file_name}',{mode})", str(error))
         return ins
 
     @staticmethod
+    def norm(f:float)->int:
+        i = int(f)
+        i = max(0,i)
+        i = min(255,i)
+        return i
+
+    @staticmethod
+    def hex2(i:int):
+        if i < 16:
+            return "0"+hex(i)[2:]
+        return hex(i)[2:]
+    @staticmethod
+    def hsl_to_rgb(t,s,l):
+        lp = l/255
+        c = (1 - abs(2*lp -1))*s
+        tp = t*6/256
+        m = l - c/2
+        x = c*(1-abs(tp % 2 -1))
+        # if t == 0 and False:
+        #     rp,gp,bp=0,0,0
+        if 0 <= tp < 1:
+            rp,gp,bp = c,x,0
+        elif 1 <= tp < 2:
+            rp,gp,bp = x,c,0
+        elif 2 <= tp < 3:
+            rp,gp,bp = 0,c,x
+        elif 3 <= tp < 4:
+            rp,gp,bp = 0,x,c
+        elif 4 <= tp < 5:
+            rp,gp,bp = x,0,c
+        else:
+            rp,gp,bp = c,0,x
+        r = PyxlWorkbook.norm(rp + m)
+        g = PyxlWorkbook.norm(gp + m)
+        b = PyxlWorkbook.norm(bp + m)
+        return PyxlWorkbook.hex2(r) + PyxlWorkbook.hex2(g) + PyxlWorkbook.hex2(b)
+    @staticmethod
+    def rgb_to_hsl(rgb):
+        # see https://fr.wikipedia.org/wiki/Teinte_saturation_luminosité
+        r = int(rgb[0:2],16)
+        g = int(rgb[2:4],16)
+        b = int(rgb[4:6],16)
+        ma = max(r,g,b)
+        mi = min(r,g,b)
+        c = ma - mi
+
+        if c == 0:
+            tp = 0
+        elif ma == r:
+            tp = ((g - b) / c) % 6
+        elif ma == g:
+            tp = ((b - r) / c + 2) % 6
+        else:
+            tp = ((r - g) / c + 4) % 6
+
+
+        t =  (tp * 255)/6 # if rgb != "FFFFFF" else 170
+        l =  ((ma+mi)/2)
+        lp = l / 255
+        s = 0.0 if  lp == 0 or lp == 1 else  (c / (1 - abs(2 * lp - 1)))
+        return t,s,l
+
+    @staticmethod
+    def tint_rgb(rgb, tint) -> str:
+        t, s, l = PyxlWorkbook.rgb_to_hsl(rgb)
+        if l == 255 or (t == 0 and l != 0):      #   strange behavior, but tests leads to this !
+            l = l * (1+tint)
+        else:
+            l = tint * (255 - l) + l  # retro-engineering of Excel behavior
+        return PyxlWorkbook.hsl_to_rgb(t, s, l)
+
+    def get_rgb_color(self, color):
+        if color is None:
+            return None
+        if color.type == 'rgb':
+            if color.rgb[0:2] == "00": # alpha = do not use color
+                return None
+            return self.tint_rgb(color.rgb[2:], color.tint)
+
+        if color.type =='theme':
+            try:
+                rgb = self.theme[color.index]
+                return self.tint_rgb(rgb, color.tint)
+            except IndexError:
+                raise PyxlSqlInternalError("Excel theme out of range ")
+
+        raise PyxlSqlInternalError("Excel unknown color not theme nor rgb")
+
+
+    @staticmethod
     def escape(excel_str: str):
         html_str = excel_str.encode('ascii', 'xmlcharrefreplace')
         html_str =  html_str.decode('utf-8')
         return html_str
 
+    def get_html_style_from_cell(self, cell):
+        # Manage bold/italic, center/left/right, number formats, date, formula
+
+        cell_format = ""
+        cell_style = 'style="'
+        v_align = cell.alignment.vertical
+        if v_align is  None:
+            # excel defaults to bottom
+            # html defaults to top
+            cell_style += " vertical-align: bottom; "
+        elif v_align == 'center':
+            cell_style += " vertical-align: middle; "
+        elif v_align == 'top':
+            cell_style += " vertical-align: top; "
+
+        cell_color = self.get_rgb_color(cell.fill.fgColor)
+        if cell_color is not None:
+            cell_format += f" bgcolor='#{cell_color}' "  # noqa
+
+        h_align = cell.alignment.horizontal
+        if h_align is not None:
+            cell_style += f" text-align: {h_align}; "
+
+
+        cell_font = cell.font
+        if cell_font is not None :
+            # rough font-size computation, from https://www.w3schools.com/css/css_font_size.asp
+            # default html font-size = 16px = 1em
+            # default excel font-size = 11
+            # rough-estimate : html-font-size = excel*16/11 px
+            cell_style += f"font-family:'{cell_font.name}';font-size:{int(cell_font.size*16/11)}px;"
+            font_color = self.get_rgb_color(cell_font.color)
+            if font_color is not None:
+                cell_style += f"color:#{font_color};"
+                # TODO: use mathplotlib to build a pie chart   # noqa
+                # https://matplotlib.org/3.1.1/gallery/pie_and_polar_charts/pie_features
+                # voir https://groups.google.com/g/openpyxl-users/c/v2FDsbDDTqU/m/rQWLAXZFkeUJ
+            if cell_font.b:
+                cell_style += "font-weight: bold; "
+            if cell_font.i:
+                cell_style += 'font-style: italic; '
+            if cell_font.u:
+                cell_style += 'text-decoration: underline; '
+
+        if cell_style != "":
+           cell_style += '"'
+
+        return cell_format + cell_style
+
+    def get_html_style_by_nb(self, sheet, line_nb: int, col_nb:int):
+        cell = sheet.cell(line_nb, col_nb)
+        return self.get_html_style_from_cell(cell)
+
+    @staticmethod
+    def get_html_value_by_nb(sheet, line_nb: int, col_nb: int):
+        cell = sheet.cell(line_nb, col_nb)
+        return PyxlSheet.get_html_value_from_cell(cell)
+
     def export_html(self, file_name: str, css: str=""):
 
         outs = self.local_open(file_name, "w")
 
         outs.writelines('<!DOCTYPE html>\n')
         outs.writelines('<html>\n')
         outs.writelines('<head>\n')
@@ -250,36 +403,39 @@
             outs.writelines(f'    <link rel="stylesheet" href="{css}" type="text/css">\n')
 
 
         outs.writelines('</head>\n')
         outs.writelines('<body>\n')
         outs.writelines(f'    <h1>{self.filename}</h1>\n')
 
-        for cur_sheet in self.sheets.values():
+        for cur_sheet in self.wb.worksheets:
             outs.writelines('   <div  class="sheet">\n')
-            outs.writelines(f'      <h2>Sheet [{cur_sheet.get_name()}]</h2>\n')
+            outs.writelines(f'      <A id="{cur_sheet.title}"><h2>Sheet [{cur_sheet.title}]</h2></a>\n')
             outs.writelines('      <br><br>\n')
             outs.writelines('      <table>\n')
             outs.writelines('        <thead>\n')                                           # noqa
             outs.writelines('          <tr><th>1</th>\n')
-            for col_name in cur_sheet.columns:
-                outs.write(f'            <th {cur_sheet.get_html_style(1, col_name)}>{col_name}</th>\n')
+            for col_nb in range(1, cur_sheet.max_column+1):
+                col_name = cur_sheet.cell(1,col_nb).value or ''
+                outs.write(f'            <th {self.get_html_style_by_nb(cur_sheet,1, col_nb)}>{col_name}</th>\n')
             outs.write('          </tr>\n')
             outs.write('        </thead>\n')                                               # noqa
 
-            for lineno in cur_sheet.get_row_range():
+            for lineno in range(2, cur_sheet.max_row+1):
                 outs.write(f'         <tr><td>{lineno}</td>\n')
-                for col_name in cur_sheet.columns:
-                    outs.write(f'           <td {cur_sheet.get_html_style(lineno, col_name)}>')
-                    outs.write(f'               {self.escape(cur_sheet.get_html_value(lineno, col_name))}</td>\n')
+                for col_nb in range(1, cur_sheet.max_column+1):
+                    outs.write(f'           <td {self.get_html_style_by_nb(cur_sheet,lineno, col_nb)}>')
+                    val = self.get_html_value_by_nb(cur_sheet,lineno, col_nb)  or ''
+                    outs.write(f'               {self.escape(val)}</td>\n')
                 outs.write('         </tr>\n')
             outs.write('      </table>\n')
             outs.write('   </div>\n')
         outs.write('</body>\n')
         outs.write('</html>\n')
+
     def get_workbook(self, name):
         if name not in self.wbs:
             self.wbs[name] = PyxlWorkbook(name, file_path=self.file_path)
         return self.wbs[name]
 
     def import_module(self, module, sub_modules=None):
         mod = importlib.import_module(module)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `excel-sql-engine-1.4/README.md` & `excel-sql-engine-1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -162,10 +162,10 @@
 Documentation is built using Sphinx https://www.sphinx-doc.org/
 
 Documentation is generated in https://fabien_battini.gitlab.io/pyxlsql/html/
 This process is achieved automatically through gitlab CI pipelines.
 
 gitlab repository: https://gitlab.com/fabien_battini/pyxlsql
 
-pypi: https://pypi.org/project/open-pyxl-sql
+pypi: https://pypi.org/project/excel-sql-engine/
 
 LinkedIN: https://www.linkedin.com/in/fabien-battini-supelec/
```

### Comparing `excel-sql-engine-1.4/excel_sql_engine.egg-info/PKG-INFO` & `excel-sql-engine-1.6/excel_sql_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-sql-engine
-Version: 1.4
+Version: 1.6
 Summary: A tiny SQL engine for Excel files, based on Openpyxl
 Home-page: https://gitlab.com/fabien.battini/pyxlsql
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: excel sql
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -180,10 +180,10 @@
 Documentation is built using Sphinx https://www.sphinx-doc.org/
 
 Documentation is generated in https://fabien_battini.gitlab.io/pyxlsql/html/
 This process is achieved automatically through gitlab CI pipelines.
 
 gitlab repository: https://gitlab.com/fabien_battini/pyxlsql
 
-pypi: https://pypi.org/project/open-pyxl-sql
+pypi: https://pypi.org/project/excel-sql-engine/
 
 LinkedIN: https://www.linkedin.com/in/fabien-battini-supelec/
```

### Comparing `excel-sql-engine-1.4/excel_sql_engine.egg-info/SOURCES.txt` & `excel-sql-engine-1.6/excel_sql_engine.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 PyxlSql/pyxlSheets.py
 PyxlSql/pyxlSql.py
 PyxlSql/pyxlStages.py
 PyxlSql/pyxlWorkbook.py
 excel_sql_engine.egg-info/PKG-INFO
 excel_sql_engine.egg-info/SOURCES.txt
 excel_sql_engine.egg-info/dependency_links.txt
+excel_sql_engine.egg-info/entry_points.txt
 excel_sql_engine.egg-info/setup.cfg
 excel_sql_engine.egg-info/top_level.txt
 tests/test_Northwind.py
 tests/test_tooling.py
```

### Comparing `excel-sql-engine-1.4/tests/test_Northwind.py` & `excel-sql-engine-1.6/tests/test_Northwind.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.4/tests/test_tooling.py` & `excel-sql-engine-1.6/tests/test_tooling.py`

 * *Files identical despite different names*

