# Comparing `tmp/stam-0.8.0.tar.gz` & `tmp/stam-0.8.1-cp39-cp39-musllinux_1_2_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

