# Comparing `tmp/odoo_addons_oca_account_invoicing-16.0.20230419.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_invoicing-16.0.20230421.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1531 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1090 b- defN 23-Apr-20 02:59 odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 02:59 odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-20 02:59 odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      441 b- defN 23-Apr-20 02:59 odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/RECORD
-4 files, 1624 bytes uncompressed, 661 bytes compressed:  59.3%
+Zip file size: 1564 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1320 b- defN 23-Apr-21 03:02 odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 03:02 odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-21 03:02 odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      441 b- defN 23-Apr-21 03:02 odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/RECORD
+4 files, 1854 bytes uncompressed, 694 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/METADATA
+Filename: odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/WHEEL
+Filename: odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/RECORD
+Filename: odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_invoicing-16.0.20230419.0.dist-info/METADATA` & `odoo_addons_oca_account_invoicing-16.0.20230421.0.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-invoicing
-Version: 16.0.20230419.0
+Version: 16.0.20230421.0
 Summary: Meta package for oca-account-invoicing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -13,11 +13,14 @@
 Requires-Dist: odoo-addon-account-invoice-fiscal-position-update (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-merge (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-refund-link (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-tax-required (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-transmit-method (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-triple-discount (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-menu-invoice-refund (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-partner-invoicing-mode (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-partner-invoicing-mode-at-shipping (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-partner-invoicing-mode-monthly (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-return-refund-option (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

