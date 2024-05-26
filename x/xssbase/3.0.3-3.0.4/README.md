# Comparing `tmp/xssbase-3.0.3.tar.gz` & `tmp/xssbase-3.0.4.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-3.0.3.tar", last modified: Sun May 26 12:23:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

