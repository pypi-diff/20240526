# Comparing `tmp/CryptoLyzer-0.9.0.tar.gz` & `tmp/CryptoLyzer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CryptoLyzer-0.9.0.tar", last modified: Mon May  1 08:45:42 2023, max compression
+gzip compressed data, was "CryptoLyzer-0.9.1.tar", last modified: Sat Jun 24 08:42:17 2023, max compression
```

## Comparing `CryptoLyzer-0.9.0.tar` & `CryptoLyzer-0.9.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:42.002791 CryptoLyzer-0.9.0/
--rw-r--r--   0 coroner   (1000) coroner   (1000)    12274 2023-04-29 11:50:32.000000 CryptoLyzer-0.9.0/CHANGELOG.rst
--rw-r--r--   0 coroner   (1000) coroner   (1000)     8624 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/CONTRIBUTING.rst
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.975790 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/
--rw-r--r--   0 coroner   (1000) coroner   (1000)     5325 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/PKG-INFO
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1849 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/SOURCES.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)        1 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/dependency_links.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)      108 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/entry_points.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)      346 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/requires.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)       12 2023-05-01 08:45:41.000000 CryptoLyzer-0.9.0/CryptoLyzer.egg-info/top_level.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)    16726 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/LICENSE.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)       39 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/MANIFEST.in
--rw-r--r--   0 coroner   (1000) coroner   (1000)     5325 2023-05-01 08:45:42.001791 CryptoLyzer-0.9.0/PKG-INFO
--rw-r--r--   0 coroner   (1000) coroner   (1000)     2835 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/README.rst
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.976790 CryptoLyzer-0.9.0/cryptolyzer/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/__init__.py
--rwxr-xr-x   0 coroner   (1000) coroner   (1000)     3682 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/__main__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      348 2023-04-29 11:50:32.000000 CryptoLyzer-0.9.0/cryptolyzer/__setup__.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.982790 CryptoLyzer-0.9.0/cryptolyzer/common/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/common/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     6603 2023-04-29 07:52:32.000000 CryptoLyzer-0.9.0/cryptolyzer/common/analyzer.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     4478 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/common/application.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    13527 2022-12-29 22:26:08.000000 CryptoLyzer-0.9.0/cryptolyzer/common/curves.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)   112140 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/common/dhparam.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     2191 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/common/exception.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    15739 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/common/prime.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     4115 2023-04-29 07:15:07.000000 CryptoLyzer-0.9.0/cryptolyzer/common/result.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    13229 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/common/transfer.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1902 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/common/utils.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     8977 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/common/x509.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.984790 CryptoLyzer-0.9.0/cryptolyzer/hassh/
--rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/hassh/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      442 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/hassh/analyzer.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1451 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/hassh/generate.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.985790 CryptoLyzer-0.9.0/cryptolyzer/httpx/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     2855 2022-12-29 22:47:54.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/analyzer.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     2365 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/client.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1713 2023-04-10 13:51:15.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/headers.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1286 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/httpx/transfer.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.987790 CryptoLyzer-0.9.0/cryptolyzer/ja3/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ja3/__init__.py
--rw-rw-r--   0 coroner   (1000) coroner   (1000)      514 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ja3/analyzer.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     4143 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ja3/decode.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1657 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/ja3/generate.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:41.991790 CryptoLyzer-0.9.0/cryptolyzer/ssh/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     3478 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/all.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1060 2022-12-29 22:26:08.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/analyzer.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     6110 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/ciphers.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    14712 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/client.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     5797 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/dhparams.py
--rw-rw-r--   0 coroner   (1000) coroner   (1000)      360 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/exception.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     4593 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/pubkeys.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     6808 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/server.py
--rw-rw-r--   0 coroner   (1000) coroner   (1000)     1178 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/transfer.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1741 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.0/cryptolyzer/ssh/versions.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:42.000790 CryptoLyzer-0.9.0/cryptolyzer/tls/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    11621 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/all.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     3244 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/analyzer.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     4712 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/application.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     8608 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/ciphers.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    54508 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/client.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     5834 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/curves.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    10170 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/dhparams.py
--rw-rw-r--   0 coroner   (1000) coroner   (1000)      270 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/exception.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    14786 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/extensions.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     4689 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/pubkeyreq.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    10841 2023-04-24 23:04:12.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/pubkeys.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    24496 2023-04-29 07:53:26.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/server.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     3705 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/sigalgos.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    14994 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/simulations.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     9279 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/versions.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     8512 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/cryptolyzer/tls/vulnerabilities.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      224 2023-04-29 12:32:57.000000 CryptoLyzer-0.9.0/requirements.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)       38 2023-05-01 08:45:42.002791 CryptoLyzer-0.9.0/setup.cfg
--rw-r--r--   0 coroner   (1000) coroner   (1000)     3950 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/setup.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-01 08:45:42.001791 CryptoLyzer-0.9.0/test/
--rw-r--r--   0 coroner   (1000) coroner   (1000)    10361 2023-04-06 21:17:28.000000 CryptoLyzer-0.9.0/test/test_main.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.199645 CryptoLyzer-0.9.1/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    12422 2023-06-23 14:52:13.000000 CryptoLyzer-0.9.1/CHANGELOG.rst
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8624 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/CONTRIBUTING.rst
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.189645 CryptoLyzer-0.9.1/CryptoLyzer.egg-info/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5528 2023-06-24 08:42:17.000000 CryptoLyzer-0.9.1/CryptoLyzer.egg-info/PKG-INFO
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1849 2023-06-24 08:42:17.000000 CryptoLyzer-0.9.1/CryptoLyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        1 2023-06-24 08:42:17.000000 CryptoLyzer-0.9.1/CryptoLyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      108 2023-06-24 08:42:17.000000 CryptoLyzer-0.9.1/CryptoLyzer.egg-info/entry_points.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      346 2023-06-24 08:42:17.000000 CryptoLyzer-0.9.1/CryptoLyzer.egg-info/requires.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       12 2023-06-24 08:42:17.000000 CryptoLyzer-0.9.1/CryptoLyzer.egg-info/top_level.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)    16726 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/LICENSE.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       39 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/MANIFEST.in
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5528 2023-06-24 08:42:17.199645 CryptoLyzer-0.9.1/PKG-INFO
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3038 2023-06-23 14:52:13.000000 CryptoLyzer-0.9.1/README.rst
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.189645 CryptoLyzer-0.9.1/cryptolyzer/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/__init__.py
+-rwxr-xr-x   0 coroner   (1000) coroner   (1000)     4153 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/__main__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      348 2023-06-23 14:52:13.000000 CryptoLyzer-0.9.1/cryptolyzer/__setup__.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.191645 CryptoLyzer-0.9.1/cryptolyzer/common/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/common/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     6689 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/common/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4478 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/common/application.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    13527 2022-12-29 22:26:08.000000 CryptoLyzer-0.9.1/cryptolyzer/common/curves.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5019 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/common/dhparam.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2191 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/common/exception.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    15739 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/common/prime.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4115 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/common/result.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    13229 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/common/transfer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1902 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/common/utils.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     9561 2023-06-22 09:58:06.000000 CryptoLyzer-0.9.1/cryptolyzer/common/x509.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.192645 CryptoLyzer-0.9.1/cryptolyzer/hassh/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.1/cryptolyzer/hassh/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      442 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.1/cryptolyzer/hassh/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1451 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.1/cryptolyzer/hassh/generate.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.193645 CryptoLyzer-0.9.1/cryptolyzer/httpx/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/httpx/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2878 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/httpx/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2365 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.1/cryptolyzer/httpx/client.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1713 2023-04-10 13:51:15.000000 CryptoLyzer-0.9.1/cryptolyzer/httpx/headers.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1414 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/httpx/transfer.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.193645 CryptoLyzer-0.9.1/cryptolyzer/ja3/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/ja3/__init__.py
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      514 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/ja3/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4143 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/ja3/decode.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1657 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.1/cryptolyzer/ja3/generate.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.195645 CryptoLyzer-0.9.1/cryptolyzer/ssh/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3478 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/all.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1060 2022-12-29 22:26:08.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     6110 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/ciphers.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    14711 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/client.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5797 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/dhparams.py
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      360 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/exception.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4593 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/pubkeys.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     6808 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/server.py
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)     1178 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/transfer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1741 2023-01-08 12:18:44.000000 CryptoLyzer-0.9.1/cryptolyzer/ssh/versions.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.199645 CryptoLyzer-0.9.1/cryptolyzer/tls/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    11626 2023-06-22 08:32:27.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/all.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3244 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/analyzer.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4712 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/application.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8608 2023-06-23 21:53:42.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/ciphers.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    54532 2023-06-22 08:32:27.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/client.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5834 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/curves.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    10037 2023-06-23 14:52:13.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/dhparams.py
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      270 2022-03-20 16:52:35.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/exception.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    14786 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/extensions.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     4689 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/pubkeyreq.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    12415 2023-06-22 08:35:19.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/pubkeys.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    24496 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/server.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3705 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/sigalgos.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    15310 2023-06-22 08:32:27.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/simulations.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     9279 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/versions.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8512 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/cryptolyzer/tls/vulnerabilities.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      224 2023-06-23 14:52:13.000000 CryptoLyzer-0.9.1/requirements.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       38 2023-06-24 08:42:17.200645 CryptoLyzer-0.9.1/setup.cfg
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3950 2023-06-23 20:38:38.000000 CryptoLyzer-0.9.1/setup.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-24 08:42:17.199645 CryptoLyzer-0.9.1/test/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    10630 2023-06-19 13:34:11.000000 CryptoLyzer-0.9.1/test/test_main.py
```

### Comparing `CryptoLyzer-0.9.0/CHANGELOG.rst` & `CryptoLyzer-0.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+0.9.1 - 2023-06-22
+------------------
+
+-  TLS (``tls``)
+
+   -  Public Keys (``pubkeys``)
+
+      -  certificate transparency (CT) log support (#47)
+
 0.9.0 - 2023-04-29
 ------------------
 
 -  TLS (``tls``)
 
    -  Generic
```

### Comparing `CryptoLyzer-0.9.0/CONTRIBUTING.rst` & `CryptoLyzer-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/CryptoLyzer.egg-info/PKG-INFO` & `CryptoLyzer-0.9.1/CryptoLyzer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CryptoLyzer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Fast and flexible cryptographic protocol analyzer
 Author: Szilárd Pfeiffer
 Author-email: coroner@pfeifferszilard.hu
 Maintainer: Szilárd Pfeiffer
 Maintainer-email: coroner@pfeifferszilard.hu
 License: MPL-2.0
 Project-URL: Homepage, https://gitlab.com/coroner/cryptolyzer
@@ -133,7 +133,13 @@
 License
 -------
 
 The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
 
 A non-comprehensive, but straightforward description of MPL 2.0 can be found at
 `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
+
+Credits
+-------
+
+-  `NLnet Foundation <https://nlnet.nl>`__ and `NGI Assure <https://www.assure.ngi.eu>`__, supports the project part of
+   the `Next Generation Internet <https://ngi.eu>`__ initiative.
```

### Comparing `CryptoLyzer-0.9.0/CryptoLyzer.egg-info/SOURCES.txt` & `CryptoLyzer-0.9.1/CryptoLyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/LICENSE.txt` & `CryptoLyzer-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/PKG-INFO` & `CryptoLyzer-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CryptoLyzer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Fast and flexible cryptographic protocol analyzer
 Author: Szilárd Pfeiffer
 Author-email: coroner@pfeifferszilard.hu
 Maintainer: Szilárd Pfeiffer
 Maintainer-email: coroner@pfeifferszilard.hu
 License: MPL-2.0
 Project-URL: Homepage, https://gitlab.com/coroner/cryptolyzer
@@ -133,7 +133,13 @@
 License
 -------
 
 The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
 
 A non-comprehensive, but straightforward description of MPL 2.0 can be found at
 `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
+
+Credits
+-------
+
+-  `NLnet Foundation <https://nlnet.nl>`__ and `NGI Assure <https://www.assure.ngi.eu>`__, supports the project part of
+   the `Next Generation Internet <https://ngi.eu>`__ initiative.
```

### Comparing `CryptoLyzer-0.9.0/README.rst` & `CryptoLyzer-0.9.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -79,7 +79,13 @@
 License
 -------
 
 The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
 
 A non-comprehensive, but straightforward description of MPL 2.0 can be found at
 `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
+
+Credits
+-------
+
+-  `NLnet Foundation <https://nlnet.nl>`__ and `NGI Assure <https://www.assure.ngi.eu>`__, supports the project part of
+   the `Next Generation Internet <https://ngi.eu>`__ initiative.
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/__main__.py` & `CryptoLyzer-0.9.1/cryptolyzer/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,23 @@
     ]
     if unsupported_schemes:
         parser.error('unsupported protocol: {}'.format(', '.join(unsupported_schemes)))
 
     return protocol_handler, analyzer, targets
 
 
+def parse_arg_socket_timeout(value):
+    value = float(value)
+
+    if value <= 0:
+        raise argparse.ArgumentTypeError("%s socket timeout must be a positive integer value" % value)
+
+    return value
+
+
 def get_argument_parser():
     parser = argparse.ArgumentParser(prog='cryptolyze')
     parser.add_argument('--version', '-v', action='version', version='%(prog)s ' + __setup__.__version__)
     parser.add_argument(
         '--log-level',
         choices=['debug', 'info', 'warning', 'error', 'critical'],
         default='info',
@@ -52,14 +61,21 @@
     )
     parser.add_argument(
         '--output-format',
         choices=['json', 'markdown'],
         default='markdown',
         help='format of the anlysis result (default: %(default)s)'
     )
+    parser.add_argument(
+        '-t', '--socket-timeout',
+        type=parse_arg_socket_timeout,
+        default=5,
+        metavar='seconds',
+        help='Maximum time to wait for server to responde (default: %(default)s seconds)'
+    )
 
     parsers_analyzer = parser.add_subparsers(title='protocol', dest='protocol')
     parsers_analyzer.required = True
     for protocol in ProtocolHandlerBase.get_protocols():
         protocol_handler = ProtocolHandlerBase.from_protocol(protocol)
         analyzers = protocol_handler.get_analyzers()
         parser_analyzer = parsers_analyzer.add_parser(protocol)
@@ -80,15 +96,15 @@
 def main():
     parser = get_argument_parser()
     arguments = parser.parse_args()
     protocol_handler, analyzer, targets = get_protocol_handler_analyzer_and_uris(parser, arguments)
 
     for target in targets:
         try:
-            analyzer_result = protocol_handler.analyze(analyzer, target)
+            analyzer_result = protocol_handler.analyze(analyzer, target, arguments.socket_timeout)
         except (NetworkError, SecurityError, InvalidDataLength, InvalidType, InvalidValue) as e:
             analyzer_result = AnalyzerResultError(str(target), str(e))
 
         if arguments.output_format == 'json':
             print(analyzer_result.as_json())
         elif arguments.output_format == 'markdown':
             print(analyzer_result.as_markdown())
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/analyzer.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,20 +97,22 @@
         for analyzer_class in cls.get_analyzers():
             for client_class in analyzer_class.get_clients():
                 if client_class.get_scheme() == uri.scheme:
                     return client_class.from_scheme(**kwargs)
 
         raise NotImplementedError()
 
-    def analyze(self, analyzer, uri):
+    def analyze(self, analyzer, uri, timeout=None):
         LogSingleton().log(level=60, msg=six.u('Analysis started; protocol="%s", analyzer="%s"') % (
             self.get_protocol(), analyzer.get_name(),
         ))
 
         l7_client = self._l7_client_from_uri(uri)
+        if timeout is not None:
+            l7_client.timeout = timeout
         args, kwargs = self._get_analyzer_args()
         return analyzer.analyze(l7_client, *args, **kwargs)
 
     @classmethod
     def analyzer_from_name(cls, name):
         analyzer_list = [
             analyzer_class
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/application.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/application.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/curves.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/curves.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/exception.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/exception.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/prime.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/prime.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/result.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/result.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/transfer.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/transfer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/utils.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/utils.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/common/x509.py` & `CryptoLyzer-0.9.1/cryptolyzer/common/x509.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import datetime
 
 from collections import OrderedDict
 
 import asn1crypto.x509
 import attr
 
+from cryptodatahub.common.algorithm import Authentication, Hash, Signature
+
 import cryptoparser.common.key
 import cryptoparser.common.utils
-from cryptodatahub.common.algorithm import Authentication, Hash, Signature
+from cryptoparser.common.x509 import SignedCertificateTimestampList
 
 
 class PublicKey(cryptoparser.common.key.PublicKey):
     @property
     @abc.abstractmethod
     def key_bytes(self):
         raise NotImplementedError()
@@ -221,14 +223,23 @@
         ]
 
     @property
     def ocsp_responders(self):
         return self.certificate.ocsp_urls
 
     @property
+    def signed_certificate_timestamps(self):
+        for extension in self.certificate['tbs_certificate']['extensions']:
+            if extension['extn_id'].dotted == '1.3.6.1.4.1.11129.2.4.2':
+                asn1_value = asn1crypto.core.load(bytes(extension['extn_value']))
+                return SignedCertificateTimestampList.parse_exact_size(bytes(asn1_value))
+
+        return SignedCertificateTimestampList([])
+
+    @property
     def is_ca(self):
         return self.certificate.ca
 
     @property
     def is_self_signed(self):
         return self.certificate.self_issued
 
@@ -259,11 +270,12 @@
                 ('period', str(self.validity_period)),
                 ('remaining', str(self.validity_remaining_time.days) if self.validity_remaining_time else None),
             ])),
             ('revocation', OrderedDict([
                 ('crl_distribution_points', self.crl_distribution_points),
                 ('ocsp_responders', self.ocsp_responders),
             ])),
+            ('signed_certificate_timestamps', self.signed_certificate_timestamps),
             ('fingerprints', self.fingerprints),
             ('public_key_pin', self.public_key_pin),
             ('version', self.certificate['tbs_certificate']['version'].native),
         ])
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/hassh/generate.py` & `CryptoLyzer-0.9.1/cryptolyzer/hassh/generate.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/httpx/analyzer.py` & `CryptoLyzer-0.9.1/cryptolyzer/httpx/analyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,20 +81,20 @@
     def get_protocol(cls):
         return 'http'
 
     @classmethod
     def _get_version(cls):
         raise NotImplementedError()
 
-    def analyze(self, analyzer, uri):
+    def analyze(self, analyzer, uri, timeout=None):
         results = []
         target = None
         for protocol_handler_class in get_leaf_classes(ProtocolHandlerHttpExactVersion):
             if isinstance(analyzer, protocol_handler_class.get_analyzers()):
-                result = protocol_handler_class().analyze(analyzer, uri)
+                result = protocol_handler_class().analyze(analyzer, uri, timeout)
                 target = result.target
 
                 results.append(
                     (protocol_handler_class._get_version(), result)  # pylint: disable=protected-access
                 )
 
         return AnalyzerResultHttpAllSupportedVersions(target, OrderedDict(results))
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/httpx/client.py` & `CryptoLyzer-0.9.1/cryptolyzer/httpx/client.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/httpx/headers.py` & `CryptoLyzer-0.9.1/cryptolyzer/httpx/headers.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/httpx/transfer.py` & `CryptoLyzer-0.9.1/cryptolyzer/httpx/transfer.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 
 
 @attr.s
 class HttpHandshakeBase(object):
     timeout = attr.ib(validator=attr.validators.instance_of((float, int)))
     response = attr.ib(init=False, validator=attr.validators.instance_of(requests.Response))
 
+    @classmethod
+    def _get_verify_path(cls):
+        return None  # use default verify path
+
     @property
     def raw_headers(self):
         raw_headers = '\r\n'.join([
             '{}: {}'.format(name, value)
             for name, value in self.response.headers.items()
         ]) + '\r\n'
 
         if len(self.response.headers) == 1:
             raw_headers += '\r\n'
 
         return raw_headers.encode('ascii')
 
     def do_handshake(self, transfer):
         try:
-            self.response = requests.head(transfer.uri, timeout=self.timeout)
+            self.response = requests.head(transfer.uri, verify=self._get_verify_path(), timeout=self.timeout)
         except (requests.exceptions.ConnectionError, requests.exceptions.Timeout) as e:
             six.raise_from(NetworkError(NetworkErrorType.NO_CONNECTION), e)
         except requests.exceptions.HTTPError as e:
             # HTTP request returned an unsuccessful status code
             six.raise_from(NetworkError(NetworkErrorType.NO_RESPONSE), e)
         except requests.exceptions.TooManyRedirects as e:
             six.raise_from(NetworkError(NetworkErrorType.NO_RESPONSE), e)
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ja3/analyzer.py` & `CryptoLyzer-0.9.1/cryptolyzer/ja3/analyzer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ja3/decode.py` & `CryptoLyzer-0.9.1/cryptolyzer/ja3/decode.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ja3/generate.py` & `CryptoLyzer-0.9.1/cryptolyzer/ja3/generate.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/all.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/all.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/analyzer.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/analyzer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/ciphers.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/ciphers.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/client.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     SshProtocolMessage,
 )
 from cryptoparser.ssh.version import SshProtocolVersion, SshSoftwareVersionUnparsed, SshVersion
 
 from cryptolyzer import __setup__
 
 from cryptolyzer.common.dhparam import (
-    WellKnownDHParams,
+    DHParamWellKnown,
     bytes_to_int,
     get_dh_ephemeral_key_forged,
     get_ecdh_ephemeral_key_forged,
     int_to_bytes,
 )
 from cryptolyzer.common.exception import NetworkError, NetworkErrorType
 from cryptolyzer.common.transfer import L4ClientTCP, L7TransferBase
@@ -270,17 +270,17 @@
                 gex_max=gex_params.gex_max,
                 gex_number=gex_params.gex_number,
             )).compose())
             raise IndexError(record_class)
 
         record_class = SshRecordKexDH
         key_size = agreed_kex_type.value.key_size
-        for dh_param in WellKnownDHParams:
+        for dh_param in DHParamWellKnown:
             if dh_param.value.key_size == key_size:
-                ephemeral_public_key = get_dh_ephemeral_key_forged(dh_param.value.dh_param_numbers.p)
+                ephemeral_public_key = get_dh_ephemeral_key_forged(dh_param.value.parameter_numbers.p)
                 ephemeral_public_key_bytes = int_to_bytes(ephemeral_public_key, key_size).lstrip(b'\x00')
                 break
         else:
             raise NotImplementedError()
 
         transfer.send(record_class(SshDHKeyExchangeInit(ephemeral_public_key_bytes)).compose())
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/dhparams.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/dhparams.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/pubkeys.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/pubkeys.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/server.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/server.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/transfer.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/transfer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/ssh/versions.py` & `CryptoLyzer-0.9.1/cryptolyzer/ssh/versions.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/all.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/all.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
         return AnalyzerAll._get_result(AnalyzerPublicKeyRequest, analyzable, protocol_version)
 
     @staticmethod
     def is_public_key_supported(cipher_suite_results):
         for protocol_version, cipher_suite_result in cipher_suite_results.items():
             for cipher_suite in cipher_suite_result.cipher_suites:
-                if cipher_suite.value.authentication != Authentication.anon:
+                if cipher_suite.value.authentication != Authentication.ANONYMOUS:
                     return protocol_version
 
         return None
 
     @staticmethod
     def get_pubkeys_result(analyzable, cipher_suite_results):
         protocol_version = AnalyzerAll.is_public_key_supported(cipher_suite_results)
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/analyzer.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/analyzer.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/application.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/application.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/ciphers.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/ciphers.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/client.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,42 +66,42 @@
     OpenVpnPacketHardResetClientV2,
 )
 
 from cryptoparser.tls.record import TlsRecord, SslRecord
 from cryptoparser.tls.version import TlsVersion, TlsProtocolVersion
 
 from cryptolyzer.common.dhparam import (
-    WellKnownDHParams,
+    DHParamWellKnown,
     get_dh_ephemeral_key_forged,
     get_ecdh_ephemeral_key_forged,
     int_to_bytes,
 )
 from cryptolyzer.common.exception import NetworkError, NetworkErrorType, SecurityError, SecurityErrorType
 from cryptolyzer.common.transfer import L4ClientTCP, L4ClientUDP, L7TransferBase
 from cryptolyzer.common.utils import buffer_flush, buffer_is_plain_text
 
 from cryptolyzer.tls.application import L7OpenVpnBase
 from cryptolyzer.tls.exception import TlsAlert
 
 
 NAMED_CURVE_TO_RFC7919_WELL_KNOWN = {
-    TlsNamedCurve.FFDHE2048: WellKnownDHParams.RFC7919_2048_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
-    TlsNamedCurve.FFDHE3072: WellKnownDHParams.RFC7919_3072_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
-    TlsNamedCurve.FFDHE4096: WellKnownDHParams.RFC7919_4096_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
-    TlsNamedCurve.FFDHE6144: WellKnownDHParams.RFC7919_6144_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
-    TlsNamedCurve.FFDHE8192: WellKnownDHParams.RFC7919_8192_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
+    TlsNamedCurve.FFDHE2048: DHParamWellKnown.RFC7919_2048_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
+    TlsNamedCurve.FFDHE3072: DHParamWellKnown.RFC7919_3072_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
+    TlsNamedCurve.FFDHE4096: DHParamWellKnown.RFC7919_4096_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
+    TlsNamedCurve.FFDHE6144: DHParamWellKnown.RFC7919_6144_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
+    TlsNamedCurve.FFDHE8192: DHParamWellKnown.RFC7919_8192_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP,
 }
 
 
 RFC7919_WELL_KNOWN_TO_NAMED_CURVE = {
-    WellKnownDHParams.RFC7919_2048_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE2048,
-    WellKnownDHParams.RFC7919_3072_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE3072,
-    WellKnownDHParams.RFC7919_4096_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE4096,
-    WellKnownDHParams.RFC7919_6144_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE6144,
-    WellKnownDHParams.RFC7919_8192_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE8192,
+    DHParamWellKnown.RFC7919_2048_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE2048,
+    DHParamWellKnown.RFC7919_3072_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE3072,
+    DHParamWellKnown.RFC7919_4096_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE4096,
+    DHParamWellKnown.RFC7919_6144_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE6144,
+    DHParamWellKnown.RFC7919_8192_BIT_FINITE_FIELD_DIFFIE_HELLMAN_GROUP: TlsNamedCurve.FFDHE8192,
 }
 
 
 def key_share_entry_from_named_curve(named_curve):
     if named_curve.value.named_group.value.group_type == NamedGroupType.ELLIPTIC_CURVE:
         return TlsKeyShareEntry(
             named_curve,
@@ -109,27 +109,27 @@
         )
 
     if named_curve.value.named_group.value.group_type == NamedGroupType.DH_PARAM:
         well_known_dh_param = NAMED_CURVE_TO_RFC7919_WELL_KNOWN[named_curve]
         return TlsKeyShareEntry(
             named_curve,
             int_to_bytes(
-                get_dh_ephemeral_key_forged(well_known_dh_param.value.dh_param_numbers.p),
+                get_dh_ephemeral_key_forged(well_known_dh_param.value.parameter_numbers.p),
                 well_known_dh_param.value.key_size // 8
             )
         )
 
     raise NotImplementedError()
 
 
 class TlsHandshakeClientHelloSpecalization(TlsHandshakeClientHello):
     @classmethod
     def _get_signature_algorithms(cls, is_tls1_3_supported, cipher_suites):
         if is_tls1_3_supported:
-            authentications_not_exist_in_tls1_3 = [Authentication.anon, Authentication.DSS]
+            authentications_not_exist_in_tls1_3 = [Authentication.ANONYMOUS, Authentication.DSS]
             signature_algorithms = [
                 signature_algorithm
                 for signature_algorithm in TlsSignatureAndHashAlgorithm
                 if (signature_algorithm.value.signature_algorithm not in authentications_not_exist_in_tls1_3 and
                     signature_algorithm.value.hash_algorithm is not None)
             ]
         else:
@@ -322,15 +322,15 @@
             for cipher_suite in TlsCipherSuite
             if (cipher_suite.value.authentication and
                 cipher_suite.value.authentication in [
                     Authentication.DSS,
                     Authentication.KRB5,
                     Authentication.PSK,
                     Authentication.SRP,
-                    Authentication.anon,
+                    Authentication.ANONYMOUS,
                 ])
         ]
 
         super(TlsHandshakeClientHelloAuthenticationRarelyUsed, self).__init__(
             hostname=hostname,
             protocol_versions=[protocol_version, ],
             cipher_suites=_cipher_suites,
@@ -1141,18 +1141,18 @@
     def _deinit_l7(self):
         pass
 
 
 @attr.s
 class ClientXMPP(L7ClientStartTlsBase):
     _STREAM_OPEN = (
-        '<stream:stream xmlns=\'jabber:client\' xmlns:stream=\'http://etherx.jabber.org/streams\' '
-        'xmlns:tls=\'http://www.ietf.org/rfc/rfc2595.txt\' to=\'{}\' xml:lang=\'en\' version=\'1.0\'>'
+        '<stream:stream xmlns="jabber:client" xmlns:stream="http://etherx.jabber.org/streams" '
+        'xmlns:tls="http://www.ietf.org/rfc/rfc2595.txt" to="{}" xml:lang="en" version="1.0">'
     )
-    _STARTTLS = b'<starttls xmlns=\'urn:ietf:params:xml:ns:xmpp-tls\'/>'
+    _STARTTLS = b'<starttls xmlns="urn:ietf:params:xml:ns:xmpp-tls"/>'
 
     @classmethod
     def get_scheme(cls):
         return 'xmpp'
 
     @classmethod
     def get_default_port(cls):
@@ -1168,26 +1168,26 @@
 
         if b'stream:error' in l4_transfer.buffer:
             raise SecurityError(SecurityErrorType.UNPARSABLE_MESSAGE)
 
         if b'stream:features' not in l4_transfer.buffer:
             l4_transfer.receive_until(b'</stream:features>')
 
-        if b'<starttls xmlns=\'urn:ietf:params:xml:ns:xmpp-tls\'>' not in l4_transfer.buffer:
+        if b'<starttls xmlns="urn:ietf:params:xml:ns:xmpp-tls">' not in l4_transfer.buffer.replace(b'\'', b'"'):
             raise SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY)
 
         l4_transfer.flush_buffer()
 
         l4_transfer.send(ClientXMPP._STARTTLS)
         l4_transfer.receive_until(b'>')
 
         if b'stream:error' in l4_transfer.buffer:
             raise SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY)
 
-        if l4_transfer.buffer != b'<proceed xmlns=\'urn:ietf:params:xml:ns:xmpp-tls\'/>':
+        if l4_transfer.buffer.replace(b'\'', b'"') != b'<proceed xmlns="urn:ietf:params:xml:ns:xmpp-tls"/>':
             raise SecurityError(SecurityErrorType.UNSUPPORTED_SECURITY)
 
         l4_transfer.flush_buffer()
 
     def _init_l7(self):
         self._l7_client = L7ClientTls(self.address, self.port, self.timeout)
         self._l7_client.init_connection()
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/curves.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/curves.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/dhparams.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/dhparams.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def _get_public_key_tls_1_3(server_messages):
         key_share_extension = AnalyzerDHParams._get_extension_key_share(server_messages)
         well_known = NAMED_CURVE_TO_RFC7919_WELL_KNOWN[key_share_extension.key_share_entry.group]
         y = int(  # pylint: disable=invalid-name
             codecs.encode(bytes(list(key_share_extension.key_share_entry.key_exchange)), 'hex_codec'), 16
         )
 
-        public_numbers = DHPublicNumbers(y, well_known.value.dh_param_numbers)
+        public_numbers = DHPublicNumbers(y, well_known.value.parameter_numbers)
 
         return DHPublicKey(public_numbers, well_known.value.key_size)
 
     @staticmethod
     def _get_public_key_tls_1_x(server_messages):
         server_key_exchange_message = server_messages[TlsHandshakeType.SERVER_KEY_EXCHANGE]
         return parse_tls_dh_params(server_key_exchange_message.param_bytes)
@@ -162,35 +162,35 @@
             if is_rfc7919_dhparam:
                 named_group = RFC7919_WELL_KNOWN_TO_NAMED_CURVE[_dhparam.well_known]
 
                 # no supported group extension, but FFDHE parameter is used
                 if not has_extenstion or named_group in named_groups:
                     dhparam = _dhparam
                     named_groups = []
-                    LogSingleton().log(level=60, msg=six.u('Server offers well-known DH public parameter %s (%s)') % (
-                        dhparam.well_known.value.name, client_hello.protocol_version,
+                    LogSingleton().log(level=60, msg=six.u('Server offers %s (%s)') % (
+                        dhparam.well_known.value, client_hello.protocol_version,
                     ))
                     break
 
                 has_extenstion = AnalyzerDHParams._remove_selected_group_among_supported_ones(client_hello, named_group)
                 named_groups.append(named_group)
-                LogSingleton().log(level=60, msg=six.u('Server offers FFDHE public parameter with size %d-bit (%s)') % (
-                    named_group.value.named_group.value.size, client_hello.protocol_version,
+                LogSingleton().log(level=60, msg=six.u('Server offers %s (%s)') % (
+                    _dhparam.well_known.value, client_hello.protocol_version,
                 ))
             else:
                 # no extension support, so only one DH parameter is possible
                 dhparam = _dhparam
                 if dhparam.well_known:
-                    LogSingleton().log(level=60, msg=six.u('Server offers well-known DH public parameter %s (%s)') % (
-                        dhparam.well_known.value.name, client_hello.protocol_version,
+                    LogSingleton().log(level=60, msg=six.u('Server offers %s (%s)') % (
+                        dhparam.well_known.value, client_hello.protocol_version,
                     ))
                 else:
                     LogSingleton().log(
                         level=60,
-                        msg=six.u('Server offers custom DH public parameter with size %d-bit (%s)') % (
+                        msg=six.u('Server offers %s-bit custom DH public parameter (%s)') % (
                             dhparam.key_size, client_hello.protocol_version,
                         )
                     )
                 break
 
         return dhparam, named_groups
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/extensions.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/extensions.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/pubkeyreq.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/pubkeyreq.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/pubkeys.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/pubkeys.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,22 @@
 
 import asn1crypto.ocsp
 import asn1crypto.x509
 import certvalidator
 
 from cryptoparser.common.base import Serializable
 import cryptoparser.common.utils
+from cryptoparser.common.x509 import SignedCertificateTimestampList
 from cryptoparser.tls.subprotocol import TlsHandshakeType, TlsAlertDescription
-from cryptoparser.tls.extension import TlsExtensionCertificateStatusRequest, TlsCertificateStatusType
+from cryptoparser.tls.extension import (
+    TlsExtensionCertificateStatusRequestClient,
+    TlsExtensionSignedCertificateTimestampClient,
+    TlsExtensionType,
+    TlsCertificateStatusType,
+)
 
 from cryptolyzer.common.analyzer import AnalyzerTlsBase
 from cryptolyzer.common.utils import LogSingleton
 from cryptolyzer.tls.client import (
     TlsHandshakeClientHelloAuthenticationDSS,
     TlsHandshakeClientHelloAuthenticationRSA,
     TlsHandshakeClientHelloAuthenticationECDSA,
@@ -84,27 +90,35 @@
     def revocation_reason(self):
         cert_status = self._response['cert_status']
         if cert_status.name != 'revoked':
             return None
 
         return cert_status.chosen['revocation_reason'].native
 
+    @property
+    def extensions(self):
+        return [
+            extension['extn_id'].dotted
+            for extension in self._response['single_extensions']
+        ]
+
     def _asdict(self):
         if self.ocsp_response is None:
             return OrderedDict()
 
         return OrderedDict([
            ('status', self.status),
            ('responder', self.responder),
            ('produced_at', str(self.produced_at)),
            ('this_update', str(self.this_update)),
            ('next_update', str(self.next_update)),
            ('update_interval', str(self.update_interval)),
            ('revocation_time', str(self.revocation_time)),
            ('revocation_time', self.revocation_reason),
+           ('extensions', self.extensions),
         ])
 
 
 @attr.s
 class TlsCertificateChain(Serializable):  # pylint: disable=too-few-public-methods
     items = attr.ib(
         validator=attr.validators.deep_iterable(attr.validators.instance_of(cryptolyzer.common.x509.PublicKeyX509)),
@@ -159,14 +173,19 @@
         validator=attr.validators.instance_of(TlsCertificateChain),
         metadata={'human_readable_name': 'Certificate Chain'}
     )
     certificate_status = attr.ib(
         default=None, eq=False,
         validator=attr.validators.optional(attr.validators.instance_of(CertificateStatus))
     )
+    scts = attr.ib(
+        default=None, eq=False,
+        validator=attr.validators.optional(attr.validators.instance_of(SignedCertificateTimestampList)),
+        metadata={'human_readable_name': 'Signed Certificate Timestamps'}
+    )
 
 
 @attr.s
 class AnalyzerResultPublicKeys(AnalyzerResultTls):  # pylint: disable=too-few-public-methods
     pubkeys = attr.ib(
         validator=attr.validators.deep_iterable(attr.validators.instance_of(TlsPublicKey)),
         metadata={'human_readable_name': 'TLS Certificates'},
@@ -192,46 +211,69 @@
         for tls_certificate in server_messages[TlsHandshakeType.CERTIFICATE].certificate_chain:
             certificate = asn1crypto.x509.Certificate.load(tls_certificate.certificate)
             certificate_chain.append(cryptolyzer.common.x509.PublicKeyX509(certificate))
 
         return TlsCertificateChain(items=certificate_chain)
 
     @classmethod
+    def _get_certificate_status(cls, server_messages):
+        if TlsHandshakeType.CERTIFICATE_STATUS in server_messages:
+            status_message = server_messages[TlsHandshakeType.CERTIFICATE_STATUS]
+            if status_message.status_type == TlsCertificateStatusType.OCSP:
+                ocsp_response = asn1crypto.ocsp.OCSPResponse.load(bytes(status_message.status))
+                if ocsp_response['response_status'].native == 'successful':
+                    return CertificateStatus(
+                        asn1crypto.ocsp.OCSPResponse.load(bytes(status_message.status))
+                    )
+
+        # Server may send the same certificate chain independently that client hello conatins SNI exetension, however
+        # OCSP staple not necessarily sent in both cases. New status values stored only if no one had # already stored.
+        raise KeyError()
+
+    @classmethod
+    def _get_signed_certificate_timestamps(cls, server_messages):
+        server_hello = server_messages[TlsHandshakeType.SERVER_HELLO]
+        sct_extension = server_hello.extensions.get_item_by_type(TlsExtensionType.SIGNED_CERTIFICATE_TIMESTAMP)
+
+        return sct_extension.scts
+
+    @classmethod
     def _add_tls_public_key_to_results(cls, analyzable, sni_sent, server_messages, results):
         try:
             certificate_chain = cls._get_tls_certificate_chain(server_messages)
         except ValueError:
             return
 
         leaf_certificate = certificate_chain.items[0]
         subject_matches = leaf_certificate.is_subject_matches(six.u(analyzable.address))
-        if ((sni_sent or subject_matches) and
-                certificate_chain not in [result.tls_certificate_chain for result in results]):
-            tls_public_key_params = {
-                'sni_sent': sni_sent,
-                'subject_matches': subject_matches,
-                'tls_certificate_chain': certificate_chain,
-            }
-
-            if TlsHandshakeType.CERTIFICATE_STATUS in server_messages:
-                status_message = server_messages[TlsHandshakeType.CERTIFICATE_STATUS]
-                if status_message.status_type == TlsCertificateStatusType.OCSP:
-                    ocsp_response = asn1crypto.ocsp.OCSPResponse.load(bytes(status_message.status))
-                    if ocsp_response['response_status'].native == 'successful':
-                        certificate_status = CertificateStatus(
-                            asn1crypto.ocsp.OCSPResponse.load(bytes(status_message.status))
-                        )
-                        tls_public_key_params['certificate_status'] = certificate_status
-
-            tls_public_key = TlsPublicKey(**tls_public_key_params)
-            LogSingleton().log(level=60, msg=six.u('Server offers %s X.509 public key (with%s SNI)') % (
-                tls_public_key.tls_certificate_chain.items[-1].key_type.name,
-                '' if tls_public_key.sni_sent else 'out',
-            ))
-            results.append(tls_public_key)
+        if sni_sent or subject_matches:
+            for result in results:
+                if certificate_chain == result.tls_certificate_chain:
+                    tls_public_key = result
+                    break
+            else:
+                tls_public_key = TlsPublicKey(
+                    sni_sent=sni_sent,
+                    subject_matches=subject_matches,
+                    tls_certificate_chain=certificate_chain,
+                )
+                LogSingleton().log(level=60, msg=six.u('Server offers %s X.509 public key (with%s SNI)') % (
+                    tls_public_key.tls_certificate_chain.items[-1].key_type.name,
+                    '' if tls_public_key.sni_sent else 'out',
+                ))
+                results.append(tls_public_key)
+
+            try:
+                tls_public_key.certificate_status = cls._get_certificate_status(server_messages)
+            except KeyError:
+                pass
+            try:
+                tls_public_key.scts = cls._get_signed_certificate_timestamps(server_messages)
+            except KeyError:
+                pass
 
     @staticmethod
     def _get_server_messages(l7_client, client_hello, sni_sent, client_hello_messages):
         server_messages = []
 
         try:
             server_messages = l7_client.do_tls_handshake(
@@ -265,15 +307,16 @@
                 TlsHandshakeClientHelloAuthenticationRSA(protocol_version, hostname),
                 TlsHandshakeClientHelloAuthenticationECDSA(protocol_version, hostname),
                 TlsHandshakeClientHelloAuthenticationGOST(protocol_version, hostname),
             ]
             for client_hello in client_hello_messages:
                 sni_sent = hostname is not None
                 client_hello.extensions.extend([
-                    TlsExtensionCertificateStatusRequest(),
+                    TlsExtensionCertificateStatusRequestClient(),
+                    TlsExtensionSignedCertificateTimestampClient(),
                 ])
                 try:
                     server_messages = self._get_server_messages(
                         analyzable, client_hello, sni_sent, client_hello_messages
                     )
                 except StopIteration:
                     break
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/server.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/server.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/sigalgos.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/sigalgos.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/simulations.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/simulations.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cryptodatahub.common.algorithm import KeyExchange
 
 from cryptodatahub.tls.algorithm import TlsNamedCurve
 from cryptodatahub.tls.client import ClientVersionedParamsBase, TlsClient
 
 from cryptoparser.tls.ciphersuite import SslCipherKind, TlsCipherSuite
 from cryptoparser.tls.extension import (
-    TlsExtensionCertificateStatusRequest,
+    TlsExtensionCertificateStatusRequestClient,
     TlsExtensionKeyShareClient,
     TlsExtensionKeyShareReservedClient,
     TlsExtensionKeyShareServer,
     TlsExtensionPadding,
     TlsExtensionRecordSizeLimit,
     TlsExtensionRenegotiationInfo,
     TlsExtensionServerNameClient,
@@ -40,15 +40,15 @@
     TlsHandshakeClientHello,
 )
 from cryptoparser.tls.version import TlsProtocolVersion, TlsVersion
 
 from cryptolyzer.common.analyzer import AnalyzerTlsBase
 from cryptolyzer.common.dhparam import (
     DHParameter,
-    WellKnownDHParams,
+    DHParamWellKnown,
     parse_tls_dh_params,
 )
 from cryptolyzer.common.exception import ErrorParams, NetworkError, SecurityError, SecurityErrorType
 from cryptolyzer.common.result import AnalyzerResultTls, AnalyzerTargetTls
 from cryptolyzer.common.utils import LogSingleton
 
 from cryptolyzer.tls.client import TlsAlert, key_share_entry_from_named_curve
@@ -80,15 +80,15 @@
 @attr.s
 class AnalyzerResultSimulationsTlsPfsNamedGroup(AnalyzerResultSimulationsTlsPfs):
     named_group = attr.ib(validator=attr.validators.instance_of(TlsNamedCurve))
 
 
 @attr.s
 class AnalyzerResultSimulationsTlsPfsDhWellKnown(AnalyzerResultSimulationsTlsPfs):
-    well_known = attr.ib(validator=attr.validators.in_(WellKnownDHParams))
+    well_known = attr.ib(validator=attr.validators.in_(DHParamWellKnown))
 
 
 @attr.s
 class AnalyzerResultSimulations(AnalyzerResultTls):
     succeeded_clients = attr.ib(validator=attr.validators.deep_mapping(
         key_validator=attr.validators.instance_of(ClientVersionedParamsBase),
         value_validator=attr.validators.instance_of((AnalyzerResultSimulationsTlsBase, AnalyzerResultSimulationsSsl)),
@@ -107,15 +107,15 @@
     @classmethod
     def get_help(cls):
         return 'Check which parameters are negotiated using different clients with the server(s)'
 
     @staticmethod
     def _get_extension(server_name, extension_type, extension_params, grease):
         extension_types_with_no_attrs = [
-            TlsExtensionRenegotiationInfo, TlsExtensionSessionTicket, TlsExtensionCertificateStatusRequest
+            TlsExtensionRenegotiationInfo, TlsExtensionSessionTicket, TlsExtensionCertificateStatusRequestClient
         ]
 
         extension_classes = TlsExtensionVariantClient.get_parsed_extensions()
         extension_class = extension_classes[extension_type][0]
         extension_params = getattr(extension_params, extension_type.name.lower(), None)
 
         if issubclass(extension_class, TlsExtensionUnusedData) or extension_class in extension_types_with_no_attrs:
@@ -292,19 +292,25 @@
             elif e.description == TlsAlertDescription.HANDSHAKE_FAILURE:
                 six.raise_from(SecurityError(SecurityErrorType.NO_SHARED_CIPHER), e)
             else:
                 six.raise_from(SecurityError(SecurityErrorType.UNKNOWN_ERROR), e)
 
         return self._get_simulation_result(server_messages)
 
+    @staticmethod
+    def _get_tls_client_key(tls_client):
+        #  neccessary only because PY2 does not preverse the order of enums
+        tls_client_name_parts = tls_client.name.split('_')
+        return (tls_client_name_parts[0], int(tls_client_name_parts[1]))
+
     def _get_results(self, analyzable):
         succeeded_clients = []
         failed_clients = []
 
-        for tls_client in TlsClient:
+        for tls_client in sorted(TlsClient, key=self._get_tls_client_key):
             client_hello = self._get_client_hello_from_client_params(tls_client.value, analyzable.address)
 
             try:
                 simulation_result = self._simulate_tls_client(analyzable, client_hello)
             except (NetworkError, SecurityError) as e:
                 failed_clients.append((tls_client.value.meta, e.error.value))
                 LogSingleton().log(
```

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/versions.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/versions.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/cryptolyzer/tls/vulnerabilities.py` & `CryptoLyzer-0.9.1/cryptolyzer/tls/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/setup.py` & `CryptoLyzer-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `CryptoLyzer-0.9.0/test/test_main.py` & `CryptoLyzer-0.9.1/test/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,18 @@
             'error: argument analyzer: invalid choice: \'unsupportedanalyzer\''
         )
         self._test_argument_error(
             ['cryptolyzer', 'tls', 'versions', 'unsupportedprotocol://localhost'],
             'error: unsupported protocol: unsupportedprotocol'
         )
         self._test_argument_error(
+            ['cryptolyzer', '--socket-timeout', '-1', 'tls', 'versions', 'unsupportedprotocol://localhost'],
+            'error: argument -t/--socket-timeout: -1.0 socket timeout must be a positive integer value'
+        )
+        self._test_argument_error(
             ['cryptolyzer', 'ja3', 'decode', 'unsupportedformat://tag'],
             'error: unsupported protocol: unsupportedformat'
         )
 
     def test_runtime_error(self):
         self._test_runtime_error(
             ['cryptolyzer', 'tls', 'versions', 'unresolvable.hostname'],
@@ -235,15 +239,15 @@
         )
         self.assertEqual(
             self._get_test_analyzer_result_markdown(**cli_arguments),
             result.as_markdown() + '\n',
         )
 
     def test_analyzer_output_tls_all(self):
-        result = test.tls.test_all.TestTlsAll.get_result('rc4-md5.badssl.com', 443, protocol_version=None)
+        result = test.tls.test_all.TestTlsAll.get_result('rc4-md5.badssl.com', 443, protocol_version=None, timeout=5)
         self.assertEqual(
             self._get_test_analyzer_result_json('tls', 'all', 'rc4-md5.badssl.com'),
             result.as_json() + '\n',
         )
 
         self.assertEqual(
             self._get_test_analyzer_result_markdown('tls', 'all', 'rc4-md5.badssl.com'),
```

