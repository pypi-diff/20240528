# Comparing `tmp/odoo_addons_oca_account_invoicing-16.0.20240518.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_invoicing-16.0.20240527.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1975 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4672 b- defN 24-May-19 03:03 odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-19 03:03 odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-19 03:03 odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      441 b- defN 24-May-19 03:03 odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/RECORD
-4 files, 5206 bytes uncompressed, 1105 bytes compressed:  78.8%
+Zip file size: 1985 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     4757 b- defN 24-May-28 02:59 odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 02:59 odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-28 02:59 odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      441 b- defN 24-May-28 02:59 odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/RECORD
+4 files, 5291 bytes uncompressed, 1115 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/METADATA
+Filename: odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/WHEEL
+Filename: odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/RECORD
+Filename: odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/METADATA` & `odoo_addons_oca_account_invoicing-16.0.20240527.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-invoicing
-Version: 16.0.20240518.0
+Version: 16.0.20240527.0
 Summary: Meta package for oca-account-invoicing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -12,14 +12,15 @@
 Requires-Dist: odoo-addon-account-invoice-alternate-payer <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-blocking <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-change-currency <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-check-total <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-crm-tag <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-currency-taxes <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-default-code-column <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-account-invoice-discount-display-amount <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-fiscal-position-update <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-fixed-discount <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-force-number <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-line-default-account <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-mass-sending <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-merge <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-payment-retention <16.1dev,>=16.0dev
```

