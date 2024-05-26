# Comparing `tmp/jumeaux-5.0.1-py3-none-any.whl.zip` & `tmp/jumeaux-5.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 100232 bytes, number of entries: 178
+Zip file size: 100231 bytes, number of entries: 178
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 jumeaux/__init__.py
 -rw-r--r--  2.0 unx     4272 b- defN 80-Jan-01 00:00 jumeaux/addons/__init__.py
 -rw-r--r--  2.0 unx      306 b- defN 80-Jan-01 00:00 jumeaux/addons/did_challenge/__init__.py
 -rw-r--r--  2.0 unx      795 b- defN 80-Jan-01 00:00 jumeaux/addons/did_challenge/sleep.py
 -rw-r--r--  2.0 unx     2526 b- defN 80-Jan-01 00:00 jumeaux/addons/did_challenge/tag.py
 -rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 jumeaux/addons/dump/__init__.py
 -rw-r--r--  2.0 unx      770 b- defN 80-Jan-01 00:00 jumeaux/addons/dump/encoding.py
@@ -168,13 +168,13 @@
 -rwxr-xr-x  2.0 unx       36 b- defN 80-Jan-01 00:00 jumeaux/sample/template/simple/requests
 -rwxr-xr-x  2.0 unx      723 b- defN 80-Jan-01 00:00 jumeaux/sample/template/xml/api/one/diff-1.xml
 -rwxr-xr-x  2.0 unx      723 b- defN 80-Jan-01 00:00 jumeaux/sample/template/xml/api/other/diff-1.xml
 -rwxr-xr-x  2.0 unx      894 b- defN 80-Jan-01 00:00 jumeaux/sample/template/xml/config.yml
 -rwxr-xr-x  2.0 unx       12 b- defN 80-Jan-01 00:00 jumeaux/sample/template/xml/requests
 -rw-r--r--  2.0 unx    17106 b- defN 80-Jan-01 00:00 jumeaux/sample/viewer/index.html
 -rw-r--r--  2.0 unx     2625 b- defN 80-Jan-01 00:00 jumeaux/utils.py
--rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 jumeaux-5.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3888 b- defN 80-Jan-01 00:00 jumeaux-5.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jumeaux-5.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 jumeaux-5.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    17362 b- defN 16-Jan-01 00:00 jumeaux-5.0.1.dist-info/RECORD
-178 files, 210865 bytes uncompressed, 71788 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 jumeaux-5.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3888 b- defN 80-Jan-01 00:00 jumeaux-5.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jumeaux-5.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 jumeaux-5.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    17362 b- defN 16-Jan-01 00:00 jumeaux-5.0.2.dist-info/RECORD
+178 files, 210865 bytes uncompressed, 71787 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -513,23 +513,23 @@
 
 Filename: jumeaux/sample/viewer/index.html
 Comment: 
 
 Filename: jumeaux/utils.py
 Comment: 
 
-Filename: jumeaux-5.0.1.dist-info/LICENSE
+Filename: jumeaux-5.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: jumeaux-5.0.1.dist-info/METADATA
+Filename: jumeaux-5.0.2.dist-info/METADATA
 Comment: 
 
-Filename: jumeaux-5.0.1.dist-info/WHEEL
+Filename: jumeaux-5.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: jumeaux-5.0.1.dist-info/entry_points.txt
+Filename: jumeaux-5.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: jumeaux-5.0.1.dist-info/RECORD
+Filename: jumeaux-5.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jumeaux/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '5.0.1'
+__version__ = '5.0.2'
```

## Comparing `jumeaux-5.0.1.dist-info/LICENSE` & `jumeaux-5.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jumeaux-5.0.1.dist-info/METADATA` & `jumeaux-5.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumeaux
-Version: 5.0.1
+Version: 5.0.2
 Summary: Check difference between two responses of API.
 Home-page: https://tadashi-aikawa.github.io/jumeaux
 License: MIT
 Keywords: diff rest api response regression test
 Author: tadashi-aikawa
 Author-email: syou.maman@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
```

## Comparing `jumeaux-5.0.1.dist-info/RECORD` & `jumeaux-5.0.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jumeaux/__init__.py,sha256=9CSey5HdvXZ_1hpc5Qhv94A2v05XpBAz4CC8v7K1bWQ,22
+jumeaux/__init__.py,sha256=9M2Y2gTlBY0gNDVCT1KWrNC60XjpOgipLYIiRgc_InE,22
 jumeaux/addons/__init__.py,sha256=gYQG-k0Uuzq9uxRX_L2rlfFLWvtl7DdlO0ao1ZX5c-k,4272
 jumeaux/addons/did_challenge/__init__.py,sha256=TgHdGs-jzSTa0xa2EWo9wyjHFIyOAuKCd3p5LuVY7oU,306
 jumeaux/addons/did_challenge/sleep.py,sha256=wQ4k4CqmOUJwphURZHfuIQ7TVcLnhRN9XyJ7LbC7Aag,795
 jumeaux/addons/did_challenge/tag.py,sha256=9OLxIZ5jymt5Wda1EFpEJ7l-V9aw7nKry_OQI6aZOKM,2526
 jumeaux/addons/dump/__init__.py,sha256=4EWZ5rhl_x_rhyLLwVMCgvT79_wNT0ll8_4WoJ8I79k,192
 jumeaux/addons/dump/encoding.py,sha256=FOE8i7UmOxYWC5ee-9x31cC70AbppI7i2og2TTVhsU8,770
 jumeaux/addons/dump/html.py,sha256=o8__lYKUQtu3MvN7nEippBAJ3_CMAOFNGJccRmvquyM,1255
@@ -167,12 +167,12 @@
 jumeaux/sample/template/simple/requests,sha256=CKesNRdVTWgdWnCY_K8ExCSqNToFtqgStiSidgK_YsI,36
 jumeaux/sample/template/xml/api/one/diff-1.xml,sha256=5taqNoq8pN-s79ly8py-ZGSRnZVLkTbm1rOdtMQvNSs,723
 jumeaux/sample/template/xml/api/other/diff-1.xml,sha256=8I9ugp9u551mKdV9OHYi8KWUy_RXPM4l2hYTgDMrkXA,723
 jumeaux/sample/template/xml/config.yml,sha256=vqt2P-nyw9i2zqlrmLwZMjE2WMZOXisyBNkLq7LtUG0,894
 jumeaux/sample/template/xml/requests,sha256=mHMfrprQFLPOo0ugwFKwu7t2Fp8634eNEUkDG_PeFVI,12
 jumeaux/sample/viewer/index.html,sha256=RZytfGSvOn5FRFi1c6PzuLdaUBxYRKR-8p7s5_nL-BA,17106
 jumeaux/utils.py,sha256=cX3H2BbEYzuLAWLO2JYxaC_0PKnotk_6Bys_NxDyE_Y,2625
-jumeaux-5.0.1.dist-info/LICENSE,sha256=IKkX_iHGJtElV0t6vav-LLicUlhxOLt0Jl65lql1Wuw,1081
-jumeaux-5.0.1.dist-info/METADATA,sha256=A05e7RdYZthqDLvm5O5kmheZfouet4rSMRwPHMcjD1E,3888
-jumeaux-5.0.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-jumeaux-5.0.1.dist-info/entry_points.txt,sha256=CyOBZ_wPw8RqgutUO-RZsifwAQrqa95A2q9Rv98CB5A,45
-jumeaux-5.0.1.dist-info/RECORD,,
+jumeaux-5.0.2.dist-info/LICENSE,sha256=IKkX_iHGJtElV0t6vav-LLicUlhxOLt0Jl65lql1Wuw,1081
+jumeaux-5.0.2.dist-info/METADATA,sha256=IbVLbbk5EbF6F31Hf8rbitoeuHUbLDrPL8nEd6pBCI8,3888
+jumeaux-5.0.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+jumeaux-5.0.2.dist-info/entry_points.txt,sha256=CyOBZ_wPw8RqgutUO-RZsifwAQrqa95A2q9Rv98CB5A,45
+jumeaux-5.0.2.dist-info/RECORD,,
```

