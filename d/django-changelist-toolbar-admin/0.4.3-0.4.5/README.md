# Comparing `tmp/django-changelist-toolbar-admin-0.4.3.tar.gz` & `tmp/django-changelist-toolbar-admin-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-changelist-toolbar-admin-0.4.3.tar", last modified: Thu Sep 14 01:56:52 2023, max compression
+gzip compressed data, was "django-changelist-toolbar-admin-0.4.5.tar", last modified: Sun May 26 02:05:37 2024, max compression
```

## Comparing `django-changelist-toolbar-admin-0.4.3.tar` & `django-changelist-toolbar-admin-0.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.903935 django-changelist-toolbar-admin-0.4.3/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      261 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     2699 2023-09-14 01:56:52.903822 django-changelist-toolbar-admin-0.4.3/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1953 2023-09-14 01:56:33.000000 django-changelist-toolbar-admin-0.4.3/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.902224 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/
--rw-r--r--   0 test       (501) staff       (20)       52 2023-07-05 08:50:38.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     2783 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/admin.py
--rw-r--r--   0 test       (501) staff       (20)      134 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.903278 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/models.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.899923 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/static/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.899963 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/static/django-changelist-toolbar-admin/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.903390 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/static/django-changelist-toolbar-admin/css/
--rw-r--r--   0 test       (501) staff       (20)       44 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/static/django-changelist-toolbar-admin/css/django-changelist-toolbar-admin.css
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.900073 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/templates/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.903608 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/templates/admin/
--rw-r--r--   0 test       (501) staff       (20)      418 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/templates/admin/change_list_object_tools.html
--rw-r--r--   0 test       (501) staff       (20)       60 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/tests.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-14 01:56:52.903160 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     2699 2023-09-14 01:56:52.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      876 2023-09-14 01:56:52.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-14 01:56:52.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-14 01:56:52.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       43 2023-09-14 01:56:52.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       32 2023-09-14 01:56:52.000000 django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       44 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.3/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-09-14 01:56:52.903972 django-changelist-toolbar-admin-0.4.3/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1626 2023-09-14 01:56:39.000000 django-changelist-toolbar-admin-0.4.3/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.718686 django-changelist-toolbar-admin-0.4.5/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-26 01:49:23.000000 django-changelist-toolbar-admin-0.4.5/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      261 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.5/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     2711 2024-05-26 02:05:37.718561 django-changelist-toolbar-admin-0.4.5/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1996 2024-05-26 02:04:16.000000 django-changelist-toolbar-admin-0.4.5/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.717133 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/
+-rw-r--r--   0 test       (501) staff       (20)       52 2023-07-05 08:50:38.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     3866 2024-05-26 02:03:59.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      134 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.717988 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/models.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.714867 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.714930 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/static/django-changelist-toolbar-admin/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.718115 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/static/django-changelist-toolbar-admin/css/
+-rw-r--r--   0 test       (501) staff       (20)       44 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/static/django-changelist-toolbar-admin/css/django-changelist-toolbar-admin.css
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.715094 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/templates/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.718279 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/templates/admin/
+-rw-r--r--   0 test       (501) staff       (20)      459 2024-05-26 01:48:18.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/templates/admin/change_list_object_tools.html
+-rw-r--r--   0 test       (501) staff       (20)       60 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/tests.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-26 02:05:37.717859 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     2711 2024-05-26 02:05:37.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      876 2024-05-26 02:05:37.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-26 02:05:37.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-26 02:05:37.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       43 2024-05-26 02:05:37.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       32 2024-05-26 02:05:37.000000 django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       44 2022-09-13 06:17:42.000000 django-changelist-toolbar-admin-0.4.5/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-26 02:05:37.718732 django-changelist-toolbar-admin-0.4.5/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1544 2024-05-26 02:04:09.000000 django-changelist-toolbar-admin-0.4.5/setup.py
```

### Comparing `django-changelist-toolbar-admin-0.4.3/LICENSE` & `django-changelist-toolbar-admin-0.4.5/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MIT License
 
-Copyright (c) 2019 zencore.cn
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-changelist-toolbar-admin-0.4.3/PKG-INFO` & `django-changelist-toolbar-admin-0.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-changelist-toolbar-admin
-Version: 0.4.3
+Version: 0.4.5
 Summary: Provides custom button management function on changelist page of django admin site.
+Home-page: UNKNOWN
 Author: Zhao Sen
-Author-email: zhaosen@zencore.cn
 Maintainer: Zhao Sen
-Maintainer-email: zhaosen@zencore.cn
 License: MIT
 Keywords: django admin extentions,django-changelist-toolbar-admin
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -76,14 +76,18 @@
 ```
 
 - A button function must returns a Button instance, dict button info, or href.
 - Another way is override `make_changelist_toolbar_button` get return the final buttons.
 
 ## Releases
 
+### v0.4.5
+
+- Add button classes support.
+
 ### v0.4.3
 
 - Doc update.
 - Add django-app-requires support.
 
 ### v0.4.0
 
@@ -97,7 +101,9 @@
 ### v0.2.0
 
 - App rename to django_changelist_toolbar_admin.
 
 ### v0.1.0
 
 - First release.
+
+
```

### Comparing `django-changelist-toolbar-admin-0.4.3/README.md` & `django-changelist-toolbar-admin-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 ```
 
 - A button function must returns a Button instance, dict button info, or href.
 - Another way is override `make_changelist_toolbar_button` get return the final buttons.
 
 ## Releases
 
+### v0.4.5
+
+- Add button classes support.
+
 ### v0.4.3
 
 - Doc update.
 - Add django-app-requires support.
 
 ### v0.4.0
```

### Comparing `django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/PKG-INFO` & `django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-changelist-toolbar-admin
-Version: 0.4.3
+Version: 0.4.5
 Summary: Provides custom button management function on changelist page of django admin site.
+Home-page: UNKNOWN
 Author: Zhao Sen
-Author-email: zhaosen@zencore.cn
 Maintainer: Zhao Sen
-Maintainer-email: zhaosen@zencore.cn
 License: MIT
 Keywords: django admin extentions,django-changelist-toolbar-admin
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -76,14 +76,18 @@
 ```
 
 - A button function must returns a Button instance, dict button info, or href.
 - Another way is override `make_changelist_toolbar_button` get return the final buttons.
 
 ## Releases
 
+### v0.4.5
+
+- Add button classes support.
+
 ### v0.4.3
 
 - Doc update.
 - Add django-app-requires support.
 
 ### v0.4.0
 
@@ -97,7 +101,9 @@
 ### v0.2.0
 
 - App rename to django_changelist_toolbar_admin.
 
 ### v0.1.0
 
 - First release.
+
+
```

### Comparing `django-changelist-toolbar-admin-0.4.3/django_changelist_toolbar_admin.egg-info/SOURCES.txt` & `django-changelist-toolbar-admin-0.4.5/django_changelist_toolbar_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-changelist-toolbar-admin-0.4.3/setup.py` & `django-changelist-toolbar-admin-0.4.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = fobj.readlines()
 requires = [x.strip() for x in requires if x.strip()]
 
 setup(
     name="django-changelist-toolbar-admin",
-    version="0.4.3",
+    version="0.4.5",
     description="Provides custom button management function on changelist page of django admin site.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Zhao Sen",
-    author_email="zhaosen@zencore.cn",
     maintainer="Zhao Sen",
-    maintainer_email="zhaosen@zencore.cn",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

