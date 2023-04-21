# Comparing `tmp/odoo12_addon_crm_sale_order_line-12.0.0.0.2-py3-none-any.whl.zip` & `tmp/odoo12_addon_crm_sale_order_line-12.0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5346 bytes, number of entries: 11
+Zip file size: 5348 bytes, number of entries: 11
 -rwxrwxr-x  2.0 unx       46 b- defN 23-Apr-21 12:14 odoo/addons/crm_sale_order_line/__init__.py
--rwxr-xr-x  2.0 unx      568 b- defN 23-Apr-21 13:15 odoo/addons/crm_sale_order_line/__manifest__.py
--rwxr-xr-x  2.0 unx       82 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line/models/__init__.py
+-rwxr-xr-x  2.0 unx      568 b- defN 23-Apr-21 13:49 odoo/addons/crm_sale_order_line/__manifest__.py
+-rwxrwxr-x  2.0 unx       82 b- defN 23-Feb-20 16:47 odoo/addons/crm_sale_order_line/models/__init__.py
 -rw-r--r--  2.0 unx     2701 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line/models/crm_lead.py
 -rw-r--r--  2.0 unx     1094 b- defN 23-Apr-21 13:06 odoo/addons/crm_sale_order_line/models/crm_sale_order_line.py
--rwxr-xr-x  2.0 unx      159 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line/security/ir.model.access.csv
+-rwxrwxr-x  2.0 unx      159 b- defN 23-Feb-20 17:13 odoo/addons/crm_sale_order_line/security/ir.model.access.csv
 -rw-r--r--  2.0 unx     1626 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line/views/crm_lead.xml
--rw-r--r--  2.0 unx      360 b- defN 23-Apr-21 13:21 odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 13:21 odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-21 13:21 odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1170 b- defN 23-Apr-21 13:21 odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/RECORD
-11 files, 7903 bytes uncompressed, 3270 bytes compressed:  58.6%
+-rw-r--r--  2.0 unx      360 b- defN 23-Apr-21 13:50 odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 13:50 odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-21 13:50 odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1170 b- defN 23-Apr-21 13:50 odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/RECORD
+11 files, 7903 bytes uncompressed, 3272 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/crm_sale_order_line/security/ir.model.access.csv
 Comment: 
 
 Filename: odoo/addons/crm_sale_order_line/views/crm_lead.xml
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/METADATA
+Filename: odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/WHEEL
+Filename: odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/top_level.txt
+Filename: odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/RECORD
+Filename: odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_sale_order_line/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Add relationship between crm lead and sale order line""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'cooperator',
-    'version': '12.0.0.0.2',
+    'version': '12.0.0.0.3',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'crm',
         'sale',
         'sale_crm'
```

## Comparing `odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/RECORD` & `odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 odoo/addons/crm_sale_order_line/__init__.py,sha256=Ax4qLxdb9ATk05MF7cSQ0BdpYCpGVYFy9n4U4zODf9o,46
-odoo/addons/crm_sale_order_line/__manifest__.py,sha256=odMeOAe4lG2adl3nqmyrUNVMD-tFDpav5j8Jah1CJBc,568
+odoo/addons/crm_sale_order_line/__manifest__.py,sha256=tcOuHyJ4z0m__0-I44tb7HbX38ZtDP-U3NovD53h0FU,568
 odoo/addons/crm_sale_order_line/models/__init__.py,sha256=x2c0XHvFeyoUQhIoHNIwcGuEl9RwTMjcpiMeg7iFSzk,82
 odoo/addons/crm_sale_order_line/models/crm_lead.py,sha256=IDY2ni6vPb8uu7LfIS0yZJ9AE82ydv40IQiMjactv8s,2701
 odoo/addons/crm_sale_order_line/models/crm_sale_order_line.py,sha256=nqpIUp2u9-OMkTDzDSKN6zgTwtnJPyW816rSRHTx2Dw,1094
 odoo/addons/crm_sale_order_line/security/ir.model.access.csv,sha256=dLVC7pGMeptJisyh4VFJRQ_nkeMURlWes8ZXfLLYZNI,159
 odoo/addons/crm_sale_order_line/views/crm_lead.xml,sha256=9iruaWU_pTYNP16cwn5Y9Ys7hR7S_I8RmvnW2RW54dc,1626
-odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/METADATA,sha256=2QdCBbVBtmRcIAOE-De16TjkvZ3Fq6RS_rUgpv1rPDE,360
-odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_crm_sale_order_line-12.0.0.0.2.dist-info/RECORD,,
+odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/METADATA,sha256=OggVBc30jIePhoemYGD6laWZXo8P3_Ug-DU2t_Ndxbs,360
+odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_crm_sale_order_line-12.0.0.0.3.dist-info/RECORD,,
```

