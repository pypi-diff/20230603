# Comparing `tmp/odoo_addons_oca_account_invoicing-16.0.20230526.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_invoicing-16.0.20230602.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1604 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1623 b- defN 23-May-27 02:45 odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 02:45 odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-27 02:45 odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      441 b- defN 23-May-27 02:45 odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/RECORD
-4 files, 2157 bytes uncompressed, 734 bytes compressed:  66.0%
+Zip file size: 1628 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1777 b- defN 23-Jun-03 02:45 odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 02:45 odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-03 02:45 odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      441 b- defN 23-Jun-03 02:45 odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/RECORD
+4 files, 2311 bytes uncompressed, 758 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/METADATA
+Filename: odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/WHEEL
+Filename: odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/RECORD
+Filename: odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_invoicing-16.0.20230526.0.dist-info/METADATA` & `odoo_addons_oca_account_invoicing-16.0.20230602.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-invoicing
-Version: 16.0.20230526.0
+Version: 16.0.20230602.1
 Summary: Meta package for oca-account-invoicing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -15,16 +15,18 @@
 Requires-Dist: odoo-addon-account-invoice-merge (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-refund-link (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-tax-required (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-transmit-method (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-triple-discount (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-menu-invoice-refund (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-receipt-journal (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-account-receipt-send (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-tax-change (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-invoicing-mode (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-invoicing-mode-at-shipping (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-invoicing-mode-monthly (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-stock-picking-return-invoicing (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-sale-order-invoicing-grouping-criteria (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-return-refund-option (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

