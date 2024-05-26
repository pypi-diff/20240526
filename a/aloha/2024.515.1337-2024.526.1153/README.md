# Comparing `tmp/aloha-2024.515.1337.tar.gz` & `tmp/aloha-2024.526.1153.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aloha-2024.515.1337.tar", last modified: Wed May 15 13:37:27 2024, max compression
+gzip compressed data, was "aloha-2024.526.1153.tar", last modified: Sun May 26 11:53:06 2024, max compression
```

## Comparing `aloha-2024.515.1337.tar` & `aloha-2024.526.1153.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.861252 aloha-2024.515.1337/
--rw-r--r--   0 root         (0) root         (0)     4489 2024-05-15 13:37:27.861252 aloha-2024.515.1337/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1599 2024-05-15 13:37:15.000000 aloha-2024.515.1337/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.845252 aloha-2024.515.1337/aloha/
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha/_version.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.845252 aloha-2024.515.1337/aloha/config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      533 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/config/hocon.py
--rw-r--r--   0 root         (0) root         (0)     2812 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/config/paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/db/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1788 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/base.py
--rw-r--r--   0 root         (0) root         (0)     2948 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     4230 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/kafka.py
--rw-r--r--   0 root         (0) root         (0)     9677 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/mongo.py
--rw-r--r--   0 root         (0) root         (0)     1527 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/mysql.py
--rw-r--r--   0 root         (0) root         (0)     1789 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/postgres.py
--rw-r--r--   0 root         (0) root         (0)     2078 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/redis.py
--rw-r--r--   0 root         (0) root         (0)     1850 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/encrypt/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3404 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/aes.py
--rw-r--r--   0 root         (0) root         (0)      486 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/hash.py
--rw-r--r--   0 root         (0) root         (0)      617 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/jwt.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/rsa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/encrypt/vault/
--rw-r--r--   0 root         (0) root         (0)      173 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/vault/__init__.py
--rw-r--r--   0 root         (0) root         (0)      831 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/vault/base.py
--rw-r--r--   0 root         (0) root         (0)     3686 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/vault/cyberark.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/vault/plain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/logger/
--rw-r--r--   0 root         (0) root         (0)      171 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1947 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/logger/handler.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/script/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/__init__.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/base.py
--rw-r--r--   0 root         (0) root         (0)     5570 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/compile.py
--rw-r--r--   0 root         (0) root         (0)       95 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/info.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/service/
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/service/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1198 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/api/v0.py
--rw-r--r--   0 root         (0) root         (0)     4880 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/api/v1.py
--rw-r--r--   0 root         (0) root         (0)     4002 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/api/v2.py
--rw-r--r--   0 root         (0) root         (0)     1526 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/service/http/
--rw-r--r--   0 root         (0) root         (0)      164 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2493 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/base_api_client.py
--rw-r--r--   0 root         (0) root         (0)     3116 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/base_api_handler.py
--rw-r--r--   0 root         (0) root         (0)     1508 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/files.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/plain_http_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/service/openapi/
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/openapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4230 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/openapi/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/service/streamer/
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6839 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/base.py
--rw-r--r--   0 root         (0) root         (0)      547 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/managed_model.py
--rw-r--r--   0 root         (0) root         (0)     4132 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/multiprocess.py
--rw-r--r--   0 root         (0) root         (0)     6200 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/redis.py
--rw-r--r--   0 root         (0) root         (0)     1516 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/threaded.py
--rw-r--r--   0 root         (0) root         (0)     2179 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/web.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/testing/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/testing/service_v1.py
--rw-r--r--   0 root         (0) root         (0)     1001 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/testing/service_v2.py
--rw-r--r--   0 root         (0) root         (0)      183 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/testing/unit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/times/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/times/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6805 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/times/timeout_async.py
--rw-r--r--   0 root         (0) root         (0)     6972 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/times/timeout_asyncio.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/times/timeout_signal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.857252 aloha-2024.515.1337/aloha/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/html.py
--rw-r--r--   0 root         (0) root         (0)      530 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/json.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/random.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/sys_cuda.py
--rw-r--r--   0 root         (0) root         (0)     4335 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/sys_gpu.py
--rw-r--r--   0 root         (0) root         (0)     4306 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/sys_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.857252 aloha-2024.515.1337/aloha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4489 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1945 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 13:37:23.000000 aloha-2024.515.1337/aloha.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      570 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 13:37:27.861252 aloha-2024.515.1337/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2251 2024-05-15 13:37:15.000000 aloha-2024.515.1337/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.590255 aloha-2024.526.1153/
+-rw-r--r--   0 root         (0) root         (0)     4512 2024-05-26 11:53:06.590255 aloha-2024.526.1153/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-05-26 11:52:52.000000 aloha-2024.526.1153/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.574255 aloha-2024.526.1153/aloha/
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-26 11:53:06.000000 aloha-2024.526.1153/aloha/_version.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.574255 aloha-2024.526.1153/aloha/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/config/hocon.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/config/paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.574255 aloha-2024.526.1153/aloha/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/base.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/kafka.py
+-rw-r--r--   0 root         (0) root         (0)     9677 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/mongo.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/redis.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/db/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.578255 aloha-2024.526.1153/aloha/encrypt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3404 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/aes.py
+-rw-r--r--   0 root         (0) root         (0)      486 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/hash.py
+-rw-r--r--   0 root         (0) root         (0)      617 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/jwt.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/rsa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.578255 aloha-2024.526.1153/aloha/encrypt/vault/
+-rw-r--r--   0 root         (0) root         (0)      173 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/vault/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/vault/base.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/vault/cyberark.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/encrypt/vault/plain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.578255 aloha-2024.526.1153/aloha/logger/
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/logger/handler.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.578255 aloha-2024.526.1153/aloha/script/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/script/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/script/base.py
+-rw-r--r--   0 root         (0) root         (0)     5570 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/script/compile.py
+-rw-r--r--   0 root         (0) root         (0)       95 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/script/info.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/script/start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.578255 aloha-2024.526.1153/aloha/service/
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.578255 aloha-2024.526.1153/aloha/service/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/api/v0.py
+-rw-r--r--   0 root         (0) root         (0)     4880 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/api/v1.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/api/v2.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.582255 aloha-2024.526.1153/aloha/service/http/
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/http/base_api_client.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/http/base_api_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/http/files.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/http/plain_http_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.582255 aloha-2024.526.1153/aloha/service/openapi/
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/openapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/openapi/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.582255 aloha-2024.526.1153/aloha/service/streamer/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/streamer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/streamer/base.py
+-rw-r--r--   0 root         (0) root         (0)      547 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/streamer/managed_model.py
+-rw-r--r--   0 root         (0) root         (0)     4132 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/streamer/multiprocess.py
+-rw-r--r--   0 root         (0) root         (0)     6200 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/streamer/redis.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/streamer/threaded.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/service/web.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.582255 aloha-2024.526.1153/aloha/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/testing/service_v1.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/testing/service_v2.py
+-rw-r--r--   0 root         (0) root         (0)      183 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/testing/unit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.582255 aloha-2024.526.1153/aloha/times/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/times/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/times/timeout_async.py
+-rw-r--r--   0 root         (0) root         (0)     6972 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/times/timeout_asyncio.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/times/timeout_signal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.586255 aloha-2024.526.1153/aloha/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/util/html.py
+-rw-r--r--   0 root         (0) root         (0)      530 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/util/json.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/util/random.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/util/sys_cuda.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/util/sys_gpu.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2024-05-26 11:52:52.000000 aloha-2024.526.1153/aloha/util/sys_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 11:53:06.586255 aloha-2024.526.1153/aloha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4512 2024-05-26 11:53:06.000000 aloha-2024.526.1153/aloha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-05-26 11:53:06.000000 aloha-2024.526.1153/aloha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 11:53:06.000000 aloha-2024.526.1153/aloha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-26 11:53:06.000000 aloha-2024.526.1153/aloha.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 11:53:02.000000 aloha-2024.526.1153/aloha.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      554 2024-05-26 11:53:06.000000 aloha-2024.526.1153/aloha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-26 11:53:06.000000 aloha-2024.526.1153/aloha.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 11:53:06.590255 aloha-2024.526.1153/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2243 2024-05-26 11:52:52.000000 aloha-2024.526.1153/setup.py
```

### Comparing `aloha-2024.515.1337/PKG-INFO` & `aloha-2024.526.1153/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aloha
-Version: 2024.515.1337
+Version: 2024.526.1153
 Summary: Aloha - a versatile Python utility package for building services
 Home-page: https://github.com/QPod/aloha
 Author: QPod
 Author-email: 45032326+QPod0@users.noreply.github.com
 License: Apache Software License
 Project-URL: Source, https://github.com/QPod/aloha
 Project-URL: CI Pipeline, https://github.com/QPod/aloha/actions
@@ -28,20 +28,20 @@
 Requires-Dist: Cython; extra == "build"
 Provides-Extra: service
 Requires-Dist: requests; extra == "service"
 Requires-Dist: tornado; extra == "service"
 Requires-Dist: psutil; extra == "service"
 Requires-Dist: pyjwt; extra == "service"
 Provides-Extra: db
-Requires-Dist: sqlalchemy<2; extra == "db"
-Requires-Dist: psycopg2-binary; extra == "db"
+Requires-Dist: sqlalchemy; extra == "db"
+Requires-Dist: psycopg[binary]; extra == "db"
 Requires-Dist: pymysql; extra == "db"
 Requires-Dist: elasticsearch; extra == "db"
 Requires-Dist: pymongo; extra == "db"
-Requires-Dist: redis>4.2.0; extra == "db"
+Requires-Dist: redis; extra == "db"
 Provides-Extra: stream
 Requires-Dist: confluent_kafka; extra == "stream"
 Provides-Extra: data
 Requires-Dist: pandas; extra == "data"
 Provides-Extra: report
 Requires-Dist: openpyxl>=3; extra == "report"
 Requires-Dist: XlsxWriter; extra == "report"
@@ -60,28 +60,28 @@
 Requires-Dist: markdown-include; extra == "all"
 Requires-Dist: mkdocs; extra == "all"
 Requires-Dist: mkdocs-material; extra == "all"
 Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: openpyxl>=3; extra == "all"
 Requires-Dist: pandas; extra == "all"
 Requires-Dist: psutil; extra == "all"
-Requires-Dist: psycopg2-binary; extra == "all"
+Requires-Dist: psycopg[binary]; extra == "all"
 Requires-Dist: pyjwt; extra == "all"
 Requires-Dist: pymongo; extra == "all"
 Requires-Dist: pymysql; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: redis>4.2.0; extra == "all"
+Requires-Dist: redis; extra == "all"
 Requires-Dist: requests; extra == "all"
-Requires-Dist: sqlalchemy<2; extra == "all"
+Requires-Dist: sqlalchemy; extra == "all"
 Requires-Dist: tornado; extra == "all"
 
 # Aloha!
 
 [![License](https://img.shields.io/github/license/QPod/aloha)](https://github.com/QPod/aloha/blob/main/LICENSE)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/QPod/aloha/build)](https://github.com/QPod/aloha/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/QPod/aloha-python/pip.yml?branch=main)](https://github.com/QPod/aloha-python/actions)
 [![Join the Gitter Chat](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/QPod/)
 [![PyPI version](https://img.shields.io/pypi/v/aloha)](https://pypi.python.org/pypi/aloha/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/aloha)](https://pepy.tech/badge/aloha/)
 [![Code Activity](https://img.shields.io/github/commit-activity/m/QPod/aloha)](https://github.com/QPod/aloha/pulse)
 [![Recent Code Update](https://img.shields.io/github/last-commit/QPod/docker-images.svg)](https://github.com/QPod/aloha/stargazers)
 
 Please generously STAR★ our project or donate to us!  [![GitHub Starts](https://img.shields.io/github/stars/QPod/aloha.svg?label=Stars&style=social)](https://github.com/QPod/aloha/stargazers)
@@ -93,10 +93,10 @@
 
 `aloha` is a versatile Python utility package for building microservices.
 
 [📚 Document & 中文文档](https://aloha-python.readthedocs.io/)
 
 ## Getting started
 
-```py
+```shell
 pip install aloha[all]
 ```
```

### Comparing `aloha-2024.515.1337/README.md` & `aloha-2024.526.1153/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Aloha!
 
 [![License](https://img.shields.io/github/license/QPod/aloha)](https://github.com/QPod/aloha/blob/main/LICENSE)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/QPod/aloha/build)](https://github.com/QPod/aloha/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/QPod/aloha-python/pip.yml?branch=main)](https://github.com/QPod/aloha-python/actions)
 [![Join the Gitter Chat](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/QPod/)
 [![PyPI version](https://img.shields.io/pypi/v/aloha)](https://pypi.python.org/pypi/aloha/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/aloha)](https://pepy.tech/badge/aloha/)
 [![Code Activity](https://img.shields.io/github/commit-activity/m/QPod/aloha)](https://github.com/QPod/aloha/pulse)
 [![Recent Code Update](https://img.shields.io/github/last-commit/QPod/docker-images.svg)](https://github.com/QPod/aloha/stargazers)
 
 Please generously STAR★ our project or donate to us!  [![GitHub Starts](https://img.shields.io/github/stars/QPod/aloha.svg?label=Stars&style=social)](https://github.com/QPod/aloha/stargazers)
@@ -17,10 +17,10 @@
 
 `aloha` is a versatile Python utility package for building microservices.
 
 [📚 Document & 中文文档](https://aloha-python.readthedocs.io/)
 
 ## Getting started
 
-```py
+```shell
 pip install aloha[all]
 ```
```

### Comparing `aloha-2024.515.1337/aloha/config/hocon.py` & `aloha-2024.526.1153/aloha/config/hocon.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/config/paths.py` & `aloha-2024.526.1153/aloha/config/paths.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/db/base.py` & `aloha-2024.526.1153/aloha/db/base.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/db/elasticsearch.py` & `aloha-2024.526.1153/aloha/db/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/db/kafka.py` & `aloha-2024.526.1153/aloha/db/kafka.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/db/mongo.py` & `aloha-2024.526.1153/aloha/db/mongo.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/db/mysql.py` & `aloha-2024.526.1153/aloha/db/mysql.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/db/postgres.py` & `aloha-2024.526.1153/aloha/db/postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __all__ = ('PostgresOperator',)
 
-import psycopg2
+import psycopg
 from sqlalchemy import create_engine
 from sqlalchemy.sql import text
 
 from .base import PasswordVault
 from ..logger import LOG
 
-LOG.debug('postgres: psycopg2 version = %s' % psycopg2.__version__)
+LOG.debug('postgres: psycopg2 version = %s' % psycopg.__version__)
 
 
 class PostgresOperator:
     def __init__(self, db_config, **kwargs):
         password_vault = PasswordVault.get_vault(db_config.get('vault_type'), db_config.get('vault_config'))
         self._config = {
             'host': db_config['host'],
@@ -22,16 +22,16 @@
         }
         connect_args = {}
         if 'schema' in db_config:
             connect_args['options'] = '-csearch_path={}'.format(db_config['schema'])
 
         try:
             self.engine = create_engine(
-                'postgresql+psycopg2://{user}:{password}@{host}:{port}/{dbname}'.format(**self._config),
-                connect_args=connect_args, client_encoding='utf8', encoding='utf-8',
+                'postgresql+psycopg://{user}:{password}@{host}:{port}/{dbname}'.format(**self._config),
+                connect_args=connect_args, client_encoding='utf8',
                 pool_size=20, max_overflow=10, pool_pre_ping=True, **kwargs
             )
             LOG.debug("PostgresSQL connected: {host}:{port}/{dbname}".format(**self._config))
         except Exception as e:
             LOG.error(e)
             raise RuntimeError('Failed to connect to PostgresSQL')
```

### Comparing `aloha-2024.515.1337/aloha/db/redis.py` & `aloha-2024.526.1153/aloha/db/redis.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/db/sqlite.py` & `aloha-2024.526.1153/aloha/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/encrypt/aes.py` & `aloha-2024.526.1153/aloha/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/encrypt/jwt.py` & `aloha-2024.526.1153/aloha/encrypt/jwt.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/encrypt/rsa.py` & `aloha-2024.526.1153/aloha/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/encrypt/vault/base.py` & `aloha-2024.526.1153/aloha/encrypt/vault/base.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/encrypt/vault/cyberark.py` & `aloha-2024.526.1153/aloha/encrypt/vault/cyberark.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/encrypt/vault/plain.py` & `aloha-2024.526.1153/aloha/encrypt/vault/plain.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/logger/handler.py` & `aloha-2024.526.1153/aloha/logger/handler.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/logger/logger.py` & `aloha-2024.526.1153/aloha/logger/logger.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/script/base.py` & `aloha-2024.526.1153/aloha/script/base.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/script/compile.py` & `aloha-2024.526.1153/aloha/script/compile.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/script/start.py` & `aloha-2024.526.1153/aloha/script/start.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/api/v0.py` & `aloha-2024.526.1153/aloha/service/api/v0.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/api/v1.py` & `aloha-2024.526.1153/aloha/service/api/v1.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/api/v2.py` & `aloha-2024.526.1153/aloha/service/api/v2.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/app.py` & `aloha-2024.526.1153/aloha/service/app.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/http/base_api_client.py` & `aloha-2024.526.1153/aloha/service/http/base_api_client.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/http/base_api_handler.py` & `aloha-2024.526.1153/aloha/service/http/base_api_handler.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/http/files.py` & `aloha-2024.526.1153/aloha/service/http/files.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/http/plain_http_handler.py` & `aloha-2024.526.1153/aloha/service/http/plain_http_handler.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/openapi/client.py` & `aloha-2024.526.1153/aloha/service/openapi/client.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/streamer/base.py` & `aloha-2024.526.1153/aloha/service/streamer/base.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/streamer/managed_model.py` & `aloha-2024.526.1153/aloha/service/streamer/managed_model.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/streamer/multiprocess.py` & `aloha-2024.526.1153/aloha/service/streamer/multiprocess.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/streamer/redis.py` & `aloha-2024.526.1153/aloha/service/streamer/redis.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/streamer/threaded.py` & `aloha-2024.526.1153/aloha/service/streamer/threaded.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/service/web.py` & `aloha-2024.526.1153/aloha/service/web.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/settings.py` & `aloha-2024.526.1153/aloha/settings.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/testing/service_v1.py` & `aloha-2024.526.1153/aloha/testing/service_v1.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/testing/service_v2.py` & `aloha-2024.526.1153/aloha/testing/service_v2.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/times/timeout_async.py` & `aloha-2024.526.1153/aloha/times/timeout_async.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/times/timeout_asyncio.py` & `aloha-2024.526.1153/aloha/times/timeout_asyncio.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/times/timeout_signal.py` & `aloha-2024.526.1153/aloha/times/timeout_signal.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/util/html.py` & `aloha-2024.526.1153/aloha/util/html.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/util/json.py` & `aloha-2024.526.1153/aloha/util/json.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/util/sys_cuda.py` & `aloha-2024.526.1153/aloha/util/sys_cuda.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/util/sys_gpu.py` & `aloha-2024.526.1153/aloha/util/sys_gpu.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha/util/sys_info.py` & `aloha-2024.526.1153/aloha/util/sys_info.py`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha.egg-info/PKG-INFO` & `aloha-2024.526.1153/aloha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aloha
-Version: 2024.515.1337
+Version: 2024.526.1153
 Summary: Aloha - a versatile Python utility package for building services
 Home-page: https://github.com/QPod/aloha
 Author: QPod
 Author-email: 45032326+QPod0@users.noreply.github.com
 License: Apache Software License
 Project-URL: Source, https://github.com/QPod/aloha
 Project-URL: CI Pipeline, https://github.com/QPod/aloha/actions
@@ -28,20 +28,20 @@
 Requires-Dist: Cython; extra == "build"
 Provides-Extra: service
 Requires-Dist: requests; extra == "service"
 Requires-Dist: tornado; extra == "service"
 Requires-Dist: psutil; extra == "service"
 Requires-Dist: pyjwt; extra == "service"
 Provides-Extra: db
-Requires-Dist: sqlalchemy<2; extra == "db"
-Requires-Dist: psycopg2-binary; extra == "db"
+Requires-Dist: sqlalchemy; extra == "db"
+Requires-Dist: psycopg[binary]; extra == "db"
 Requires-Dist: pymysql; extra == "db"
 Requires-Dist: elasticsearch; extra == "db"
 Requires-Dist: pymongo; extra == "db"
-Requires-Dist: redis>4.2.0; extra == "db"
+Requires-Dist: redis; extra == "db"
 Provides-Extra: stream
 Requires-Dist: confluent_kafka; extra == "stream"
 Provides-Extra: data
 Requires-Dist: pandas; extra == "data"
 Provides-Extra: report
 Requires-Dist: openpyxl>=3; extra == "report"
 Requires-Dist: XlsxWriter; extra == "report"
@@ -60,28 +60,28 @@
 Requires-Dist: markdown-include; extra == "all"
 Requires-Dist: mkdocs; extra == "all"
 Requires-Dist: mkdocs-material; extra == "all"
 Requires-Dist: mkdocstrings[python]; extra == "all"
 Requires-Dist: openpyxl>=3; extra == "all"
 Requires-Dist: pandas; extra == "all"
 Requires-Dist: psutil; extra == "all"
-Requires-Dist: psycopg2-binary; extra == "all"
+Requires-Dist: psycopg[binary]; extra == "all"
 Requires-Dist: pyjwt; extra == "all"
 Requires-Dist: pymongo; extra == "all"
 Requires-Dist: pymysql; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: redis>4.2.0; extra == "all"
+Requires-Dist: redis; extra == "all"
 Requires-Dist: requests; extra == "all"
-Requires-Dist: sqlalchemy<2; extra == "all"
+Requires-Dist: sqlalchemy; extra == "all"
 Requires-Dist: tornado; extra == "all"
 
 # Aloha!
 
 [![License](https://img.shields.io/github/license/QPod/aloha)](https://github.com/QPod/aloha/blob/main/LICENSE)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/QPod/aloha/build)](https://github.com/QPod/aloha/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/QPod/aloha-python/pip.yml?branch=main)](https://github.com/QPod/aloha-python/actions)
 [![Join the Gitter Chat](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/QPod/)
 [![PyPI version](https://img.shields.io/pypi/v/aloha)](https://pypi.python.org/pypi/aloha/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/aloha)](https://pepy.tech/badge/aloha/)
 [![Code Activity](https://img.shields.io/github/commit-activity/m/QPod/aloha)](https://github.com/QPod/aloha/pulse)
 [![Recent Code Update](https://img.shields.io/github/last-commit/QPod/docker-images.svg)](https://github.com/QPod/aloha/stargazers)
 
 Please generously STAR★ our project or donate to us!  [![GitHub Starts](https://img.shields.io/github/stars/QPod/aloha.svg?label=Stars&style=social)](https://github.com/QPod/aloha/stargazers)
@@ -93,10 +93,10 @@
 
 `aloha` is a versatile Python utility package for building microservices.
 
 [📚 Document & 中文文档](https://aloha-python.readthedocs.io/)
 
 ## Getting started
 
-```py
+```shell
 pip install aloha[all]
 ```
```

### Comparing `aloha-2024.515.1337/aloha.egg-info/SOURCES.txt` & `aloha-2024.526.1153/aloha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aloha-2024.515.1337/aloha.egg-info/requires.txt` & `aloha-2024.526.1153/aloha.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 markdown-include
 mkdocs
 mkdocs-material
 mkdocstrings[python]
 openpyxl>=3
 pandas
 psutil
-psycopg2-binary
+psycopg[binary]
 pyjwt
 pymongo
 pymysql
 pytest-cov
-redis>4.2.0
+redis
 requests
-sqlalchemy<2
+sqlalchemy
 tornado
 
 [build]
 Cython
 
 [data]
 pandas
 
 [db]
-sqlalchemy<2
-psycopg2-binary
+sqlalchemy
+psycopg[binary]
 pymysql
 elasticsearch
 pymongo
-redis>4.2.0
+redis
 
 [docs]
 mkdocs
 mkdocstrings[python]
 markdown-include
 mkdocs-material
```

### Comparing `aloha-2024.515.1337/setup.py` & `aloha-2024.526.1153/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('./aloha/_version.py', 'wt') as fp:
     fp.write('__version__ = "%s"\n' % _version)
 
 dict_extra_requires = {
     'build': ['Cython'],
     'service': ['requests', 'tornado', 'psutil', 'pyjwt'],
-    'db': ['sqlalchemy<2', 'psycopg2-binary', 'pymysql', 'elasticsearch', 'pymongo', 'redis>4.2.0'],
+    'db': ['sqlalchemy', 'psycopg[binary]', 'pymysql', 'elasticsearch', 'pymongo', 'redis'],
     'stream': ['confluent_kafka'],
     'data': ['pandas'],
     'report': ['openpyxl>=3', 'XlsxWriter'],
     'test': ['pytest-cov'],
     'docs': ['mkdocs', 'mkdocstrings[python]', 'markdown-include', 'mkdocs-material'],
 }
```

