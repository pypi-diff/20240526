# Comparing `tmp/heatmap_cli-0.9.2.tar.gz` & `tmp/heatmap_cli-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatmap_cli-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "heatmap_cli-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `heatmap_cli-0.9.2.tar` & `heatmap_cli-0.9.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      262 2024-01-15 16:49:13.849832 heatmap_cli-0.9.2/.coveragerc
--rw-r--r--   0        0        0     3108 2023-09-01 10:19:26.293033 heatmap_cli-0.9.2/.gitignore
--rw-r--r--   0        0        0     2932 2024-01-05 04:30:36.855297 heatmap_cli-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       36 2023-12-28 08:52:51.352603 heatmap_cli-0.9.2/.python-version
--rw-r--r--   0        0        0     7830 2024-01-21 07:21:54.568631 heatmap_cli-0.9.2/CHANGELOG.md
--rw-r--r--   0        0        0     2913 2024-01-08 19:19:14.452954 heatmap_cli-0.9.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/LICENSE.md
--rw-r--r--   0        0        0      566 2023-12-27 09:14:12.415426 heatmap_cli-0.9.2/Pipfile
--rw-r--r--   0        0        0   139806 2024-01-20 10:59:48.370512 heatmap_cli-0.9.2/Pipfile.lock
--rw-r--r--   0        0        0     5061 2024-01-15 17:08:58.339656 heatmap_cli-0.9.2/README.md
--rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/docs/Makefile
--rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/docs/source/_static/logo.jpg
--rw-r--r--   0        0        0     1555 2024-01-02 17:09:12.600466 heatmap_cli-0.9.2/docs/source/conf.py
--rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.9.2/docs/source/index.rst
--rw-r--r--   0        0        0      785 2024-01-21 07:22:06.064843 heatmap_cli-0.9.2/heatmap_cli/__init__.py
--rw-r--r--   0        0        0      842 2024-01-01 16:18:02.442090 heatmap_cli-0.9.2/heatmap_cli/__main__.py
--rw-r--r--   0        0        0    16950 2024-01-15 17:09:45.525438 heatmap_cli-0.9.2/heatmap_cli/cli.py
--rw-r--r--   0        0        0     1156 2023-12-22 19:55:48.738462 heatmap_cli-0.9.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0      944 2023-11-26 08:28:13.575524 heatmap_cli-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0    11620 2024-01-07 08:02:50.696917 heatmap_cli-0.9.2/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      308 2023-12-10 08:07:08.205127 heatmap_cli-0.9.2/tests/test_annotate_flag.py
--rw-r--r--   0        0        0      262 2023-10-29 07:33:51.465372 heatmap_cli-0.9.2/tests/test_cbar_flag.py
--rw-r--r--   0        0        0      704 2023-10-29 07:33:51.501374 heatmap_cli-0.9.2/tests/test_cmap_option.py
--rw-r--r--   0        0        0      432 2024-01-07 07:57:51.786434 heatmap_cli-0.9.2/tests/test_cmax_option.py
--rw-r--r--   0        0        0      428 2024-01-07 07:57:51.778434 heatmap_cli-0.9.2/tests/test_cmin_option.py
--rw-r--r--   0        0        0      717 2023-10-29 07:33:51.501374 heatmap_cli-0.9.2/tests/test_debug_flag.py
--rw-r--r--   0        0        0      382 2023-12-27 09:38:12.126646 heatmap_cli-0.9.2/tests/test_demo_option.py
--rw-r--r--   0        0        0      281 2023-12-27 09:38:16.014675 heatmap_cli-0.9.2/tests/test_help_flag.py
--rw-r--r--   0        0        0      333 2024-01-07 08:03:25.201194 heatmap_cli-0.9.2/tests/test_output_dir_option.py
--rw-r--r--   0        0        0     1143 2023-12-02 07:03:39.906801 heatmap_cli-0.9.2/tests/test_purge_flag.py
--rw-r--r--   0        0        0      527 2023-10-29 07:33:51.477373 heatmap_cli-0.9.2/tests/test_quiet_flag.py
--rw-r--r--   0        0        0      925 2023-12-27 09:41:39.927589 heatmap_cli-0.9.2/tests/test_title_option.py
--rw-r--r--   0        0        0      504 2023-10-29 07:33:51.501374 heatmap_cli-0.9.2/tests/test_verbose_flag.py
--rw-r--r--   0        0        0      261 2023-10-29 07:33:51.465372 heatmap_cli-0.9.2/tests/test_version_flag.py
--rw-r--r--   0        0        0      535 2024-01-07 08:03:57.689453 heatmap_cli-0.9.2/tests/test_week_option.py
--rw-r--r--   0        0        0      477 2023-10-29 07:33:51.501374 heatmap_cli-0.9.2/tests/test_year_option.py
--rw-r--r--   0        0        0      259 2023-11-19 06:26:47.998517 heatmap_cli-0.9.2/tests/test_yes_flag.py
--rw-r--r--   0        0        0      658 2023-10-11 17:53:17.567924 heatmap_cli-0.9.2/tox.ini
--rw-r--r--   0        0        0     6110 1970-01-01 00:00:00.000000 heatmap_cli-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      262 2024-01-15 16:49:13.849832 heatmap_cli-0.9.3/.coveragerc
+-rw-r--r--   0        0        0     3108 2023-09-01 10:19:26.293033 heatmap_cli-0.9.3/.gitignore
+-rw-r--r--   0        0        0     2931 2024-01-26 19:48:47.301088 heatmap_cli-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       36 2023-12-28 08:52:51.352603 heatmap_cli-0.9.3/.python-version
+-rw-r--r--   0        0        0     7935 2024-01-28 12:12:10.743045 heatmap_cli-0.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2913 2024-01-08 19:19:14.452954 heatmap_cli-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/LICENSE.md
+-rw-r--r--   0        0        0      566 2023-12-27 09:14:12.415426 heatmap_cli-0.9.3/Pipfile
+-rw-r--r--   0        0        0   139806 2024-01-27 20:08:07.278397 heatmap_cli-0.9.3/Pipfile.lock
+-rw-r--r--   0        0        0     5157 2024-01-21 17:49:09.178032 heatmap_cli-0.9.3/README.md
+-rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/docs/source/_static/logo.jpg
+-rw-r--r--   0        0        0     1555 2024-01-02 17:09:12.600466 heatmap_cli-0.9.3/docs/source/conf.py
+-rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.9.3/docs/source/index.rst
+-rw-r--r--   0        0        0      785 2024-01-28 12:12:53.907379 heatmap_cli-0.9.3/heatmap_cli/__init__.py
+-rw-r--r--   0        0        0      842 2024-01-01 16:18:02.442090 heatmap_cli-0.9.3/heatmap_cli/__main__.py
+-rw-r--r--   0        0        0    16942 2024-01-22 20:48:19.902245 heatmap_cli-0.9.3/heatmap_cli/cli.py
+-rw-r--r--   0        0        0     1156 2023-12-22 19:55:48.738462 heatmap_cli-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0      944 2023-11-26 08:28:13.575524 heatmap_cli-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0    11620 2024-01-07 08:02:50.696917 heatmap_cli-0.9.3/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      308 2023-12-10 08:07:08.205127 heatmap_cli-0.9.3/tests/test_annotate_flag.py
+-rw-r--r--   0        0        0      262 2023-10-29 07:33:51.465372 heatmap_cli-0.9.3/tests/test_cbar_flag.py
+-rw-r--r--   0        0        0      704 2023-10-29 07:33:51.501374 heatmap_cli-0.9.3/tests/test_cmap_option.py
+-rw-r--r--   0        0        0      432 2024-01-07 07:57:51.786434 heatmap_cli-0.9.3/tests/test_cmax_option.py
+-rw-r--r--   0        0        0      428 2024-01-07 07:57:51.778434 heatmap_cli-0.9.3/tests/test_cmin_option.py
+-rw-r--r--   0        0        0      717 2023-10-29 07:33:51.501374 heatmap_cli-0.9.3/tests/test_debug_flag.py
+-rw-r--r--   0        0        0      382 2023-12-27 09:38:12.126646 heatmap_cli-0.9.3/tests/test_demo_option.py
+-rw-r--r--   0        0        0      281 2023-12-27 09:38:16.014675 heatmap_cli-0.9.3/tests/test_help_flag.py
+-rw-r--r--   0        0        0      333 2024-01-07 08:03:25.201194 heatmap_cli-0.9.3/tests/test_output_dir_option.py
+-rw-r--r--   0        0        0     1143 2023-12-02 07:03:39.906801 heatmap_cli-0.9.3/tests/test_purge_flag.py
+-rw-r--r--   0        0        0      527 2023-10-29 07:33:51.477373 heatmap_cli-0.9.3/tests/test_quiet_flag.py
+-rw-r--r--   0        0        0      925 2023-12-27 09:41:39.927589 heatmap_cli-0.9.3/tests/test_title_option.py
+-rw-r--r--   0        0        0      504 2023-10-29 07:33:51.501374 heatmap_cli-0.9.3/tests/test_verbose_flag.py
+-rw-r--r--   0        0        0      261 2023-10-29 07:33:51.465372 heatmap_cli-0.9.3/tests/test_version_flag.py
+-rw-r--r--   0        0        0      535 2024-01-07 08:03:57.689453 heatmap_cli-0.9.3/tests/test_week_option.py
+-rw-r--r--   0        0        0      477 2023-10-29 07:33:51.501374 heatmap_cli-0.9.3/tests/test_year_option.py
+-rw-r--r--   0        0        0      259 2023-11-19 06:26:47.998517 heatmap_cli-0.9.3/tests/test_yes_flag.py
+-rw-r--r--   0        0        0      658 2023-10-11 17:53:17.567924 heatmap_cli-0.9.3/tox.ini
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 heatmap_cli-0.9.3/PKG-INFO
```

### Comparing `heatmap_cli-0.9.2/.gitignore` & `heatmap_cli-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/.pre-commit-config.yaml` & `heatmap_cli-0.9.3/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - id: debug-statements
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.16
     hooks:
       - id: validate-pyproject
         name: validate-pyproject
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
@@ -44,15 +44,15 @@
           - isort[pyproject]
         args:
           - --profile=black
           - --line-length=79
           - --py=312
 
   - repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.1.0
     hooks:
       - id: black
         args:
           - --line-length=79
           - --target-version=py38
           - --target-version=py39
           - --target-version=py310
```

### Comparing `heatmap_cli-0.9.2/CHANGELOG.md` & `heatmap_cli-0.9.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [0-based versioning](https://0ver.org/).
 
 ## [Unreleased]
 
+## v0.9.3 (2024-01-28)
+
+### Added
+
+- Add instruction on upgrade
+
+### Fixed
+
+- Fix incorrect return type
+
 ## v0.9.2 (2024-01-21)
 
 ### Fixed
 
 - Fix incorrect long title option name
 
 ### Changed
```

### Comparing `heatmap_cli-0.9.2/CONTRIBUTING.md` & `heatmap_cli-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/LICENSE.md` & `heatmap_cli-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/Pipfile` & `heatmap_cli-0.9.3/Pipfile`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/Pipfile.lock` & `heatmap_cli-0.9.3/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978328024758291%*

 * *Differences: {"'default'": "{'seaborn': {'hashes': "*

 * *              "['sha256:636f8336facf092165e27924f223d3c62ca560b1f2bb5dff7ab7fad265361987', "*

 * *              "'sha256:93e60a40988f4d65e9f4885df477e2fdaff6b73a9ded434c1ab356dd57eefff7'], "*

 * *              "'version': '==0.13.2'}}",*

 * * "'develop'": "{'coverage': {'hashes': "*

 * *              "['sha256:0193657651f5399d433c92f8ae264aff31fc1d066deee4b831549526433f3f61', "*

 * *              "'sha256:02f2edb575d62172aa28fe00efe821ae31f25dc3d589055b3fb64d51e52e4ab1', "*

 * *              "'sha […]*

```diff
@@ -471,20 +471,20 @@
                 "sha256:7b4fddbeb94a1eba4b557da24f19fdf9db575192544270a9101d8509f9f43d7b",
                 "sha256:ce42d816b81b68506614c11e8937d3aa9e41007ceb50bfdcb0749b921bf646c7"
             ],
             "version": "==2023.3.post1"
         },
         "seaborn": {
             "hashes": [
-                "sha256:6baa69b6d1169ae59037971491c450c0b73332b42bd4b23570b62a546bc61cb8",
-                "sha256:bfad65e9c5989e5e1897e61bdbd2f22e62455940ca76fd49eca3ed69345b9179"
+                "sha256:636f8336facf092165e27924f223d3c62ca560b1f2bb5dff7ab7fad265361987",
+                "sha256:93e60a40988f4d65e9f4885df477e2fdaff6b73a9ded434c1ab356dd57eefff7"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==0.13.1"
+            "version": "==0.13.2"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -695,69 +695,69 @@
             "version": "==1.1.1"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:04387a4a6ecb330c1878907ce0dc04078ea72a869263e53c72a1ba5bbdf380ca",
-                "sha256:0676cd0ba581e514b7f726495ea75aba3eb20899d824636c6f59b0ed2f88c471",
-                "sha256:0e8d06778e8fbffccfe96331a3946237f87b1e1d359d7fbe8b06b96c95a5407a",
-                "sha256:0eb3c2f32dabe3a4aaf6441dde94f35687224dfd7eb2a7f47f3fd9428e421058",
-                "sha256:109f5985182b6b81fe33323ab4707011875198c41964f014579cf82cebf2bb85",
-                "sha256:13eaf476ec3e883fe3e5fe3707caeb88268a06284484a3daf8250259ef1ba143",
-                "sha256:164fdcc3246c69a6526a59b744b62e303039a81e42cfbbdc171c91a8cc2f9446",
-                "sha256:26776ff6c711d9d835557ee453082025d871e30b3fd6c27fcef14733f67f0590",
-                "sha256:26f66da8695719ccf90e794ed567a1549bb2644a706b41e9f6eae6816b398c4a",
-                "sha256:29f3abe810930311c0b5d1a7140f6395369c3db1be68345638c33eec07535105",
-                "sha256:316543f71025a6565677d84bc4df2114e9b6a615aa39fb165d697dba06a54af9",
-                "sha256:36b0ea8ab20d6a7564e89cb6135920bc9188fb5f1f7152e94e8300b7b189441a",
-                "sha256:3cc9d4bc55de8003663ec94c2f215d12d42ceea128da8f0f4036235a119c88ac",
-                "sha256:485e9f897cf4856a65a57c7f6ea3dc0d4e6c076c87311d4bc003f82cfe199d25",
-                "sha256:5040148f4ec43644702e7b16ca864c5314ccb8ee0751ef617d49aa0e2d6bf4f2",
-                "sha256:51456e6fa099a8d9d91497202d9563a320513fcf59f33991b0661a4a6f2ad450",
-                "sha256:53d7d9158ee03956e0eadac38dfa1ec8068431ef8058fe6447043db1fb40d932",
-                "sha256:5a10a4920def78bbfff4eff8a05c51be03e42f1c3735be42d851f199144897ba",
-                "sha256:5b14b4f8760006bfdb6e08667af7bc2d8d9bfdb648351915315ea17645347137",
-                "sha256:5b2ccb7548a0b65974860a78c9ffe1173cfb5877460e5a229238d985565574ae",
-                "sha256:697d1317e5290a313ef0d369650cfee1a114abb6021fa239ca12b4849ebbd614",
-                "sha256:6ae8c9d301207e6856865867d762a4b6fd379c714fcc0607a84b92ee63feff70",
-                "sha256:707c0f58cb1712b8809ece32b68996ee1e609f71bd14615bd8f87a1293cb610e",
-                "sha256:74775198b702868ec2d058cb92720a3c5a9177296f75bd97317c787daf711505",
-                "sha256:756ded44f47f330666843b5781be126ab57bb57c22adbb07d83f6b519783b870",
-                "sha256:76f03940f9973bfaee8cfba70ac991825611b9aac047e5c80d499a44079ec0bc",
-                "sha256:79287fd95585ed36e83182794a57a46aeae0b64ca53929d1176db56aacc83451",
-                "sha256:799c8f873794a08cdf216aa5d0531c6a3747793b70c53f70e98259720a6fe2d7",
-                "sha256:7d360587e64d006402b7116623cebf9d48893329ef035278969fa3bbf75b697e",
-                "sha256:80b5ee39b7f0131ebec7968baa9b2309eddb35b8403d1869e08f024efd883566",
-                "sha256:815ac2d0f3398a14286dc2cea223a6f338109f9ecf39a71160cd1628786bc6f5",
-                "sha256:83c2dda2666fe32332f8e87481eed056c8b4d163fe18ecc690b02802d36a4d26",
-                "sha256:846f52f46e212affb5bcf131c952fb4075b55aae6b61adc9856222df89cbe3e2",
-                "sha256:936d38794044b26c99d3dd004d8af0035ac535b92090f7f2bb5aa9c8e2f5cd42",
-                "sha256:9864463c1c2f9cb3b5db2cf1ff475eed2f0b4285c2aaf4d357b69959941aa555",
-                "sha256:995ea5c48c4ebfd898eacb098164b3cc826ba273b3049e4a889658548e321b43",
-                "sha256:a1526d265743fb49363974b7aa8d5899ff64ee07df47dd8d3e37dcc0818f09ed",
-                "sha256:a56de34db7b7ff77056a37aedded01b2b98b508227d2d0979d373a9b5d353daa",
-                "sha256:a7c97726520f784239f6c62506bc70e48d01ae71e9da128259d61ca5e9788516",
-                "sha256:b8e99f06160602bc64da35158bb76c73522a4010f0649be44a4e167ff8555952",
-                "sha256:bb1de682da0b824411e00a0d4da5a784ec6496b6850fdf8c865c1d68c0e318dd",
-                "sha256:bf477c355274a72435ceb140dc42de0dc1e1e0bf6e97195be30487d8eaaf1a09",
-                "sha256:bf635a52fc1ea401baf88843ae8708591aa4adff875e5c23220de43b1ccf575c",
-                "sha256:bfd5db349d15c08311702611f3dccbef4b4e2ec148fcc636cf8739519b4a5c0f",
-                "sha256:c530833afc4707fe48524a44844493f36d8727f04dcce91fb978c414a8556cc6",
-                "sha256:cc6d65b21c219ec2072c1293c505cf36e4e913a3f936d80028993dd73c7906b1",
-                "sha256:cd3c1e4cb2ff0083758f09be0f77402e1bdf704adb7f89108007300a6da587d0",
-                "sha256:cfd2a8b6b0d8e66e944d47cdec2f47c48fef2ba2f2dff5a9a75757f64172857e",
-                "sha256:d0ca5c71a5a1765a0f8f88022c52b6b8be740e512980362f7fdbb03725a0d6b9",
-                "sha256:e7defbb9737274023e2d7af02cac77043c86ce88a907c58f42b580a97d5bcca9",
-                "sha256:e9d1bf53c4c8de58d22e0e956a79a5b37f754ed1ffdbf1a260d9dcfa2d8a325e",
-                "sha256:ea81d8f9691bb53f4fb4db603203029643caffc82bf998ab5b59ca05560f4c06"
+                "sha256:0193657651f5399d433c92f8ae264aff31fc1d066deee4b831549526433f3f61",
+                "sha256:02f2edb575d62172aa28fe00efe821ae31f25dc3d589055b3fb64d51e52e4ab1",
+                "sha256:0491275c3b9971cdbd28a4595c2cb5838f08036bca31765bad5e17edf900b2c7",
+                "sha256:077d366e724f24fc02dbfe9d946534357fda71af9764ff99d73c3c596001bbd7",
+                "sha256:10e88e7f41e6197ea0429ae18f21ff521d4f4490aa33048f6c6f94c6045a6a75",
+                "sha256:18e961aa13b6d47f758cc5879383d27b5b3f3dcd9ce8cdbfdc2571fe86feb4dd",
+                "sha256:1a78b656a4d12b0490ca72651fe4d9f5e07e3c6461063a9b6265ee45eb2bdd35",
+                "sha256:1ed4b95480952b1a26d863e546fa5094564aa0065e1e5f0d4d0041f293251d04",
+                "sha256:23b27b8a698e749b61809fb637eb98ebf0e505710ec46a8aa6f1be7dc0dc43a6",
+                "sha256:23f5881362dcb0e1a92b84b3c2809bdc90db892332daab81ad8f642d8ed55042",
+                "sha256:32a8d985462e37cfdab611a6f95b09d7c091d07668fdc26e47a725ee575fe166",
+                "sha256:3468cc8720402af37b6c6e7e2a9cdb9f6c16c728638a2ebc768ba1ef6f26c3a1",
+                "sha256:379d4c7abad5afbe9d88cc31ea8ca262296480a86af945b08214eb1a556a3e4d",
+                "sha256:3cacfaefe6089d477264001f90f55b7881ba615953414999c46cc9713ff93c8c",
+                "sha256:3e3424c554391dc9ef4a92ad28665756566a28fecf47308f91841f6c49288e66",
+                "sha256:46342fed0fff72efcda77040b14728049200cbba1279e0bf1188f1f2078c1d70",
+                "sha256:536d609c6963c50055bab766d9951b6c394759190d03311f3e9fcf194ca909e1",
+                "sha256:5d6850e6e36e332d5511a48a251790ddc545e16e8beaf046c03985c69ccb2676",
+                "sha256:6008adeca04a445ea6ef31b2cbaf1d01d02986047606f7da266629afee982630",
+                "sha256:64e723ca82a84053dd7bfcc986bdb34af8d9da83c521c19d6b472bc6880e191a",
+                "sha256:6b00e21f86598b6330f0019b40fb397e705135040dbedc2ca9a93c7441178e74",
+                "sha256:6d224f0c4c9c98290a6990259073f496fcec1b5cc613eecbd22786d398ded3ad",
+                "sha256:6dceb61d40cbfcf45f51e59933c784a50846dc03211054bd76b421a713dcdf19",
+                "sha256:7ac8f8eb153724f84885a1374999b7e45734bf93a87d8df1e7ce2146860edef6",
+                "sha256:85ccc5fa54c2ed64bd91ed3b4a627b9cce04646a659512a051fa82a92c04a448",
+                "sha256:869b5046d41abfea3e381dd143407b0d29b8282a904a19cb908fa24d090cc018",
+                "sha256:8bdb0285a0202888d19ec6b6d23d5990410decb932b709f2b0dfe216d031d218",
+                "sha256:8dfc5e195bbef80aabd81596ef52a1277ee7143fe419efc3c4d8ba2754671756",
+                "sha256:8e738a492b6221f8dcf281b67129510835461132b03024830ac0e554311a5c54",
+                "sha256:918440dea04521f499721c039863ef95433314b1db00ff826a02580c1f503e45",
+                "sha256:9641e21670c68c7e57d2053ddf6c443e4f0a6e18e547e86af3fad0795414a628",
+                "sha256:9d2f9d4cc2a53b38cabc2d6d80f7f9b7e3da26b2f53d48f05876fef7956b6968",
+                "sha256:a07f61fc452c43cd5328b392e52555f7d1952400a1ad09086c4a8addccbd138d",
+                "sha256:a3277f5fa7483c927fe3a7b017b39351610265308f5267ac6d4c2b64cc1d8d25",
+                "sha256:a4a3907011d39dbc3e37bdc5df0a8c93853c369039b59efa33a7b6669de04c60",
+                "sha256:aeb2c2688ed93b027eb0d26aa188ada34acb22dceea256d76390eea135083950",
+                "sha256:b094116f0b6155e36a304ff912f89bbb5067157aff5f94060ff20bbabdc8da06",
+                "sha256:b8ffb498a83d7e0305968289441914154fb0ef5d8b3157df02a90c6695978295",
+                "sha256:b9bb62fac84d5f2ff523304e59e5c439955fb3b7f44e3d7b2085184db74d733b",
+                "sha256:c61f66d93d712f6e03369b6a7769233bfda880b12f417eefdd4f16d1deb2fc4c",
+                "sha256:ca6e61dc52f601d1d224526360cdeab0d0712ec104a2ce6cc5ccef6ed9a233bc",
+                "sha256:ca7b26a5e456a843b9b6683eada193fc1f65c761b3a473941efe5a291f604c74",
+                "sha256:d12c923757de24e4e2110cf8832d83a886a4cf215c6e61ed506006872b43a6d1",
+                "sha256:d17bbc946f52ca67adf72a5ee783cd7cd3477f8f8796f59b4974a9b59cacc9ee",
+                "sha256:dfd1e1b9f0898817babf840b77ce9fe655ecbe8b1b327983df485b30df8cc011",
+                "sha256:e0860a348bf7004c812c8368d1fc7f77fe8e4c095d661a579196a9533778e156",
+                "sha256:f2f5968608b1fe2a1d00d01ad1017ee27efd99b3437e08b83ded9b7af3f6f766",
+                "sha256:f3771b23bb3675a06f5d885c3630b1d01ea6cac9e84a01aaf5508706dba546c5",
+                "sha256:f68ef3660677e6624c8cace943e4765545f8191313a07288a53d3da188bd8581",
+                "sha256:f86f368e1c7ce897bf2457b9eb61169a44e2ef797099fb5728482b8d69f3f016",
+                "sha256:f90515974b39f4dea2f27c0959688621b46d96d5a626cf9c53dbc653a895c05c",
+                "sha256:fe558371c1bdf3b8fa03e097c523fb9645b8730399c14fe7721ee9c9e2a545d3"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.4.0"
+            "version": "==7.4.1"
         },
         "cycler": {
             "hashes": [
                 "sha256:85cef7cff222d8644161529808465972e51340599459b8ac3ccbac5a854e0d30",
                 "sha256:88bb128f02ba341da8ef447245a9e138fae777f6a23943da4540077d3601eb1c"
             ],
             "markers": "python_version >= '3.8'",
@@ -1313,19 +1313,19 @@
                 "sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==4.1.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12",
-                "sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7"
+                "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981",
+                "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==1.3.0"
+            "version": "==1.4.0"
         },
         "pre-commit": {
             "hashes": [
                 "sha256:5804465c675b659b0862f07907f96295d490822a450c4c40e747d0b1c6ebcb32",
                 "sha256:841dc9aef25daba9a0238cd27984041fa0467b4199fc4852e27950664919f660"
             ],
             "index": "pypi",
@@ -1502,20 +1502,20 @@
                 "sha256:951cfc25219b0cd003493a565f2e621fd791beaae9f9a3bdd7024d8626419c38"
             ],
             "index": "pypi",
             "version": "==1.3"
         },
         "seaborn": {
             "hashes": [
-                "sha256:6baa69b6d1169ae59037971491c450c0b73332b42bd4b23570b62a546bc61cb8",
-                "sha256:bfad65e9c5989e5e1897e61bdbd2f22e62455940ca76fd49eca3ed69345b9179"
+                "sha256:636f8336facf092165e27924f223d3c62ca560b1f2bb5dff7ab7fad265361987",
+                "sha256:93e60a40988f4d65e9f4885df477e2fdaff6b73a9ded434c1ab356dd57eefff7"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==0.13.1"
+            "version": "==0.13.2"
         },
         "setuptools": {
             "hashes": [
                 "sha256:385eb4edd9c9d5c17540511303e39a147ce2fc04bc55289c322b9e5904fe2c05",
                 "sha256:be1af57fc409f93647f2e8e4573a142ed38724b8cdd389706a867bb4efcf1e78"
             ],
             "markers": "python_version >= '3.8'",
@@ -1980,20 +1980,20 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
             "version": "==7.1.2"
         },
         "sphinx-autodoc-typehints": {
             "hashes": [
-                "sha256:3cabc2537e17989b2f92e64a399425c4c8bf561ed73f087bc7414a5003616a50",
-                "sha256:5ed05017d23ad4b937eab3bee9fae9ab0dd63f0b42aa360031f1fad47e47f673"
+                "sha256:70db10b391acf4e772019765991d2de0ff30ec0899b9ba137706dc0b3c4835e0",
+                "sha256:d3da7fa9a9761eff6ff09f8b1956ae3090a2d4f4ad54aebcade8e458d6340835"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==1.25.2"
+            "version": "==1.25.3"
         },
         "sphinx-copybutton": {
             "hashes": [
                 "sha256:4cf17c82fb9646d1bc9ca92ac280813a3b605d8c421225fd9913154103ee1fbd",
                 "sha256:fb543fd386d917746c9a2c50360c7905b605726b9355cd26e9974857afeae06e"
             ],
             "index": "pypi",
```

### Comparing `heatmap_cli-0.9.2/README.md` & `heatmap_cli-0.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 
 Stable version From PyPI using `pip`:
 
 ```console
 python -m pip install heatmap_cli
 ```
 
+Upgrade to latest stable version:
+
+```console
+python3 -m pip install heatmap_cli --upgrade
+```
+
 Latest development version from GitHub:
 
 ```console
 python -m pip install -e git+https://github.com/kianmeng/heatmap_cli.git
 ```
 
 ## Usage
```

### Comparing `heatmap_cli-0.9.2/docs/Makefile` & `heatmap_cli-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/docs/make.bat` & `heatmap_cli-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/docs/source/_static/logo.jpg` & `heatmap_cli-0.9.3/docs/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/docs/source/conf.py` & `heatmap_cli-0.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/heatmap_cli/__init__.py` & `heatmap_cli-0.9.3/heatmap_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap."""
 
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
```

### Comparing `heatmap_cli-0.9.2/heatmap_cli/__main__.py` & `heatmap_cli-0.9.3/heatmap_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/heatmap_cli/cli.py` & `heatmap_cli-0.9.3/heatmap_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ) -> argparse.Namespace:
     """Parse the CLI arguments.
 
     Args:
         args (List | None): Argument passed through the command line
 
     Returns:
-        argparse.ArgumentNamespace
+        argparse.Namespace
     """
     parser = argparse.ArgumentParser(
         add_help=False,
         description=__doc__,
         formatter_class=lambda prog: argparse.RawTextHelpFormatter(
             prog,
             max_help_position=6,
```

### Comparing `heatmap_cli-0.9.2/pyproject.toml` & `heatmap_cli-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tests/conftest.py` & `heatmap_cli-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tests/fixtures/sample.csv` & `heatmap_cli-0.9.3/tests/fixtures/sample.csv`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tests/test_cmap_option.py` & `heatmap_cli-0.9.3/tests/test_cmap_option.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tests/test_debug_flag.py` & `heatmap_cli-0.9.3/tests/test_debug_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tests/test_purge_flag.py` & `heatmap_cli-0.9.3/tests/test_purge_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tests/test_quiet_flag.py` & `heatmap_cli-0.9.3/tests/test_quiet_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tests/test_title_option.py` & `heatmap_cli-0.9.3/tests/test_title_option.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tests/test_week_option.py` & `heatmap_cli-0.9.3/tests/test_week_option.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/tox.ini` & `heatmap_cli-0.9.3/tox.ini`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.9.2/PKG-INFO` & `heatmap_cli-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatmap_cli
-Version: 0.9.2
+Version: 0.9.3
 Summary: A console program that generates yearly calendar heatmap.
 Keywords: heatmap,cli
 Author-email: Kian-Meng Ang <kianmeng@cpan.org>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -36,14 +36,20 @@
 
 Stable version From PyPI using `pip`:
 
 ```console
 python -m pip install heatmap_cli
 ```
 
+Upgrade to latest stable version:
+
+```console
+python3 -m pip install heatmap_cli --upgrade
+```
+
 Latest development version from GitHub:
 
 ```console
 python -m pip install -e git+https://github.com/kianmeng/heatmap_cli.git
 ```
 
 ## Usage
```

