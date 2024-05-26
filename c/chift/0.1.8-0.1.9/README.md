# Comparing `tmp/chift-0.1.8.tar.gz` & `tmp/chift-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chift-0.1.8.tar", last modified: Tue Aug 22 15:36:25 2023, max compression
+gzip compressed data, was "chift-0.1.9.tar", last modified: Thu Sep  7 08:50:57 2023, max compression
```

## Comparing `chift-0.1.8.tar` & `chift-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,70 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.754534 chift-0.1.8/
--rw-r--r--   0 thomas     (501) staff       (20)     1777 2023-08-22 15:36:25.753970 chift-0.1.8/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     1618 2023-08-21 11:26:22.000000 chift-0.1.8/README.md
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.716790 chift-0.1.8/chift/
--rw-r--r--   0 thomas     (501) staff       (20)      188 2023-08-21 10:50:13.000000 chift-0.1.8/chift/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.726976 chift-0.1.8/chift/api/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-08-21 10:50:13.000000 chift-0.1.8/chift/api/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     7749 2023-08-22 15:29:29.000000 chift-0.1.8/chift/api/client.py
--rw-r--r--   0 thomas     (501) staff       (20)      346 2023-08-21 10:50:13.000000 chift-0.1.8/chift/api/exceptions.py
--rw-r--r--   0 thomas     (501) staff       (20)     4144 2023-08-21 10:50:13.000000 chift-0.1.8/chift/api/mixins.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.727507 chift-0.1.8/chift/models/
--rw-r--r--   0 thomas     (501) staff       (20)      315 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.728415 chift-0.1.8/chift/models/consumers/
--rw-r--r--   0 thomas     (501) staff       (20)       31 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/consumers/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.728789 chift-0.1.8/chift/models/consumers/accounting/
--rw-r--r--   0 thomas     (501) staff       (20)     3283 2023-08-22 15:29:29.000000 chift-0.1.8/chift/models/consumers/accounting/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.729297 chift-0.1.8/chift/models/consumers/commerce/
--rw-r--r--   0 thomas     (501) staff       (20)     1853 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/consumers/commerce/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.729836 chift-0.1.8/chift/models/consumers/connection/
--rw-r--r--   0 thomas     (501) staff       (20)      322 2023-08-22 15:27:03.000000 chift-0.1.8/chift/models/consumers/connection/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      619 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/consumers/consumer.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.730530 chift-0.1.8/chift/models/consumers/custom/
--rw-r--r--   0 thomas     (501) staff       (20)     1157 2023-08-22 15:29:29.000000 chift-0.1.8/chift/models/consumers/custom/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.735196 chift-0.1.8/chift/models/consumers/data/
--rw-r--r--   0 thomas     (501) staff       (20)      989 2023-08-22 15:27:03.000000 chift-0.1.8/chift/models/consumers/data/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.735871 chift-0.1.8/chift/models/consumers/invoicing/
--rw-r--r--   0 thomas     (501) staff       (20)     1865 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/consumers/invoicing/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.736311 chift-0.1.8/chift/models/consumers/log/
--rw-r--r--   0 thomas     (501) staff       (20)      393 2023-08-22 15:26:23.000000 chift-0.1.8/chift/models/consumers/log/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.736839 chift-0.1.8/chift/models/consumers/pos/
--rw-r--r--   0 thomas     (501) staff       (20)     2134 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/consumers/pos/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.737283 chift-0.1.8/chift/models/consumers/sync/
--rw-r--r--   0 thomas     (501) staff       (20)      279 2023-08-22 15:27:03.000000 chift-0.1.8/chift/models/consumers/sync/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.737741 chift-0.1.8/chift/models/datastores/
--rw-r--r--   0 thomas     (501) staff       (20)      425 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/datastores/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.738263 chift-0.1.8/chift/models/integrations/
--rw-r--r--   0 thomas     (501) staff       (20)      438 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/integrations/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.738838 chift-0.1.8/chift/models/syncs/
--rw-r--r--   0 thomas     (501) staff       (20)     1703 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/syncs/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.739189 chift-0.1.8/chift/models/webhooks/
--rw-r--r--   0 thomas     (501) staff       (20)      985 2023-08-21 10:50:13.000000 chift-0.1.8/chift/models/webhooks/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.740541 chift-0.1.8/chift/openapi/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-08-21 10:50:13.000000 chift-0.1.8/chift/openapi/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     5831 2023-08-22 15:29:29.000000 chift-0.1.8/chift/openapi/models.py
--rw-r--r--   0 thomas     (501) staff       (20)   109823 2023-08-22 15:27:09.000000 chift-0.1.8/chift/openapi/openapi.py
--rw-r--r--   0 thomas     (501) staff       (20)       18 2023-08-22 15:27:38.000000 chift-0.1.8/chift/version.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.724142 chift-0.1.8/chift.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     1777 2023-08-22 15:36:25.000000 chift-0.1.8/chift.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     1239 2023-08-22 15:36:25.000000 chift-0.1.8/chift.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-08-22 15:36:25.000000 chift-0.1.8/chift.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       89 2023-08-22 15:36:25.000000 chift-0.1.8/chift.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        6 2023-08-22 15:36:25.000000 chift-0.1.8/chift.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)       38 2023-08-22 15:36:25.754588 chift-0.1.8/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)      853 2023-08-21 12:36:58.000000 chift-0.1.8/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-08-22 15:36:25.753037 chift-0.1.8/tests/
--rw-r--r--   0 thomas     (501) staff       (20)     2978 2023-08-21 10:50:13.000000 chift-0.1.8/tests/test_accounting.py
--rw-r--r--   0 thomas     (501) staff       (20)      586 2023-08-21 10:50:13.000000 chift-0.1.8/tests/test_client.py
--rw-r--r--   0 thomas     (501) staff       (20)     1415 2023-08-21 10:50:13.000000 chift-0.1.8/tests/test_commerce.py
--rw-r--r--   0 thomas     (501) staff       (20)     1436 2023-08-22 15:25:27.000000 chift-0.1.8/tests/test_connection.py
--rw-r--r--   0 thomas     (501) staff       (20)     3552 2023-08-21 12:33:32.000000 chift-0.1.8/tests/test_custom.py
--rw-r--r--   0 thomas     (501) staff       (20)      178 2023-08-21 10:50:13.000000 chift-0.1.8/tests/test_datastore.py
--rw-r--r--   0 thomas     (501) staff       (20)      169 2023-08-21 10:50:13.000000 chift-0.1.8/tests/test_integration.py
--rw-r--r--   0 thomas     (501) staff       (20)     3944 2023-08-21 15:17:11.000000 chift-0.1.8/tests/test_invoicing.py
--rw-r--r--   0 thomas     (501) staff       (20)      623 2023-08-22 15:20:48.000000 chift-0.1.8/tests/test_log.py
--rw-r--r--   0 thomas     (501) staff       (20)     2310 2023-08-21 10:50:13.000000 chift-0.1.8/tests/test_pos.py
--rw-r--r--   0 thomas     (501) staff       (20)     9150 2023-08-22 15:27:08.000000 chift-0.1.8/tests/test_sync.py
--rw-r--r--   0 thomas     (501) staff       (20)      329 2023-08-21 10:50:13.000000 chift-0.1.8/tests/test_webhook.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.034442 chift-0.1.9/
+-rw-r--r--   0 thomas     (501) staff       (20)     2044 2023-09-07 08:50:57.034158 chift-0.1.9/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     1618 2023-08-21 11:26:22.000000 chift-0.1.9/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.012452 chift-0.1.9/chift/
+-rw-r--r--   0 thomas     (501) staff       (20)      188 2023-08-21 10:50:13.000000 chift-0.1.9/chift/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.016744 chift-0.1.9/chift/api/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2023-08-21 10:50:13.000000 chift-0.1.9/chift/api/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     7749 2023-08-30 09:08:32.000000 chift-0.1.9/chift/api/client.py
+-rw-r--r--   0 thomas     (501) staff       (20)      346 2023-08-21 10:50:13.000000 chift-0.1.9/chift/api/exceptions.py
+-rw-r--r--   0 thomas     (501) staff       (20)     4144 2023-08-21 10:50:13.000000 chift-0.1.9/chift/api/mixins.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.017119 chift-0.1.9/chift/models/
+-rw-r--r--   0 thomas     (501) staff       (20)      315 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.018127 chift-0.1.9/chift/models/consumers/
+-rw-r--r--   0 thomas     (501) staff       (20)       31 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/consumers/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.019297 chift-0.1.9/chift/models/consumers/accounting/
+-rw-r--r--   0 thomas     (501) staff       (20)     3283 2023-08-30 09:08:32.000000 chift-0.1.9/chift/models/consumers/accounting/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.019701 chift-0.1.9/chift/models/consumers/commerce/
+-rw-r--r--   0 thomas     (501) staff       (20)     1853 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/consumers/commerce/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.020905 chift-0.1.9/chift/models/consumers/connection/
+-rw-r--r--   0 thomas     (501) staff       (20)      322 2023-08-22 16:58:24.000000 chift-0.1.9/chift/models/consumers/connection/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      619 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/consumers/consumer.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.021340 chift-0.1.9/chift/models/consumers/custom/
+-rw-r--r--   0 thomas     (501) staff       (20)     1157 2023-08-30 09:08:32.000000 chift-0.1.9/chift/models/consumers/custom/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.022431 chift-0.1.9/chift/models/consumers/data/
+-rw-r--r--   0 thomas     (501) staff       (20)      989 2023-08-22 16:58:24.000000 chift-0.1.9/chift/models/consumers/data/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.022857 chift-0.1.9/chift/models/consumers/invoicing/
+-rw-r--r--   0 thomas     (501) staff       (20)     1865 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/consumers/invoicing/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.023351 chift-0.1.9/chift/models/consumers/log/
+-rw-r--r--   0 thomas     (501) staff       (20)      393 2023-08-22 16:58:24.000000 chift-0.1.9/chift/models/consumers/log/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.023848 chift-0.1.9/chift/models/consumers/payment/
+-rw-r--r--   0 thomas     (501) staff       (20)      494 2023-09-07 08:49:15.000000 chift-0.1.9/chift/models/consumers/payment/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.024197 chift-0.1.9/chift/models/consumers/pos/
+-rw-r--r--   0 thomas     (501) staff       (20)     2134 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/consumers/pos/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.024610 chift-0.1.9/chift/models/consumers/sync/
+-rw-r--r--   0 thomas     (501) staff       (20)      279 2023-08-22 16:58:24.000000 chift-0.1.9/chift/models/consumers/sync/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.024991 chift-0.1.9/chift/models/datastores/
+-rw-r--r--   0 thomas     (501) staff       (20)      425 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/datastores/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.025340 chift-0.1.9/chift/models/integrations/
+-rw-r--r--   0 thomas     (501) staff       (20)      438 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/integrations/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.025666 chift-0.1.9/chift/models/syncs/
+-rw-r--r--   0 thomas     (501) staff       (20)     1703 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/syncs/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.026179 chift-0.1.9/chift/models/webhooks/
+-rw-r--r--   0 thomas     (501) staff       (20)      985 2023-08-21 10:50:13.000000 chift-0.1.9/chift/models/webhooks/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.027095 chift-0.1.9/chift/openapi/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2023-08-21 10:50:13.000000 chift-0.1.9/chift/openapi/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     6067 2023-09-07 08:49:15.000000 chift-0.1.9/chift/openapi/models.py
+-rw-r--r--   0 thomas     (501) staff       (20)   110132 2023-09-07 08:49:15.000000 chift-0.1.9/chift/openapi/openapi.py
+-rw-r--r--   0 thomas     (501) staff       (20)       18 2023-09-07 08:49:15.000000 chift-0.1.9/chift/version.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.015021 chift-0.1.9/chift.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)     2044 2023-09-07 08:50:56.000000 chift-0.1.9/chift.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     1305 2023-09-07 08:50:57.000000 chift-0.1.9/chift.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-09-07 08:50:56.000000 chift-0.1.9/chift.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       89 2023-09-07 08:50:56.000000 chift-0.1.9/chift.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        6 2023-09-07 08:50:56.000000 chift-0.1.9/chift.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2023-09-07 08:50:57.034491 chift-0.1.9/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)      853 2023-08-22 16:58:24.000000 chift-0.1.9/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-07 08:50:57.033459 chift-0.1.9/tests/
+-rw-r--r--   0 thomas     (501) staff       (20)     2978 2023-08-21 10:50:13.000000 chift-0.1.9/tests/test_accounting.py
+-rw-r--r--   0 thomas     (501) staff       (20)      586 2023-08-21 10:50:13.000000 chift-0.1.9/tests/test_client.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1415 2023-08-21 10:50:13.000000 chift-0.1.9/tests/test_commerce.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1436 2023-08-22 16:58:24.000000 chift-0.1.9/tests/test_connection.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3517 2023-08-24 08:40:01.000000 chift-0.1.9/tests/test_custom.py
+-rw-r--r--   0 thomas     (501) staff       (20)      178 2023-08-21 10:50:13.000000 chift-0.1.9/tests/test_datastore.py
+-rw-r--r--   0 thomas     (501) staff       (20)      169 2023-08-21 10:50:13.000000 chift-0.1.9/tests/test_integration.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3944 2023-08-22 16:58:24.000000 chift-0.1.9/tests/test_invoicing.py
+-rw-r--r--   0 thomas     (501) staff       (20)      623 2023-08-22 16:58:24.000000 chift-0.1.9/tests/test_log.py
+-rw-r--r--   0 thomas     (501) staff       (20)      282 2023-09-07 08:49:15.000000 chift-0.1.9/tests/test_paymentd.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2310 2023-08-21 10:50:13.000000 chift-0.1.9/tests/test_pos.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9160 2023-08-23 06:33:16.000000 chift-0.1.9/tests/test_sync.py
+-rw-r--r--   0 thomas     (501) staff       (20)      329 2023-08-21 10:50:13.000000 chift-0.1.9/tests/test_webhook.py
```

### Comparing `chift-0.1.8/PKG-INFO` & `chift-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: chift
-Version: 0.1.8
-Summary: Chift API client
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # Chift Python Library
 
 [![pypi](https://img.shields.io/pypi/v/chift.svg)](https://pypi.python.org/pypi/chift)
 [![Build Status](https://github.com/chift-oneapi/chift-python-sdk/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/chift-oneapi/chift-python-sdk/actions?query=branch:main)
 [![Coverage Status](https://coveralls.io/repos/github/chift-oneapi/chift-python-sdk/badge.svg?branch=main)](https://coveralls.io/github/chift-oneapi/chift-python-sdk?branch=master)
```

### Comparing `chift-0.1.8/chift/api/client.py` & `chift-0.1.9/chift/api/client.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/api/mixins.py` & `chift-0.1.9/chift/api/mixins.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/consumers/accounting/__init__.py` & `chift-0.1.9/chift/models/consumers/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/consumers/commerce/__init__.py` & `chift-0.1.9/chift/models/consumers/commerce/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/consumers/consumer.py` & `chift-0.1.9/chift/models/consumers/consumer.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/consumers/custom/__init__.py` & `chift-0.1.9/chift/models/consumers/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/consumers/data/__init__.py` & `chift-0.1.9/chift/models/consumers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/consumers/invoicing/__init__.py` & `chift-0.1.9/chift/models/consumers/invoicing/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/consumers/pos/__init__.py` & `chift-0.1.9/chift/models/consumers/pos/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/syncs/__init__.py` & `chift-0.1.9/chift/models/syncs/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/models/webhooks/__init__.py` & `chift-0.1.9/chift/models/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/chift/openapi/models.py` & `chift-0.1.9/chift/openapi/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import List, Optional
 
 from pydantic import BaseModel, Extra
 
 from .openapi import (
     AccountItem,
     AnalyticAccountItemOut,
-    BackboneBackboneApiAppRoutersAccountingVatCode,
-    BackboneBackboneApiAppRoutersCommerceProductItem,
+    AppRoutersAccountingVatCode,
+    AppRoutersCommerceProductItem,
     ClientItemOut,
     ClosureItem,
     CommerceCustomerItem,
     CommerceLocationItemOut,
     ConnectionItem,
     ConsumerItem,
     ContactItemOut,
@@ -34,14 +34,15 @@
     POSLocationItem,
     ProductItemOut,
     ReadFlowItem,
     SalesItem,
     SupplierItemOut,
     SyncConsumerItem,
     SyncItem,
+    TransactionItemOut,
     VariantItem,
     WebhookInstanceGetItem,
     WebhookItem,
 )
 
 # UNPUBLISHED MODELS
 
@@ -144,14 +145,22 @@
         from chift.models.consumers.commerce import (
             CommerceRouter,
         )  # avoid circular import
 
         return CommerceRouter(self.consumerid, self.connectionid)
 
     @property
+    def payment(self):
+        from chift.models.consumers.payment import (
+            PaymentRouter,
+        )  # avoid circular import
+
+        return PaymentRouter(self.consumerid, self.connectionid)
+
+    @property
     def custom(self):
         from chift.models.consumers.custom import CustomRouter  # avoid circular import
 
         return CustomRouter(self.consumerid, self.connectionid)
 
     @property
     def Connection(self):
@@ -258,15 +267,15 @@
 
 
 # accouting
 class AnalyticPlan(AnalyticAccountItemOut):
     pass
 
 
-class TaxAccounting(BackboneBackboneApiAppRoutersAccountingVatCode):
+class TaxAccounting(AppRoutersAccountingVatCode):
     pass
 
 
 class MiscellaneousOperation(MiscellaneousOperationOut):
     pass
 
 
@@ -325,21 +334,28 @@
 
 
 # e-commerce
 class CommerceCustomer(CommerceCustomerItem):
     pass
 
 
-class CommerceProduct(BackboneBackboneApiAppRoutersCommerceProductItem):
+class CommerceProduct(AppRoutersCommerceProductItem):
     pass
 
 
 class CommerceLocation(CommerceLocationItemOut):
     pass
 
 
 class CommerceOrder(OrderItemOut):
     pass
 
 
 class CommerceVariant(VariantItem):
     pass
+
+
+# payment
+
+
+class PaymentTransaction(TransactionItemOut):
+    pass
```

### Comparing `chift-0.1.8/chift/openapi/openapi.py` & `chift-0.1.9/chift/openapi/openapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-08-22T13:17:15+00:00
+#   timestamp: 2023-08-30T09:08:08+00:00
 
 from __future__ import annotations
 
 from datetime import date, datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
@@ -37,16 +37,16 @@
     )
 
 
 class AccountItemType(Enum):
     bank = "bank"
     cash = "cash"
     other_financial = "other_financial"
-    accounts_receivable = "accounts_receivable"
-    accounts_payable = "accounts_payable"
+    receivable = "receivable"
+    payable = "payable"
     vat = "vat"
     other = "other"
 
 
 class AddressItem(BaseModel):
     address_type: Optional[str] = Field(None, title="Address Type")
     name: Optional[str] = Field(None, title="Name")
@@ -842,19 +842,47 @@
 
 class TotalTaxItem(BaseModel):
     tax_rate: float = Field(..., title="Tax Rate")
     tax_amount: float = Field(..., title="Tax Amount")
     total: float = Field(..., title="Total")
 
 
+class TransactionAccountingCategory(Enum):
+    all = "all"
+    unknown = "unknown"
+    test = "test"
+
+
 class TransactionFilterDateType(Enum):
     value_date = "value_date"
     execution_date = "execution_date"
 
 
+class TransactionItemOut(BaseModel):
+    id: str = Field(..., description="Technical id in Chift", title="Id")
+    source_ref: Ref = Field(
+        ..., description="Technical id in the target software", title="Source Ref"
+    )
+    total: float = Field(..., description="Total amount incl. fee", title="Total")
+    fee: float = Field(..., description="Total fee", title="Fee")
+    currency: str = Field(..., description="Currency", title="Currency")
+    exchange_rate: float = Field(
+        ..., description="Exchange rate", title="Exchange Rate"
+    )
+    create_date: datetime = Field(..., description="Create Date", title="Create Date")
+    application_type: str = Field(
+        ...,
+        description="Type of the transaction as recorded in the target software",
+        title="Application Type",
+    )
+    accounting_category: TransactionAccountingCategory = Field(
+        ..., description="Accounting category"
+    )
+
+
 class TriggerResponse(BaseModel):
     status: str = Field(..., title="Status")
     message: str = Field(..., title="Message")
     data: Optional[Dict[str, Any]] = Field(None, title="Data")
 
 
 class TriggerType(Enum):
@@ -959,55 +987,55 @@
     url: str = Field(..., title="Url")
     accountid: str = Field(..., title="Accountid")
     createdon: datetime = Field(..., title="Createdon")
     httpstatus: int = Field(..., title="Httpstatus")
     integrationid: Optional[int] = Field(None, title="Integrationid")
 
 
-class BackboneBackboneApiAppRoutersAccountingInvoiceType(Enum):
+class AppRoutersAccountingInvoiceType(Enum):
     customer_invoice = "customer_invoice"
     customer_refund = "customer_refund"
     supplier_invoice = "supplier_invoice"
     supplier_refund = "supplier_refund"
 
 
-class BackboneBackboneApiAppRoutersAccountingPaymentStatus(Enum):
+class AppRoutersAccountingPaymentStatus(Enum):
     all = "all"
     unpaid = "unpaid"
     paid = "paid"
 
 
-class BackboneBackboneApiAppRoutersAccountingVatCodeScope(Enum):
+class AppRoutersAccountingVatCodeScope(Enum):
     nat = "nat"
     eu = "eu"
     int = "int"
     unknown = "unknown"
 
 
-class BackboneBackboneApiAppRoutersAccountingVatCodeType(Enum):
+class AppRoutersAccountingVatCodeType(Enum):
     sale = "sale"
     purchase = "purchase"
     both = "both"
     unknown = "unknown"
 
 
-class BackboneBackboneApiAppRoutersCommerceAddressItemIn(BaseModel):
+class AppRoutersCommerceAddressItemIn(BaseModel):
     first_name: str = Field(..., title="First Name")
     last_name: str = Field(..., title="Last Name")
     street: str = Field(..., title="Street")
     number: str = Field(..., title="Number")
     box: Optional[str] = Field(None, title="Box")
     city: str = Field(..., title="City")
     postal_code: Optional[str] = Field(None, title="Postal Code")
     country: str = Field(..., description="Format: ISO 3166-1 codes.", title="Country")
     phone: Optional[str] = Field(None, title="Phone")
     email: Optional[str] = Field(None, title="Email")
 
 
-class BackboneBackboneApiAppRoutersCommerceAddressItemOut(BaseModel):
+class AppRoutersCommerceAddressItemOut(BaseModel):
     address_type: AddressType
     first_name: Optional[str] = Field(None, title="First Name")
     last_name: Optional[str] = Field(None, title="Last Name")
     street: Optional[str] = Field(None, title="Street")
     number: Optional[str] = Field(None, title="Number")
     box: Optional[str] = Field(None, title="Box")
     city: Optional[str] = Field(None, title="City")
@@ -1015,60 +1043,60 @@
     country: Optional[str] = Field(
         None, description="Format: ISO 3166-1 codes.", title="Country"
     )
     phone: Optional[str] = Field(None, title="Phone")
     email: Optional[str] = Field(None, title="Email")
 
 
-class BackboneBackboneApiAppRoutersCommerceDiscountItem(BaseModel):
+class AppRoutersCommerceDiscountItem(BaseModel):
     name: str = Field(..., title="Name")
     description: str = Field(..., title="Description")
     amount: float = Field(..., title="Amount")
 
 
-class BackboneBackboneApiAppRoutersConnectionsCredentialItem(BaseModel):
+class AppRoutersConnectionsCredentialItem(BaseModel):
     key: str = Field(..., title="Key")
     value: str = Field(..., title="Value")
 
 
-class BackboneBackboneApiAppRoutersConnectionsStatus(Enum):
+class AppRoutersConnectionsStatus(Enum):
     active = "active"
     inactive = "inactive"
 
 
-class BackboneBackboneApiAppRoutersDatastoresStatus(Enum):
+class AppRoutersDatastoresStatus(Enum):
     active = "active"
     inactive = "inactive"
 
 
-class BackboneBackboneApiAppRoutersIntegrationsCredentialItem(BaseModel):
+class AppRoutersIntegrationsCredentialItem(BaseModel):
     name: str = Field(..., title="Name")
     optional: Optional[bool] = Field(False, title="Optional")
 
 
-class BackboneBackboneApiAppRoutersIntegrationsStatus(Enum):
+class AppRoutersIntegrationsStatus(Enum):
     active = "active"
     inactive = "inactive"
 
 
-class BackboneBackboneApiAppRoutersPosDiscountItem(BaseModel):
+class AppRoutersPosDiscountItem(BaseModel):
     name: Optional[str] = Field(None, title="Name")
     total: float = Field(..., title="Total")
 
 
-class BackboneBackboneApiAppRoutersPosPaymentStatus(Enum):
+class AppRoutersPosPaymentStatus(Enum):
     Pending = "Pending"
     Completed = "Completed"
     Canceled = "Canceled"
     Failed = "Failed"
     Unknown = "Unknown"
     Authorised = "Authorised"
 
 
-class BackboneBackboneApiAppRoutersWebhooksStatus(Enum):
+class AppRoutersWebhooksStatus(Enum):
     active = "active"
     inactive = "inactive"
 
 
 class ModelsCommonAddressItemIn(BaseModel):
     address_type: AddressType
     name: Optional[str] = Field(None, title="Name")
@@ -1365,17 +1393,17 @@
     )
     internal_notes: Optional[str] = Field(None, title="Internal Notes")
     currency: Optional[str] = Field(
         None,
         description="Indicates the currency of the client (e.g. EUR).",
         title="Currency",
     )
-    addresses: Optional[
-        List[BackboneBackboneApiAppRoutersCommerceAddressItemOut]
-    ] = Field([], title="Addresses")
+    addresses: Optional[List[AppRoutersCommerceAddressItemOut]] = Field(
+        [], title="Addresses"
+    )
     created_on: Optional[datetime] = Field(None, title="Created On")
 
 
 class CommerceLocationItemOut(BaseModel):
     id: str = Field(
         ..., description="Technical id of the location in Chift", title="Id"
     )
@@ -1390,15 +1418,15 @@
 class ConnectionItem(BaseModel):
     connectionid: UUID = Field(..., title="Connectionid")
     name: str = Field(..., title="Name")
     integration: str = Field(..., title="Integration")
     integrationid: int = Field(..., title="Integrationid")
     api: str = Field(..., title="Api")
     data: Optional[Dict[str, Any]] = Field(None, title="Data")
-    status: BackboneBackboneApiAppRoutersConnectionsStatus
+    status: AppRoutersConnectionsStatus
 
 
 class ContactItemIn(BaseModel):
     is_prospect: Optional[bool] = Field(
         None, description="Is a prospect?", title="Is Prospect"
     )
     is_customer: Optional[bool] = Field(
@@ -1512,30 +1540,30 @@
         [], description="Addresses", title="Addresses"
     )
 
 
 class DataStoreItem(BaseModel):
     id: str = Field(..., title="Id")
     name: str = Field(..., title="Name")
-    status: Optional[BackboneBackboneApiAppRoutersDatastoresStatus] = "active"
+    status: Optional[AppRoutersDatastoresStatus] = "active"
     definition: DatastoreDef
 
 
 class FeesItem(BaseModel):
     type: FeesType
     tax_rate: float = Field(..., title="Tax Rate")
     untaxed_amount: float = Field(..., title="Untaxed Amount")
     tax_amount: float = Field(..., title="Tax Amount")
     total: float = Field(..., title="Total")
 
 
 class FlowDataStoreItem(BaseModel):
     id: Optional[str] = Field(None, title="Id")
     name: str = Field(..., title="Name")
-    status: Optional[BackboneBackboneApiAppRoutersDatastoresStatus] = "active"
+    status: Optional[AppRoutersDatastoresStatus] = "active"
     definition: DatastoreDef
 
 
 class FlowExecution(BaseModel):
     type: ExecutionType
     data: Optional[Union[FlowExecutionChain, FlowExecutionCode]] = Field(
         None, title="Data"
@@ -1554,19 +1582,17 @@
     status: Optional[str] = Field("error", title="Status")
     detail: Optional[List[ValidationError]] = Field(None, title="Detail")
 
 
 class IntegrationItem(BaseModel):
     integrationid: int = Field(..., title="Integrationid")
     name: str = Field(..., title="Name")
-    status: BackboneBackboneApiAppRoutersIntegrationsStatus
+    status: AppRoutersIntegrationsStatus
     api: Api
-    credentials: Optional[
-        List[BackboneBackboneApiAppRoutersIntegrationsCredentialItem]
-    ] = Field(
+    credentials: Optional[List[AppRoutersIntegrationsCredentialItem]] = Field(
         [],
         description="List of credentials that must be specified to create a connection. Can be used if you want to pass credentials on connection creation. Not compatible with oAuth2 routes.",
         title="Credentials",
     )
 
 
 class InvoiceItem(BaseModel):
@@ -1602,15 +1628,15 @@
     )
     journal_ref: Optional[FieldRef] = Field(
         None, description="Journal", title="Journal Ref"
     )
 
 
 class InvoiceItemInMonoAnalyticPlan(BaseModel):
-    invoice_type: BackboneBackboneApiAppRoutersAccountingInvoiceType
+    invoice_type: AppRoutersAccountingInvoiceType
     invoice_number: Optional[str] = Field(
         None,
         description="Number of the invoice. If left empty, will be automatically generated by the accounting system at creation.",
         title="Invoice Number",
     )
     invoice_date: date = Field(..., title="Invoice Date")
     due_date: date = Field(..., title="Due Date")
@@ -1687,15 +1713,15 @@
     )
     journal_ref: Optional[FieldRef] = Field(
         None, description="Journal", title="Journal Ref"
     )
 
 
 class InvoiceItemOutMonoAnalyticPlan(BaseModel):
-    invoice_type: BackboneBackboneApiAppRoutersAccountingInvoiceType
+    invoice_type: AppRoutersAccountingInvoiceType
     invoice_number: Optional[str] = Field(
         None,
         description="Number of the invoice. If left empty, will be automatically generated by the accounting system at creation.",
         title="Invoice Number",
     )
     invoice_date: date = Field(..., title="Invoice Date")
     due_date: date = Field(..., title="Due Date")
@@ -1833,17 +1859,15 @@
     id: str = Field(..., title="Id")
     quantity: float = Field(..., title="Quantity")
     unit_price: float = Field(..., title="Unit Price")
     total: float = Field(..., title="Total")
     tax_amount: float = Field(..., title="Tax Amount")
     tax_rate: Optional[float] = Field(None, title="Tax Rate")
     description: str = Field(..., title="Description")
-    discounts: Optional[List[BackboneBackboneApiAppRoutersPosDiscountItem]] = Field(
-        [], title="Discounts"
-    )
+    discounts: Optional[List[AppRoutersPosDiscountItem]] = Field([], title="Discounts")
 
 
 class Journal(BaseModel):
     id: str = Field(..., title="Id")
     code: str = Field(..., title="Code")
     name: str = Field(..., title="Name")
     journal_type: JournalType
@@ -1971,16 +1995,16 @@
     owner_ref: Optional[FieldRef] = Field(
         None, description="Employee/User", title="Owner Ref"
     )
 
 
 class OrderItemIn(BaseModel):
     customer: OrderCustomerItem
-    billing_address: BackboneBackboneApiAppRoutersCommerceAddressItemIn
-    shipping_address: BackboneBackboneApiAppRoutersCommerceAddressItemIn
+    billing_address: AppRoutersCommerceAddressItemIn
+    shipping_address: AppRoutersCommerceAddressItemIn
     currency: str = Field(
         ...,
         description="Indicates the currency of the order (e.g. EUR).",
         title="Currency",
     )
     note: Optional[str] = Field(None, title="Note")
     lines: List[OrderLineItemIn] = Field(..., title="Lines")
@@ -2016,17 +2040,17 @@
     )
     tax_amount: float = Field(
         ..., description="Total taxes applied to the order line.", title="Tax Amount"
     )
     total: float = Field(
         ..., description="Total of the order line with discount.", title="Total"
     )
-    discounts: Optional[
-        List[BackboneBackboneApiAppRoutersCommerceDiscountItem]
-    ] = Field([], title="Discounts")
+    discounts: Optional[List[AppRoutersCommerceDiscountItem]] = Field(
+        [], title="Discounts"
+    )
 
 
 class OrderRefundItem(BaseModel):
     created_on: Optional[datetime] = Field(None, title="Created On")
     total: float = Field(..., title="Total")
     reason: Optional[str] = Field(None, title="Reason")
     order_lines: Optional[List[RefundOrderLineItem]] = Field([], title="Order Lines")
@@ -2128,41 +2152,46 @@
 class PagePayment(BaseModel):
     items: List[Payment] = Field(..., title="Items")
     total: conint(ge=0) = Field(..., title="Total")
     page: conint(ge=1) = Field(..., title="Page")
     size: conint(ge=1) = Field(..., title="Size")
 
 
+class PageTransactionItemOut(BaseModel):
+    items: List[TransactionItemOut] = Field(..., title="Items")
+    total: conint(ge=0) = Field(..., title="Total")
+    page: conint(ge=1) = Field(..., title="Page")
+    size: conint(ge=1) = Field(..., title="Size")
+
+
 class PatchConnectionItem(BaseModel):
     redirect: Optional[bool] = Field(
         False,
         description="Indicates whether you want to return to the consumer's redirectUrl after update (true) or whether you want to return on the connection page (false)",
         title="Redirect",
     )
     name: Optional[str] = Field(
         None,
         description="Can be used to update the name of an existing connection",
         title="Name",
     )
-    credentials: Optional[
-        List[BackboneBackboneApiAppRoutersConnectionsCredentialItem]
-    ] = Field(
+    credentials: Optional[List[AppRoutersConnectionsCredentialItem]] = Field(
         None,
         description="Can be used to update the credentials of an existing connection. Please use the getIntegrations route to see the available credentials for each integration",
         title="Credentials",
     )
 
 
 class PaymentItem(BaseModel):
     id: Optional[str] = Field(None, title="Id")
     payment_method_id: Optional[str] = Field(None, title="Payment Method Id")
     payment_method_name: Optional[str] = Field(None, title="Payment Method Name")
     total: float = Field(..., title="Total")
     tip: Optional[float] = Field(0, title="Tip")
-    status: Optional[BackboneBackboneApiAppRoutersPosPaymentStatus] = "Unknown"
+    status: Optional[AppRoutersPosPaymentStatus] = "Unknown"
     currency: Optional[str] = Field(None, title="Currency")
     date: Optional[datetime] = Field(None, title="Date")
 
 
 class PostConnectionItem(BaseModel):
     integrationid: Optional[int] = Field(
         None,
@@ -2170,17 +2199,15 @@
         title="Integrationid",
     )
     name: Optional[str] = Field(
         None,
         description="Can be used to specify the name of the connection. Must be used in combination with an integrationid.",
         title="Name",
     )
-    credentials: Optional[
-        List[BackboneBackboneApiAppRoutersConnectionsCredentialItem]
-    ] = Field(
+    credentials: Optional[List[AppRoutersConnectionsCredentialItem]] = Field(
         None,
         description="Can be used to specify the credentials of your connection. Must be used in combination with an integrationid and a name. Please use the getIntegrations route to see the available credentials for each integration",
         title="Credentials",
     )
 
 
 class ProductItemOut(BaseModel):
@@ -2413,34 +2440,34 @@
 class WebhookInstanceGetItem(BaseModel):
     webhookid: UUID = Field(..., title="Webhookid")
     accountid: UUID = Field(..., title="Accountid")
     createdby: Optional[UUID] = Field(None, title="Createdby")
     createdon: datetime = Field(..., title="Createdon")
     event: str = Field(..., title="Event")
     url: str = Field(..., title="Url")
-    status: BackboneBackboneApiAppRoutersWebhooksStatus
+    status: AppRoutersWebhooksStatus
     integrationid: Optional[int] = Field(None, title="Integrationid")
 
 
 class WebhookInstancePatchItem(BaseModel):
-    status: Optional[BackboneBackboneApiAppRoutersWebhooksStatus] = None
+    status: Optional[AppRoutersWebhooksStatus] = None
     url: Optional[constr(max_length=500)] = Field(None, title="Url")
     signingsecret: Optional[constr(max_length=100)] = Field(None, title="Signingsecret")
 
 
-class BackboneBackboneApiAppRoutersAccountingVatCode(BaseModel):
+class AppRoutersAccountingVatCode(BaseModel):
     id: str = Field(..., title="Id")
     code: Optional[str] = Field(None, title="Code")
     label: str = Field(..., title="Label")
-    scope: Optional[BackboneBackboneApiAppRoutersAccountingVatCodeScope] = "unknown"
+    scope: Optional[AppRoutersAccountingVatCodeScope] = "unknown"
     rate: float = Field(..., title="Rate")
-    type: BackboneBackboneApiAppRoutersAccountingVatCodeType
+    type: AppRoutersAccountingVatCodeType
 
 
-class BackboneBackboneApiAppRoutersCommerceProductItem(BaseModel):
+class AppRoutersCommerceProductItem(BaseModel):
     id: str = Field(..., description="Technical id in Chift", title="Id")
     source_ref: Ref = Field(
         ..., description="Technical id in the target software", title="Source Ref"
     )
     name: str = Field(..., title="Name")
     description: Optional[str] = Field(None, title="Description")
     description_html: Optional[str] = Field(None, title="Description Html")
@@ -2481,15 +2508,15 @@
     )
     doorkeyFields: Optional[List[Dict[str, Any]]] = Field(None, title="Doorkeyfields")
     customFields: Optional[List[Dict[str, Any]]] = Field(None, title="Customfields")
     datastores: Optional[List[FlowDataStoreItem]] = Field([], title="Datastores")
 
 
 class InvoiceItemInMultiAnalyticPlans(BaseModel):
-    invoice_type: BackboneBackboneApiAppRoutersAccountingInvoiceType
+    invoice_type: AppRoutersAccountingInvoiceType
     invoice_number: Optional[str] = Field(
         None,
         description="Number of the invoice. If left empty, will be automatically generated by the accounting system at creation.",
         title="Invoice Number",
     )
     invoice_date: date = Field(..., title="Invoice Date")
     due_date: date = Field(..., title="Due Date")
@@ -2526,15 +2553,15 @@
         description="Information used to add a correction line when roundings have an impact on the total amount of the invoice.",
         title="Invoice Correction",
     )
     lines: List[InvoiceLineItemInMultiAnalyticPlans] = Field(..., title="Lines")
 
 
 class InvoiceItemOutMultiAnalyticPlans(BaseModel):
-    invoice_type: BackboneBackboneApiAppRoutersAccountingInvoiceType
+    invoice_type: AppRoutersAccountingInvoiceType
     invoice_number: Optional[str] = Field(
         None,
         description="Number of the invoice. If left empty, will be automatically generated by the accounting system at creation.",
         title="Invoice Number",
     )
     invoice_date: date = Field(..., title="Invoice Date")
     due_date: date = Field(..., title="Due Date")
@@ -2635,20 +2662,16 @@
 class OrderItemOut(BaseModel):
     id: str = Field(..., description="Technical id in Chift", title="Id")
     source_ref: Ref = Field(
         ..., description="Technical id in the target software", title="Source Ref"
     )
     order_number: Optional[str] = Field(None, title="Order Number")
     customer: Optional[OrderCustomerItemOut] = None
-    billing_address: Optional[
-        BackboneBackboneApiAppRoutersCommerceAddressItemOut
-    ] = None
-    shipping_address: Optional[
-        BackboneBackboneApiAppRoutersCommerceAddressItemOut
-    ] = None
+    billing_address: Optional[AppRoutersCommerceAddressItemOut] = None
+    shipping_address: Optional[AppRoutersCommerceAddressItemOut] = None
     created_on: Optional[datetime] = Field(None, title="Created On")
     last_updated_on: Optional[datetime] = Field(None, title="Last Updated On")
     confirmed_on: Optional[datetime] = Field(None, title="Confirmed On")
     cancelled_on: Optional[datetime] = Field(None, title="Cancelled On")
     status: OrderStatus
     discount_amount: float = Field(..., title="Discount Amount")
     untaxed_amount_without_fees: float = Field(
@@ -2732,17 +2755,15 @@
     items: List[ProductItemOut] = Field(..., title="Items")
     total: conint(ge=0) = Field(..., title="Total")
     page: conint(ge=1) = Field(..., title="Page")
     size: conint(ge=1) = Field(..., title="Size")
 
 
 class PageProductItem(BaseModel):
-    items: List[BackboneBackboneApiAppRoutersCommerceProductItem] = Field(
-        ..., title="Items"
-    )
+    items: List[AppRoutersCommerceProductItem] = Field(..., title="Items")
     total: conint(ge=0) = Field(..., title="Total")
     page: conint(ge=1) = Field(..., title="Page")
     size: conint(ge=1) = Field(..., title="Size")
 
 
 class PageSupplierItemOut(BaseModel):
     items: List[SupplierItemOut] = Field(..., title="Items")
@@ -2802,21 +2823,19 @@
 class SyncItem(BaseModel):
     syncid: UUID = Field(..., title="Syncid")
     name: constr(min_length=1) = Field(..., title="Name")
     consumers: List[str] = Field(..., title="Consumers")
     flows: List[ReadFlowItem] = Field(..., title="Flows")
 
 
-class BackboneBackboneApiAppRoutersAccountingPageVatCode(BaseModel):
-    items: List[BackboneBackboneApiAppRoutersAccountingVatCode] = Field(
-        ..., title="Items"
-    )
+class AppRoutersAccountingPageVatCode(BaseModel):
+    items: List[AppRoutersAccountingVatCode] = Field(..., title="Items")
     total: conint(ge=0) = Field(..., title="Total")
     page: conint(ge=1) = Field(..., title="Page")
     size: conint(ge=1) = Field(..., title="Size")
 
 
-class BackboneBackboneApiAppRoutersInvoicingPageVatCode(BaseModel):
+class AppRoutersInvoicingPageVatCode(BaseModel):
     items: List[ModelsInvoicingVatCode] = Field(..., title="Items")
     total: conint(ge=0) = Field(..., title="Total")
     page: conint(ge=1) = Field(..., title="Page")
     size: conint(ge=1) = Field(..., title="Size")
```

### Comparing `chift-0.1.8/chift.egg-info/PKG-INFO` & `chift-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Metadata-Version: 2.1
 Name: chift
-Version: 0.1.8
+Version: 0.1.9
 Summary: Chift API client
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: pydantic<2,>=1.10
+Requires-Dist: requests>=2.20
 Provides-Extra: dev
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: autoflake; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
 
 # Chift Python Library
 
 [![pypi](https://img.shields.io/pypi/v/chift.svg)](https://pypi.python.org/pypi/chift)
 [![Build Status](https://github.com/chift-oneapi/chift-python-sdk/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/chift-oneapi/chift-python-sdk/actions?query=branch:main)
 [![Coverage Status](https://coveralls.io/repos/github/chift-oneapi/chift-python-sdk/badge.svg?branch=main)](https://coveralls.io/github/chift-oneapi/chift-python-sdk?branch=master)
```

### Comparing `chift-0.1.8/chift.egg-info/SOURCES.txt` & `chift-0.1.9/chift.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 chift/models/consumers/accounting/__init__.py
 chift/models/consumers/commerce/__init__.py
 chift/models/consumers/connection/__init__.py
 chift/models/consumers/custom/__init__.py
 chift/models/consumers/data/__init__.py
 chift/models/consumers/invoicing/__init__.py
 chift/models/consumers/log/__init__.py
+chift/models/consumers/payment/__init__.py
 chift/models/consumers/pos/__init__.py
 chift/models/consumers/sync/__init__.py
 chift/models/datastores/__init__.py
 chift/models/integrations/__init__.py
 chift/models/syncs/__init__.py
 chift/models/webhooks/__init__.py
 chift/openapi/__init__.py
@@ -35,10 +36,11 @@
 tests/test_commerce.py
 tests/test_connection.py
 tests/test_custom.py
 tests/test_datastore.py
 tests/test_integration.py
 tests/test_invoicing.py
 tests/test_log.py
+tests/test_paymentd.py
 tests/test_pos.py
 tests/test_sync.py
 tests/test_webhook.py
```

### Comparing `chift-0.1.8/setup.py` & `chift-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/tests/test_accounting.py` & `chift-0.1.9/tests/test_accounting.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/tests/test_client.py` & `chift-0.1.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/tests/test_commerce.py` & `chift-0.1.9/tests/test_commerce.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/tests/test_connection.py` & `chift-0.1.9/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/tests/test_custom.py` & `chift-0.1.9/tests/test_custom.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,31 +51,28 @@
     }
 
     contact = consumer.custom.Custom.create("regate", "contacts", data)
 
     assert contact
 
     data = {"legal_fixed_compensation": "12345"}
+    contact = consumer.custom.Custom.update("regate", "contacts", contact["id"], data)
 
-    contact = consumer.custom.Custom.update(
-        "regate", "contacts", contact["customer"]["id"], data
-    )
-
-    assert contact["customer"]["legal_fixed_compensation"] == "12345"
+    assert contact["legal_fixed_compensation"] == "12345"
 
 
 def test_create_product(custom_regate_consumer: Consumer):
     consumer = custom_regate_consumer
 
     data = {
         "sales_vat_account_id": "ee37ef01-725b-4bd6-a096-06d8093f2c82",
-        "reference": str(uuid.uuid5),
+        "reference": str(uuid.uuid4()),
         "price_cents": 1000,
         "description": "A toothbrush is an oral hygiene tool used to clean the teeth, gums, and tongue. It consists of a head of tightly clustered bristles, atop of which toothpaste can be applied, mounted on a handle which facilitates the cleaning of hard-to-reach areas of the mouth.",
-        "name": str(uuid.uuid5),
+        "name": str(uuid.uuid4()),
         "price_currency": 100,
     }
 
     product = consumer.custom.Custom.create("regate", "products", data)
 
     assert product
```

### Comparing `chift-0.1.8/tests/test_invoicing.py` & `chift-0.1.9/tests/test_invoicing.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/tests/test_log.py` & `chift-0.1.9/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/tests/test_pos.py` & `chift-0.1.9/tests/test_pos.py`

 * *Files identical despite different names*

### Comparing `chift-0.1.8/tests/test_sync.py` & `chift-0.1.9/tests/test_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     assert syncs
 
     expected_sync = syncs[0]
 
     actual_sync = chift.Sync.get(expected_sync.syncid)
 
-    assert expected_sync == actual_sync
+    assert expected_sync.name == actual_sync.name
 
 
 def test_flow_update(chift):
     syncs = chift.Sync.all()
 
     sync: Sync = syncs[0]
```

