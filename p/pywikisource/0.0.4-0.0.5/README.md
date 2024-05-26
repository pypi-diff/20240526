# Comparing `tmp/pywikisource-0.0.4.tar.gz` & `tmp/pywikisource-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywikisource-0.0.4.tar", last modified: Fri Sep 10 13:20:17 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

