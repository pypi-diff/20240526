# Comparing `tmp/otsucfgmng-1.3.4.37.tar.gz` & `tmp/otsucfgmng-1.3.5.311-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otsucfgmng-1.3.4.37.tar", last modified: Wed Apr 26 00:05:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

