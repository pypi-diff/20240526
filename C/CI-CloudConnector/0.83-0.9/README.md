# Comparing `tmp/ci_cloudconnector-0.83.tar.gz` & `tmp/CI_CloudConnector-0.9.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.83.tar", last modified: Sun May 26 13:08:43 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

