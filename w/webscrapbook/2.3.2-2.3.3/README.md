# Comparing `tmp/webscrapbook-2.3.2.tar.gz` & `tmp/webscrapbook-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapbook-2.3.2.tar", last modified: Thu Mar 14 14:23:38 2024, max compression
+gzip compressed data, was "webscrapbook-2.3.3.tar", last modified: Sun May 26 15:12:37 2024, max compression
```

## Comparing `webscrapbook-2.3.2.tar` & `webscrapbook-2.3.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.469802 webscrapbook-2.3.2/
--rw-rw-rw-   0        0        0     1092 2024-01-23 09:40:32.000000 webscrapbook-2.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0       13 2023-06-04 12:28:32.000000 webscrapbook-2.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6283 2024-03-14 14:23:38.468832 webscrapbook-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2024-01-19 06:19:28.000000 webscrapbook-2.3.2/README.md
--rw-rw-rw-   0        0        0     2550 2024-03-14 14:23:38.474796 webscrapbook-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0       63 2023-06-04 12:28:32.000000 webscrapbook-2.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:37.758801 webscrapbook-2.3.2/webscrapbook/
--rw-rw-rw-   0        0        0     7410 2024-03-14 14:21:37.000000 webscrapbook-2.3.2/webscrapbook/__init__.py
--rw-rw-rw-   0        0        0      165 2024-01-17 12:45:15.000000 webscrapbook-2.3.2/webscrapbook/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:37.821021 webscrapbook-2.3.2/webscrapbook/_polyfill/
--rw-rw-rw-   0        0        0        0 2023-06-04 12:28:32.000000 webscrapbook-2.3.2/webscrapbook/_polyfill/__init__.py
--rw-rw-rw-   0        0        0     1507 2024-01-31 11:27:22.000000 webscrapbook-2.3.2/webscrapbook/_polyfill/argparse.py
--rw-rw-rw-   0        0        0     3302 2024-01-31 11:27:22.000000 webscrapbook-2.3.2/webscrapbook/_polyfill/mimetypes.py
--rw-rw-rw-   0        0        0      393 2023-06-04 12:28:32.000000 webscrapbook-2.3.2/webscrapbook/_polyfill/zipfile.py
--rw-rw-rw-   0        0        0    61243 2024-01-25 15:59:40.000000 webscrapbook-2.3.2/webscrapbook/app.py
--rw-rw-rw-   0        0        0    47660 2024-01-31 11:27:22.000000 webscrapbook-2.3.2/webscrapbook/cli.py
--rw-rw-rw-   0        0        0     3131 2023-06-04 12:28:32.000000 webscrapbook-2.3.2/webscrapbook/locales.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:37.875236 webscrapbook-2.3.2/webscrapbook/resources/
--rw-rw-rw-   0        0        0      144 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/resources/app.py
--rw-rw-rw-   0        0        0     1024 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/resources/config.ini
--rw-rw-rw-   0        0        0    12833 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/resources/config.md
--rw-rw-rw-   0        0        0     2025 2024-01-31 11:27:22.000000 webscrapbook-2.3.2/webscrapbook/resources/mimetypes.md
--rw-rw-rw-   0        0        0      128 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/resources/serve.py
--rw-rw-rw-   0        0        0     1543 2024-01-31 11:27:22.000000 webscrapbook-2.3.2/webscrapbook/resources/themes.md
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.017488 webscrapbook-2.3.2/webscrapbook/scrapbook/
--rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/__init__.py
--rw-rw-rw-   0        0        0    53174 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/book.py
--rw-rw-rw-   0        0        0    38584 2024-01-25 15:59:40.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/cache.py
--rw-rw-rw-   0        0        0    27996 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/check.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.095829 webscrapbook-2.3.2/webscrapbook/scrapbook/convert/
--rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/convert/__init__.py
--rw-rw-rw-   0        0        0    11915 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/convert/file2wsb.py
--rw-rw-rw-   0        0        0    13635 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/convert/items.py
--rw-rw-rw-   0        0        0    41602 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/convert/migrate.py
--rw-rw-rw-   0        0        0    15430 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/convert/sb2wsb.py
--rw-rw-rw-   0        0        0     5914 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/convert/wsb2file.py
--rw-rw-rw-   0        0        0    25978 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/convert/wsb2sb.py
--rw-rw-rw-   0        0        0     9372 2024-01-25 15:59:40.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/exporter.py
--rw-rw-rw-   0        0        0     6939 2024-01-25 15:59:40.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/exporter1.py
--rw-rw-rw-   0        0        0    16540 2024-01-31 11:27:22.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/host.py
--rw-rw-rw-   0        0        0    20670 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/importer.py
--rw-rw-rw-   0        0        0    20236 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/importer1.py
--rw-rw-rw-   0        0        0    38988 2024-01-25 15:59:40.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/indexer.py
--rw-rw-rw-   0        0        0    21179 2024-01-24 12:34:32.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/search.py
--rw-rw-rw-   0        0        0     7614 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/scrapbook/util.py
--rw-rw-rw-   0        0        0     2356 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/server.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:37.666807 webscrapbook-2.3.2/webscrapbook/themes/
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:37.670869 webscrapbook-2.3.2/webscrapbook/themes/default/
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:37.669871 webscrapbook-2.3.2/webscrapbook/themes/default/locales/
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.096933 webscrapbook-2.3.2/webscrapbook/themes/default/locales/ar/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/locales/ar/messages.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.097936 webscrapbook-2.3.2/webscrapbook/themes/default/locales/en/
--rw-rw-rw-   0        0        0     8087 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/themes/default/locales/en/messages.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.125274 webscrapbook-2.3.2/webscrapbook/themes/default/locales/es/
--rw-rw-rw-   0        0        0     9322 2024-01-31 11:27:22.000000 webscrapbook-2.3.2/webscrapbook/themes/default/locales/es/messages.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.132921 webscrapbook-2.3.2/webscrapbook/themes/default/locales/fa/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/locales/fa/messages.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.133913 webscrapbook-2.3.2/webscrapbook/themes/default/locales/he/
--rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/locales/he/messages.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.134915 webscrapbook-2.3.2/webscrapbook/themes/default/locales/zh/
--rw-rw-rw-   0        0        0     8240 2024-01-28 09:04:02.000000 webscrapbook-2.3.2/webscrapbook/themes/default/locales/zh/messages.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.149016 webscrapbook-2.3.2/webscrapbook/themes/default/locales/zh_cn/
--rw-rw-rw-   0        0        0     8263 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/themes/default/locales/zh_cn/messages.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.315271 webscrapbook-2.3.2/webscrapbook/themes/default/static/
--rw-rw-rw-   0        0        0      281 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/collapse.png
--rw-rw-rw-   0        0        0      728 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/comment.png
--rw-rw-rw-   0        0        0      877 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/common.css
--rw-rw-rw-   0        0        0     3900 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/common.js
--rw-rw-rw-   0        0        0     1055 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/edit.css
--rw-rw-rw-   0        0        0     1563 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/edit.js
--rw-rw-rw-   0        0        0     2438 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/editx.js
--rw-rw-rw-   0        0        0      279 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/expand.png
--rw-rw-rw-   0        0        0      523 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/external.png
--rw-rw-rw-   0        0        0      752 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/fclose.png
--rw-rw-rw-   0        0        0      449 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/file.png
--rw-rw-rw-   0        0        0      790 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/fopen.png
--rw-rw-rw-   0        0        0     3810 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/index-ex.css
--rw-rw-rw-   0        0        0    61846 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/index-ex.js
--rw-rw-rw-   0        0        0     2210 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/index.css
--rw-rw-rw-   0        0        0     2156 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/index.js
--rw-rw-rw-   0        0        0      502 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/item.png
--rw-rw-rw-   0        0        0      387 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/link.png
--rw-rw-rw-   0        0        0      445 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/note.png
--rw-rw-rw-   0        0        0      515 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/postit.png
--rw-rw-rw-   0        0        0      661 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/search.png
--rw-rw-rw-   0        0        0      807 2023-04-08 19:20:00.000000 webscrapbook-2.3.2/webscrapbook/themes/default/static/toggle.png
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.382622 webscrapbook-2.3.2/webscrapbook/themes/default/templates/
--rw-rw-rw-   0        0        0      482 2024-01-28 07:27:55.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/base.html
--rw-rw-rw-   0        0        0      632 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/cli.html
--rw-rw-rw-   0        0        0     1053 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/edit.html
--rw-rw-rw-   0        0        0      965 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/editx.html
--rw-rw-rw-   0        0        0     6340 2024-01-28 07:37:44.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/index.html
--rw-rw-rw-   0        0        0      510 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/maff_index.html
--rw-rw-rw-   0        0        0      490 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/markdown.html
--rw-rw-rw-   0        0        0      568 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/static_frame.html
--rw-rw-rw-   0        0        0     1751 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/static_index.html
--rw-rw-rw-   0        0        0    12917 2023-05-14 13:37:39.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/static_map.html
--rw-rw-rw-   0        0        0    26414 2023-06-17 15:42:14.000000 webscrapbook-2.3.2/webscrapbook/themes/default/templates/static_search.html
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.454600 webscrapbook-2.3.2/webscrapbook/util/
--rw-rw-rw-   0        0        0       72 2023-06-04 12:28:32.000000 webscrapbook-2.3.2/webscrapbook/util/__init__.py
--rw-rw-rw-   0        0        0     7308 2024-03-14 14:21:38.000000 webscrapbook-2.3.2/webscrapbook/util/css.py
--rw-rw-rw-   0        0        0    44450 2024-01-25 15:59:40.000000 webscrapbook-2.3.2/webscrapbook/util/fs.py
--rw-rw-rw-   0        0        0    15295 2024-03-14 14:21:38.000000 webscrapbook-2.3.2/webscrapbook/util/html.py
--rw-rw-rw-   0        0        0    37640 2024-03-14 14:21:38.000000 webscrapbook-2.3.2/webscrapbook/util/util.py
-drwxrwxrwx   0        0        0        0 2024-03-14 14:23:38.458601 webscrapbook-2.3.2/webscrapbook.egg-info/
--rw-rw-rw-   0        0        0     6283 2024-03-14 14:23:37.000000 webscrapbook-2.3.2/webscrapbook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3500 2024-03-14 14:23:37.000000 webscrapbook-2.3.2/webscrapbook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 14:23:37.000000 webscrapbook-2.3.2/webscrapbook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-03-14 14:23:37.000000 webscrapbook-2.3.2/webscrapbook.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      266 2024-03-14 14:23:37.000000 webscrapbook-2.3.2/webscrapbook.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-14 14:23:37.000000 webscrapbook-2.3.2/webscrapbook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.610064 webscrapbook-2.3.3/
+-rw-rw-rw-   0        0        0     1092 2024-01-23 09:40:32.000000 webscrapbook-2.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       13 2023-06-04 12:28:32.000000 webscrapbook-2.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6283 2024-05-26 15:12:37.610064 webscrapbook-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2024-01-19 06:19:28.000000 webscrapbook-2.3.3/README.md
+-rw-rw-rw-   0        0        0     2550 2024-05-26 15:12:37.610064 webscrapbook-2.3.3/setup.cfg
+-rw-rw-rw-   0        0        0       63 2023-06-04 12:28:32.000000 webscrapbook-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.472053 webscrapbook-2.3.3/webscrapbook/
+-rw-rw-rw-   0        0        0     7410 2024-05-26 15:11:39.000000 webscrapbook-2.3.3/webscrapbook/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-01-17 12:45:15.000000 webscrapbook-2.3.3/webscrapbook/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.472053 webscrapbook-2.3.3/webscrapbook/_polyfill/
+-rw-rw-rw-   0        0        0        0 2023-06-04 12:28:32.000000 webscrapbook-2.3.3/webscrapbook/_polyfill/__init__.py
+-rw-rw-rw-   0        0        0     1507 2024-01-31 11:27:22.000000 webscrapbook-2.3.3/webscrapbook/_polyfill/argparse.py
+-rw-rw-rw-   0        0        0     3302 2024-01-31 11:27:22.000000 webscrapbook-2.3.3/webscrapbook/_polyfill/mimetypes.py
+-rw-rw-rw-   0        0        0      393 2023-06-04 12:28:32.000000 webscrapbook-2.3.3/webscrapbook/_polyfill/zipfile.py
+-rw-rw-rw-   0        0        0    61243 2024-01-25 15:59:40.000000 webscrapbook-2.3.3/webscrapbook/app.py
+-rw-rw-rw-   0        0        0    47660 2024-01-31 11:27:22.000000 webscrapbook-2.3.3/webscrapbook/cli.py
+-rw-rw-rw-   0        0        0     3131 2023-06-04 12:28:32.000000 webscrapbook-2.3.3/webscrapbook/locales.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.487677 webscrapbook-2.3.3/webscrapbook/resources/
+-rw-rw-rw-   0        0        0      144 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/resources/app.py
+-rw-rw-rw-   0        0        0     1024 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/resources/config.ini
+-rw-rw-rw-   0        0        0    12833 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/resources/config.md
+-rw-rw-rw-   0        0        0     2025 2024-01-31 11:27:22.000000 webscrapbook-2.3.3/webscrapbook/resources/mimetypes.md
+-rw-rw-rw-   0        0        0      128 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/resources/serve.py
+-rw-rw-rw-   0        0        0     1543 2024-01-31 11:27:22.000000 webscrapbook-2.3.3/webscrapbook/resources/themes.md
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.494181 webscrapbook-2.3.3/webscrapbook/scrapbook/
+-rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/__init__.py
+-rw-rw-rw-   0        0        0    53174 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/book.py
+-rw-rw-rw-   0        0        0    38584 2024-01-25 15:59:40.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/cache.py
+-rw-rw-rw-   0        0        0    27996 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/check.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.494181 webscrapbook-2.3.3/webscrapbook/scrapbook/convert/
+-rw-rw-rw-   0        0        0        0 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/convert/__init__.py
+-rw-rw-rw-   0        0        0    11915 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/convert/file2wsb.py
+-rw-rw-rw-   0        0        0    13635 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/convert/items.py
+-rw-rw-rw-   0        0        0    41602 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/convert/migrate.py
+-rw-rw-rw-   0        0        0    15430 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/convert/sb2wsb.py
+-rw-rw-rw-   0        0        0     5914 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/convert/wsb2file.py
+-rw-rw-rw-   0        0        0    25978 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/convert/wsb2sb.py
+-rw-rw-rw-   0        0        0     9372 2024-01-25 15:59:40.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/exporter.py
+-rw-rw-rw-   0        0        0     6939 2024-01-25 15:59:40.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/exporter1.py
+-rw-rw-rw-   0        0        0    16540 2024-01-31 11:27:22.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/host.py
+-rw-rw-rw-   0        0        0    20670 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/importer.py
+-rw-rw-rw-   0        0        0    20236 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/importer1.py
+-rw-rw-rw-   0        0        0    38988 2024-01-25 15:59:40.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/indexer.py
+-rw-rw-rw-   0        0        0    21179 2024-01-24 12:34:32.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/search.py
+-rw-rw-rw-   0        0        0     7614 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/scrapbook/util.py
+-rw-rw-rw-   0        0        0     2356 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/server.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.456429 webscrapbook-2.3.3/webscrapbook/themes/
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.456429 webscrapbook-2.3.3/webscrapbook/themes/default/
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.456429 webscrapbook-2.3.3/webscrapbook/themes/default/locales/
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.494181 webscrapbook-2.3.3/webscrapbook/themes/default/locales/ar/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/locales/ar/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.494181 webscrapbook-2.3.3/webscrapbook/themes/default/locales/en/
+-rw-rw-rw-   0        0        0     8087 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/themes/default/locales/en/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.494181 webscrapbook-2.3.3/webscrapbook/themes/default/locales/es/
+-rw-rw-rw-   0        0        0     9322 2024-01-31 11:27:22.000000 webscrapbook-2.3.3/webscrapbook/themes/default/locales/es/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.509809 webscrapbook-2.3.3/webscrapbook/themes/default/locales/fa/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/locales/fa/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.509809 webscrapbook-2.3.3/webscrapbook/themes/default/locales/he/
+-rw-rw-rw-   0        0        0       36 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/locales/he/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.509809 webscrapbook-2.3.3/webscrapbook/themes/default/locales/zh/
+-rw-rw-rw-   0        0        0     8240 2024-01-28 09:04:02.000000 webscrapbook-2.3.3/webscrapbook/themes/default/locales/zh/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.509809 webscrapbook-2.3.3/webscrapbook/themes/default/locales/zh_cn/
+-rw-rw-rw-   0        0        0     8263 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/themes/default/locales/zh_cn/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.525433 webscrapbook-2.3.3/webscrapbook/themes/default/static/
+-rw-rw-rw-   0        0        0      281 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/collapse.png
+-rw-rw-rw-   0        0        0      728 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/comment.png
+-rw-rw-rw-   0        0        0      877 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/common.css
+-rw-rw-rw-   0        0        0     3900 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/common.js
+-rw-rw-rw-   0        0        0     1055 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/edit.css
+-rw-rw-rw-   0        0        0     1563 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/edit.js
+-rw-rw-rw-   0        0        0     2438 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/editx.js
+-rw-rw-rw-   0        0        0      279 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/expand.png
+-rw-rw-rw-   0        0        0      523 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/external.png
+-rw-rw-rw-   0        0        0      752 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/fclose.png
+-rw-rw-rw-   0        0        0      449 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/file.png
+-rw-rw-rw-   0        0        0      790 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/fopen.png
+-rw-rw-rw-   0        0        0     3810 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/index-ex.css
+-rw-rw-rw-   0        0        0    61846 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/index-ex.js
+-rw-rw-rw-   0        0        0     2210 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/index.css
+-rw-rw-rw-   0        0        0     2156 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/index.js
+-rw-rw-rw-   0        0        0      502 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/item.png
+-rw-rw-rw-   0        0        0      387 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/link.png
+-rw-rw-rw-   0        0        0      445 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/note.png
+-rw-rw-rw-   0        0        0      515 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/postit.png
+-rw-rw-rw-   0        0        0      661 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/search.png
+-rw-rw-rw-   0        0        0      807 2023-04-08 19:20:00.000000 webscrapbook-2.3.3/webscrapbook/themes/default/static/toggle.png
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.587930 webscrapbook-2.3.3/webscrapbook/themes/default/templates/
+-rw-rw-rw-   0        0        0      482 2024-01-28 07:27:55.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/base.html
+-rw-rw-rw-   0        0        0      632 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/cli.html
+-rw-rw-rw-   0        0        0     1053 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/edit.html
+-rw-rw-rw-   0        0        0      965 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/editx.html
+-rw-rw-rw-   0        0        0     6340 2024-01-28 07:37:44.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/index.html
+-rw-rw-rw-   0        0        0      510 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/maff_index.html
+-rw-rw-rw-   0        0        0      490 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/markdown.html
+-rw-rw-rw-   0        0        0      568 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/static_frame.html
+-rw-rw-rw-   0        0        0     1751 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/static_index.html
+-rw-rw-rw-   0        0        0    12917 2023-05-14 13:37:39.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/static_map.html
+-rw-rw-rw-   0        0        0    26414 2023-06-17 15:42:14.000000 webscrapbook-2.3.3/webscrapbook/themes/default/templates/static_search.html
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.594435 webscrapbook-2.3.3/webscrapbook/util/
+-rw-rw-rw-   0        0        0       72 2023-06-04 12:28:32.000000 webscrapbook-2.3.3/webscrapbook/util/__init__.py
+-rw-rw-rw-   0        0        0     7308 2024-05-26 07:18:08.000000 webscrapbook-2.3.3/webscrapbook/util/css.py
+-rw-rw-rw-   0        0        0    44450 2024-01-25 15:59:40.000000 webscrapbook-2.3.3/webscrapbook/util/fs.py
+-rw-rw-rw-   0        0        0    15295 2024-05-26 07:18:08.000000 webscrapbook-2.3.3/webscrapbook/util/html.py
+-rw-rw-rw-   0        0        0    37640 2024-05-26 07:18:08.000000 webscrapbook-2.3.3/webscrapbook/util/util.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:12:37.594435 webscrapbook-2.3.3/webscrapbook.egg-info/
+-rw-rw-rw-   0        0        0     6283 2024-05-26 15:12:37.000000 webscrapbook-2.3.3/webscrapbook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3500 2024-05-26 15:12:37.000000 webscrapbook-2.3.3/webscrapbook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:12:37.000000 webscrapbook-2.3.3/webscrapbook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-05-26 15:12:37.000000 webscrapbook-2.3.3/webscrapbook.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      266 2024-05-26 15:12:37.000000 webscrapbook-2.3.3/webscrapbook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-26 15:12:37.000000 webscrapbook-2.3.3/webscrapbook.egg-info/top_level.txt
```

### Comparing `webscrapbook-2.3.2/LICENSE.txt` & `webscrapbook-2.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/PKG-INFO` & `webscrapbook-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 2.3.2
+Version: 2.3.3
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -34,15 +34,15 @@
 Provides-Extra: adhoc-ssl
 Requires-Dist: cryptography; extra == "adhoc-ssl"
 Provides-Extra: dev
 Requires-Dist: flake8>=4.0; extra == "dev"
 Requires-Dist: pep8-naming>=0.13.2; extra == "dev"
 Requires-Dist: flake8-comprehensions>=3.7; extra == "dev"
 Requires-Dist: flake8-string-format>=0.3; extra == "dev"
-Requires-Dist: flake8-quotes>=3.0; extra == "dev"
+Requires-Dist: flake8-quotes>=3.4; extra == "dev"
 Requires-Dist: flake8-bugbear>=22.0; extra == "dev"
 Requires-Dist: flake8-isort>=4.2; extra == "dev"
 Requires-Dist: isort>=5.5; extra == "dev"
 Requires-Dist: tox>=4.0; extra == "dev"
 
 PyWebScrapBook is a command line toolkit and backend server for
 [WebScrapBook browser extension](https://github.com/danny0838/webscrapbook).
```

### Comparing `webscrapbook-2.3.2/README.md` & `webscrapbook-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/setup.cfg` & `webscrapbook-2.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 00000560: 7620 3d20 0d0a 0966 6c61 6b65 3820 3e3d  v = ...flake8 >=
 00000570: 2034 2e30 0d0a 0970 6570 382d 6e61 6d69   4.0...pep8-nami
 00000580: 6e67 203e 3d20 302e 3133 2e32 0d0a 0966  ng >= 0.13.2...f
 00000590: 6c61 6b65 382d 636f 6d70 7265 6865 6e73  lake8-comprehens
 000005a0: 696f 6e73 203e 3d20 332e 370d 0a09 666c  ions >= 3.7...fl
 000005b0: 616b 6538 2d73 7472 696e 672d 666f 726d  ake8-string-form
 000005c0: 6174 203e 3d20 302e 330d 0a09 666c 616b  at >= 0.3...flak
-000005d0: 6538 2d71 756f 7465 7320 3e3d 2033 2e30  e8-quotes >= 3.0
+000005d0: 6538 2d71 756f 7465 7320 3e3d 2033 2e34  e8-quotes >= 3.4
 000005e0: 0d0a 0966 6c61 6b65 382d 6275 6762 6561  ...flake8-bugbea
 000005f0: 7220 3e3d 2032 322e 300d 0a09 666c 616b  r >= 22.0...flak
 00000600: 6538 2d69 736f 7274 203e 3d20 342e 320d  e8-isort >= 4.2.
 00000610: 0a09 6973 6f72 7420 3e3d 2035 2e35 0d0a  ..isort >= 5.5..
 00000620: 0974 6f78 203e 3d20 342e 300d 0a0d 0a5b  .tox >= 4.0....[
 00000630: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
 00000640: 2e66 696e 645d 0d0a 696e 636c 7564 6520  .find]..include
```

### Comparing `webscrapbook-2.3.2/webscrapbook/__init__.py` & `webscrapbook-2.3.3/webscrapbook/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from collections import OrderedDict
 from configparser import ConfigParser
 from copy import deepcopy
 
 __all__ = ['WSB_EXTENSION_MIN_VERSION', 'WSB_USER_DIR', 'WSB_USER_CONFIG', 'WSB_DIR', 'WSB_CONFIG', 'config']
 
-__version__ = '2.3.2'
+__version__ = '2.3.3'
 
 WSB_EXTENSION_MIN_VERSION = '2.0.1'
 WSB_USER_DIR = os.environ.get('WSB_USER_DIR') or '.config/wsb'
 WSB_USER_CONFIG = os.environ.get('WSB_USER_CONFIG') or '.wsbconfig'
 WSB_DIR = os.environ.get('WSB_DIR') or '.wsb'
 WSB_CONFIG = os.environ.get('WSB_CONFIG') or 'config.ini'
```

### Comparing `webscrapbook-2.3.2/webscrapbook/_polyfill/argparse.py` & `webscrapbook-2.3.3/webscrapbook/_polyfill/argparse.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/_polyfill/mimetypes.py` & `webscrapbook-2.3.3/webscrapbook/_polyfill/mimetypes.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/app.py` & `webscrapbook-2.3.3/webscrapbook/app.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/cli.py` & `webscrapbook-2.3.3/webscrapbook/cli.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/locales.py` & `webscrapbook-2.3.3/webscrapbook/locales.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/resources/config.ini` & `webscrapbook-2.3.3/webscrapbook/resources/config.ini`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/resources/config.md` & `webscrapbook-2.3.3/webscrapbook/resources/config.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/resources/mimetypes.md` & `webscrapbook-2.3.3/webscrapbook/resources/mimetypes.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/resources/themes.md` & `webscrapbook-2.3.3/webscrapbook/resources/themes.md`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/book.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/book.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/cache.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/cache.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/check.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/check.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/convert/file2wsb.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/convert/file2wsb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/convert/items.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/convert/items.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/convert/migrate.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/convert/migrate.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/convert/sb2wsb.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/convert/sb2wsb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/convert/wsb2file.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/convert/wsb2file.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/convert/wsb2sb.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/convert/wsb2sb.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/exporter.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/exporter.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/exporter1.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/exporter1.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/host.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/host.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/importer.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/importer.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/importer1.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/importer1.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/indexer.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/indexer.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/search.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/search.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/scrapbook/util.py` & `webscrapbook-2.3.3/webscrapbook/scrapbook/util.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/server.py` & `webscrapbook-2.3.3/webscrapbook/server.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/locales/en/messages.py` & `webscrapbook-2.3.3/webscrapbook/themes/default/locales/en/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/locales/es/messages.py` & `webscrapbook-2.3.3/webscrapbook/themes/default/locales/es/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/locales/zh/messages.py` & `webscrapbook-2.3.3/webscrapbook/themes/default/locales/zh/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/locales/zh_cn/messages.py` & `webscrapbook-2.3.3/webscrapbook/themes/default/locales/zh_cn/messages.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/comment.png` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/comment.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/common.css` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/common.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/common.js` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/common.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/edit.css` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/edit.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/edit.js` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/edit.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/editx.js` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/editx.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/external.png` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/external.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/fclose.png` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/fclose.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/fopen.png` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/fopen.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/index-ex.css` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/index-ex.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/index-ex.js` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/index-ex.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/index.css` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/index.css`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/index.js` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/index.js`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/postit.png` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/postit.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/search.png` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/search.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/static/toggle.png` & `webscrapbook-2.3.3/webscrapbook/themes/default/static/toggle.png`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/templates/cli.html` & `webscrapbook-2.3.3/webscrapbook/themes/default/templates/cli.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/templates/edit.html` & `webscrapbook-2.3.3/webscrapbook/themes/default/templates/edit.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/templates/editx.html` & `webscrapbook-2.3.3/webscrapbook/themes/default/templates/editx.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/templates/index.html` & `webscrapbook-2.3.3/webscrapbook/themes/default/templates/index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/templates/static_frame.html` & `webscrapbook-2.3.3/webscrapbook/themes/default/templates/static_frame.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/templates/static_index.html` & `webscrapbook-2.3.3/webscrapbook/themes/default/templates/static_index.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/templates/static_map.html` & `webscrapbook-2.3.3/webscrapbook/themes/default/templates/static_map.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/themes/default/templates/static_search.html` & `webscrapbook-2.3.3/webscrapbook/themes/default/templates/static_search.html`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/util/css.py` & `webscrapbook-2.3.3/webscrapbook/util/css.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/util/fs.py` & `webscrapbook-2.3.3/webscrapbook/util/fs.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/util/html.py` & `webscrapbook-2.3.3/webscrapbook/util/html.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook/util/util.py` & `webscrapbook-2.3.3/webscrapbook/util/util.py`

 * *Files identical despite different names*

### Comparing `webscrapbook-2.3.2/webscrapbook.egg-info/PKG-INFO` & `webscrapbook-2.3.3/webscrapbook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapbook
-Version: 2.3.2
+Version: 2.3.3
 Summary: A backend toolkit for management of WebScrapBook collection.
 Home-page: https://github.com/danny0838/PyWebScrapBook
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -34,15 +34,15 @@
 Provides-Extra: adhoc-ssl
 Requires-Dist: cryptography; extra == "adhoc-ssl"
 Provides-Extra: dev
 Requires-Dist: flake8>=4.0; extra == "dev"
 Requires-Dist: pep8-naming>=0.13.2; extra == "dev"
 Requires-Dist: flake8-comprehensions>=3.7; extra == "dev"
 Requires-Dist: flake8-string-format>=0.3; extra == "dev"
-Requires-Dist: flake8-quotes>=3.0; extra == "dev"
+Requires-Dist: flake8-quotes>=3.4; extra == "dev"
 Requires-Dist: flake8-bugbear>=22.0; extra == "dev"
 Requires-Dist: flake8-isort>=4.2; extra == "dev"
 Requires-Dist: isort>=5.5; extra == "dev"
 Requires-Dist: tox>=4.0; extra == "dev"
 
 PyWebScrapBook is a command line toolkit and backend server for
 [WebScrapBook browser extension](https://github.com/danny0838/webscrapbook).
```

### Comparing `webscrapbook-2.3.2/webscrapbook.egg-info/SOURCES.txt` & `webscrapbook-2.3.3/webscrapbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

