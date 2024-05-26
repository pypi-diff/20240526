# Comparing `tmp/Printrun-2.0.1.tar.gz` & `tmp/Printrun-2.1.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Printrun-2.0.1.tar", last modified: Wed May 24 08:25:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

