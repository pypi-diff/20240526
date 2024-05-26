# Comparing `tmp/half_orm-0.9.8.tar.gz` & `tmp/half_orm-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "half_orm-0.9.8.tar", last modified: Tue Feb  6 09:04:13 2024, max compression
+gzip compressed data, was "half_orm-0.9.9.tar", last modified: Thu Feb 22 08:35:06 2024, max compression
```

## Comparing `half_orm-0.9.8.tar` & `half_orm-0.9.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.170532 half_orm-0.9.8/
--rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-11-29 16:16:06.000000 half_orm-0.9.8/AUTHORS
--rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-11-29 16:16:06.000000 half_orm-0.9.8/LICENSE
--rw-r--r--   0 joel      (1000) joel      (1000)    27398 2024-02-06 09:04:13.170532 half_orm-0.9.8/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)    26336 2024-02-06 09:00:54.000000 half_orm-0.9.8/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.170532 half_orm-0.9.8/half_orm/
--rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5585 2023-12-22 14:48:23.000000 half_orm-0.9.8/half_orm/field.py
--rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/field_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5549 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/fkey.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3513 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/hotest.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    15040 2023-12-22 14:48:23.000000 half_orm-0.9.8/half_orm/model.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1143 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/model_errors.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      405 2023-12-22 14:48:23.000000 half_orm-0.9.8/half_orm/null.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.170532 half_orm-0.9.8/half_orm/packager/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4166 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/changelog.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4527 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/database.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4643 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/db_conn.py
--rw-r--r--   0 joel      (1000) joel      (1000)     7485 2024-02-06 07:59:23.000000 half_orm-0.9.8/half_orm/packager/hgit.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     5364 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/hop.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1265 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/manifest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     8813 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/modules.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    13474 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/patch.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.170532 half_orm-0.9.8/half_orm/packager/patches/
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.166532 half_orm-0.9.8/half_orm/packager/patches/0/
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.166532 half_orm-0.9.8/half_orm/packager/patches/0/1/
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.170532 half_orm-0.9.8/half_orm/packager/patches/0/1/0/
--rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
--rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
--rw-r--r--   0 joel      (1000) joel      (1000)      306 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/patches/0/1/0/02_half_orm_meta.view.hop_penultimate_release.sql
--rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/patches/log
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.170532 half_orm-0.9.8/half_orm/packager/patches/sql/
--rw-r--r--   0 joel      (1000) joel      (1000)     5864 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/patches/sql/half_orm_meta.sql
--rw-r--r--   0 joel      (1000) joel      (1000)     8661 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/repo.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.170532 half_orm-0.9.8/half_orm/packager/templates/
--rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/.gitignore
--rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/MANIFEST.in
--rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/Pipfile
--rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/README
--rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/base_test
--rw-r--r--   0 joel      (1000) joel      (1000)      169 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/init_module_template
--rw-r--r--   0 joel      (1000) joel      (1000)      220 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/module_template_1
--rw-r--r--   0 joel      (1000) joel      (1000)      108 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/module_template_2
--rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/module_template_3
--rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/relation_test
--rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/setup.py
--rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/packager/templates/warning
--rw-r--r--   0 joel      (1000) joel      (1000)        8 2024-02-06 09:01:21.000000 half_orm-0.9.8/half_orm/packager/version.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)    17049 2023-12-22 14:48:23.000000 half_orm-0.9.8/half_orm/pg_meta.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    40084 2023-12-22 14:48:23.000000 half_orm-0.9.8/half_orm/relation.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1520 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/relation_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3867 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/relation_factory.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2743 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/transaction.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2135 2023-11-29 16:16:06.000000 half_orm-0.9.8/half_orm/utils.py
--rw-r--r--   0 joel      (1000) joel      (1000)        6 2024-02-06 09:01:39.000000 half_orm-0.9.8/half_orm/version.txt
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-06 09:04:13.170532 half_orm-0.9.8/half_orm.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)    27398 2024-02-06 09:04:13.000000 half_orm-0.9.8/half_orm.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)     1660 2024-02-06 09:04:13.000000 half_orm-0.9.8/half_orm.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2024-02-06 09:04:13.000000 half_orm-0.9.8/half_orm.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       51 2024-02-06 09:04:13.000000 half_orm-0.9.8/half_orm.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       46 2024-02-06 09:04:13.000000 half_orm-0.9.8/half_orm.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       27 2024-02-06 09:04:13.000000 half_orm-0.9.8/half_orm.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-11-29 16:16:06.000000 half_orm-0.9.8/pyproject.toml
--rw-rw-r--   0 joel      (1000) joel      (1000)       38 2024-02-06 09:04:13.170532 half_orm-0.9.8/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-11-29 16:16:06.000000 half_orm-0.9.8/setup.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/
+-rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-11-29 16:16:06.000000 half_orm-0.9.9/AUTHORS
+-rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-11-29 16:16:06.000000 half_orm-0.9.9/LICENSE
+-rw-r--r--   0 joel      (1000) joel      (1000)    27398 2024-02-22 08:35:06.817550 half_orm-0.9.9/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)    26336 2024-02-22 08:22:34.000000 half_orm-0.9.9/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm/
+-rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5585 2023-12-22 14:48:23.000000 half_orm-0.9.9/half_orm/field.py
+-rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/field_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5549 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/fkey.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3513 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/hotest.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    15040 2023-12-22 14:48:23.000000 half_orm-0.9.9/half_orm/model.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1143 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/model_errors.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      405 2023-12-22 14:48:23.000000 half_orm-0.9.9/half_orm/null.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm/packager/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4166 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/changelog.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4527 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/database.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4643 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/db_conn.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     7485 2024-02-06 07:59:23.000000 half_orm-0.9.9/half_orm/packager/hgit.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     5364 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/hop.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1265 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/manifest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     8813 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/modules.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    13474 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/patch.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm/packager/patches/
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm/packager/patches/0/
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm/packager/patches/0/1/
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm/packager/patches/0/1/0/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)      306 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/patches/0/1/0/02_half_orm_meta.view.hop_penultimate_release.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/patches/log
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm/packager/patches/sql/
+-rw-r--r--   0 joel      (1000) joel      (1000)     5864 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/patches/sql/half_orm_meta.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)     8661 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/repo.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm/packager/templates/
+-rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/.gitignore
+-rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/MANIFEST.in
+-rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/Pipfile
+-rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/README
+-rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/base_test
+-rw-r--r--   0 joel      (1000) joel      (1000)      169 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/init_module_template
+-rw-r--r--   0 joel      (1000) joel      (1000)      220 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/module_template_1
+-rw-r--r--   0 joel      (1000) joel      (1000)      108 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/module_template_2
+-rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/module_template_3
+-rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/relation_test
+-rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/setup.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/packager/templates/warning
+-rw-r--r--   0 joel      (1000) joel      (1000)        8 2024-02-06 09:01:21.000000 half_orm-0.9.9/half_orm/packager/version.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)    17049 2023-12-22 14:48:23.000000 half_orm-0.9.9/half_orm/pg_meta.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    40084 2023-12-22 14:48:23.000000 half_orm-0.9.9/half_orm/relation.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1520 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/relation_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3867 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/relation_factory.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2743 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/transaction.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2135 2023-11-29 16:16:06.000000 half_orm-0.9.9/half_orm/utils.py
+-rw-r--r--   0 joel      (1000) joel      (1000)        6 2024-02-22 08:22:39.000000 half_orm-0.9.9/half_orm/version.txt
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-02-22 08:35:06.817550 half_orm-0.9.9/half_orm.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)    27398 2024-02-22 08:35:06.000000 half_orm-0.9.9/half_orm.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)     1660 2024-02-22 08:35:06.000000 half_orm-0.9.9/half_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2024-02-22 08:35:06.000000 half_orm-0.9.9/half_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       51 2024-02-22 08:35:06.000000 half_orm-0.9.9/half_orm.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       46 2024-02-22 08:35:06.000000 half_orm-0.9.9/half_orm.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       27 2024-02-22 08:35:06.000000 half_orm-0.9.9/half_orm.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-11-29 16:16:06.000000 half_orm-0.9.9/pyproject.toml
+-rw-rw-r--   0 joel      (1000) joel      (1000)       38 2024-02-22 08:35:06.817550 half_orm-0.9.9/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-11-29 16:16:06.000000 half_orm-0.9.9/setup.py
```

### Comparing `half_orm-0.9.8/LICENSE` & `half_orm-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/PKG-INFO` & `half_orm-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half_orm
-Version: 0.9.8
+Version: 0.9.9
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 License-File: AUTHORS
 Requires-Dist: psycopg2-binary
 Requires-Dist: PyYAML
 Requires-Dist: pydash
 Requires-Dist: click
 Requires-Dist: GitPython
 
-# A simple PostgreSQL to Python mapper [0.9.8] and its packager [0.1.0a7]
+# A simple PostgreSQL to Python mapper [0.9.9] and its packager [0.1.0a7]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
 ![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
```

### Comparing `half_orm-0.9.8/README.md` & `half_orm-0.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# A simple PostgreSQL to Python mapper [0.9.8] and its packager [0.1.0a7]
+# A simple PostgreSQL to Python mapper [0.9.9] and its packager [0.1.0a7]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
 ![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
```

### Comparing `half_orm-0.9.8/half_orm/field.py` & `half_orm-0.9.9/half_orm/field.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/fkey.py` & `half_orm-0.9.9/half_orm/fkey.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/hotest.py` & `half_orm-0.9.9/half_orm/hotest.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/model.py` & `half_orm-0.9.9/half_orm/model.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/model_errors.py` & `half_orm-0.9.9/half_orm/model_errors.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/changelog.py` & `half_orm-0.9.9/half_orm/packager/changelog.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/database.py` & `half_orm-0.9.9/half_orm/packager/database.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/db_conn.py` & `half_orm-0.9.9/half_orm/packager/db_conn.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/hgit.py` & `half_orm-0.9.9/half_orm/packager/hgit.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/hop.py` & `half_orm-0.9.9/half_orm/packager/hop.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/manifest.py` & `half_orm-0.9.9/half_orm/packager/manifest.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/modules.py` & `half_orm-0.9.9/half_orm/packager/modules.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/patch.py` & `half_orm-0.9.9/half_orm/packager/patch.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql` & `half_orm-0.9.9/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/patches/sql/half_orm_meta.sql` & `half_orm-0.9.9/half_orm/packager/patches/sql/half_orm_meta.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/repo.py` & `half_orm-0.9.9/half_orm/packager/repo.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/templates/README` & `half_orm-0.9.9/half_orm/packager/templates/README`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/packager/templates/setup.py` & `half_orm-0.9.9/half_orm/packager/templates/setup.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/pg_meta.py` & `half_orm-0.9.9/half_orm/pg_meta.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/relation.py` & `half_orm-0.9.9/half_orm/relation.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/relation_errors.py` & `half_orm-0.9.9/half_orm/relation_errors.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/relation_factory.py` & `half_orm-0.9.9/half_orm/relation_factory.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/transaction.py` & `half_orm-0.9.9/half_orm/transaction.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm/utils.py` & `half_orm-0.9.9/half_orm/utils.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/half_orm.egg-info/PKG-INFO` & `half_orm-0.9.9/half_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half_orm
-Version: 0.9.8
+Version: 0.9.9
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 License-File: AUTHORS
 Requires-Dist: psycopg2-binary
 Requires-Dist: PyYAML
 Requires-Dist: pydash
 Requires-Dist: click
 Requires-Dist: GitPython
 
-# A simple PostgreSQL to Python mapper [0.9.8] and its packager [0.1.0a7]
+# A simple PostgreSQL to Python mapper [0.9.9] and its packager [0.1.0a7]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/badge/Python-%20&ge;%203.7-blue)
 ![PostgreSQL versions](https://img.shields.io/badge/PostgreSQL-%20&ge;%209.6-blue)
 ![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
 ![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
```

### Comparing `half_orm-0.9.8/half_orm.egg-info/SOURCES.txt` & `half_orm-0.9.9/half_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `half_orm-0.9.8/setup.py` & `half_orm-0.9.9/setup.py`

 * *Files identical despite different names*

