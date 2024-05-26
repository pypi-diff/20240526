# Comparing `tmp/apache_airflow_providers_apache_spark-4.8.0rc2.tar.gz` & `tmp/apache_airflow_providers_apache_spark-4.8.1rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_spark-4.8.0rc2.tar", last modified: Tue Apr 30 11:17:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

