# Comparing `tmp/apache_airflow_providers_cloudant-3.5.0rc2.tar.gz` & `tmp/apache_airflow_providers_cloudant-3.5.1rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_cloudant-3.5.0rc2.tar", last modified: Tue Apr 30 11:19:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
