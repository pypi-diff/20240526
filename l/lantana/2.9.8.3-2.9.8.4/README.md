# Comparing `tmp/lantana-2.9.8.3.tar.gz` & `tmp/lantana-2.9.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lantana-2.9.8.3.tar", last modified: Sun May 26 09:07:15 2024, max compression
+gzip compressed data, was "lantana-2.9.8.4.tar", last modified: Sun May 26 09:21:45 2024, max compression
```

## Comparing `lantana-2.9.8.3.tar` & `lantana-2.9.8.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:07:15.442484 lantana-2.9.8.3/
--rw-rw-rw-   0        0        0     1083 2022-10-28 14:22:28.000000 lantana-2.9.8.3/LICENCE.md
--rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.9.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0      239 2024-05-26 09:07:15.442484 lantana-2.9.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.9.8.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 09:07:15.411210 lantana-2.9.8.3/lantana/
--rw-rw-rw-   0        0        0      829 2024-04-03 03:18:14.000000 lantana-2.9.8.3/lantana/404.html
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8.3/lantana/__init__.py
--rw-rw-rw-   0        0        0     2731 2024-03-07 12:04:46.000000 lantana-2.9.8.3/lantana/__main__.py
--rw-rw-rw-   0        0        0        0 2023-06-28 13:19:19.000000 lantana-2.9.8.3/lantana/after_header.html
--rw-rw-rw-   0        0        0        0 2024-05-26 09:06:46.000000 lantana-2.9.8.3/lantana/after_nav_tool.html
--rw-rw-rw-   0        0        0     9493 2024-04-19 06:39:06.000000 lantana-2.9.8.3/lantana/base.html
--rw-rw-rw-   0        0        0        0 2023-06-28 13:14:52.000000 lantana-2.9.8.3/lantana/before_header.html
--rw-rw-rw-   0        0        0      306 2023-08-26 17:00:51.000000 lantana-2.9.8.3/lantana/breadcrumb.html
-drwxrwxrwx   0        0        0        0 2024-05-26 09:07:15.426835 lantana-2.9.8.3/lantana/css/
--rw-rw-rw-   0        0        0    85883 2024-04-19 06:40:56.000000 lantana-2.9.8.3/lantana/css/bootstrap-icons.min.css
--rw-rw-rw-   0        0        0   224443 2024-03-18 09:06:45.000000 lantana-2.9.8.3/lantana/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     1152 2024-03-18 13:45:00.000000 lantana-2.9.8.3/lantana/css/default.min.css
-drwxrwxrwx   0        0        0        0 2024-05-26 09:07:15.426835 lantana-2.9.8.3/lantana/css/fonts/
--rw-rw-rw-   0        0        0   176032 2024-04-19 06:23:31.000000 lantana-2.9.8.3/lantana/css/fonts/bootstrap-icons.woff.css
--rw-rw-rw-   0        0        0   130396 2024-04-19 06:23:31.000000 lantana-2.9.8.3/lantana/css/fonts/bootstrap-icons.woff2.css
--rw-rw-rw-   0        0        0     3949 2024-05-06 12:45:53.000000 lantana-2.9.8.3/lantana/css/theme.css
--rw-rw-rw-   0        0        0     1927 2024-03-18 13:47:24.000000 lantana-2.9.8.3/lantana/css/vs.min.css
-drwxrwxrwx   0        0        0        0 2024-05-26 09:07:15.426835 lantana-2.9.8.3/lantana/extensions/
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8.3/lantana/extensions/__init__.py
--rw-rw-rw-   0        0        0     2714 2024-03-18 13:02:35.000000 lantana-2.9.8.3/lantana/extensions/accordion.py
--rw-rw-rw-   0        0        0     3930 2024-05-06 13:25:21.000000 lantana-2.9.8.3/lantana/extensions/alerts.py
--rw-rw-rw-   0        0        0     4704 2024-05-06 17:26:51.000000 lantana-2.9.8.3/lantana/extensions/alerts2.py
--rw-rw-rw-   0        0        0     4553 2024-04-03 02:58:18.000000 lantana-2.9.8.3/lantana/extensions/cards.py
--rw-rw-rw-   0        0        0     2116 2024-03-11 07:11:53.000000 lantana-2.9.8.3/lantana/extensions/codeblock_copybtn.py
--rw-rw-rw-   0        0        0     1889 2024-05-06 17:43:29.000000 lantana-2.9.8.3/lantana/extensions/lantana.py
--rw-rw-rw-   0        0        0      882 2024-03-11 07:41:11.000000 lantana-2.9.8.3/lantana/extensions/link_opennewtab.py
--rw-rw-rw-   0        0        0     1996 2024-05-06 10:05:23.000000 lantana-2.9.8.3/lantana/extensions/mdx_embedly.py
--rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.9.8.3/lantana/extensions/mdx_wsid.py
--rw-rw-rw-   0        0        0     1380 2024-03-11 05:31:11.000000 lantana-2.9.8.3/lantana/extensions/mermaid_precompile.py
--rw-rw-rw-   0        0        0     2021 2024-05-06 17:30:11.000000 lantana-2.9.8.3/lantana/extensions/selector.py
--rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.9.8.3/lantana/favicon.png
--rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.9.8.3/lantana/favicon.svg
-drwxrwxrwx   0        0        0        0 2024-05-26 09:07:15.442484 lantana-2.9.8.3/lantana/js/
--rw-rw-rw-   0        0        0    78749 2023-07-07 13:01:47.000000 lantana-2.9.8.3/lantana/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.9.8.3/lantana/js/highlight.min.js
--rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.9.8.3/lantana/js/jquery-3.6.1.slim.min.js
--rw-rw-rw-   0        0        0     3727 2024-03-11 07:44:04.000000 lantana-2.9.8.3/lantana/js/theme.js
--rw-rw-rw-   0        0        0     5691 2024-05-26 08:49:50.000000 lantana-2.9.8.3/lantana/main.html
--rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.9.8.3/lantana/mkdocs_theme.yml
--rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.9.8.3/lantana/nav.html
--rw-rw-rw-   0        0        0     1994 2024-04-19 06:45:51.000000 lantana-2.9.8.3/lantana/statics.html
--rw-rw-rw-   0        0        0      396 2024-04-03 03:19:38.000000 lantana-2.9.8.3/lantana/toc.html
-drwxrwxrwx   0        0        0        0 2024-05-26 09:07:15.411210 lantana-2.9.8.3/lantana.egg-info/
--rw-rw-rw-   0        0        0      239 2024-05-26 09:07:15.000000 lantana-2.9.8.3/lantana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1317 2024-05-26 09:07:15.000000 lantana-2.9.8.3/lantana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:07:15.000000 lantana-2.9.8.3/lantana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      852 2024-05-26 09:07:15.000000 lantana-2.9.8.3/lantana.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-26 09:07:15.000000 lantana-2.9.8.3/lantana.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      275 2024-05-26 09:07:15.000000 lantana-2.9.8.3/lantana.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 09:07:15.000000 lantana-2.9.8.3/lantana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 09:07:15.442484 lantana-2.9.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1877 2024-05-26 09:06:56.000000 lantana-2.9.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:21:45.926012 lantana-2.9.8.4/
+-rw-rw-rw-   0        0        0     1083 2022-10-28 14:22:28.000000 lantana-2.9.8.4/LICENCE.md
+-rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.9.8.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      239 2024-05-26 09:21:45.926012 lantana-2.9.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.9.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 09:21:45.892570 lantana-2.9.8.4/lantana/
+-rw-rw-rw-   0        0        0      829 2024-04-03 03:18:14.000000 lantana-2.9.8.4/lantana/404.html
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8.4/lantana/__init__.py
+-rw-rw-rw-   0        0        0     2731 2024-03-07 12:04:46.000000 lantana-2.9.8.4/lantana/__main__.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 13:19:19.000000 lantana-2.9.8.4/lantana/after_header.html
+-rw-rw-rw-   0        0        0        0 2024-05-26 09:17:07.000000 lantana-2.9.8.4/lantana/after_nav_tool.html
+-rw-rw-rw-   0        0        0     9493 2024-04-19 06:39:06.000000 lantana-2.9.8.4/lantana/base.html
+-rw-rw-rw-   0        0        0        0 2023-06-28 13:14:52.000000 lantana-2.9.8.4/lantana/before_header.html
+-rw-rw-rw-   0        0        0      306 2023-08-26 17:00:51.000000 lantana-2.9.8.4/lantana/breadcrumb.html
+drwxrwxrwx   0        0        0        0 2024-05-26 09:21:45.907577 lantana-2.9.8.4/lantana/css/
+-rw-rw-rw-   0        0        0    85883 2024-04-19 06:40:56.000000 lantana-2.9.8.4/lantana/css/bootstrap-icons.min.css
+-rw-rw-rw-   0        0        0   224443 2024-03-18 09:06:45.000000 lantana-2.9.8.4/lantana/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1152 2024-03-18 13:45:00.000000 lantana-2.9.8.4/lantana/css/default.min.css
+drwxrwxrwx   0        0        0        0 2024-05-26 09:21:45.909349 lantana-2.9.8.4/lantana/css/fonts/
+-rw-rw-rw-   0        0        0   176032 2024-04-19 06:23:31.000000 lantana-2.9.8.4/lantana/css/fonts/bootstrap-icons.woff.css
+-rw-rw-rw-   0        0        0   130396 2024-04-19 06:23:31.000000 lantana-2.9.8.4/lantana/css/fonts/bootstrap-icons.woff2.css
+-rw-rw-rw-   0        0        0     3949 2024-05-06 12:45:53.000000 lantana-2.9.8.4/lantana/css/theme.css
+-rw-rw-rw-   0        0        0     1927 2024-03-18 13:47:24.000000 lantana-2.9.8.4/lantana/css/vs.min.css
+drwxrwxrwx   0        0        0        0 2024-05-26 09:21:45.909349 lantana-2.9.8.4/lantana/extensions/
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8.4/lantana/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2714 2024-03-18 13:02:35.000000 lantana-2.9.8.4/lantana/extensions/accordion.py
+-rw-rw-rw-   0        0        0     3930 2024-05-06 13:25:21.000000 lantana-2.9.8.4/lantana/extensions/alerts.py
+-rw-rw-rw-   0        0        0     4704 2024-05-06 17:26:51.000000 lantana-2.9.8.4/lantana/extensions/alerts2.py
+-rw-rw-rw-   0        0        0     4553 2024-04-03 02:58:18.000000 lantana-2.9.8.4/lantana/extensions/cards.py
+-rw-rw-rw-   0        0        0     2116 2024-03-11 07:11:53.000000 lantana-2.9.8.4/lantana/extensions/codeblock_copybtn.py
+-rw-rw-rw-   0        0        0     1889 2024-05-06 17:43:29.000000 lantana-2.9.8.4/lantana/extensions/lantana.py
+-rw-rw-rw-   0        0        0      882 2024-03-11 07:41:11.000000 lantana-2.9.8.4/lantana/extensions/link_opennewtab.py
+-rw-rw-rw-   0        0        0     1996 2024-05-06 10:05:23.000000 lantana-2.9.8.4/lantana/extensions/mdx_embedly.py
+-rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.9.8.4/lantana/extensions/mdx_wsid.py
+-rw-rw-rw-   0        0        0     1380 2024-03-11 05:31:11.000000 lantana-2.9.8.4/lantana/extensions/mermaid_precompile.py
+-rw-rw-rw-   0        0        0     2021 2024-05-06 17:30:11.000000 lantana-2.9.8.4/lantana/extensions/selector.py
+-rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.9.8.4/lantana/favicon.png
+-rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.9.8.4/lantana/favicon.svg
+drwxrwxrwx   0        0        0        0 2024-05-26 09:21:45.926012 lantana-2.9.8.4/lantana/js/
+-rw-rw-rw-   0        0        0    78749 2023-07-07 13:01:47.000000 lantana-2.9.8.4/lantana/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.9.8.4/lantana/js/highlight.min.js
+-rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.9.8.4/lantana/js/jquery-3.6.1.slim.min.js
+-rw-rw-rw-   0        0        0     3727 2024-03-11 07:44:04.000000 lantana-2.9.8.4/lantana/js/theme.js
+-rw-rw-rw-   0        0        0     5678 2024-05-26 09:16:05.000000 lantana-2.9.8.4/lantana/main.html
+-rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.9.8.4/lantana/mkdocs_theme.yml
+-rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.9.8.4/lantana/nav.html
+-rw-rw-rw-   0        0        0     1994 2024-04-19 06:45:51.000000 lantana-2.9.8.4/lantana/statics.html
+-rw-rw-rw-   0        0        0      396 2024-04-03 03:19:38.000000 lantana-2.9.8.4/lantana/toc.html
+drwxrwxrwx   0        0        0        0 2024-05-26 09:21:45.892570 lantana-2.9.8.4/lantana.egg-info/
+-rw-rw-rw-   0        0        0      239 2024-05-26 09:21:45.000000 lantana-2.9.8.4/lantana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1317 2024-05-26 09:21:45.000000 lantana-2.9.8.4/lantana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 09:21:45.000000 lantana-2.9.8.4/lantana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      852 2024-05-26 09:21:45.000000 lantana-2.9.8.4/lantana.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-26 09:21:45.000000 lantana-2.9.8.4/lantana.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      275 2024-05-26 09:21:45.000000 lantana-2.9.8.4/lantana.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 09:21:45.000000 lantana-2.9.8.4/lantana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 09:21:45.926012 lantana-2.9.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1877 2024-05-26 09:21:41.000000 lantana-2.9.8.4/setup.py
```

### Comparing `lantana-2.9.8.3/LICENCE.md` & `lantana-2.9.8.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/README.md` & `lantana-2.9.8.4/README.md`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/404.html` & `lantana-2.9.8.4/lantana/404.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/__main__.py` & `lantana-2.9.8.4/lantana/__main__.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/base.html` & `lantana-2.9.8.4/lantana/base.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/css/bootstrap-icons.min.css` & `lantana-2.9.8.4/lantana/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/css/bootstrap.min.css` & `lantana-2.9.8.4/lantana/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/css/default.min.css` & `lantana-2.9.8.4/lantana/css/default.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/css/fonts/bootstrap-icons.woff.css` & `lantana-2.9.8.4/lantana/css/fonts/bootstrap-icons.woff.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/css/fonts/bootstrap-icons.woff2.css` & `lantana-2.9.8.4/lantana/css/fonts/bootstrap-icons.woff2.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/css/theme.css` & `lantana-2.9.8.4/lantana/css/theme.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/css/vs.min.css` & `lantana-2.9.8.4/lantana/css/vs.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/accordion.py` & `lantana-2.9.8.4/lantana/extensions/accordion.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/alerts.py` & `lantana-2.9.8.4/lantana/extensions/alerts.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/alerts2.py` & `lantana-2.9.8.4/lantana/extensions/alerts2.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/cards.py` & `lantana-2.9.8.4/lantana/extensions/cards.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/codeblock_copybtn.py` & `lantana-2.9.8.4/lantana/extensions/codeblock_copybtn.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/lantana.py` & `lantana-2.9.8.4/lantana/extensions/lantana.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/link_opennewtab.py` & `lantana-2.9.8.4/lantana/extensions/link_opennewtab.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/mdx_embedly.py` & `lantana-2.9.8.4/lantana/extensions/mdx_embedly.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/mdx_wsid.py` & `lantana-2.9.8.4/lantana/extensions/mdx_wsid.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/mermaid_precompile.py` & `lantana-2.9.8.4/lantana/extensions/mermaid_precompile.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/extensions/selector.py` & `lantana-2.9.8.4/lantana/extensions/selector.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/favicon.png` & `lantana-2.9.8.4/lantana/favicon.png`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/favicon.svg` & `lantana-2.9.8.4/lantana/favicon.svg`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/js/bootstrap.bundle.min.js` & `lantana-2.9.8.4/lantana/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/js/highlight.min.js` & `lantana-2.9.8.4/lantana/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/js/jquery-3.6.1.slim.min.js` & `lantana-2.9.8.4/lantana/js/jquery-3.6.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/js/theme.js` & `lantana-2.9.8.4/lantana/js/theme.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/main.html` & `lantana-2.9.8.4/lantana/main.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,15 @@
         {% if page.next_page %}
         <a class="btn text-primary print-hide" href="{{ page.next_page.url|url }}" title="{{ page.next_page.title }}"><i class="bi bi-chevron-right"></i></a>
         {% else %}
         <a class="btn text-muted print-hide"><i class="bi bi-chevron-right"></i></a>
         {% endif %}
       </div>
       {% endif %}
-      {% block after_nav_tool %}
-      {% endblock %}
+      {% include "after_nav_tool.html" %}
       <div>
         <div>
           {% if page and page.meta.author %}
           {% if page and page.meta.author_url %}
           <a href="{{ page.meta.author_url }}" class="unnewtab">{{ page.meta.author }}</a>
           {% else %}
           <span>{{ page.meta.author }}</span>
```

#### html2text {}

```diff
@@ -22,15 +22,15 @@
 {% if page and page.meta.summary %}
 {{ page.meta.summary }}
 ===============================================================================
 {% endif %} {% if page and not page.meta.disable_tools %}
 {% if page and not page.meta.disable_nav_tool %}
 {% if page.previous_page %} {% else %} {% endif %} {% if page.next_page %} {%
 else %} {% endif %}
-{% endif %} {% block after_nav_tool %} {% endblock %}
+{% endif %} {% include "after_nav_tool.html" %}
 {% if page and page.meta.author %} {% if page and page.meta.author_url %} _{
 _{_ _p_a_g_e_._m_e_t_a_._a_u_t_h_o_r_ _}_} {% else %} {{ page.meta.author }} {% endif %} | {% else
 %} {% if git_page_authors %} {{ git_page_authors | default('enable mkdocs-git-
 authors-plugin') }} | {% endif %} {% endif %} {% if page and page.meta.date %}
 {{ page.meta.date }} {% else %} {% if page.meta.revision_date %} {
 { page.meta.revision_date }} {% endif %} {% endif %} {% if page and not
 page.meta.disable_edit %} {% if page and page.edit_url %} {% elif
```

### Comparing `lantana-2.9.8.3/lantana/nav.html` & `lantana-2.9.8.4/lantana/nav.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana/statics.html` & `lantana-2.9.8.4/lantana/statics.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana.egg-info/SOURCES.txt` & `lantana-2.9.8.4/lantana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/lantana.egg-info/entry_points.txt` & `lantana-2.9.8.4/lantana.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.3/setup.py` & `lantana-2.9.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.9.8.3'
+VERSION = '2.9.8.4'
 
 setup(
     name="lantana",
     version=VERSION,
     url='https://lantana.wsoft.ws/',
     license='MIT',
     description='Bootstrap theme for MkDocs',
```

