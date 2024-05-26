# Comparing `tmp/owlmixin-6.2.1-py3-none-any.whl.zip` & `tmp/owlmixin-6.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -3,12 +3,12 @@
 -rw-r--r--  2.0 unx     3228 b- defN 80-Jan-01 00:00 owlmixin/errors.py
 -rw-r--r--  2.0 unx    26711 b- defN 80-Jan-01 00:00 owlmixin/owlcollections.py
 -rw-r--r--  2.0 unx     1443 b- defN 80-Jan-01 00:00 owlmixin/owlenum.py
 -rw-r--r--  2.0 unx     4435 b- defN 80-Jan-01 00:00 owlmixin/owloption.py
 -rw-r--r--  2.0 unx      796 b- defN 80-Jan-01 00:00 owlmixin/samples.py
 -rw-r--r--  2.0 unx    15771 b- defN 80-Jan-01 00:00 owlmixin/transformers.py
 -rw-r--r--  2.0 unx     8204 b- defN 80-Jan-01 00:00 owlmixin/util.py
--rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 owlmixin-6.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5777 b- defN 80-Jan-01 00:00 owlmixin-6.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 owlmixin-6.2.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      919 b- defN 16-Jan-01 00:00 owlmixin-6.2.1.dist-info/RECORD
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 owlmixin-6.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5777 b- defN 80-Jan-01 00:00 owlmixin-6.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 owlmixin-6.2.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx      919 b- defN 16-Jan-01 00:00 owlmixin-6.2.2.dist-info/RECORD
 12 files, 103717 bytes uncompressed, 18940 bytes compressed:  81.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: owlmixin/transformers.py
 Comment: 
 
 Filename: owlmixin/util.py
 Comment: 
 
-Filename: owlmixin-6.2.1.dist-info/LICENSE
+Filename: owlmixin-6.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: owlmixin-6.2.1.dist-info/METADATA
+Filename: owlmixin-6.2.2.dist-info/METADATA
 Comment: 
 
-Filename: owlmixin-6.2.1.dist-info/WHEEL
+Filename: owlmixin-6.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: owlmixin-6.2.1.dist-info/RECORD
+Filename: owlmixin-6.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `owlmixin-6.2.1.dist-info/LICENSE` & `owlmixin-6.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `owlmixin-6.2.1.dist-info/METADATA` & `owlmixin-6.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlmixin
-Version: 6.2.1
+Version: 6.2.2
 Summary: Mixin which converts ``data class instance`` and others each other more simple.
 Home-page: https://github.com/tadashi-aikawa/owlmixin
 License: MIT
 Keywords: dict,json,yaml,parser,mixin
 Author: tadashi-aikawa
 Author-email: syou.maman@gmail.com
 Requires-Python: >=3.8,<4.0
```

## Comparing `owlmixin-6.2.1.dist-info/RECORD` & `owlmixin-6.2.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 owlmixin/errors.py,sha256=jtqoVSk1D9AMP1Wi76qD5dETWJLrHkTyfRpFoFw3jqM,3228
 owlmixin/owlcollections.py,sha256=4dHCJLuWiOBJtTdcnhbX6DRtefMYBU3A0v0edBIbE2M,26711
 owlmixin/owlenum.py,sha256=8cBUbv1deBuMbpOsVIp0UEdVaq9-xi1s5lROQlwqaJk,1443
 owlmixin/owloption.py,sha256=PvW_aY64utzo7IAhy9pWx1eWDBTGghCQ4ojcc3yzjeg,4435
 owlmixin/samples.py,sha256=410ugbfgk-MRMhYLL8hvTcaVdBFwCJHJFWH9mLtTFSw,796
 owlmixin/transformers.py,sha256=yayFPoFVJ0zcqZQW6HafAxeBO4ao9mDBaMNAStEUmy8,15771
 owlmixin/util.py,sha256=F6kCR1W-cM29qovTqNSO54LTKNPY9eLGfcmN1debwOg,8204
-owlmixin-6.2.1.dist-info/LICENSE,sha256=m8HbUtjSkJ7qDYcQDtCkQBGvx-w0aL-UEUiA2J0tSrg,1071
-owlmixin-6.2.1.dist-info/METADATA,sha256=gO71n5BKDlSr3meCofhkV_diXWL_MmN6indXFtfxZ_g,5777
-owlmixin-6.2.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-owlmixin-6.2.1.dist-info/RECORD,,
+owlmixin-6.2.2.dist-info/LICENSE,sha256=m8HbUtjSkJ7qDYcQDtCkQBGvx-w0aL-UEUiA2J0tSrg,1071
+owlmixin-6.2.2.dist-info/METADATA,sha256=YhykwNcpHntW0uuAV9CTrqNVeKIhVKdOf3vojZZoknE,5777
+owlmixin-6.2.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+owlmixin-6.2.2.dist-info/RECORD,,
```

