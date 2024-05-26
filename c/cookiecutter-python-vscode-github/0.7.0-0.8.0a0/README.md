# Comparing `tmp/cookiecutter_python_vscode_github-0.7.0.tar.gz` & `tmp/cookiecutter_python_vscode_github-0.8.0a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter_python_vscode_github-0.7.0.tar", last modified: Thu May  2 00:12:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

