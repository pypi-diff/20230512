# Comparing `tmp/odoo14_addons_oca_edi-14.0.20230227.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_edi-14.0.20230511.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1654 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2886 b- defN 23-Feb-28 04:23 odoo14_addons_oca_edi-14.0.20230227.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-28 04:23 odoo14_addons_oca_edi-14.0.20230227.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-28 04:23 odoo14_addons_oca_edi-14.0.20230227.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      393 b- defN 23-Feb-28 04:23 odoo14_addons_oca_edi-14.0.20230227.0.dist-info/RECORD
-4 files, 3372 bytes uncompressed, 880 bytes compressed:  73.9%
+Zip file size: 1664 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2954 b- defN 23-May-12 04:19 odoo14_addons_oca_edi-14.0.20230511.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 04:19 odoo14_addons_oca_edi-14.0.20230511.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-12 04:19 odoo14_addons_oca_edi-14.0.20230511.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      393 b- defN 23-May-12 04:19 odoo14_addons_oca_edi-14.0.20230511.0.dist-info/RECORD
+4 files, 3440 bytes uncompressed, 890 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_edi-14.0.20230227.0.dist-info/METADATA
+Filename: odoo14_addons_oca_edi-14.0.20230511.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230227.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_edi-14.0.20230511.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230227.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_edi-14.0.20230511.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230227.0.dist-info/RECORD
+Filename: odoo14_addons_oca_edi-14.0.20230511.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_edi-14.0.20230227.0.dist-info/METADATA` & `odoo14_addons_oca_edi-14.0.20230511.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-edi
-Version: 14.0.20230227.0
+Version: 14.0.20230511.0
 Summary: Meta package for oca-edi Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -53,12 +53,13 @@
 Requires-Dist: odoo14-addon-product-import-ubl
 Requires-Dist: odoo14-addon-purchase-order-ubl
 Requires-Dist: odoo14-addon-purchase-stock-ubl
 Requires-Dist: odoo14-addon-sale-order-customer-free-ref
 Requires-Dist: odoo14-addon-sale-order-import
 Requires-Dist: odoo14-addon-sale-order-import-ubl
 Requires-Dist: odoo14-addon-sale-order-import-ubl-customer-free-ref
+Requires-Dist: odoo14-addon-sale-order-import-ubl-line-customer-ref
 Requires-Dist: odoo14-addon-sale-order-packaging-import
 Requires-Dist: odoo14-addon-sale-order-ubl
 
 UNKNOWN
```

