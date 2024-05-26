# Comparing `tmp/meetlify-0.1.6.tar.gz` & `tmp/meetlify-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meetlify-0.1.6.tar", last modified: Fri May 24 01:59:05 2024, max compression
+gzip compressed data, was "meetlify-0.1.7.tar", last modified: Sun May 26 10:14:18 2024, max compression
```

## Comparing `meetlify-0.1.6.tar` & `meetlify-0.1.7.tar`

### file list

```diff
@@ -1,118 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.823558 meetlify-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-24 01:58:58.000000 meetlify-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 01:58:58.000000 meetlify-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-24 01:59:05.823558 meetlify-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-24 01:58:58.000000 meetlify-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-24 01:58:58.000000 meetlify-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 01:59:05.823558 meetlify-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-24 01:58:58.000000 meetlify-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.795558 meetlify-0.1.6/src/meetlify/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/meetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.795558 meetlify-0.1.6/src/meetlify/share/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/configs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/meetlify/share/content/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.795558 meetlify-0.1.6/src/meetlify/share/content/images/
--rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/images/fatureimage.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.795558 meetlify-0.1.6/src/meetlify/share/content/meetups/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/meetups/0001.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/meetups/0002.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/meetups/0003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.799558 meetlify-0.1.6/src/meetlify/share/content/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/pages/contact.md
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/pages/home.md
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/pages/privacy.md
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/content/pages/terms.md
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/share/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/meetlify/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/meetlify/themes/lindau/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.791558 meetlify-0.1.6/src/meetlify/themes/lindau/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.799558 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/about.png
--rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/author.png
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.811558 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
--rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/cookiealert.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.811558 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   238502 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.819558 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
--rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/cookiealert.js
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/static/js/scripts.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.819558 meetlify-0.1.6/src/meetlify/themes/lindau/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/meetup.html
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/meetups.html
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/sitemap-index.xml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/themes/lindau/templates/sitemap.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-24 01:58:58.000000 meetlify-0.1.6/src/meetlify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.819558 meetlify-0.1.6/src/meetlify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 01:59:05.000000 meetlify-0.1.6/src/meetlify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:59:05.819558 meetlify-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-24 01:58:58.000000 meetlify-0.1.6/tests/test_meetups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.780792 meetlify-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-26 10:14:10.000000 meetlify-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-26 10:14:10.000000 meetlify-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-26 10:14:18.780792 meetlify-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-26 10:14:10.000000 meetlify-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-26 10:14:10.000000 meetlify-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 10:14:18.780792 meetlify-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-26 10:14:10.000000 meetlify-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.740792 meetlify-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.744792 meetlify-0.1.7/src/meetlify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/meetups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/robots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.748792 meetlify-0.1.7/src/meetlify/share/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/configs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.740792 meetlify-0.1.7/src/meetlify/share/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.748792 meetlify-0.1.7/src/meetlify/share/content/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/content/images/fatureimage.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.748792 meetlify-0.1.7/src/meetlify/share/content/meetups/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/content/meetups/0001.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/content/meetups/0002.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/content/meetups/0003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.748792 meetlify-0.1.7/src/meetlify/share/content/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/content/pages/contact.md
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/content/pages/home.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/content/pages/privacy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/content/pages/terms.md
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/share/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/sitemaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.740792 meetlify-0.1.7/src/meetlify/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.740792 meetlify-0.1.7/src/meetlify/themes/lindau/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.740792 meetlify-0.1.7/src/meetlify/themes/lindau/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.752792 meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/author.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.768792 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/cookiealert.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.768792 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   238987 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.776792 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
+-rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/cookiealert.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/static/js/scripts.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.776792 meetlify-0.1.7/src/meetlify/themes/lindau/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/meetup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/meetups.html
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/post.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/posts.html
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/sitemap-index.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/themes/lindau/templates/sitemap.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-26 10:14:10.000000 meetlify-0.1.7/src/meetlify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.776792 meetlify-0.1.7/src/meetlify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-26 10:14:18.000000 meetlify-0.1.7/src/meetlify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-26 10:14:18.000000 meetlify-0.1.7/src/meetlify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:14:18.000000 meetlify-0.1.7/src/meetlify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-26 10:14:18.000000 meetlify-0.1.7/src/meetlify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:14:18.000000 meetlify-0.1.7/src/meetlify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-26 10:14:18.000000 meetlify-0.1.7/src/meetlify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 10:14:18.000000 meetlify-0.1.7/src/meetlify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:14:18.776792 meetlify-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-26 10:14:10.000000 meetlify-0.1.7/tests/test_meetups.py
```

### Comparing `meetlify-0.1.6/LICENSE` & `meetlify-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/PKG-INFO` & `meetlify-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.6.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.7.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -17,29 +17,26 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: markdown
 Requires-Dist: Jinja2
 Requires-Dist: python-slugify
 Provides-Extra: dev
@@ -54,25 +51,25 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
+Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: mkdocs-gen-files; extra == "all"
-Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: mkdocstrings[python]; extra == "all"
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: black; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: mkdocs; extra == "all"
 Requires-Dist: twine; extra == "all"
 Requires-Dist: setuptools; extra == "all"
+Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: mkdocstrings[python]; extra == "all"
+Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: wheel; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -111,20 +108,25 @@
 
 destination_path = Path("/home/user/Desktop/sample_webiste/")
 
 # Now initialize configurationn file
 initialize(dest_=destination_path)
 
 # Modify newly created config.json file as per your need.
-mlfy = Meetlify(dest_=destination_path) # Create Meetlify object with destination folder
-mlfy.parse_meetups() # Parse meetups markdown files
-mlfy.render_meetups() # Render meetups
-mlfy.render_home() # Render Home Page
-mlfy.render_pages() # Render Static Pages
-mlfy.copy_assests() # Copy assets e.g. Favicon, Images, JS, CSS files
+mtlfy = Meetlify(dest_=destination_path)
+mtlfy.render_home()
+mtlfy.render_404_page()
+mtlfy.render_meetups()
+mtlfy.render_posts()
+mtlfy.render_pages()
+mtlfy.render_redirects()
+mtlfy.render_sitemaps()
+mtlfy.render_robots_txt()
+mtlfy.copy_assests()
+
 ```
 
 ## How to Extend ?
 - Clone or download this repository to your computer.
 - Create a virtual environment using ``python -m .venv venv``
 - Navigate to the downloaded directory and then install all required dependencies using ``pip install -e .``
 - Now you can open ``api.py`` file and start editing it. Feel free to extend it or even submit a pull request if you have a useful feature.
```

### Comparing `meetlify-0.1.6/README.md` & `meetlify-0.1.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -39,20 +39,25 @@
 
 destination_path = Path("/home/user/Desktop/sample_webiste/")
 
 # Now initialize configurationn file
 initialize(dest_=destination_path)
 
 # Modify newly created config.json file as per your need.
-mlfy = Meetlify(dest_=destination_path) # Create Meetlify object with destination folder
-mlfy.parse_meetups() # Parse meetups markdown files
-mlfy.render_meetups() # Render meetups
-mlfy.render_home() # Render Home Page
-mlfy.render_pages() # Render Static Pages
-mlfy.copy_assests() # Copy assets e.g. Favicon, Images, JS, CSS files
+mtlfy = Meetlify(dest_=destination_path)
+mtlfy.render_home()
+mtlfy.render_404_page()
+mtlfy.render_meetups()
+mtlfy.render_posts()
+mtlfy.render_pages()
+mtlfy.render_redirects()
+mtlfy.render_sitemaps()
+mtlfy.render_robots_txt()
+mtlfy.copy_assests()
+
 ```
 
 ## How to Extend ?
 - Clone or download this repository to your computer.
 - Create a virtual environment using ``python -m .venv venv``
 - Navigate to the downloaded directory and then install all required dependencies using ``pip install -e .``
 - Now you can open ``api.py`` file and start editing it. Feel free to extend it or even submit a pull request if you have a useful feature.
```

### Comparing `meetlify-0.1.6/setup.py` & `meetlify-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 from src.meetlify import __version__
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # DATABASE/CONSTANTS LIST
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-python_minor_min = 8
+python_minor_min = 11
 python_minor_max = 12
 confirmed_python_versions = [
     "Programming Language :: Python :: 3.{MINOR:d}".format(MINOR=minor)
     for minor in range(python_minor_min, python_minor_max + 1)
 ]
 
 # Fetch readme file
```

### Comparing `meetlify-0.1.6/src/meetlify/__init__.py` & `meetlify-0.1.7/src/meetlify/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/api.py` & `meetlify-0.1.7/src/meetlify/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,399 +31,376 @@
 """
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # STANDARD LIBARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-import codecs
 import shutil
+import logging
 from pathlib import Path
-from datetime import datetime
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # 3rd PARTY LIBRARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-import markdown
 from jinja2 import Environment, FileSystemLoader
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # INTERNAL IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 from .configs import Configs
-from .post import Post
-from .page import Page
-from .meetup import Meetup
-from .sitemap import Sitemap
+from .posts import Posts
+from .pages import Pages
+from .meetups import Meetups
+from .sitemaps import Sitemaps
+from .redirects import Redirects
+from .robots import Robots
 from .constants import STATUS
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
+logging.getLogger("meetlify").addHandler(logging.NullHandler())
+
 
 class Meetlify:
     """Meetlify Static Site Generator for Meetups"""
 
     def __init__(self, dest_: Path) -> None:
         assert isinstance(dest_, Path)
 
         self.dest = dest_
         self.src = Path(__file__).resolve().parent
         self.configs = Configs.from_json(Path(self.dest, "configs.json"))
 
         self.renderer = Environment(
             loader=FileSystemLoader(
-                Path(self.dest, "themes", self.configs.theme, "templates")
+                Path(
+                    self.dest,
+                    self.configs.folders.themes,
+                    self.configs.theme,
+                    "templates",
+                )
             )
         )
-        self.meetups = []
-        self.posts = []
-        self.pages = []
-        self.sitemaps = []
+
+        self.meetups = Meetups(
+            path_=Path(
+                self.dest,
+                self.configs.folders.content,
+                self.configs.folders.meetups,
+            ),
+            reverse_=True,
+        )
+
+        self.posts = Posts(
+            path_=Path(
+                self.dest, self.configs.folders.content, self.configs.folders.posts
+            ),
+            reverse_=True,
+        )
+
+        self.pages = Pages(
+            path_=Path(
+                self.dest, self.configs.folders.content, self.configs.folders.pages
+            ),
+            reverse_=True,
+        )
+
+        self.sitemaps = Sitemaps(
+            sitemap_items_=[
+                {
+                    "name": "meetup",
+                    "items": self.meetups[STATUS.PUBLISHED, STATUS.DONE],
+                },
+                {"name": "posts", "items": self.posts[STATUS.PUBLISHED, STATUS.DONE]},
+                {"name": "pages", "items": self.pages[STATUS.PUBLISHED, STATUS.DONE]},
+            ]
+        )
+
+        self.redirects = Redirects.from_json(Path(self.dest, "redirects.json"))
+        self.robots = Robots.from_json(Path(self.dest, "robots.json"))
 
     def setup(self) -> None:
         """Setup Current Folder for Meetlify Website."""
-
         Path(self.dest, self.configs.folders.output).mkdir(parents=True, exist_ok=True)
-
         # TODO: Support to update themes folder - switch between multiple folders
         shutil.copytree(
-            Path(self.src, "themes", self.configs.theme),
-            Path(self.dest, "themes", self.configs.theme),
+            Path(self.src, self.configs.folders.themes, self.configs.theme),
+            Path(self.dest, self.configs.folders.themes, self.configs.theme),
             dirs_exist_ok=True,
         )
 
         shutil.copytree(
             Path(self.src, "share", "content"),
             Path(self.dest, self.configs.folders.content),
             dirs_exist_ok=True,
         )
 
     def clean(self):
         """Cleanup output folder"""
 
-        _output_folder = Path(self.dest, self.configs.folders.output)
+        output_folder = Path(self.dest, self.configs.folders.output)
 
-        if not _output_folder.exists():
-            _output_folder.mkdir()
+        if not output_folder.exists():
+            output_folder.mkdir()
         else:
-            for path in _output_folder.iterdir():
+            for path in output_folder.iterdir():
                 if path.is_file():
                     path.unlink()
                 elif path.is_dir():
                     shutil.rmtree(path)
 
-    def parse_meetups(self):
-        """Parse all Meetup events available as Markdown"""
-
-        self.meetups = [
-            Meetup.from_markdown(mt)
-            for mt in Path(self.dest, self.configs.folders.content, "meetups").iterdir()
-            if mt.is_file() and mt.suffix == ".md"
-        ]
-        self.meetups = [
-            mt
-            for mt in self.meetups
-            if mt.status in [STATUS.PUBLISHED.value, STATUS.DONE.value]
-        ]
-        self.meetups = sorted(self.meetups, key=lambda x: x.id, reverse=True)
-
-        self.sitemaps.append(
-            Sitemap.from_dict(
-                {
-                    "name": "meetups",
-                    "slug": "/meetups/",
-                    "modifieddate": datetime.now(),
-                    "items": self.meetups,
-                }
-            )
-        )
-
-    def parse_pages(self):
-        """Parse Pages avaialable as Markdown"""
-
-        self.pages = [
-            Page.from_markdown(mt)
-            for mt in Path(self.dest, self.configs.folders.content, "pages").iterdir()
-            if mt.is_file() and mt.name in ["privacy.md", "terms.md", "contact.md"]
-        ]
-
-        self.sitemaps.append(
-            Sitemap.from_dict(
-                {
-                    "name": "pages",
-                    "slug": "/",
-                    "modifieddate": datetime.now(),
-                    "items": self.pages,
-                }
-            )
-        )
-
-    def parse_posts(self):
-        """Parse Posts avaialable as Markdown"""
-
-        self.posts = [
-            Post.from_markdown(mt)
-            for mt in Path(self.dest, self.configs.folders.content, "posts").iterdir()
-            if mt.is_file() and mt.suffix == ".md"
-        ]
-
-        self.sitemaps.append(
-            Sitemap.from_dict(
-                {
-                    "name": "posts",
-                    "slug": "/",
-                    "modifieddate": datetime.now(),
-                    "items": self.posts,
-                }
-            )
-        )
-
     def render_home(self):
-        """Render home page"""
-        with codecs.open(
-            Path(
-                self.dest,
-                self.configs.folders.content,
-                self.configs.folders.pages,
-                f"{self.configs.home}.md",
-            ),
-            "r",
-            encoding="utf-8",
-        ) as f:
-            data = f.read()
-            home_content = markdown.Markdown(extensions=["meta", "attr_list"]).convert(
-                data
-            )
-
         with open(
             Path(self.dest, self.configs.folders.output, "index.html"),
             mode="w",
             encoding="utf-8",
         ) as file:
             file.write(
                 self.renderer.get_template("index.html").render(
                     meta=self.configs,
-                    home_content="".join(home_content),
-                    meetups=self.meetups[0:3],
-                    posts=self.posts[0:3],
+                    about_us_paragraphs=self.configs.about_us,
+                    meetups=self.meetups[STATUS.PUBLISHED, STATUS.DONE][0:3],
+                    posts=self.posts[STATUS.PUBLISHED, STATUS.DONE][0:3],
                 )
             )
-            print("... wrote output/home")
+            logging.info("... wrote output/home")
 
+    def render_404_page(self):
         with open(
             Path(self.dest, self.configs.folders.output, "404.html"),
             mode="w",
             encoding="utf-8",
         ) as file:
             file.write(
                 self.renderer.get_template("404.html").render(
-                    meta=self.configs, meetups=self.meetups[0:3]
+                    meta=self.configs,
+                    meetups=self.meetups[STATUS.PUBLISHED, STATUS.DONE][0:3],
+                    posts=self.posts[STATUS.PUBLISHED, STATUS.DONE][0:3],
                 )
             )
-            print("... wrote output/404")
-
-    def render_pages(self):
-        """Render permanent pages"""
-
-        for _page in self.pages:
-            Path(self.dest, self.configs.folders.output, _page.slug).mkdir(
-                parents=True, exist_ok=True
-            )
+            logging.info("... wrote output/404")
 
-            with open(
-                Path(self.dest, self.configs.folders.output, _page.slug, "index.html"),
-                mode="w",
-                encoding="utf-8",
-            ) as file:
-                file.write(
-                    self.renderer.get_template("page.html").render(
-                        meta=self.configs, front=_page
-                    )
-                )
-                print(f"... wrote output/{_page.slug}")
+    def render_meetups(self):
+        """Render meetup pages and Meetup index page"""
 
-    def render_sitemaps(self):
-        """Render Sitemaps"""
+        # TODO: Check if there are less than 3 meetups and runs without error? make 3 config variable
+        for meetup in self.meetups[STATUS.PUBLISHED, STATUS.DONE]:
+            Path(
+                self.dest,
+                self.configs.folders.output,
+                self.configs.folders.meetups,
+                meetup.slug,
+            ).mkdir(parents=True, exist_ok=True)
 
-        for sitemap in self.sitemaps:
             with open(
                 Path(
                     self.dest,
                     self.configs.folders.output,
-                    f"sitemap-{sitemap.name}.xml",
+                    self.configs.folders.meetups,
+                    meetup.slug,
+                    "index.html",
                 ),
                 mode="w",
                 encoding="utf-8",
             ) as file:
                 file.write(
-                    self.renderer.get_template("sitemap.xml").render(
+                    self.renderer.get_template("meetup.html").render(
                         meta=self.configs,
-                        category=sitemap.slug,
-                        items=sitemap.items,
+                        meetup=meetup,
                     )
                 )
-                print(f"... wrote output/{sitemap.name}/sitemap")
+                logging.info(f"...... wrote output/meetups/{meetup.slug}")
 
+        # save meetup index page
         with open(
             Path(
                 self.dest,
                 self.configs.folders.output,
-                "sitemap-index.xml",
+                self.configs.folders.meetups,
+                "index.html",
             ),
             mode="w",
             encoding="utf-8",
         ) as file:
             file.write(
-                self.renderer.get_template("sitemap-index.xml").render(
-                    meta=self.configs, sitemaps=self.sitemaps
+                self.renderer.get_template("meetups.html").render(
+                    meta=self.configs,
+                    meetups=self.meetups[STATUS.PUBLISHED, STATUS.DONE],
                 )
             )
-            print("... wrote output/sitemap-index")
+            logging.info("... wrote output/meetups")
 
-    def render_meetups(self):
-        """Render meetup pages and Meetup index page"""
+    def render_posts(self):
+        """Render posts and Meetup index page"""
 
-        # TODO: Check if there are less than 3 meetups and runs without error? make 3 config variable
-        for _meetup in self.meetups:
-            Path(self.dest, self.configs.folders.output, "meetups", _meetup.slug).mkdir(
-                parents=True, exist_ok=True
-            )
+        # TODO: Check if there are less than 3 posts  and runs without error? make 3 config variable
+        for post in self.posts[STATUS.PUBLISHED, STATUS.DONE]:
+            Path(
+                self.dest,
+                self.configs.folders.output,
+                self.configs.folders.posts,
+                post.slug,
+            ).mkdir(parents=True, exist_ok=True)
 
             with open(
                 Path(
                     self.dest,
                     self.configs.folders.output,
-                    "meetups",
-                    _meetup.slug,
+                    self.configs.folders.posts,
+                    post.slug,
                     "index.html",
                 ),
                 mode="w",
                 encoding="utf-8",
             ) as file:
                 file.write(
-                    self.renderer.get_template("meetup.html").render(
+                    self.renderer.get_template("post.html").render(
                         meta=self.configs,
-                        content=_meetup.content,
-                        front=_meetup,
+                        post=post,
+                        banner=self.configs.get_banner(banner_name=post.banner),
                     )
                 )
-                print(f"...... wrote output/meetups/{_meetup.slug}")
+                logging.info(f"...... wrote output/posts/{post.slug}")
 
         # save meetup index page
         with open(
-            Path(self.dest, self.configs.folders.output, "meetups", "index.html"),
+            Path(
+                self.dest,
+                self.configs.folders.output,
+                self.configs.folders.posts,
+                "index.html",
+            ),
             mode="w",
             encoding="utf-8",
         ) as file:
             file.write(
-                self.renderer.get_template("meetups.html").render(
-                    meta=self.configs, meetups=self.meetups
+                self.renderer.get_template("posts.html").render(
+                    meta=self.configs, posts=self.posts[STATUS.PUBLISHED, STATUS.DONE]
                 )
             )
-            print("... wrote output/meetups")
+            logging.info("... wrote output/posts")
 
-    def render_posts(self):
-        """Render posts and Meetup index page"""
+    def render_pages(self):
+        """Render permanent pages"""
 
-        # TODO: Check if there are less than 3 meetups and runs without error? make 3 config variable
-        for _post in self.posts:
-            Path(self.dest, self.configs.folders.output, "posts", _post.slug).mkdir(
+        for page in self.pages[STATUS.PUBLISHED, STATUS.DONE]:
+            Path(self.dest, self.configs.folders.output, page.slug).mkdir(
                 parents=True, exist_ok=True
             )
 
-            _admonition = {
-                "type": "hint",
-                "title": "Update",
-                "message": "This is work in progress. Please checkback later for an updated version of this post.",
-            }
+            with open(
+                Path(self.dest, self.configs.folders.output, page.slug, "index.html"),
+                mode="w",
+                encoding="utf-8",
+            ) as file:
+                file.write(
+                    self.renderer.get_template("page.html").render(
+                        meta=self.configs, page=page
+                    )
+                )
+                logging.info(f"... wrote output/{page.slug}")
 
+    def render_sitemaps(self):
+        """Render Sitemaps"""
+
+        for sitemap in self.sitemaps[STATUS.PUBLISHED]:
             with open(
                 Path(
                     self.dest,
                     self.configs.folders.output,
-                    "posts",
-                    _post.slug,
-                    "index.html",
+                    f"sitemap-{sitemap.name}.xml",
                 ),
                 mode="w",
                 encoding="utf-8",
             ) as file:
                 file.write(
-                    self.renderer.get_template("post.html").render(
-                        meta=self.configs,
-                        content=_post.content,
-                        front=_post,
-                        admonition=_admonition,
+                    self.renderer.get_template("sitemap.xml").render(
+                        meta=self.configs, sitemap=sitemap
                     )
                 )
-                print(f"...... wrote output/posts/{_post.slug}")
+                logging.info(f"... wrote output/{sitemap.name}/sitemap")
 
-        # save meetup index page
         with open(
-            Path(self.dest, self.configs.folders.output, "posts", "index.html"),
+            Path(
+                self.dest,
+                self.configs.folders.output,
+                "sitemap-index.xml",
+            ),
             mode="w",
             encoding="utf-8",
         ) as file:
             file.write(
-                self.renderer.get_template("posts.html").render(
-                    meta=self.configs, posts=self.posts
+                self.renderer.get_template("sitemap-index.xml").render(
+                    meta=self.configs, sitemaps=self.sitemaps[STATUS.PUBLISHED]
                 )
             )
-            print("... wrote output/posts")
+            logging.info("... wrote output/sitemap-index")
 
-    def copy_assests(self):
-        """Copy Assets e.g. Static Folders, Images, Feeds, and Sitemaps"""
+    def render_redirects(self):
+        with open(
+            Path(
+                self.dest,
+                self.configs.folders.output,
+                "_redirects",
+            ),
+            mode="w",
+            encoding="utf-8",
+        ) as file:
+            file.write(str(self.redirects))
+            logging.info("... wrote output/redirects file")
+
+    def render_robots_txt(self):
+        if self.configs.robots:
+            with open(
+                Path(
+                    self.dest,
+                    self.configs.folders.output,
+                    "robots.txt",
+                ),
+                mode="w",
+                encoding="utf-8",
+            ) as file:
+                file.write(str(self.robots))
+                logging.info("... wrote output/robots.txt file")
 
+    def copy_assests(self):
         # copy static folders
         shutil.copytree(
-            Path(self.dest, "themes", self.configs.theme, "static"),
+            Path(self.dest, self.configs.folders.themes, self.configs.theme, "static"),
             Path(
                 self.dest,
                 self.configs.folders.output,
                 "static",
             ),
             dirs_exist_ok=True,
         )
-        print("... copied output/themes static folder")
+        logging.info("... copied output/themes static folder")
 
         # copy images folder
         shutil.copytree(
-            Path(self.dest, self.configs.folders.content, "images"),
+            Path(self.dest, self.configs.folders.content, self.configs.folders.images),
             Path(
                 self.dest,
                 self.configs.folders.output,
-                "images",
+                self.configs.folders.images,
             ),
             dirs_exist_ok=True,
         )
-        print("... copied output/images folder")
-
-        # copy robots.txt file
-        if self.configs.robots:
-            shutil.copyfile(
-                Path(self.src, "share", "robots.txt"),
-                Path(
-                    self.dest,
-                    self.configs.folders.output,
-                    "robots.txt",
-                ),
-            )
-            print("... copied output/robots.txt filed")
+        logging.info("... copied output/images folder")
 
     def make(self):
-        """Make Static Site and Save to Output folder"""
-
-        self.parse_meetups()
-        self.parse_pages()
-        self.parse_posts()
         self.render_home()
+        self.render_404_page()
         self.render_meetups()
         self.render_posts()
         self.render_pages()
+        self.render_redirects()
         self.render_sitemaps()
+        self.render_robots_txt()
         self.copy_assests()
```

### Comparing `meetlify-0.1.6/src/meetlify/cli.py` & `meetlify-0.1.7/src/meetlify/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # STANDARD LIBARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import os
+import logging
+
 from pathlib import Path
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # 3rd PARTY LIBRARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
@@ -54,14 +56,19 @@
 from .utils import initialize
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
+logging.basicConfig(
+    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
+)
+logging.getLogger("meetlify").propagate = True
+
 
 @click.group()
 def main():
     pass
 
 
 @main.command("init", help="Initialize Meetlify Project")
@@ -87,35 +94,40 @@
 @click.option("--home/--no-home", default=False)
 @click.option("--pages/--no-pages", default=False)
 @click.option("--posts/--no-posts", default=False)
 @click.option("--assets/--no-assets", default=False)
 @click.option("--sitemap/--no-sitemap", default=False)
 def make(meetups, home, pages, posts, assets, sitemap):
     click.echo("Make Current Project")
-    _mlfy = Meetlify(dest_=Path(os.getcwd()))
-
-    if meetups:
-        _mlfy.parse_meetups()
-        _mlfy.render_meetups()
+    mtlfy = Meetlify(dest_=Path(os.getcwd()))
 
     if home:
-        _mlfy.parse_meetups()
-        _mlfy.render_home()
+        mtlfy.render_home()
+        mtlfy.render_404_page()
+
+    if meetups:
+        mtlfy.render_meetups()
 
     if pages:
-        _mlfy.parse_pages()
-        _mlfy.render_pages()
+        mtlfy.render_pages()
 
     if posts:
-        _mlfy.parse_posts()
-        # _mlfy.render_()
-
-    if assets:
-        _mlfy.copy_assests()
+        mtlfy.render_posts()
 
     if sitemap:
-        _mlfy.parse_meetups()
-        _mlfy.parse_pages()
-        _mlfy.render_sitemaps()
+        mtlfy.render_redirects()
+        mtlfy.render_robots_txt()
+        mtlfy.render_sitemaps()
+
+    if assets:
+        mtlfy.copy_assests()
 
     if not any([meetups, home, pages, posts, assets, sitemap]):
-        _mlfy.make()
+        mtlfy.render_home()
+        mtlfy.render_404_page()
+        mtlfy.render_meetups()
+        mtlfy.render_posts()
+        mtlfy.render_pages()
+        mtlfy.render_redirects()
+        mtlfy.render_sitemaps()
+        mtlfy.render_robots_txt()
+        mtlfy.copy_assests()
```

### Comparing `meetlify-0.1.6/src/meetlify/configs.py` & `meetlify-0.1.7/src/meetlify/robots.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 Meetlify: Static Site Generator for Meetup Websites
 A Python Package for Generating Static Website for Meetups.
 https://github.com/pybodensee/meetlify
 
-    src\meetlify\configs.py
+    src\meetlify\\robots.py
 
     Copyright (C) 2024-2024 Faisal Shahzad <info@serpwings.com>
 
 <LICENSE_BLOCK>
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -26,98 +26,73 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 </LICENSE_BLOCK>
 """
 
-
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # STANDARD LIBARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import json
 import codecs
 from pathlib import Path
 from dataclasses import dataclass
-
+from typing import Self
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
 @dataclass
-class Menu:
-    """Menu Data Class to hold Header and footer menus"""
+class RobotAgent:
+    name: str
+    allow: list[str]
+    disallow: list[str]
 
-    header: dict
-    footer: dict
+    def __str__(self) -> str:
+        allows = "\nAllow: " if self.allow else ""
+        allows += "\nAllow: ".join(self.allow)
 
+        disallows = "\nDisallow: " if self.disallow else ""
+        disallows += "\nDisallow: ".join(self.disallow)
 
-@dataclass
-class Folders:
-    """Folder data class for differnt types of folder used in Processing"""
-
-    output: str
-    content: str
-    meetups: str
-    pages: str
-    posts: str
+        return f"User-agent: {self.name}{allows}{disallows}\n\n"
 
+    @classmethod
+    def from_dict(cls, object_: dict) -> Self:
+        return cls(**object_)
 
-@dataclass
-class Configs:
-    """Config Data Class to hold Project Configurations"""
 
-    name: str
-    URL: str
-    language: str
-    theme: str
-    title: str
-    author: str
-    email: str
-    description: str
-    sitemap: bool
-    feeds: bool
-    robots: bool
-    logo: str
-    favicon: str
-    copyright: str
-    home: str
-    folders: dict
-    menu: Menu
+class Robots:
+    def __init__(self, *, robots_items_: dict) -> None:
+        self.all_robots = [
+            RobotAgent.from_dict(
+                {
+                    "name": robot_name,
+                    "allow": robot_values.get("allow"),
+                    "disallow": robot_values.get("disallow"),
+                }
+            )
+            for robot_name, robot_values in robots_items_.items()
+            if robot_name != "sitemaps"
+        ]
+
+        self.sitemaps = robots_items_.get("sitemaps")
+
+    def __str__(self) -> str:
+        sitemap_as_str = "\nSitemap: " if self.sitemaps else ""
+        sitemap_as_str += "\nSitemap: ".join(self.sitemaps)
+
+        return (
+            "\n".join([str(robot_agent) for robot_agent in self.all_robots])
+            + sitemap_as_str
+        )
 
     @classmethod
-    def from_json(cls, json_file_: Path):
-        """Generate Config data class from json file
-
-        Args:
-            json_file (Path): Json file containing Project Configurations
-
-        Returns:
-            Configs: Return Configs Data object
-        """
+    def from_json(cls, json_file_: Path) -> Self:
         assert isinstance(json_file_, Path)
         assert json_file_.exists()
-
-        with codecs.open(json_file_, "r", encoding="utf-8") as f:
-            cfgs = json.load(f)
-            return cls(
-                name=cfgs["name"],
-                URL=cfgs["URL"],
-                language=cfgs["language"],
-                theme=cfgs["theme"],
-                title=cfgs["title"],
-                author=cfgs["author"],
-                email=cfgs["email"],
-                description=cfgs["description"],
-                sitemap=cfgs["sitemap"],
-                feeds=cfgs["feeds"],
-                robots=cfgs["robots"],
-                logo=cfgs["logo"],
-                favicon=cfgs["favicon"],
-                copyright=cfgs["copyright"],
-                home=cfgs["home"],
-                folders=Folders(**cfgs["folders"]),
-                menu=Menu(**cfgs["menu"]),
-            )
+        with codecs.open(str(json_file_), "r", encoding="utf-8") as f:
+            return cls(robots_items_=json.load(f))
```

### Comparing `meetlify-0.1.6/src/meetlify/constants.py` & `meetlify-0.1.7/src/meetlify/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # DATABASE/CONSTANTS LIST
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
-VERSION_REVISION = 6
+VERSION_REVISION = 7
 
 FULL_VERSION = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_REVISION}"
 
 
 class ExtendedEnum(Enum):
     """An extended enum class to convert list of items in an enumration."""
 
@@ -61,13 +61,13 @@
 
     DRAFT = "draft"
     PLANNING = "planning"
     PUBLISHED = "published"
     DONE = "done"
 
 
-class ADMONITION(ExtendedEnum):
-    """An enum for the different Admonitions."""
+class BANNER(ExtendedEnum):
+    """An enum for the different Banners."""
 
     DRAFT = "draft"
     INCOMPLETE = "incomplete"
     COMPLETE = "complete"
```

### Comparing `meetlify-0.1.6/src/meetlify/post.py` & `meetlify-0.1.7/src/meetlify/pages.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 Meetlify: Static Site Generator for Meetup Websites
 A Python Package for Generating Static Website for Meetups.
 https://github.com/pybodensee/meetlify
 
-    src\meetlify\post.py
+    src\meetlify\page.py
 
     Copyright (C) 2024-2024 Faisal Shahzad <info@serpwings.com>
 
 <LICENSE_BLOCK>
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -30,80 +30,83 @@
 </LICENSE_BLOCK>
 """
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # STANDARD LIBARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-import codecs
+from pathlib import Path
 from dataclasses import dataclass
 from datetime import datetime, timezone
-from pathlib import Path
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # 3rd PARTY LIBRARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-import markdown
-
+from slugify import slugify
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # INTERNAL IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-from .utils import get_slug
+from .utils import markdown_convertor
+from .constants import STATUS
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
 @dataclass
-class Post:
-    """Post Data Class"""
-
+class Page:
     title: str
-    date: str
-    modifieddate: str
-    featureimage: str
     author: str
-    slug: str
-    status: str
-    tags: str
-    admonition: str
     description: str
+    slug: str
+    create_date: datetime
+    last_modified: datetime
     toc: str
     content: str
+    add_to_sitemap: bool
+    status: str
 
-    @classmethod
-    def from_markdown(cls, page_):
-        """Genreate Post Data Class from Markdown File
-
-        Args:
-            page_ (dict): Post as dict file
+    def __lt__(self, other_):
+        return self.create_date < other_.create_date
 
-        Returns:
-            Post: Return Constructed Post Object
-        """
-        _md = markdown.Markdown(extensions=["meta", "attr_list", "toc"])
-        with codecs.open(page_, "r", encoding="utf-8") as f:
-            data = f.read()
-            content_ = _md.convert(data)
-
-            return cls(
-                content=content_,
-                date="".join(_md.Meta["date"]),
-                modifieddate=datetime.fromtimestamp(
-                    Path(page_).stat().st_mtime, tz=timezone.utc
-                ),
-                author="".join(_md.Meta["author"]),
-                title="".join(_md.Meta["title"]),
-                description="".join(_md.Meta["description"]),
-                slug=get_slug(
-                    _md.Meta["slug"] if "slug" in _md.Meta else [""], _md.Meta["title"]
-                ),
-                tags=_md.Meta["tags"],
-                admonition=_md.Meta["admonition"],
-                featureimage="".join(_md.Meta["featureimage"]),
-                toc=_md.toc,
-                status="".join(_md.Meta["status"]),
-            )
+    @classmethod
+    def from_markdown(cls, page_md_: Path):
+        meta, toc, content = markdown_convertor(page_md_)
+        return cls(
+            title=meta.get("title"),
+            author=meta.get("author"),
+            description=meta.get("description"),
+            slug=meta.get("slug") or slugify(meta.get("title")),
+            create_date=datetime.strptime(meta.get("create_date"), "%Y-%m-%d::%H:%M"),
+            last_modified=datetime.fromtimestamp(
+                page_md_.stat().st_mtime, tz=timezone.utc
+            ),
+            toc=toc,
+            content=content,
+            add_to_sitemap=bool(meta.get("add_to_sitemap")),
+            status=meta.get("status"),
+        )
+
+
+class Pages:
+    def __init__(self, *, path_: Path, reverse_: bool = True) -> None:
+        self.content = sorted(
+            [
+                Page.from_markdown(page_md)
+                for page_md in path_.iterdir()
+                if page_md.is_file() and page_md.suffix == ".md"
+            ],
+            reverse=reverse_,
+        )
+
+    def __getitem__(self, status_: list[STATUS] | STATUS) -> list[Page]:
+        if isinstance(status_, STATUS):
+            status_ = [status_]
+        return [
+            content
+            for content in self.content
+            if content.status in [stat.value for stat in status_]
+        ]
```

### Comparing `meetlify-0.1.6/src/meetlify/share/__init__.py` & `meetlify-0.1.7/src/meetlify/share/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/configs.json` & `meetlify-0.1.7/src/meetlify/share/configs.json`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/content/images/fatureimage.png` & `meetlify-0.1.7/src/meetlify/share/content/images/fatureimage.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/content/meetups/0001.md` & `meetlify-0.1.7/src/meetlify/share/content/meetups/0001.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/content/meetups/0002.md` & `meetlify-0.1.7/src/meetlify/share/content/meetups/0002.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/content/meetups/0003.md` & `meetlify-0.1.7/src/meetlify/share/content/meetups/0003.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/content/pages/contact.md` & `meetlify-0.1.7/src/meetlify/share/content/pages/contact.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/content/pages/home.md` & `meetlify-0.1.7/src/meetlify/share/content/pages/home.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/content/pages/privacy.md` & `meetlify-0.1.7/src/meetlify/share/content/pages/privacy.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/share/content/pages/terms.md` & `meetlify-0.1.7/src/meetlify/share/content/pages/terms.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/sitemap.py` & `meetlify-0.1.7/src/meetlify/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 Meetlify: Static Site Generator for Meetup Websites
 A Python Package for Generating Static Website for Meetups.
 https://github.com/pybodensee/meetlify
 
-    src\meetlify\sitemap.py
+    src\meetlify\\utils.py
 
     Copyright (C) 2024-2024 Faisal Shahzad <info@serpwings.com>
 
 <LICENSE_BLOCK>
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -27,44 +27,53 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 </LICENSE_BLOCK>
 """
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
-# STANDARD LIBARY IMPORTS
+# INTERNAL IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-from dataclasses import dataclass
-from datetime import datetime
+import codecs
+import shutil
+from pathlib import Path
 
+# +++++++++++++++++++++++++++++++++++++++++++++++++++++
+# 3rd PARTY LIBRARY IMPORTS
+# +++++++++++++++++++++++++++++++++++++++++++++++++++++
+
+import markdown
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
-@dataclass
-class Sitemap:
-    """Sitemap Data Class"""
-
-    name: str
-    slug: str
-    modifieddate: str
-    items: list
-
-    @classmethod
-    def from_dict(cls, object_):
-        """Genreate Sitemaps Class from object_ dictionary
-
-        Args:
-            object_ (dict): Sitemap object_ as dictionary
-
-        Returns:
-            Page: Return Constructed Sitemap Object
-        """
-        return cls(
-            name=object_["name"],
-            slug=object_["slug"],
-            modifieddate=datetime.now(),
-            items=object_["items"],
+def initialize(dest_: Path) -> None:
+    """Intialze Meetlify Website
+
+    Args:
+        dest_ (Path): Speficy folder for Destitaion folder.
+    """
+    assert isinstance(dest_, Path)
+    assert dest_.exists()
+
+    shutil.copyfile(
+        Path(Path(__file__).resolve().parent, "share", "configs.json"),
+        Path(dest_, "configs.json"),
+    )
+
+
+def markdown_convertor(md_file_: Path) -> tuple:
+    assert isinstance(md_file_, Path)
+    assert md_file_.exists()
+
+    md_convertor = markdown.Markdown(extensions=["meta", "attr_list", "toc"])
+    with codecs.open(md_file_, "r", encoding="utf-8") as f:
+        data = f.read()
+        content = md_convertor.convert(data)
+        return (
+            {k: "".join(v) for k, v in md_convertor.Meta.items()},
+            md_convertor.toc,
+            content,
         )
```

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/about.png` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/about.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/author.png` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/author.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/banner.png` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/banner.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/favicon.png` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/assets/logo.png` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/assets/logo.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-icons.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.min.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/css/styles.css` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/css/styles.css`

 * *Files 0% similar despite different names*

```diff
@@ -12654,17 +12654,42 @@
   font-weight: 400 !important;
   margin-bottom: 1.15rem !important;
   font-size: 1.15rem;
   margin-top: 0;
   margin-bottom: 1rem;
 }
 
-h1,
-h2,
-h3,
-h4,
-h5,
+h1 {
+  font-weight: bolder !important;
+  margin-bottom: 1.12rem !important;
+  font-size: 1.70rem;
+}
+
+h2 {
+  font-weight: bolder !important;
+  margin-bottom: 1.12rem !important;
+  font-size: 1.60rem;
+}
+
+h3 {
+  font-weight: bolder !important;
+  margin-bottom: 1.12rem !important;
+  font-size: 1.50rem;
+}
+
+h4 {
+  font-weight: bolder !important;
+  margin-bottom: 1.12rem !important;
+  font-size: 1.40rem;
+}
+
+h5 {
+  font-weight: bolder !important;
+  margin-bottom: 1.12rem !important;
+  font-size: 1.30rem;
+}
+
 h6 {
   font-weight: bolder !important;
   margin-bottom: 1.12rem !important;
-  font-size: 1.75rem;
+  font-size: 1.10rem;
 }
```

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.js` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.js` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.js.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.min.js` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/cookiealert.js` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/cookiealert.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/static/js/scripts.js` & `meetlify-0.1.7/src/meetlify/themes/lindau/static/js/scripts.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/templates/404.html` & `meetlify-0.1.7/src/meetlify/themes/lindau/templates/404.html`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,16 @@
                     <h1 class="display-5 fw-bolder text-white mb-2">Oops! This page doen not exists.
                     </h1>
                     <p class="lead fw-normal text-white-50 mb-4"> You hit an invalid route and this page does not exist.
                         You can visit our home page or meetups page to get more information about our website.
                     </p>
                     <div class="d-grid gap-3 d-sm-flex justify-content-sm-center justify-content-xl-start">
                         <a class="btn btn-primary btn-lg px-4 me-sm-3" href="{{meta.URL}}/">Home</a>
-                        <a class="btn btn-primary btn-lg px-4 me-sm-3" href="{{meta.URL}}/meetups/">Meetups</a>
+                        <a class="btn btn-primary btn-lg px-4 me-sm-3"
+                            href="{{meta.URL}}/{{meta.folders.meetups}}/">Meetups</a>
                     </div>
                 </div>
             </div>
             <div class="col-xl-5 col-xxl-6 d-none d-xl-block text-center"><img class="img-fluid rounded-3 my-5"
                     src="{{meta.URL}}/static/assets/banner.png" alt="{{meta.name}} about us banner" /></div>
         </div>
     </div>
@@ -44,20 +45,20 @@
                 </div>
             </div>
         </div>
         <div class="row gx-5">
             {% for meetup in meetups%}
             <div class="col-lg-4 mb-5">
                 <div class="card h-100 shadow border-0">
-                    <img class="card-img-top" src="{{meta.URL}}/images/{{meetup.featureimage}}"
+                    <img class="card-img-top" src="{{meta.URL}}/images/{{meetup.feature_image}}"
                         alt="Feature Image for Meetup">
                     <div class="card-body p-4">
                         <div class="badge bg-primary bg-gradient rounded-pill mb-2">Meetup</div>
                         <a class="text-decoration-none link-dark stretched-link"
-                            href="{{meta.URL}}/meetups/{{meetup.slug}}/">
+                            href="{{meta.URL}}/{{meta.folders.meetups}}/{{meetup.slug}}/">
                             <h5 class="card-title mb-3"> {{meetup.title}}
                             </h5>
                         </a>
                         <p class="card-text mb-0">Agenda: {{meetup.description}}</p>
                     </div>
                     <div class="card-footer p-4 pt-0 bg-transparent border-top-0">
                         <div class="d-flex align-items-end justify-content-between">
@@ -74,15 +75,15 @@
                         </div>
                     </div>
                 </div>
             </div>
             {% endfor%}
         </div>
         <div class="text-end mb-5 mb-xl-0">
-            <a class="text-decoration-none" href="{{meta.URL}}/meetups/">
+            <a class="text-decoration-none" href="{{meta.URL}}/{{meta.folders.meetups}}/">
                 Older Meetups
                 <i class="bi bi-arrow-right"></i>
             </a>
         </div>
     </div>
 </section>
 {% endblock main_content %}
```

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/templates/base.html` & `meetlify-0.1.7/src/meetlify/themes/lindau/templates/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     <meta name="apple-mobile-web-app-title" content="{{meta.name}}" />
     <meta name="application-name" content="{{meta.name}}" />
     <meta property="og:image" content="{{meta.url}}/static/assets/logo.png" />
     <meta content="282" property="og:image:width" />
     <meta content="104" property="og:image:height" />
     <meta content="image/png" property="og:image:type" />
 
-    <link rel="icon" type="image/x-icon" href="{{meta.url}}/favicon.icon" />
-    <link rel="shortcut icon" href="{{meta.url}}/favicon.ico" />
+    <link rel="icon" type="image/x-icon" href="{{meta.url}}/static/assets/favicon.png" />
+    <link rel="shortcut icon" href="{{meta.url}}/static/assets/favicon.png" />
     <meta content="{{meta.url}}/favicon.ico" name="msapplication-TileImage">
 
     <meta name="generator" content="meetlify" />
     <meta name="language" content="english" />
     <meta name="format-detection" content="telephone=yes" />
     <meta name="HandheldFriendly" content="true" />
     <meta name="distribution" content="web" />
@@ -42,14 +42,15 @@
 
     <!-- Favicon-->
     <link rel="icon" type="image/x-icon" href="{{meta.URL}}/static/assets/favicon.png" />
     <!-- Bootstrap icons-->
     <link href="{{meta.URL}}/static/css/bootstrap-icons.css" rel="stylesheet" />
     <!-- Core theme CSS (includes Bootstrap)-->
     <link href="{{meta.URL}}/static/css/styles.css" rel="stylesheet" />
+    <link href="{{meta.URL}}/static/css/custom.css" rel="stylesheet" />
     <!-- Cookies Alert-->
     <link href="{{meta.URL}}/static/css/cookiealert.css" rel="stylesheet">
 </head>
 
 <body class="d-flex flex-column h-100">
     <main class="flex-shrink-0">
         <!-- Navigation-->
@@ -95,15 +96,15 @@
                     <span class="text-white mx-1">{{ "&middot;" if not loop.last else "" }}</span>
                     {% endfor %}
                 </div>
             </div>
         </div>
     </footer>
 
-    <div id="cb-cookie-banner" class="alert alert-dark bg-dark text-white text-center mb-0" role="alert">
+    <div id="cb-cookie-banner" class="alert bg-dark text-white text-center mb-0" role="alert">
         We and our selected third parties use cookies 🍪 or similar technologies to ensure
         you get the best experience on our website as specified in the our <a class="text-white"
             href="{{meta.url}}/privacy/" target="_blank">Privacy Policy</a> and <a class="text-white"
             href="{{meta.url}}/terms/" target="_blank">Terms of
             Services</a>. If you continue to use this site we will
         assume that you are happy with it.
         <button type="button" class="btn btn-primary btn-sm ms-3" onclick="window.cb_hideCookieBanner()">
```

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/templates/index.html` & `meetlify-0.1.7/src/meetlify/themes/lindau/templates/meetup.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,81 @@
 {% extends "base.html" %}
 
 {% block main_header %}
-<meta name="description" content="{{meta.description}}" />
-<meta name="author" content="{{meta.author}}" />
-<link href="{{meta.URL}}" rel="canonical" />
-<title>{{meta.title}}</title>
-<meta content="{{meta.title}}" property="og:title" />
-<meta content="{{meta.description}}" property="og:description" />
-<meta content="{{meta.url}}" property="og:url" />
+<meta name="description" content="{{meetup.description}}" />
+<meta name="author" content="{{meetup.author}}" />
+<link href="{{meta.URL}}/{{meta.folders.meetups}}/{{meetup.slug}}/" rel="canonical" />
+<title>{{meetup.title}}</title>
+<meta content="{{meetup.title}}" property="og:title" />
+<meta content="{{meetup.description}}" property="og:description" />
+<meta content="{{meta.URL}}/{{meta.folders.meetups}}/{{meetup.slug}}/" property="og:url" />
 {% endblock main_header %}
 
+
 {% block main_content %}
-<!-- Header-->
-<header class="bg-dark py-5" id="home">
-    <div class="container px-5">
-        <div class="row gx-5 align-items-center justify-content-center">
-            <div class="col-lg-8 col-xl-7 col-xxl-6">
-                <div class="my-5 text-center text-xl-start">
-                    <h1 class="display-5 fw-bolder text-white mb-2">{{meta.title}}
-                    </h1>
-                    <p class="text-white-50 mb-4"> Our next meetup is in <em class="text-white mb-4">Wangen im
-                            Allgäu</em> on
-                        <em class="text-white mb-4"> {{meetups[0].date}}</em>.
-                    </p>
-                    <p class="text-white-50 mb-4">
-                        Drop us an email at <em class="text-white mb-4">{{meta.email}}</em>
-                        if you plan to join. This will help to better organize the event.
-                    </p>
-                    <div class="d-grid gap-3 d-sm-flex justify-content-sm-center justify-content-xl-start">
-                        <a class="btn btn-primary btn-lg px-4 me-sm-3"
-                            href="{{meta.URL}}/meetups/{{meetups[0].slug}}/">More Details</a>
-                        <a class="btn btn-outline-light btn-lg px-4" href="{{meta.URL}}/meetups/">Future Meetups</a>
-                    </div>
-                </div>
-            </div>
-            <div class="col-xl-5 col-xxl-6 d-none d-xl-block text-center"><img class="img-fluid rounded-3 my-5"
-                    src="{{meta.URL}}/static/assets/banner.png" alt="{{meta.name}} about us banner" /></div>
-        </div>
-    </div>
-</header>
-<section class="py-5" id="about">
+<!-- Page Content-->
+<section class="py-5">
     <div class="container px-5 my-5">
-        <div class="row gx-5 align-items-center">
-            <div class="col-lg-6 order-first order-lg-last"><img class="img-fluid rounded mb-5 mb-lg-0"
-                    src="{{meta.URL}}/static/assets/about.png" alt="{{meta.author}} image"></div>
-            <div class="col-lg-6">
-                {{home_content}}
+        <div class="row gx-5">
+            <div class="col-lg-8">
+                <!-- Post content-->
+                <article>
+                    <!-- Post header-->
+                    <header class="mb-4">
+                        <!-- Post title-->
+                        <h1 class="fw-bolder mb-1">{{meetup.title}}</h1>
+                        <!-- Post tags-->
+                        <a class="badge bg-secondary text-decoration-none link-light mt-3" href="/">Python</a>
+                        <a class="badge bg-secondary text-decoration-none link-light mt-3" href="/">Meetup</a>
+                    </header>
+                    <section class="mb-5">
+                        {{ meetup.content }}
+                    </section>
+                </article>
             </div>
-        </div>
-    </div>
-</section>
+            <div class="col-lg-4">
+                <div class="py-2 sidebar">
+                    <div class="d-flex align-items-center mt-lg-4 mb-4">
+                        <img class="img-fluid rounded-circle" src="{{meta.URL}}/static/assets/author.png" width="60"
+                            height="60" alt="{{meta.author}} Image" />
+                        <div class="ms-3">
+                            <h4 class="fw-bold">{{meetup.organizer}} </h4>
+                            <div class="text-muted">Organizer</div>
+                        </div>
+                    </div>
+                    <div class="card border-0 bg-light mt-xl-3">
+                        <div class="card-body p-4 py-lg-4">
+                            <div class="text-muted mb-2">Meetup Date: <div class="fw-bold">
+                                    {{meetup.event_datetime.strftime('%Y-%m-%d @ %H:%M')}}
+                                </div>
+                            </div>
+                            <div class="text-muted mb-2">Meetup Location: <div class="fw-bold">{{meetup.address}}</div>
+                            </div>
+                        </div>
+                    </div>
 
-<section class="py-5 bg-light" id="meetups">
-    <div class="container px-5 my-5">
-        <div class="row gx-5 justify-content-left">
-            <div class="col-lg-12">
-                <div class="text-left">
-                    <h2 class="fw-bolder  mb-4">Meetups</h2>
-                    <p class="mb-5">Here is the list of upcoming meetups organized by
-                        PyBodensee. </p>
-                </div>
-            </div>
-        </div>
-        <div class="row gx-5">
-            {% for meetup in meetups%}
-            <div class="col-lg-4 mb-5">
-                <div class="card h-100 shadow border-0">
-                    <img class="card-img-top" src="{{meta.URL}}/images/{{meetup.featureimage}}"
-                        alt="Feature Image for Meetup">
-                    <div class="card-body p-4">
-                        <div class="badge bg-primary bg-gradient rounded-pill mb-2">Meetup</div>
-                        <a class="text-decoration-none link-dark stretched-link"
-                            href="{{meta.URL}}/meetups/{{meetup.slug}}/">
-                            <h5 class="card-title mb-3"> {{meetup.title}}
-                            </h5>
-                        </a>
-                        <p class="card-text mb-0">Agenda: {{meetup.description}}</p>
+                    <div class="card border-0 bg-light mt-xl-3">
+                        <div class="card-body p-4 py-lg-4">
+                            <img class="img-fluid rounded mb-5 mb-lg-0"
+                                src="{{meta.URL}}/images/{{meetup.feature_image}}" alt="{{meta.author}} image">
+                        </div>
                     </div>
-                    <div class="card-footer p-4 pt-0 bg-transparent border-top-0">
-                        <div class="d-flex align-items-end justify-content-between">
-                            <div class="d-flex align-items-center">
-                                <div class="small">
-                                    <div class="fw-bold">Date: {{meetup.date}} · Status:
-                                        <em>{{meetup.status}}</em>
-                                    </div>
-                                    <div class="text-muted">Location: {{meetup.address}}
-                                    </div>
-                                    <div class="text-muted">Organizer: {{meetup.author}}</div>
+
+                    <div class="card border-0 bg-light mt-xl-3">
+                        <div class="card-body p-4 py-lg-4">
+                            <div class="d-flex align-items-center justify-content-center">
+                                <div class="text-center">
+                                    <div class="h6 fw-bolder">Have more questions?</div>
+                                    <p class="text-muted mb-4">
+                                        Check out our <a href=" {{meta.URL}}/contact/">Contact us</a> page to get in
+                                        touch or send us an email at <br><code>pybodensee at gmail dot com</code>
+                                    </p>
                                 </div>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
-            {% endfor%}
-        </div>
-        <div class="text-end mb-5 mb-xl-0">
-            <a class="text-decoration-none" href="{{meta.URL}}/meetups/">
-                Older Meetups
-                <i class="bi bi-arrow-right"></i>
-            </a>
         </div>
     </div>
 </section>
 {% endblock main_content %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,23 +1,16 @@
 {% extends "base.html" %} {% block main_header %}
 {% endblock main_header %} {% block main_content %}
-************ {{{{mmeettaa..ttiittllee}}}} ************
-Our next meetup is in WWaannggeenn iimm AAllllgg?Ã?¤uu on {{{{mmeeeettuuppss[[00]]..ddaattee}}}}.
-Drop us an email at {{{{mmeettaa..eemmaaiill}}}} if you plan to join. This will help to
-better organize the event.
-_M_o_r_e_ _D_e_t_a_i_l_s _F_u_t_u_r_e_ _M_e_e_t_u_p_s
-[{{meta.name}} about us banner]
+************ {{{{mmeeeettuupp..ttiittllee}}}} ************
+_P_y_t_h_o_n _M_e_e_t_u_p {{ meetup.content }}
+[{{meta.author}} Image]
+****** {{{{mmeeeettuupp..oorrggaanniizzeerr}}}} ******
+Organizer
+Meetup Date:
+{{meetup.event_datetime.strftime('%Y-%m-%d @ %H:%M')}}
+Meetup Location:
+{{meetup.address}}
 [{{meta.author}} image]
-{{home_content}}
-********** MMeeeettuuppss **********
-Here is the list of upcoming meetups organized by PyBodensee.
-{% for meetup in meetups%}
-[Feature Image for Meetup]
-Meetup
-_**_**_ _{{_{{_mm_ee_ee_tt_uu_pp_.._tt_ii_tt_ll_ee_}}_}}_ _**_**
-Agenda: {{meetup.description}}
-Date: {{meetup.date}} Â· Status: {{{{mmeeeettuupp..ssttaattuuss}}}}
-Location: {{meetup.address}}
-Organizer: {{meetup.author}}
-{% endfor%}
-_O_l_d_e_r_ _M_e_e_t_u_p_s
+Have more questions?
+Check out our _C_o_n_t_a_c_t_ _u_s page to get in touch or send us an email at
+pybodensee at gmail dot com
 {% endblock main_content %}
```

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/templates/meetup.html` & `meetlify-0.1.7/src/meetlify/themes/lindau/templates/post.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,71 @@
 {% extends "base.html" %}
 
 {% block main_header %}
-<meta name="description" content="{{front.description}}" />
-<meta name="author" content="{{front.author}}" />
-<link href="{{meta.URL}}/meetups/{{front.slug}}/" rel="canonical" />
-<title>{{front.title}}</title>
-<meta content="{{front.title}}" property="og:title" />
-<meta content="{{front.description}}" property="og:description" />
-<meta content="{{meta.URL}}/meetups/{{front.slug}}/" property="og:url" />
+<meta name="description" content="{{post.description}}" />
+<meta name="author" content="{{post.author}}" />
+<link href="{{meta.URL}}/{{meta.folders.posts}}/{{post.slug}}/" rel="canonical" />
+<title>{{post.title}}</title>
+<meta content="{{post.title}}" property="og:title" />
+<meta content="{{post.description}}" property="og:description" />
+<meta content="{{meta.URL}}/{{meta.folders.posts}}/{{post.slug}}/" property="og:url" />
 {% endblock main_header %}
 
 
 {% block main_content %}
 <!-- Page Content-->
 <section class="py-5">
     <div class="container px-5 my-5">
         <div class="row gx-5">
             <div class="col-lg-8">
                 <!-- Post content-->
                 <article>
                     <!-- Post header-->
                     <header class="mb-4">
                         <!-- Post title-->
-                        <h1 class="fw-bolder mb-1">{{front.title}}</h1>
+                        <h1 class="fw-bolder mb-1">{{post.title}}</h1>
+                        <div class="text-muted fst-italic mt-2">Published on {{post.create_date.strftime('%Y-%m-%d')}}
+                            by {{meta.author}}
+                        </div>
                         <!-- Post categories-->
-                        <a class="badge bg-secondary text-decoration-none link-light mt-3" href="/">Python</a>
-                        <a class="badge bg-secondary text-decoration-none link-light mt-3" href="/">Meetup</a>
+                        {% for tag in post.tags %}
+                        <a class="badge bg-secondary text-decoration-none link-light mt-3"
+                            href="/">{{tag|trim|capitalize}}</a>
+                        {% endfor %}
                     </header>
                     <section class="mb-5">
-                        {{ content }}
+                        {% if banner.name %}
+                        <div class="admonition {{banner.type_}}">
+                            <p class="admonition-title text-white fw-bolder">{{banner.name}}</p>
+                            <p>{{banner.message}}</p>
+                        </div>
+                        {% endif %}
+                        {{ post.content }}
                     </section>
                 </article>
             </div>
             <div class="col-lg-4">
                 <div class="py-2 sidebar">
-                    <div class="d-flex align-items-center mt-lg-4 mb-4">
-                        <img class="img-fluid rounded-circle" src="{{meta.URL}}/static/assets/author.png" width="60"
-                            height="60" alt="{{meta.author}} Image" />
-                        <div class="ms-3">
-                            <h4 class="fw-bold">{{front.author}} </h4>
-                            <div class="text-muted">Organizer</div>
-                        </div>
-                    </div>
                     <div class="card border-0 bg-light mt-xl-3">
                         <div class="card-body p-4 py-lg-4">
-                            <div class="text-muted mb-2">Meetup Date: <div class="fw-bold">{{front.date}}</div>
-                            </div>
-                            <div class="text-muted mb-2">Meetup Location: <div class="fw-bold">{{front.address}}</div>
+                            <div class="h5 fw-bolder px-2">Table of Contents</div>
+                            <div class="fw-bold mt-2">
+                                {{post.toc}}
                             </div>
                         </div>
                     </div>
 
                     <div class="card border-0 bg-light mt-xl-3">
                         <div class="card-body p-4 py-lg-4">
-                            <img class="img-fluid rounded mb-5 mb-lg-0" src="{{meta.URL}}/images/{{front.featureimage}}"
-                                alt="{{meta.author}} image">
-                        </div>
-                    </div>
-
-                    <div class="card border-0 bg-light mt-xl-3">
-                        <div class="card-body p-4 py-lg-4">
                             <div class="d-flex align-items-center justify-content-center">
                                 <div class="text-center">
                                     <div class="h6 fw-bolder">Have more questions?</div>
                                     <p class="text-muted mb-4">
                                         Check out our <a href=" {{meta.URL}}/contact/">Contact us</a> page to get in
-                                        touch
-                                        or to get in touch send us an email at <code>pybodensee at gmail dot com</code>
+                                        touch or send us an email at <br><code>pybodensee at gmail dot com</code>
                                     </p>
                                 </div>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
 {% extends "base.html" %} {% block main_header %}
 {% endblock main_header %} {% block main_content %}
-************ {{{{ffrroonntt..ttiittllee}}}} ************
-_P_y_t_h_o_n _M_e_e_t_u_p {{ content }}
-[{{meta.author}} Image]
-****** {{{{ffrroonntt..aauutthhoorr}}}} ******
-Organizer
-Meetup Date:
-{{front.date}}
-Meetup Location:
-{{front.address}}
-[{{meta.author}} image]
+************ {{{{ppoosstt..ttiittllee}}}} ************
+Published on {{post.create_date.strftime('%Y-%m-%d')}} by {{meta.author}}
+{% for tag in post.tags %} _{_{_t_a_g_|_t_r_i_m_|_c_a_p_i_t_a_l_i_z_e_}_} {% endfor %} {% if
+banner.name %}
+{{banner.name}}
+{{banner.message}}
+{% endif %} {{ post.content }}
+Table of Contents
+{{post.toc}}
 Have more questions?
-Check out our _C_o_n_t_a_c_t_ _u_s page to get in touch or to get in touch send us an
-email at pybodensee at gmail dot com
+Check out our _C_o_n_t_a_c_t_ _u_s page to get in touch or send us an email at
+pybodensee at gmail dot com
 {% endblock main_content %}
```

### Comparing `meetlify-0.1.6/src/meetlify/themes/lindau/templates/meetups.html` & `meetlify-0.1.7/src/meetlify/themes/lindau/templates/meetups.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% extends "base.html" %}
 
 {% block main_header %}
 <meta name="description" content="Here is the list of upcoming Meetups organized by {{meta.name}}" />
 <meta name="author" content="{{meta.author}}" />
-<link href="{{meta.URL}}/meetups/" rel="canonical" />
+<link href="{{meta.URL}}/{{meta.folders.meetups}}/" rel="canonical" />
 <title>Python Meetups in Bodensee Regions</title>
 <meta content="upcoming Meetups organized by {{meta.name}}" property="og:title" />
 <meta content="Here is the list of upcoming Meetups organized by {{meta.name}}" property="og:description" />
-<meta content="{{meta.URL}}/meetups/" property="og:url" />
+<meta content="{{meta.URL}}/{{meta.folders.meetups}}/" property="og:url" />
 {% endblock main_header %}
 
 
 {% block main_content %}
 <!-- Page Content-->
 <section class="py-5 bg-light">
     <div class="container px-5">
@@ -21,22 +21,22 @@
                 <div class="row gx-0">
                     <div class="col-lg-6 col-xl-5 py-lg-5">
                         <div class="p-4 p-md-5">
                             <div class="badge bg-primary bg-gradient rounded-pill mb-2">Meetup</div>
                             <div class="h2 fw-bolder"> {{meetups[0].title}}</div>
                             <p>{{meetups[0].description}}</p>
                             <a class="stretched-link text-decoration-none"
-                                href="{{meta.URL}}/meetups/{{meetups[0].slug}}/">
+                                href="{{meta.URL}}/{{meta.folders.meetups}}/{{meetups[0].slug}}/">
                                 Read more <i class="bi bi-arrow-right"></i>
                             </a>
                         </div>
                     </div>
                     <div class="col-lg-6 col-xl-7">
                         <div class="bg-featured-blog"
-                            style="background-image: url('{{meta.URL}}/images/{{meetups[0].featureimage}}')">
+                            style="background-image: url('{{meta.URL}}/images/{{meetups[0].feature_image}}')">
                         </div>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 </section>
@@ -45,35 +45,36 @@
 <section class="py-5">
     <div class="container px-5">
         <h2 class="fw-bolder mb-4">Recent Meetups</h2>
         <div class="row gx-5">
             {% for meetup in meetups[1:]%}
             <div class="col-lg-4 mb-5">
                 <div class="card h-100 shadow border-0">
-                    <img class="card-img-top" src="{{meta.URL}}/images/{{meetup.featureimage}}"
+                    <img class="card-img-top" src="{{meta.URL}}/images/{{meetup.feature_image}}"
                         alt="Feautre Image for Meetup">
                     <div class="card-body p-4">
                         <div class="badge bg-primary bg-gradient rounded-pill mb-2">Meetup</div>
                         <a class="text-decoration-none link-dark stretched-link"
-                            href="{{meta.URL}}/meetups/{{meetup.slug}}/">
+                            href="{{meta.URL}}/{{meta.folders.meetups}}/{{meetup.slug}}/">
                             <h5 class="card-title mb-3">{{meetup.title}}
                             </h5>
                         </a>
                         <p class="card-text mb-0">Agenda: {{meetup.description}}</p>
                     </div>
                     <div class="card-footer p-4 pt-0 bg-transparent border-top-0">
                         <div class="d-flex align-items-end justify-content-between">
                             <div class="d-flex align-items-center">
                                 <div class="small">
-                                    <div class="fw-bold">Date: {{meetup.date}} · Status:
+                                    <div class="fw-bold">Date: {{meetup.event_datetime.strftime('%Y-%m-%d @ %H:%M')}} ·
+                                        Status:
                                         <em>{{meetup.status}}</em>
                                     </div>
                                     <div class="text-muted">Location: {{meetup.address}}
                                     </div>
-                                    <div class="text-muted">Organizer: {{meetup.author}}</div>
+                                    <div class="text-muted">Organizer: {{meetup.organizer}}</div>
                                 </div>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
             {% endfor%}
```

#### html2text {}

```diff
@@ -7,12 +7,13 @@
 _R_e_a_d_ _m_o_r_e
 ********** RReecceenntt MMeeeettuuppss **********
 {% for meetup in meetups[1:]%}
 [Feautre Image for Meetup]
 Meetup
 _**_**_ _{{_{{_mm_ee_ee_tt_uu_pp_.._tt_ii_tt_ll_ee_}}_}}_ _**_**
 Agenda: {{meetup.description}}
-Date: {{meetup.date}} Â· Status: {{{{mmeeeettuupp..ssttaattuuss}}}}
+Date: {{meetup.event_datetime.strftime('%Y-%m-%d @ %H:%M')}} Â· Status: {{
+{{mmeeeettuupp..ssttaattuuss}}}}
 Location: {{meetup.address}}
-Organizer: {{meetup.author}}
+Organizer: {{meetup.organizer}}
 {% endfor%}
 {% endblock main_content %}
```

### Comparing `meetlify-0.1.6/src/meetlify/utils.py` & `meetlify-0.1.7/tests/test_meetups.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 Meetlify: Static Site Generator for Meetup Websites
 A Python Package for Generating Static Website for Meetups.
 https://github.com/pybodensee/meetlify
 
-    src\meetlify\\utils.py
+    tests\test_meetups.py
     
     Copyright (C) 2024-2024 Faisal Shahzad <info@serpwings.com>
 
 <LICENSE_BLOCK>
 Permission is hereby granted, free of charge, to any person obtaining a copy of 
 this software and associated documentation files (the "Software"), to deal in 
 the Software without restriction, including without limitation the rights to 
@@ -26,48 +26,10 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
 SOFTWARE.
 </LICENSE_BLOCK>
 """
 
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++
-# INTERNAL IMPORTS
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-from pathlib import Path
-import shutil
-
-
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++
-# 3rd PARTY LIBRARY IMPORTS
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++
-
-from slugify import slugify
-
-
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++
-# IMPLEMENATIONS
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++
-
-
-def initialize(dest_: Path) -> None:
-    """Intialze Meetlify Website
-
-    Args:
-        dest_ (Path): Speficy folder for Destitaion folder.
-    """
-    assert isinstance(dest_, Path)
-    assert dest_.exists()
-
-    shutil.copyfile(
-        Path(Path(__file__).resolve().parent, "share", "configs.json"),
-        Path(dest_, "configs.json"),
-    )
-
-
-def get_slug(slug_, title_):
-    # slug_ = "".join(_md.Meta["slug"])
-    # slug_ = slugify("".join(_md.Meta["title"])) if not slug_ else slug_
-
-    slug_ = "".join(slug_)
-    return slugify("".join(title_)) if not slug_ else slug_
+def test_init():
+    pass
```

### Comparing `meetlify-0.1.6/src/meetlify.egg-info/PKG-INFO` & `meetlify-0.1.7/src/meetlify.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.6.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.7.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -17,29 +17,26 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: markdown
 Requires-Dist: Jinja2
 Requires-Dist: python-slugify
 Provides-Extra: dev
@@ -54,25 +51,25 @@
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
+Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: mkdocs-gen-files; extra == "all"
-Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: mkdocstrings[python]; extra == "all"
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: black; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: mkdocs; extra == "all"
 Requires-Dist: twine; extra == "all"
 Requires-Dist: setuptools; extra == "all"
+Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: mkdocstrings[python]; extra == "all"
+Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: wheel; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -111,20 +108,25 @@
 
 destination_path = Path("/home/user/Desktop/sample_webiste/")
 
 # Now initialize configurationn file
 initialize(dest_=destination_path)
 
 # Modify newly created config.json file as per your need.
-mlfy = Meetlify(dest_=destination_path) # Create Meetlify object with destination folder
-mlfy.parse_meetups() # Parse meetups markdown files
-mlfy.render_meetups() # Render meetups
-mlfy.render_home() # Render Home Page
-mlfy.render_pages() # Render Static Pages
-mlfy.copy_assests() # Copy assets e.g. Favicon, Images, JS, CSS files
+mtlfy = Meetlify(dest_=destination_path)
+mtlfy.render_home()
+mtlfy.render_404_page()
+mtlfy.render_meetups()
+mtlfy.render_posts()
+mtlfy.render_pages()
+mtlfy.render_redirects()
+mtlfy.render_sitemaps()
+mtlfy.render_robots_txt()
+mtlfy.copy_assests()
+
 ```
 
 ## How to Extend ?
 - Clone or download this repository to your computer.
 - Create a virtual environment using ``python -m .venv venv``
 - Navigate to the downloaded directory and then install all required dependencies using ``pip install -e .``
 - Now you can open ``api.py`` file and start editing it. Feel free to extend it or even submit a pull request if you have a useful feature.
```

### Comparing `meetlify-0.1.6/src/meetlify.egg-info/SOURCES.txt` & `meetlify-0.1.7/src/meetlify.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 setup.cfg
 setup.py
 src/meetlify/__init__.py
 src/meetlify/api.py
 src/meetlify/cli.py
 src/meetlify/configs.py
 src/meetlify/constants.py
-src/meetlify/meetup.py
-src/meetlify/page.py
-src/meetlify/post.py
-src/meetlify/sitemap.py
+src/meetlify/meetups.py
+src/meetlify/pages.py
+src/meetlify/posts.py
+src/meetlify/redirects.py
+src/meetlify/robots.py
+src/meetlify/sitemaps.py
 src/meetlify/utils.py
 src/meetlify.egg-info/PKG-INFO
 src/meetlify.egg-info/SOURCES.txt
 src/meetlify.egg-info/dependency_links.txt
 src/meetlify.egg-info/entry_points.txt
 src/meetlify.egg-info/not-zip-safe
 src/meetlify.egg-info/requires.txt
@@ -67,14 +69,15 @@
 src/meetlify/themes/lindau/static/css/bootstrap.min.css
 src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
 src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
 src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
 src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
 src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
 src/meetlify/themes/lindau/static/css/cookiealert.css
+src/meetlify/themes/lindau/static/css/custom.css
 src/meetlify/themes/lindau/static/css/styles.css
 src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
 src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
 src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
 src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
 src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
 src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
@@ -90,10 +93,12 @@
 src/meetlify/themes/lindau/static/js/scripts.js
 src/meetlify/themes/lindau/templates/404.html
 src/meetlify/themes/lindau/templates/base.html
 src/meetlify/themes/lindau/templates/index.html
 src/meetlify/themes/lindau/templates/meetup.html
 src/meetlify/themes/lindau/templates/meetups.html
 src/meetlify/themes/lindau/templates/page.html
+src/meetlify/themes/lindau/templates/post.html
+src/meetlify/themes/lindau/templates/posts.html
 src/meetlify/themes/lindau/templates/sitemap-index.xml
 src/meetlify/themes/lindau/templates/sitemap.xml
 tests/test_meetups.py
```

