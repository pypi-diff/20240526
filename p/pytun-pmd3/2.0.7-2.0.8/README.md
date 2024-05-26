# Comparing `tmp/pytun_pmd3-2.0.7.tar.gz` & `tmp/pytun_pmd3-2.0.8-cp38-cp38-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytun_pmd3-2.0.7.tar", last modified: Mon Apr 22 11:36:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

