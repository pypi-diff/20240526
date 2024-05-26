# Comparing `tmp/nanoarrow-0.4.0.tar.gz` & `tmp/nanoarrow-0.5.0-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoarrow-0.4.0.tar", last modified: Mon Jan 29 14:34:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

