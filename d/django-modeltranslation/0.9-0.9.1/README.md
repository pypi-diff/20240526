# Comparing `tmp/django-modeltranslation-0.9.tar.gz` & `tmp/django-modeltranslation-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-modeltranslation-0.9.tar", last modified: Thu Apr 16 09:00:14 2015, max compression
+gzip compressed data, was "dist/django-modeltranslation-0.9.1.tar", last modified: Thu May 14 11:41:52 2015, max compression
```

## Comparing `django-modeltranslation-0.9.tar` & `django-modeltranslation-0.9.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/modeltranslation/
--rw-r--r--   0 deschler  (1000) deschler  (1000)     2088 2015-04-16 08:39:18.000000 django-modeltranslation-0.9/modeltranslation/__init__.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)    16825 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/fields.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)    23968 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/translator.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)    20405 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/manager.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)    18001 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/admin.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)     1345 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/forms.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)     2891 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/settings.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)      311 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/apps.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)     5317 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/utils.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)     4065 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/widgets.py
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/modeltranslation/static/
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/modeltranslation/static/modeltranslation/
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/modeltranslation/static/modeltranslation/css/
--rw-r--r--   0 deschler  (1000) deschler  (1000)     4121 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/static/modeltranslation/css/tabbed_translation_fields.css
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/modeltranslation/static/modeltranslation/js/
--rw-r--r--   0 deschler  (1000) deschler  (1000)    19670 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/static/modeltranslation/js/tabbed_translation_fields.js
--rw-r--r--   0 deschler  (1000) deschler  (1000)       45 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/static/modeltranslation/js/force_jquery.js
--rw-r--r--   0 deschler  (1000) deschler  (1000)      523 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/static/modeltranslation/js/clearable_inputs.js
--rw-r--r--   0 deschler  (1000) deschler  (1000)     3280 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/models.py
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/modeltranslation/management/
--rw-r--r--   0 deschler  (1000) deschler  (1000)        0 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/management/__init__.py
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/modeltranslation/management/commands/
--rw-r--r--   0 deschler  (1000) deschler  (1000)     5236 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/management/commands/sync_translation_fields.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)        0 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/management/commands/__init__.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)     2572 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/management/commands/loaddata.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)     1476 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/modeltranslation/management/commands/update_translation_fields.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)     1543 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/LICENSE.txt
--rw-r--r--   0 deschler  (1000) deschler  (1000)    20549 2015-04-16 08:37:46.000000 django-modeltranslation-0.9/CHANGELOG.txt
-lrwxrwxrwx   0 deschler  (1000) deschler  (1000)        0 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/README -> README.rst
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/docs/
-drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/docs/modeltranslation/
--rw-r--r--   0 deschler  (1000) deschler  (1000)     4864 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/contribute.rst
-lrwxrwxrwx   0 deschler  (1000) deschler  (1000)        0 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/readme.rst -> ../../README.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)       61 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/changelog.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)    11738 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/admin.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)     5130 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/make.bat
--rw-r--r--   0 deschler  (1000) deschler  (1000)    13893 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/usage.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)     5632 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/Makefile
--rw-r--r--   0 deschler  (1000) deschler  (1000)    14179 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/registration.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)      367 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/index.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)    12379 2015-04-16 08:40:49.000000 django-modeltranslation-0.9/docs/modeltranslation/installation.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)     3333 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/commands.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)     1485 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/caveats.rst
-lrwxrwxrwx   0 deschler  (1000) deschler  (1000)        0 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/authors.rst -> ../../AUTHORS.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)    10168 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/conf.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)     1739 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/related_projects.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)     3773 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/docs/modeltranslation/forms.rst
--rwxr-xr-x   0 deschler  (1000) deschler  (1000)     1972 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/setup.py
--rw-r--r--   0 deschler  (1000) deschler  (1000)      797 2015-04-16 08:38:57.000000 django-modeltranslation-0.9/AUTHORS.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)     2107 2015-04-16 08:30:14.000000 django-modeltranslation-0.9/README.rst
--rw-r--r--   0 deschler  (1000) deschler  (1000)     1324 2015-04-16 09:00:14.000000 django-modeltranslation-0.9/PKG-INFO
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/
+-rw-r--r--   0 deschler  (1000) deschler  (1000)      865 2015-05-14 11:39:18.000000 django-modeltranslation-0.9.1/AUTHORS.rst
+lrwxrwxrwx   0 deschler  (1000) deschler  (1000)        0 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/README -> README.rst
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/modeltranslation/
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     2088 2015-05-14 11:36:17.000000 django-modeltranslation-0.9.1/modeltranslation/__init__.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     3280 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/models.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     1345 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/forms.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)      311 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/apps.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     2891 2015-04-03 18:18:46.000000 django-modeltranslation-0.9.1/modeltranslation/settings.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     4065 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/widgets.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    18001 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/admin.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    16825 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/fields.py
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/modeltranslation/management/
+-rw-r--r--   0 deschler  (1000) deschler  (1000)        0 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/management/__init__.py
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/modeltranslation/management/commands/
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     2572 2015-05-14 11:23:21.000000 django-modeltranslation-0.9.1/modeltranslation/management/commands/loaddata.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)        0 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/management/commands/__init__.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     1476 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/management/commands/update_translation_fields.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     5440 2015-05-14 11:23:21.000000 django-modeltranslation-0.9.1/modeltranslation/management/commands/sync_translation_fields.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     5317 2015-05-14 11:23:21.000000 django-modeltranslation-0.9.1/modeltranslation/utils.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    20699 2015-05-14 11:23:21.000000 django-modeltranslation-0.9.1/modeltranslation/manager.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    24145 2015-05-14 11:23:21.000000 django-modeltranslation-0.9.1/modeltranslation/translator.py
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/modeltranslation/static/
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/css/
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     4121 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/css/tabbed_translation_fields.css
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/js/
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    19670 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/js/tabbed_translation_fields.js
+-rw-r--r--   0 deschler  (1000) deschler  (1000)       45 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/js/force_jquery.js
+-rw-r--r--   0 deschler  (1000) deschler  (1000)      523 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/js/clearable_inputs.js
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     1328 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/PKG-INFO
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     2107 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/README.rst
+-rwxr-xr-x   0 deschler  (1000) deschler  (1000)     1972 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/setup.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    21101 2015-05-14 11:35:42.000000 django-modeltranslation-0.9.1/CHANGELOG.txt
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/docs/
+drwxr-xr-x   0 deschler  (1000) deschler  (1000)        0 2015-05-14 11:41:52.000000 django-modeltranslation-0.9.1/docs/modeltranslation/
+lrwxrwxrwx   0 deschler  (1000) deschler  (1000)        0 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/authors.rst -> ../../AUTHORS.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     5130 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/make.bat
+lrwxrwxrwx   0 deschler  (1000) deschler  (1000)        0 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/readme.rst -> ../../README.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    14179 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/registration.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    13893 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/usage.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)      367 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/index.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     4864 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/contribute.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    12379 2015-05-14 11:23:21.000000 django-modeltranslation-0.9.1/docs/modeltranslation/installation.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     5632 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/Makefile
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    11738 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/admin.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     1485 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/caveats.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     1739 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/related_projects.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     3333 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/commands.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)       61 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/changelog.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)    10168 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/conf.py
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     3773 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/docs/modeltranslation/forms.rst
+-rw-r--r--   0 deschler  (1000) deschler  (1000)     1543 2015-04-02 10:06:55.000000 django-modeltranslation-0.9.1/LICENSE.txt
```

### Comparing `django-modeltranslation-0.9/modeltranslation/__init__.py` & `django-modeltranslation-0.9.1/modeltranslation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Version code adopted from Django development version.
 https://github.com/django/django
 """
-VERSION = (0, 9, 0, 'final', 0)
+VERSION = (0, 9, 1, 'final', 0)
 default_app_config = 'modeltranslation.apps.ModeltranslationConfig'
 
 
 def get_version(version=None):
     """
     Returns a PEP 386-compliant version number from VERSION.
     """
```

### Comparing `django-modeltranslation-0.9/modeltranslation/fields.py` & `django-modeltranslation-0.9.1/modeltranslation/fields.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/translator.py` & `django-modeltranslation-0.9.1/modeltranslation/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,20 @@
             # django model fields and therefore adds them via add_to_class
             model.add_to_class(localized_field_name, translation_field)
             opts.add_translation_field(field_name, translation_field)
 
     # Rebuild information about parents fields. If there are opts.local_fields, field cache would be
     # invalidated (by model._meta.add_field() function). Otherwise, we need to do it manually.
     if len(opts.local_fields) == 0:
-        model._meta._fill_fields_cache()
+        try:
+            model._meta._fill_fields_cache()
+        except AttributeError:
+            # Django 1.8 removed _fill_fields_cache
+            model._meta._expire_cache()
+            model._meta.get_fields()
 
 
 def has_custom_queryset(manager):
     "Check whether manager (or its parents) has declared some custom get_queryset method."
     old_diff = getattr(manager, 'get_query_set', None) != getattr(Manager, 'get_query_set', None)
     new_diff = getattr(manager, 'get_queryset', None) != getattr(Manager, 'get_queryset', None)
     return old_diff or new_diff
```

### Comparing `django-modeltranslation-0.9/modeltranslation/manager.py` & `django-modeltranslation-0.9.1/modeltranslation/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,19 @@
 def get_fields_to_translatable_models(model):
     if model in _F2TM_CACHE:
         return _F2TM_CACHE[model]
 
     results = []
     if NEW_META_API:
         for f in model._meta.get_fields():
-            if f.is_relation:
+            if f.is_relation and f.related_model:
+                # The new get_field() will find GenericForeignKey relations.
+                # In that case the 'related_model' attribute is set to None
+                # so it is necessary to check for this value before trying to
+                # get translatable fields.
                 if get_translatable_fields_for_model(f.related_model) is not None:
                     results.append((f.name, f.related_model))
     else:
         for field_name in model._meta.get_all_field_names():
             field_object, modelclass, direct, m2m = model._meta.get_field_by_name(field_name)
             # Direct relationship
             if direct and isinstance(field_object, RelatedField):
```

### Comparing `django-modeltranslation-0.9/modeltranslation/admin.py` & `django-modeltranslation-0.9.1/modeltranslation/admin.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/forms.py` & `django-modeltranslation-0.9.1/modeltranslation/forms.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/settings.py` & `django-modeltranslation-0.9.1/modeltranslation/settings.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/utils.py` & `django-modeltranslation-0.9.1/modeltranslation/utils.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/widgets.py` & `django-modeltranslation-0.9.1/modeltranslation/widgets.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/static/modeltranslation/css/tabbed_translation_fields.css` & `django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/css/tabbed_translation_fields.css`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/static/modeltranslation/js/tabbed_translation_fields.js` & `django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/js/tabbed_translation_fields.js`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/static/modeltranslation/js/clearable_inputs.js` & `django-modeltranslation-0.9.1/modeltranslation/static/modeltranslation/js/clearable_inputs.js`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/models.py` & `django-modeltranslation-0.9.1/modeltranslation/models.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/management/commands/sync_translation_fields.py` & `django-modeltranslation-0.9.1/modeltranslation/management/commands/sync_translation_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
     1. When you add new languages to settings.LANGUAGES.
     2. When you add new translatable fields to your models.
 
 Credits: Heavily inspired by django-transmeta's sync_transmeta_db command.
 """
 from optparse import make_option
+import django
 from django.core.management.base import NoArgsCommand
 from django.core.management.color import no_style
 from django.db import connection, transaction
 from django.utils.six import moves
 
 from modeltranslation.settings import AVAILABLE_LANGUAGES
 from modeltranslation.translator import translator
@@ -63,15 +64,19 @@
         self.introspection = connection.introspection
         self.interactive = options['interactive']
 
         found_missing_fields = False
         models = translator.get_registered_models(abstract=False)
         for model in models:
             db_table = model._meta.db_table
-            model_full_name = '%s.%s' % (model._meta.app_label, model._meta.module_name)
+            if django.VERSION < (1, 8):
+                model_name = model._meta.module_name
+            else:
+                model_name = model._meta.model_name
+            model_full_name = '%s.%s' % (model._meta.app_label, model_name)
             opts = translator.get_options_for_model(model)
             for field_name, fields in opts.local_fields.items():
                 # Take `db_column` attribute into account
                 field = list(fields)[0]
                 column_name = field.db_column if field.db_column else field_name
                 missing_langs = list(self.get_missing_languages(column_name, db_table))
                 if missing_langs:
@@ -84,15 +89,16 @@
                         print('Executing SQL...')
                         for sentence in sql_sentences:
                             self.cursor.execute(sentence)
                         print('Done')
                     else:
                         print('SQL not executed')
 
-        transaction.commit_unless_managed()
+        if django.VERSION < (1, 6):
+            transaction.commit_unless_managed()
 
         if not found_missing_fields:
             print('No new translatable fields detected')
 
     def get_table_fields(self, db_table):
         """
         Gets table fields from schema.
```

### Comparing `django-modeltranslation-0.9/modeltranslation/management/commands/loaddata.py` & `django-modeltranslation-0.9.1/modeltranslation/management/commands/loaddata.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/modeltranslation/management/commands/update_translation_fields.py` & `django-modeltranslation-0.9.1/modeltranslation/management/commands/update_translation_fields.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/LICENSE.txt` & `django-modeltranslation-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/CHANGELOG.txt` & `django-modeltranslation-0.9.1/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v0.9.1
+======
+Date: 2015-05-14
+
+  FIXED: Handled deprecation of _meta._fill_fields_cache() for Django 1.8
+         in add_translation_fields.
+         (resolves issue #304, thanks Mathias Ettinger and Daniel Loeb)
+  FIXED: Handled deprecation of transaction.commit_unless_managed for
+         Django 1.8 in sync_translation_fields management command.
+         (resolves issue #310)
+  FIXED: Fixed translatable fields discovery with the new _meta API and
+         generic relations for Django 1.8.
+         (resolves issue #309, thanks Morgan Aubert)
+
+
 v0.9
 ====
 Date: 2015-04-16
 
   ADDED: Support for Django 1.8 and the new meta API.
          (resolves issue #299, thanks Luca Corti and Jacek Tomaszewski)
```

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/contribute.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/contribute.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/admin.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/admin.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/make.bat` & `django-modeltranslation-0.9.1/docs/modeltranslation/make.bat`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/usage.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/usage.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/Makefile` & `django-modeltranslation-0.9.1/docs/modeltranslation/Makefile`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/registration.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/registration.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/installation.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/installation.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/commands.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/commands.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/caveats.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/caveats.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/conf.py` & `django-modeltranslation-0.9.1/docs/modeltranslation/conf.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/related_projects.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/related_projects.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/docs/modeltranslation/forms.rst` & `django-modeltranslation-0.9.1/docs/modeltranslation/forms.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/setup.py` & `django-modeltranslation-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/AUTHORS.rst` & `django-modeltranslation-0.9.1/AUTHORS.rst`

 * *Files 18% similar despite different names*

```diff
@@ -31,10 +31,14 @@
 * Mathieu Leplatre
 * Thom Wiggers
 * Warnar Boekkooi
 * Alex Marandon
 * Fabio Caccamo
 * Vladimir Sinitsin
 * Luca Corti
+* Morgan Aubert
+* Mathias Ettinger
+* Daniel Loeb
+* Stephen McDonald
 * And many more ... (if you miss your name here, please let us know!)
 
 .. _django-linguo: https://github.com/zmathew/django-linguo
```

### Comparing `django-modeltranslation-0.9/README.rst` & `django-modeltranslation-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-modeltranslation-0.9/PKG-INFO` & `django-modeltranslation-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: django-modeltranslation
-Version: 0.9
+Version: 0.9.1
 Summary: Translates Django models using a registration approach.
 Home-page: https://github.com/deschler/django-modeltranslation
 Author: Dirk Eschler
 Author-email: eschler@gmail.com
 License: New BSD
-Download-URL: https://github.com/deschler/django-modeltranslation/archive/0.9.tar.gz
+Download-URL: https://github.com/deschler/django-modeltranslation/archive/0.9.1.tar.gz
 Description: The modeltranslation application can be used to translate dynamic content of existing models to an arbitrary number of languages without having to change the original model classes. It uses a registration approach (comparable to Django's admin app) to be able to add translations to existing or new projects and is fully integrated into the Django admin backend.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
```

