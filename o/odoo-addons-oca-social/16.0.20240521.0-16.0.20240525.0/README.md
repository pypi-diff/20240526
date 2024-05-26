# Comparing `tmp/odoo_addons_oca_social-16.0.20240521.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_social-16.0.20240525.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1705 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3024 b- defN 24-May-22 06:49 odoo_addons_oca_social-16.0.20240521.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-22 06:49 odoo_addons_oca_social-16.0.20240521.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-22 06:49 odoo_addons_oca_social-16.0.20240521.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      397 b- defN 24-May-22 06:49 odoo_addons_oca_social-16.0.20240521.0.dist-info/RECORD
-4 files, 3514 bytes uncompressed, 923 bytes compressed:  73.7%
+Zip file size: 1728 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3216 b- defN 24-May-26 07:26 odoo_addons_oca_social-16.0.20240525.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-26 07:26 odoo_addons_oca_social-16.0.20240525.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-26 07:26 odoo_addons_oca_social-16.0.20240525.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      397 b- defN 24-May-26 07:26 odoo_addons_oca_social-16.0.20240525.0.dist-info/RECORD
+4 files, 3706 bytes uncompressed, 946 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_social-16.0.20240521.0.dist-info/METADATA
+Filename: odoo_addons_oca_social-16.0.20240525.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_social-16.0.20240521.0.dist-info/WHEEL
+Filename: odoo_addons_oca_social-16.0.20240525.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_social-16.0.20240521.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_social-16.0.20240525.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_social-16.0.20240521.0.dist-info/RECORD
+Filename: odoo_addons_oca_social-16.0.20240525.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_social-16.0.20240521.0.dist-info/METADATA` & `odoo_addons_oca_social-16.0.20240525.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-social
-Version: 16.0.20240521.0
+Version: 16.0.20240525.0
 Summary: Meta package for oca-social Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -19,14 +19,17 @@
 Requires-Dist: odoo-addon-mail-activity-team <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-attach-existing-attachment <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-autosubscribe <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-composer-cc-bcc <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-composer-cc-bcc-account <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-debrand <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-drop-target <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-mail-gateway <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-mail-gateway-telegram <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-mail-gateway-whatsapp <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-improved-tracking-value <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-inline-css <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-layout-force <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-layout-preview <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-optional-autofollow <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-optional-follower-notification <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-mail-outbound-static <16.1dev,>=16.0dev
```

