# Comparing `tmp/odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1-py3-none-any.whl.zip` & `tmp/odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 3879 bytes, number of entries: 10
--rwxr-xr-x  2.0 unx      149 b- defN 23-Mar-07 17:36 odoo/addons/crm_sale_order_line_rest_api/README.rst
--rwxr-xr-x  2.0 unx       23 b- defN 23-Mar-07 17:36 odoo/addons/crm_sale_order_line_rest_api/__init__.py
--rwxr-xr-x  2.0 unx      501 b- defN 23-Apr-19 16:25 odoo/addons/crm_sale_order_line_rest_api/__manifest__.py
--rwxr-xr-x  2.0 unx       32 b- defN 23-Mar-07 17:36 odoo/addons/crm_sale_order_line_rest_api/services/__init__.py
--rwxr-xr-x  2.0 unx      790 b- defN 23-Mar-07 17:36 odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
--rwxr-xr-x  2.0 unx      329 b- defN 23-Mar-07 17:36 odoo/addons/crm_sale_order_line_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      592 b- defN 23-Apr-19 16:32 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 16:32 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-19 16:32 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1136 b- defN 23-Apr-19 16:32 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/RECORD
-10 files, 3649 bytes uncompressed, 1829 bytes compressed:  49.9%
+-rwxr-xr-x  2.0 unx      149 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/README.rst
+-rwxr-xr-x  2.0 unx       23 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/__init__.py
+-rwxr-xr-x  2.0 unx      501 b- defN 23-Apr-21 13:16 odoo/addons/crm_sale_order_line_rest_api/__manifest__.py
+-rwxr-xr-x  2.0 unx       32 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/services/__init__.py
+-rwxr-xr-x  2.0 unx      790 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
+-rwxr-xr-x  2.0 unx      332 b- defN 23-Apr-21 12:57 odoo/addons/crm_sale_order_line_rest_api/services/schemas.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Apr-21 13:23 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 13:23 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-21 13:23 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1136 b- defN 23-Apr-21 13:23 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/RECORD
+10 files, 3652 bytes uncompressed, 1829 bytes compressed:  49.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_sale_order_line_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/METADATA
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/WHEEL
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/top_level.txt
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/RECORD
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_sale_order_line_rest_api/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Expose CRM order lines on the Rest API""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'api',
-    'version': '12.0.0.0.1',
+    'version': '12.0.0.0.2',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'crm_rest_api',
         'crm_sale_order_line'
     ],
```

## odoo/addons/crm_sale_order_line_rest_api/services/schemas.py

```diff
@@ -2,12 +2,12 @@
     "order_lines": {
         "type": "list",
         "empty": True,
         "schema": {
             "type": "dict",
             "schema": {
                 "product_id": {"type": "integer", "required": True},
-                "quantity": {"type": "integer", "required": True}
+                "price_unit": {"type": "integer", "required": False}
             }
         }
     }
 }
```

## Comparing `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/METADATA` & `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-crm-sale-order-line-rest-api
-Version: 12.0.0.0.1
+Version: 12.0.0.0.2
 Summary: Expose CRM order lines on the Rest API
 Home-page: 
 Author: Coopdevs Treball SCCL
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 12.0
 Requires-Python: >=3.5
```

## Comparing `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/RECORD` & `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/crm_sale_order_line_rest_api/README.rst,sha256=TbC3DjY4NLfKhsHanGsOWW_jEi0eFHD4Hbq0nKihPxY,149
 odoo/addons/crm_sale_order_line_rest_api/__init__.py,sha256=qksdRxAxHhEXpY0NZlTEolhxFILjRI5o7J0O4UrAE04,23
-odoo/addons/crm_sale_order_line_rest_api/__manifest__.py,sha256=V44ubiTnF5FVvTlz70IBGgZ8ylq5JxO9Urx9zYVQwUw,501
+odoo/addons/crm_sale_order_line_rest_api/__manifest__.py,sha256=L3_O_HLNw_nTD0E6u2zPTbDutkAIi0sw35GBPwdF9WY,501
 odoo/addons/crm_sale_order_line_rest_api/services/__init__.py,sha256=gyXaE_NlVgF1KawzsiRb0DeYYTT13kmL4Ya1LgcRg5c,32
 odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py,sha256=e1GEjo_Q2qz2ucNj1oQhQHhnm-pVEH1os47aFE3-x-M,790
-odoo/addons/crm_sale_order_line_rest_api/services/schemas.py,sha256=2AcTByjd1vUteVs60y_yp9RfEdMMzFrGMQh2SFJrfOY,329
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/METADATA,sha256=sDq4n7FZJQcBxQczSVgQG_G-UjoLGARZt59BYQsRHdo,592
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.1.dist-info/RECORD,,
+odoo/addons/crm_sale_order_line_rest_api/services/schemas.py,sha256=tTudvFX7WOVnZ_58fjiEzl4m8LnXuvw2j_gGgqcmIEE,332
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/METADATA,sha256=0j9w1ZOc_ybJP6eVej-tSjXzksZPPZFsSm1YsYq5JvU,592
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/RECORD,,
```

